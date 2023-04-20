# Comparing `tmp/dbt-coverage-0.3.2.tar.gz` & `tmp/dbt_coverage-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-coverage-0.3.2.tar", last modified: Fri Nov 18 11:27:30 2022, max compression
+gzip compressed data, was "dbt_coverage-0.3.3.tar", max compression
```

## Comparing `dbt-coverage-0.3.2.tar` & `dbt_coverage-0.3.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1076 2022-11-17 15:50:45.038105 dbt-coverage-0.3.2/LICENSE.md
--rw-r--r--   0        0        0    11594 2022-11-17 17:14:14.471747 dbt-coverage-0.3.2/README.md
--rw-r--r--   0        0        0    33633 2022-11-17 19:32:50.689258 dbt-coverage-0.3.2/dbt_coverage/__init__.py
--rw-r--r--   0        0        0     1081 2022-11-18 11:27:26.813066 dbt-coverage-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    12585 1970-01-01 00:00:00.000000 dbt-coverage-0.3.2/setup.py
--rw-r--r--   0        0        0    12666 1970-01-01 00:00:00.000000 dbt-coverage-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2021-11-22 15:44:35.000000 dbt_coverage-0.3.3/LICENSE.md
+-rw-r--r--   0        0        0    11594 2022-11-21 18:01:55.219725 dbt_coverage-0.3.3/README.md
+-rw-r--r--   0        0        0    32417 2023-04-20 11:34:06.923234 dbt_coverage-0.3.3/dbt_coverage/__init__.py
+-rw-r--r--   0        0        0     1194 2023-04-20 11:48:46.212663 dbt_coverage-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    12968 1970-01-01 00:00:00.000000 dbt_coverage-0.3.3/PKG-INFO
```

### Comparing `dbt-coverage-0.3.2/LICENSE.md` & `dbt_coverage-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-coverage-0.3.2/README.md` & `dbt_coverage-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-coverage-0.3.2/dbt_coverage/__init__.py` & `dbt_coverage-0.3.3/dbt_coverage/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,109 +52,81 @@
         return tests is not None and tests
 
 
 @dataclass
 class Table:
     """Dataclass containing the information about a database table and its columns."""
 
-    name: str
     unique_id: str
-    original_file_path: None
+    name: str
+    original_file_path: str
     columns: Dict[str, Column]
 
     @staticmethod
-    def from_node(node) -> Table:
+    def from_node(node, manifest: Manifest) -> Table:
+        unique_id = node["unique_id"]
+        manifest_table = manifest.get_table(unique_id)
         columns = [Column.from_node(col) for col in node["columns"].values()]
+        original_file_path = manifest_table["original_file_path"] if manifest_table else None
+
+        if original_file_path is None:
+            logging.warning("original_file_path value not found in manifest for %s", unique_id)
+
         return Table(
-            f"{node['metadata']['schema']}.{node['metadata']['name']}".lower(),
-            node["unique_id"],
-            None,
+            unique_id,
+            # Take table name from manifest.json instead of catalog.json since in catalog.json the
+            # name is actually an alias in case it is defined.
+            manifest_table["name"].lower(),
+            original_file_path,
             {col.name: col for col in columns},
         )
 
-    def update_original_file_path(self, manifest: Manifest) -> None:
-        """
-        Update Table's ``original_file_path`` attribute by retrieving this information from a
-        Manifest.
-
-        :param manifest: the Manifest used which contains the ``original_file_path`` for a Table
-        :returns: None
-        """
-        old_original_file_path_value = self.original_file_path
-
-        manifest_attributes = vars(manifest)
-        for attribute_type_name, attribute_type_dict in manifest_attributes.items():
-            for (
-                attribute_instance_name,
-                attribute_instance,
-            ) in attribute_type_dict.items():
-
-                if self.unique_id in attribute_instance.values():
-                    self.original_file_path = attribute_instance["original_file_path"]
-
-        if (
-            self.original_file_path is None
-            or self.original_file_path == old_original_file_path_value
-        ):
-            logging.info(
-                f"original_file_path value not found in manifest for {self.unique_id}"
-            )
-
     def get_column(self, column_name):
         return self.columns.get(column_name)
 
 
 @dataclass
 class Catalog:
     """Dataclass containing the information about a database catalog, its tables and columns."""
 
     tables: Dict[str, Table]
 
-    def filter_catalog(self, model_path_filter: List[str]) -> Catalog:
+    def filter_tables(self, model_path_filter: List[str]) -> Catalog:
         """
-        Filter ``Catalog``'s ``tables`` attribute to ``Tables`` that have the``model_path_filter``
-        value at the start of their ``original_file_path``.
+        Filters ``Catalog``'s ``tables`` attribute to ``Tables`` that have the
+        ``model_path_filter`` value at the start of their ``original_file_path``.
 
-        :param model_path_filter: the model_path string(s) to filter tables on, (matches using
-        the ``startswith`` operator)
+        Args:
+            model_path_filter: the model_path string(s) to filter tables on, (matches using
+                the ``startswith`` operator)
 
-        :returns: Catalog
-        :raises ValueError: if no ``Table`` in the ``tables`` Catalog attribute have an
-        ``original_file_path`` that contains any ``model_path_filter`` value
+        Returns:
+            New ``Catalog`` instance containing only ``Table``s that passed the filter
         """
-        filtered_tables = {}
 
-        original_tables_dict = {key: val for key, val in self.tables.items()}
-        for key, table in original_tables_dict.items():
-            for path in model_path_filter:
-                if table.original_file_path.startswith(path):
-                    filtered_tables[key] = table
-                    break
+        model_path_filter = tuple(model_path_filter)
+        tables = {
+            t_id: t
+            for t_id, t in self.tables.items()
+            if t.original_file_path.startswith(model_path_filter)
+        }
 
-        if len(filtered_tables) < 1:
-            logging.error("len(filtered_tables) < 1", exc_info=True)
-            raise ValueError(
-                "After filtering the Catalog contains no tables. Ensure your model_path_filter "
-                "is correct"
-            )
-        else:
-            logging.info(
-                "Successfully filtered tables. Total tables post-filtering: %d tables",
-                len(filtered_tables),
-            )
+        logging.info(
+            "Successfully filtered tables. Total tables post-filtering: %d tables", len(tables)
+        )
 
-            return Catalog(tables=filtered_tables)
+        return Catalog(tables=tables)
 
     @staticmethod
-    def from_nodes(nodes):
-        tables = [Table.from_node(table) for table in nodes]
-        return Catalog({table.name: table for table in tables})
+    def from_nodes(nodes, manifest: Manifest):
+        tables = [Table.from_node(table, manifest) for table in nodes]
+        return Catalog({table.unique_id: table for table in tables})
 
-    def get_table(self, table_name):
-        return self.tables.get(table_name)
+    def get_table(self, table_id):
+        return self.tables.get(table_id)
 
 
 @dataclass
 class Manifest:
     sources: Dict[str, Dict[str, Dict[str, Dict]]]
     models: Dict[str, Dict[str, Dict[str, Dict]]]
     seeds: Dict[str, Dict[str, Dict[str, Dict]]]
@@ -162,122 +134,122 @@
     tests: Dict[str, Dict[str, List[Dict]]]
 
     @classmethod
     def from_nodes(cls, manifest_nodes: Dict[str, Dict]) -> Manifest:
         """Constructs a ``Manifest`` by parsing from manifest.json nodes."""
 
         sources = [
-            table
-            for table in manifest_nodes.values()
-            if table["resource_type"] == "source"
+            table for table in manifest_nodes.values() if table["resource_type"] == "source"
         ]
         sources = {
-            cls._full_table_name(table): {
+            table["unique_id"]: {
                 "columns": cls._normalize_column_names(table["columns"]),
                 "original_file_path": cls._normalize_path(table["original_file_path"]),
-                "unique_id": table["unique_id"],
+                "name": cls._full_table_name(table),
             }
             for table in sources
         }
 
-        models = [
-            table
-            for table in manifest_nodes.values()
-            if table["resource_type"] == "model"
-        ]
+        models = [table for table in manifest_nodes.values() if table["resource_type"] == "model"]
         models = {
-            cls._full_table_name(table): {
+            table["unique_id"]: {
                 "columns": cls._normalize_column_names(table["columns"]),
                 "original_file_path": cls._normalize_path(table["original_file_path"]),
-                "unique_id": table["unique_id"],
+                "name": cls._full_table_name(table),
             }
             for table in models
         }
 
-        seeds = [
-            table
-            for table in manifest_nodes.values()
-            if table["resource_type"] == "seed"
-        ]
+        seeds = [table for table in manifest_nodes.values() if table["resource_type"] == "seed"]
         seeds = {
-            cls._full_table_name(table): {
+            table["unique_id"]: {
                 "columns": cls._normalize_column_names(table["columns"]),
                 "original_file_path": cls._normalize_path(table["original_file_path"]),
-                "unique_id": table["unique_id"],
+                "name": cls._full_table_name(table),
             }
             for table in seeds
         }
 
         snapshots = [
-            table
-            for table in manifest_nodes.values()
-            if table["resource_type"] == "snapshot"
+            table for table in manifest_nodes.values() if table["resource_type"] == "snapshot"
         ]
         snapshots = {
-            cls._full_table_name(table): {
+            table["unique_id"]: {
                 "columns": cls._normalize_column_names(table["columns"]),
                 "original_file_path": cls._normalize_path(table["original_file_path"]),
-                "unique_id": table["unique_id"],
+                "name": cls._full_table_name(table),
             }
             for table in snapshots
         }
 
         tests = cls._parse_tests(manifest_nodes)
 
         return Manifest(sources, models, seeds, snapshots, tests)
 
+    def get_table(self, table_id):
+        source_candidate = self.sources.get(table_id)
+        models_candidate = self.models.get(table_id)
+        seeds_candidate = self.seeds.get(table_id)
+        snapshots_candidate = self.snapshots.get(table_id)
+
+        all_candidates = [
+            source_candidate,
+            models_candidate,
+            seeds_candidate,
+            snapshots_candidate,
+        ]
+        non_empty_candidates = [c for c in all_candidates if c]
+
+        if len(non_empty_candidates) > 1:
+            raise ValueError(
+                f"Duplicate unique_id: {table_id}, duplicate entries: {non_empty_candidates}"
+            )
+
+        return non_empty_candidates[0] if non_empty_candidates else None
+
     @classmethod
-    def _parse_tests(
-        cls, manifest_nodes: Dict[str, Dict]
-    ) -> Dict[str, Dict[str, List[Dict]]]:
+    def _parse_tests(cls, manifest_nodes: Dict[str, Dict]) -> Dict[str, Dict[str, List[Dict]]]:
         """Parses tests from manifest.json nodes.
 
         The logic is taken from the dbt-docs official source code:
         https://github.com/dbt-labs/dbt-docs/blob/02731092389b18d69649fdc322d969b5d5b61b20/src/app/services/project_service.js#L155-L221
         """
 
-        id_to_table_name = {
-            table_id: cls._full_table_name(table)
-            for table_id, table in manifest_nodes.items()
-            if table["resource_type"] in ["source", "model", "seed", "snapshot"]
-        }
-
         tests = {}
         for node in manifest_nodes.values():
             if node["resource_type"] != "test" or "test_metadata" not in node:
                 continue
 
             depends_on = node["depends_on"]["nodes"]
             if not depends_on:
                 continue
 
             if node["test_metadata"]["name"] == "relationships":
                 table_id = depends_on[-1]
             else:
                 table_id = depends_on[0]
-            table_name = id_to_table_name[table_id]
 
             column_name = (
                 node.get("column_name")
                 or node["test_metadata"]["kwargs"].get("column_name")
                 or node["test_metadata"]["kwargs"].get("arg")
             )
             if not column_name:
                 continue
 
             column_name = column_name.lower()
-            table_tests = tests.setdefault(table_name, {})
+            table_tests = tests.setdefault(table_id, {})
             column_tests = table_tests.setdefault(column_name, [])
             column_tests.append(node)
 
         return tests
 
     @staticmethod
     def _full_table_name(table):
-        return f'{table["schema"]}.{table["name"]}'.lower()
+        return f"{table['schema']}.{table['name']}".lower()
 
     @staticmethod
     def _normalize_column_names(columns):
         for col in columns.values():
             col["name"] = col["name"].lower()
         return {col["name"]: col for col in columns.values()}
 
@@ -320,43 +292,36 @@
     covered: Set[ColumnRef]
     total: Set[ColumnRef]
     misses: Set[ColumnRef] = field(init=False)
     coverage: float = field(init=False)
     subentities: Dict[str, CoverageReport]
 
     def __post_init__(self):
-        if self.covered is not None and self.total is not None:
+        if self.covered is not None and self.total is not None and self.total != 0:
             self.misses = self.total - self.covered
             self.coverage = len(self.covered) / len(self.total)
         else:
             self.misses = None
             self.coverage = None
 
     @classmethod
     def from_catalog(cls, catalog: Catalog, cov_type: CoverageType):
         subentities = {
             table.name: CoverageReport.from_table(table, cov_type)
             for table in catalog.tables.values()
         }
-        covered = set(
-            col for table_report in subentities.values() for col in table_report.covered
-        )
-        total = set(
-            col for table_report in subentities.values() for col in table_report.total
-        )
+        covered = set(col for table_report in subentities.values() for col in table_report.covered)
+        total = set(col for table_report in subentities.values() for col in table_report.total)
 
-        return CoverageReport(
-            cls.EntityType.CATALOG, cov_type, None, covered, total, subentities
-        )
+        return CoverageReport(cls.EntityType.CATALOG, cov_type, None, covered, total, subentities)
 
     @classmethod
     def from_table(cls, table: Table, cov_type: CoverageType):
         subentities = {
-            col.name: CoverageReport.from_column(col, cov_type)
-            for col in table.columns.values()
+            col.name: CoverageReport.from_column(col, cov_type) for col in table.columns.values()
         }
         covered = set(
             replace(col, table_name=table.name)
             for col_report in subentities.values()
             for col in col_report.covered
         )
         total = set(
@@ -377,17 +342,15 @@
             covered = column.test
         else:
             raise ValueError(f"Unsupported cov_type {cov_type}")
 
         covered = {CoverageReport.ColumnRef(None, column.name)} if covered else set()
         total = {CoverageReport.ColumnRef(None, column.name)}
 
-        return CoverageReport(
-            cls.EntityType.COLUMN, cov_type, column.name, covered, total, {}
-        )
+        return CoverageReport(cls.EntityType.COLUMN, cov_type, column.name, covered, total, {})
 
     def to_markdown_table(self):
         if self.entity_type == CoverageReport.EntityType.TABLE:
             return (
                 f"| {self.entity_name:70} | {len(self.covered):5}/{len(self.total):<5} | "
                 f"{self.coverage * 100:5.1f}% |"
             )
@@ -447,32 +410,27 @@
             }
         elif self.entity_type == CoverageReport.EntityType.TABLE:
             return {
                 "name": self.entity_name,
                 "covered": len(self.covered),
                 "total": len(self.total),
                 "coverage": self.coverage,
-                "columns": [
-                    col_report.to_dict() for col_report in self.subentities.values()
-                ],
+                "columns": [col_report.to_dict() for col_report in self.subentities.values()],
             }
         elif self.entity_type == CoverageReport.EntityType.CATALOG:
             return {
                 "cov_type": self.cov_type.value,
                 "covered": len(self.covered),
                 "total": len(self.total),
                 "coverage": self.coverage,
-                "tables": [
-                    table_report.to_dict() for table_report in self.subentities.values()
-                ],
+                "tables": [table_report.to_dict() for table_report in self.subentities.values()],
             }
         else:
             raise TypeError(
-                f"Unsupported report_type for to_dict method: "
-                f"{type(self.entity_type)}"
+                f"Unsupported report_type for to_dict method: " f"{type(self.entity_type)}"
             )
 
     @staticmethod
     def from_dict(report, cov_type: CoverageType):
         if "tables" in report:
             subentities = {
                 table_report["name"]: CoverageReport.from_dict(table_report, cov_type)
@@ -510,17 +468,15 @@
             )
         else:
             column_name = report["name"]
             return CoverageReport(
                 CoverageReport.EntityType.COLUMN,
                 cov_type,
                 column_name,
-                {CoverageReport.ColumnRef(None, column_name)}
-                if report["covered"] > 0
-                else set(),
+                {CoverageReport.ColumnRef(None, column_name)} if report["covered"] > 0 else set(),
                 {CoverageReport.ColumnRef(None, column_name)},
                 {},
             )
 
     def to_json(self):
         return json.dumps(self.to_dict(), indent=2)
 
@@ -534,30 +490,26 @@
     new_misses: Dict[str, CoverageDiff] = field(init=False)
 
     def __post_init__(self):
         assert self.before is None or self.before.cov_type == self.after.cov_type, (
             f"Cannot compare reports with different cov_types: {self.before.cov_type} and "
             f"{self.after.cov_type}"
         )
-        assert (
-            self.before is None or self.before.entity_type == self.after.entity_type
-        ), (
+        assert self.before is None or self.before.entity_type == self.after.entity_type, (
             f"Cannot compare reports with different report_types: {self.before.report_type} and "
             f"{self.after.entity_type}"
         )
 
         self.new_misses = self.find_new_misses()
 
     def find_new_misses(self):
         if self.after.entity_type == CoverageReport.EntityType.COLUMN:
             return None
 
-        new_misses = self.after.misses - (
-            self.before.misses if self.before is not None else set()
-        )
+        new_misses = self.after.misses - (self.before.misses if self.before is not None else set())
 
         res: Dict[str, CoverageDiff] = {}
         for new_miss in new_misses:
             new_misses_entity_name = (
                 new_miss.table_name
                 if self.after.entity_type == CoverageReport.EntityType.CATALOG
                 else new_miss.column_name
@@ -573,16 +525,15 @@
         return res
 
     def summary(self):
         buf = io.StringIO()
 
         if self.after.entity_type != CoverageReport.EntityType.CATALOG:
             raise TypeError(
-                f"Unsupported report_type for summary method: "
-                f"{self.after.entity_type}"
+                f"Unsupported report_type for summary method: " f"{self.after.entity_type}"
             )
 
         buf.write(f"{'':10}{'before':>10}{'after':>10}{'+/-':>15}\n")
         buf.write("=" * 45 + "\n")
         buf.write(
             f"{'Coverage':10}{self.before.coverage:10.2%}{self.after.coverage:10.2%}"
             f"{(self.after.coverage - self.before.coverage):+15.2%}\n"
@@ -679,17 +630,15 @@
             if self.after.entity_type == CoverageReport.EntityType.CATALOG
             else self.after.entity_name
         )
         title = title_prefix + title
 
         before_covered = len(self.before.covered) if self.before is not None else "-"
         before_total = len(self.before.total) if self.before is not None else "-"
-        before_coverage = (
-            f"({self.before.coverage:.2%})" if self.before is not None else "(-)"
-        )
+        before_coverage = f"({self.before.coverage:.2%})" if self.before is not None else "(-)"
         after_covered = len(self.after.covered)
         after_total = len(self.after.total)
         after_coverage = f"({self.after.coverage:.2%})"
 
         buf = io.StringIO()
         buf.write(f"{title:50}")
         buf.write(f"{before_covered:>5}/{before_total:<5}{before_coverage:^9}")
@@ -708,15 +657,15 @@
             "https://github.com/slidoapp/dbt-coverage/tree/main#supported-dbt-versions for more "
             "details.",
             manifest_version,
             SUPPORTED_MANIFEST_SCHEMA_VERSIONS,
         )
 
 
-def load_catalog(project_dir: Path, run_artifacts_dir: Path) -> Catalog:
+def load_catalog(project_dir: Path, run_artifacts_dir: Path, manifest: Manifest) -> Catalog:
     if run_artifacts_dir is None:
         catalog_path = project_dir / "target/catalog.json"
     else:
         catalog_path = run_artifacts_dir / "catalog.json"
 
     if not catalog_path.exists():
         raise FileNotFoundError(
@@ -724,15 +673,15 @@
             "before using dbt-coverage, run: dbt docs generate"
         )
 
     with open(catalog_path) as f:
         catalog_json = json.load(f)
 
     catalog_nodes = {**catalog_json["sources"], **catalog_json["nodes"]}
-    catalog = Catalog.from_nodes(catalog_nodes.values())
+    catalog = Catalog.from_nodes(catalog_nodes.values(), manifest)
 
     logging.info("Successfully loaded %d tables from catalog", len(catalog.tables))
 
     return catalog
 
 
 def load_manifest(project_dir: Path, run_artifacts_dir: Path) -> Manifest:
@@ -757,47 +706,34 @@
     manifest = Manifest.from_nodes(manifest_nodes)
 
     return manifest
 
 
 def load_files(project_dir: Path, run_artifacts_dir: Path) -> Catalog:
     if run_artifacts_dir is None:
-        logging.info(
-            "Loading catalog and manifest files from project dir: %s", project_dir
-        )
+        logging.info("Loading catalog and manifest files from project dir: %s", project_dir)
     else:
-        logging.info(
-            "Loading catalog and manifest files from custom dir: %s", run_artifacts_dir
-        )
+        logging.info("Loading catalog and manifest files from custom dir: %s", run_artifacts_dir)
 
-    catalog = load_catalog(project_dir, run_artifacts_dir)
     manifest = load_manifest(project_dir, run_artifacts_dir)
+    catalog = load_catalog(project_dir, run_artifacts_dir, manifest)
 
-    for table_name in catalog.tables:
-        catalog_table = catalog.get_table(table_name)
-        catalog_table.update_original_file_path(manifest)
-        manifest_source_table = manifest.sources.get(table_name, {"columns": {}})
-        manifest_model_table = manifest.models.get(table_name, {"columns": {}})
-        manifest_seed_table = manifest.seeds.get(table_name, {"columns": {}})
-        manifest_snapshot_table = manifest.snapshots.get(table_name, {"columns": {}})
-        manifest_table_tests = manifest.tests.get(table_name, {})
+    for table_id in catalog.tables:
+        catalog_table = catalog.get_table(table_id)
+        manifest_source_table = manifest.sources.get(table_id, {"columns": {}})
+        manifest_model_table = manifest.models.get(table_id, {"columns": {}})
+        manifest_seed_table = manifest.seeds.get(table_id, {"columns": {}})
+        manifest_snapshot_table = manifest.snapshots.get(table_id, {"columns": {}})
+        manifest_table_tests = manifest.tests.get(table_id, {})
 
         for catalog_column in catalog_table.columns.values():
-            manifest_source_column = manifest_source_table["columns"].get(
-                catalog_column.name
-            )
-            manifest_model_column = manifest_model_table["columns"].get(
-                catalog_column.name
-            )
-            manifest_seed_column = manifest_seed_table["columns"].get(
-                catalog_column.name
-            )
-            manifest_snapshot_column = manifest_snapshot_table["columns"].get(
-                catalog_column.name
-            )
+            manifest_source_column = manifest_source_table["columns"].get(catalog_column.name)
+            manifest_model_column = manifest_model_table["columns"].get(catalog_column.name)
+            manifest_seed_column = manifest_seed_table["columns"].get(catalog_column.name)
+            manifest_snapshot_column = manifest_snapshot_table["columns"].get(catalog_column.name)
             manifest_column_tests = manifest_table_tests.get(catalog_column.name)
 
             manifest_column = (
                 manifest_source_column
                 or manifest_model_column
                 or manifest_seed_column
                 or manifest_snapshot_column
@@ -852,16 +788,15 @@
 def fail_compare(coverage_report: CoverageReport, compare_path: Path):
     compare_report = read_coverage_report(compare_path)
 
     diff = compare_reports(coverage_report, compare_report)
 
     if diff.after.coverage < diff.before.coverage:
         raise RuntimeError(
-            f"Coverage decreased from {diff.before.coverage:.2%} to "
-            f"{diff.after.coverage:.2%}"
+            f"Coverage decreased from {diff.before.coverage:.2%} to " f"{diff.after.coverage:.2%}"
         )
 
 
 def do_compute(
     project_dir: Path = Path("."),
     run_artifacts_dir: Path = None,
     cov_report: Path = Path("coverage.json"),
@@ -874,17 +809,21 @@
     """
     Computes coverage for a dbt project.
 
     Use this method in your Python code to bypass typer.
     """
 
     catalog = load_files(project_dir, run_artifacts_dir)
-
-    if len(model_path_filter) >= 1:
-        catalog = catalog.filter_catalog(model_path_filter)
+    if model_path_filter:
+        catalog = catalog.filter_tables(model_path_filter)
+        if not catalog.tables:
+            raise ValueError(
+                "After filtering, the Catalog contains no tables. Ensure your model_path_filter "
+                "is correct."
+            )
 
     coverage_report = compute_coverage(catalog, cov_type)
 
     if cov_format == CoverageFormat.MARKDOWN_TABLE:
         print(coverage_report.to_markdown_table())
     else:
         print(coverage_report.to_formatted_string())
@@ -915,37 +854,32 @@
     return diff
 
 
 @app.command()
 def compute(
     project_dir: Path = typer.Option(".", help="dbt project directory path."),
     run_artifacts_dir: Path = typer.Option(
-        None, help="custom directory path for " "catalog and manifest files"
-    ),
-    cov_report: Path = typer.Option(
-        "coverage.json", help="Output coverage report path."
+        None, help="Custom directory path for catalog and manifest files"
     ),
+    cov_report: Path = typer.Option("coverage.json", help="Output coverage report path."),
     cov_type: CoverageType = typer.Argument(..., help="Type of coverage to compute."),
     cov_fail_under: float = typer.Option(
-        None, help="Fail if coverage is lower than " "provided threshold."
+        None, help="Fail if coverage is lower than provided threshold."
     ),
     cov_fail_compare: Path = typer.Option(
         None,
-        help="Path to coverage report to compare "
-        "with and fail if current coverage "
-        "is lower. Normally used to prevent "
-        "coverage drop between subsequent "
-        "tests.",
+        help="Path to coverage report to compare with and fail if current coverage is lower. "
+        "Normally used to prevent coverage drop between subsequent tests.",
     ),
     model_path_filter: Optional[List[str]] = typer.Option(
-        None, help="The model_path " "string(s) to " "filter tables " "on."
+        None, help="The model_path string(s) to filter tables on."
     ),
     cov_format: CoverageFormat = typer.Option(
         CoverageFormat.STRING_TABLE,
-        help="The output format to print, either " "`string` or `markdown`",
+        help="The output format to print, either `string` or `markdown`",
     ),
 ):
     """Compute coverage for project in PROJECT_DIR from catalog.json and manifest.json."""
 
     return do_compute(
         project_dir,
         run_artifacts_dir,
@@ -967,17 +901,15 @@
 ):
     """Compare two coverage reports generated by the compute command."""
 
     return do_compare(report, compare_report)
 
 
 @app.callback()
-def main(
-    verbose: bool = typer.Option(False, help="Turn verbose logging messages on or off.")
-):
+def main(verbose: bool = typer.Option(False, help="Turn verbose logging messages on or off.")):
     if verbose:
         logging.basicConfig(level=logging.INFO)
     else:
         logging.basicConfig(level=logging.WARNING)
 
 
 if __name__ == "__main__":
```

### Comparing `dbt-coverage-0.3.2/pyproject.toml` & `dbt_coverage-0.3.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt-coverage"
-version = "0.3.2"
+version = "0.3.3"
 description = "One-stop-shop for docs and test coverage of dbt projects"
 authors = ["Andrej Švec <asvec@slido.com>"]
 readme = 'README.md'
 license = "MIT"
 repository = "https://github.com/slidoapp/dbt-coverage"
 homepage = "https://github.com/slidoapp/dbt-coverage"
 documentation = "https://github.com/slidoapp/dbt-coverage"
@@ -22,13 +22,19 @@
   "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.6"
 typer = "^0.4.0"
 
+[tool.poetry.group.dev.dependencies]
+black = { version = "*", python = ">=3.7" }
+
 [tool.poetry.scripts]
 dbt-coverage = 'dbt_coverage.__init__:app'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 99
```

### Comparing `dbt-coverage-0.3.2/setup.py` & `dbt_coverage-0.3.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,276 @@
-# -*- coding: utf-8 -*-
-from distutils.core import setup
+Metadata-Version: 2.1
+Name: dbt-coverage
+Version: 0.3.3
+Summary: One-stop-shop for docs and test coverage of dbt projects
+Home-page: https://github.com/slidoapp/dbt-coverage
+License: MIT
+Author: Andrej Švec
+Author-email: asvec@slido.com
+Requires-Python: >=3.6,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: typer (>=0.4.0,<0.5.0)
+Project-URL: Documentation, https://github.com/slidoapp/dbt-coverage
+Project-URL: Repository, https://github.com/slidoapp/dbt-coverage
+Description-Content-Type: text/markdown
 
-packages = \
-['dbt_coverage']
+# dbt-coverage
 
-package_data = \
-{'': ['*']}
+<a href="https://pypi.org/project/dbt-coverage/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dbt-coverage"></a>
+<a href="https://pepy.tech/project/dbt-coverage"><img alt="Downloads" src="https://pepy.tech/badge/dbt-coverage"></a>
+![GitHub last commit](https://img.shields.io/github/last-commit/slidoapp/dbt-coverage)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-coverage)
+![PyPI - Format](https://img.shields.io/pypi/format/dbt-coverage)
+![dbt versions](https://img.shields.io/badge/dbt-1.0-blue)
+<a href="https://github.com/slidoapp/dbt-coverage/blob/main/LICENSE.md"><img alt="License: MIT" src="https://img.shields.io/github/license/slidoapp/dbt-coverage"></a>
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield)
 
-install_requires = \
-['typer>=0.4.0,<0.5.0']
-
-entry_points = \
-{'console_scripts': ['dbt-coverage = dbt_coverage.__init__:app']}
-
-setup_kwargs = {
-    'name': 'dbt-coverage',
-    'version': '0.3.2',
-    'description': 'One-stop-shop for docs and test coverage of dbt projects',
-    'long_description': '# dbt-coverage\n\n<a href="https://pypi.org/project/dbt-coverage/"><img alt="PyPI" src="https://img.shields.io/pypi/v/dbt-coverage"></a>\n<a href="https://pepy.tech/project/dbt-coverage"><img alt="Downloads" src="https://pepy.tech/badge/dbt-coverage"></a>\n![GitHub last commit](https://img.shields.io/github/last-commit/slidoapp/dbt-coverage)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-coverage)\n![PyPI - Format](https://img.shields.io/pypi/format/dbt-coverage)\n![dbt versions](https://img.shields.io/badge/dbt-1.0-blue)\n<a href="https://github.com/slidoapp/dbt-coverage/blob/main/LICENSE.md"><img alt="License: MIT" src="https://img.shields.io/github/license/slidoapp/dbt-coverage"></a>\n[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield)\n\n\n_One-stop-shop for docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._\n\nOptimized for dbt 1.0, see [full support matrix](#supported-dbt-versions).\n\n## Why do I need something like this?\n\n_**[`dbt-coverage`](https://github.com/slidoapp/dbt-coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what [`coverage.py`](https://github.com/nedbat/coveragepy) and [`interrogate`](https://interrogate.readthedocs.io/en/latest/) are to Python.**_\n\nIt is a single CLI tool which checks your `dbt` project for missing documentation and tests.\n\nKeeping documentation and tests close to the actual SQL code that generates the final model is one of the best design choices of `dbt`. It ensures documentation is actually useful and tests are actually used. But how do you make adding those a habit in your [`dbt`](https://github.com/dbt-labs/dbt) project?\n\nThat is exactly where `dbt-coverage` comes in. It will\n\n- Give you a better sense of the level of documentation and test coverage in your project;\n- Help your CI/CD pipeline make sure new changes include documentation and tests;\n- Let you quickly assess the documentation and tests of a new `dbt` project you get your hands on.\n\nStill not convinced? Here are some more features:\n\n- ✨ **zero-config**: just install it and run it, there is nothing to set up\n- 🏁 **minimal dependences**: the only dependencies are [`click`](https://click.palletsprojects.com/en/8.0.x/) (already installed with [`dbt`](https://github.com/dbt-labs/dbt)) and [`typer`](https://typer.tiangolo.com/tutorial/)\n- 📦 **very small**: at ~480 [SLOC](https://en.wikipedia.org/wiki/Source_lines_of_code), you can easily validate it works as advertised\n\n\n## Demo\nThe package was presented during [Coalesce](https://coalesce.getdbt.com/),\nthe annual dbt conference, as a part of the talk\n[_From 100 spreadsheets to 100 data analysts: the story of dbt at Slido_](https://www.getdbt.com/coalesce-2021/from-spreadsheets-to-data-analysts-the-story-of-dbt-at-slido/).\nWatch a demo in the video below.\n\n[![Demo video](assets/demo.png)](https://youtu.be/YA0yqYSs9BQ?t=936)\n\n## Installation\n\n```\npip install dbt-coverage\n```\n\n## Usage\n\n`dbt-coverage` comes with two basic commands: `compute` and `compare`. The\ndocumentation for the individual commands can be shown by using the `--help`\noption.\n\n### Compute\n\nCompute coverage from `target/catalog.json` and `target/manifest.json` files\nfound in a dbt project, e.g.\n[jaffle_shop](https://github.com/dbt-labs/jaffle_shop). \n\nTo choose between documentation and test coverage, pass `doc` or `test` as the CLI argument.\n\n```console\n$ cd jaffle_shop\n$ dbt run  # Materialize models\n$ dbt docs generate  # Generate catalog.json and manifest.json\n$ dbt-coverage compute doc --cov-report coverage-doc.json  # Compute doc coverage, print it and write it to coverage-doc.json file\n\nCoverage report\n=====================================================================\njaffle_shop.customers                                  6/7      85.7%\njaffle_shop.orders                                     9/9     100.0%\njaffle_shop.raw_customers                              0/3       0.0%\njaffle_shop.raw_orders                                 0/4       0.0%\njaffle_shop.raw_payments                               0/4       0.0%\njaffle_shop.stg_customers                              0/3       0.0%\njaffle_shop.stg_orders                                 0/4       0.0%\njaffle_shop.stg_payments                               0/4       0.0%\n=====================================================================\nTotal                                                 15/38     39.5%\n\n$ dbt-coverage compute test --cov-report coverage-test.json  # Compute test coverage, print it and write it to coverage-test.json file\n\nCoverage report\n=====================================================================\njaffle_shop.customers                                  1/7      14.3%\njaffle_shop.orders                                     8/9      88.9%\njaffle_shop.raw_customers                              0/3       0.0%\njaffle_shop.raw_orders                                 0/4       0.0%\njaffle_shop.raw_payments                               0/4       0.0%\njaffle_shop.stg_customers                              1/3      33.3%\njaffle_shop.stg_orders                                 2/4      50.0%\njaffle_shop.stg_payments                               2/4      50.0%\n=====================================================================\nTotal                                                 14/38     36.8%\n```\n\n#### Filtering model paths with `--model-path-filter`\n\nYou can also choose a subset of tables to compare using one or multiple `--model-path-filter` options.\n\n```console\n$ cd jaffle_shop\n$ dbt run  # Materialize models\n$ dbt docs generate  # Generate catalog.json and manifest.json\n$ dbt-coverage compute doc --cov-report coverage-doc.json --model-path-filter models/staging/  # Compute doc coverage for a subset of tables, print it and write it to coverage-doc.json file\n\nCoverage report\n======================================================\njaffle_shop.stg_customers              0/3       0.0%\njaffle_shop.stg_orders                 0/4       0.0%\njaffle_shop.stg_payments               0/4       0.0%\n======================================================\nTotal                                  0/11      0.0%\n\n$ dbt-coverage compute doc --cov-report coverage-doc.json --model-path-filter models/orders.sql --model-path-filter models/staging/  # Compute doc coverage for a subset of tables, print it and write it to coverage-doc.json file\n\nCoverage report\n======================================================\njaffle_shop.orders                     0/9       0.0%\njaffle_shop.stg_customers              0/3       0.0%\njaffle_shop.stg_orders                 0/4       0.0%\njaffle_shop.stg_payments               0/4       0.0%\n======================================================\nTotal                                  0/20      0.0%\n```\n\n#### Markdown output with `--cov-format`\n\nYou can also choose to print the output in the Markdown table format by specifying the `--cov-format` option.\nThis can be especially useful when using `dbt-coverage` in CI/CD pipelines.\n\n```console\n$ cd jaffle_shop\n$ dbt run  # Materialize models\n$ dbt docs generate  # Generate catalog.json and manifest.json\n$ dbt-coverage compute doc --model-path-filter models/staging/ --cov-format markdown\n\n# Coverage report\n| Model | Columns Covered | % |\n|:------|----------------:|:-:|\n| jaffle_shop.stg_customers                         |     0/3     |   0.0% |\n| jaffle_shop.stg_orders                            |     0/4     |   0.0% |\n| jaffle_shop.stg_payments                          |     0/4     |   0.0% |\n| Total                                             |     0/11    |   0.0% |\n```\n\n#### Custom run artifacts path with `--run-artifacts-dir`\n\nTo compute the coverages, `dbt-coverage` looks up the artefacts from the `dbt run` execution in the\n`./target/` folder in the current directory. You can specify a custom path via the `--run-artifacts-dir`\noption.\n\n```console\n$ dbt-coverage compute doc --run-artifacts-dir jaffle_shop/target --cov-report coverage-doc.json  # Compute doc coverage from the artefacts located in jaffle_shop/target, print it and write it to coverage-doc.json file\n\nCoverage report\n================================================\njaffle_shop.customers             0/7       0.0%\njaffle_shop.orders                0/9       0.0%\njaffle_shop.raw_customers         0/3       0.0%\njaffle_shop.raw_orders            0/4       0.0%\njaffle_shop.raw_payments          0/4       0.0%\njaffle_shop.stg_customers         0/3       0.0%\njaffle_shop.stg_orders            0/4       0.0%\njaffle_shop.stg_payments          0/4       0.0%\n================================================\nTotal                             0/38      0.0%\n```\n\n### Compare\n\nCompare two `coverage.json` files generated by the `compute` command. This is\nuseful to ensure that the coverage does not drop while making changes to the\nproject.\n\n```console\n$ dbt-coverage compare coverage-after.json coverage-before.json\n\n# Coverage delta summary\n              before     after            +/-\n=============================================\nCoverage      39.47%    38.46%         -1.01%\n=============================================\nTables             8         8          +0/+0\nColumns           38        39          +1/+0\n=============================================\nHits              15        15          +0/+0\nMisses            23        24          +1/+0\n=============================================\n\n# New misses\n=========================================================================\nCatalog                         15/38   (39.47%)  ->    15/39   (38.46%) \n=========================================================================\n- jaffle_shop.customers          6/7    (85.71%)  ->     6/8    (75.00%) \n-- new_col                       -/-       (-)    ->     0/1     (0.00%) \n=========================================================================\n```\n\n### Combined use-case\n\n```console\n$ cd my-dbt-project\n\n$ dbt run  # Materialize models\n$ dbt docs generate  # Generate catalog.json and manifest.json\n$ dbt-coverage compute doc --cov-report before.json --cov-fail-under 0.5  # Fail if coverage is lower than 50%\n\n# Make changes to the dbt project, e.g. add some columns to the DWH, document some columns, etc.\n\n$ dbt run  # Materialize the changed models\n$ dbt docs generate  # Generate catalog.json and manifest.json\n$ dbt-coverage compute doc --cov-report after.json --cov-fail-compare before.json  # Fail if the current coverage is lower than coverage in before.json\n$ dbt-coverage compare after.json before.json  # Generate a detailed coverage delta report\n```\n\n## Supported `dbt` versions\n\nDifferent version of `dbt-coverage` support different versions of `dbt`. Here is\nthe support matrix.\n\n| `dbt`       | `dbt-coverage` |\n|-------------|----------------|\n| <0.20       | not tested     |\n| 0.20 - 0.21 | 0.1            |\n| 1.0 - 1.3   | 0.2, 0.3       |\n\n## Related packages\n\n- https://github.com/mikaelene/dbt-test-coverage\n- [interrogate](https://interrogate.readthedocs.io/en/latest/) (docs coverage for Python)\n- [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for Python)\n\n## License\n\nLicensed under the MIT license (see [LICENSE.md](LICENSE.md) file for more\ndetails).\n\n[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_large)\n',
-    'author': 'Andrej Švec',
-    'author_email': 'asvec@slido.com',
-    'url': 'https://github.com/slidoapp/dbt-coverage',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
 
+_One-stop-shop for docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._
+
+Optimized for dbt 1.0, see [full support matrix](#supported-dbt-versions).
+
+## Why do I need something like this?
+
+_**[`dbt-coverage`](https://github.com/slidoapp/dbt-coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what [`coverage.py`](https://github.com/nedbat/coveragepy) and [`interrogate`](https://interrogate.readthedocs.io/en/latest/) are to Python.**_
+
+It is a single CLI tool which checks your `dbt` project for missing documentation and tests.
+
+Keeping documentation and tests close to the actual SQL code that generates the final model is one of the best design choices of `dbt`. It ensures documentation is actually useful and tests are actually used. But how do you make adding those a habit in your [`dbt`](https://github.com/dbt-labs/dbt) project?
+
+That is exactly where `dbt-coverage` comes in. It will
+
+- Give you a better sense of the level of documentation and test coverage in your project;
+- Help your CI/CD pipeline make sure new changes include documentation and tests;
+- Let you quickly assess the documentation and tests of a new `dbt` project you get your hands on.
+
+Still not convinced? Here are some more features:
+
+- ✨ **zero-config**: just install it and run it, there is nothing to set up
+- 🏁 **minimal dependences**: the only dependencies are [`click`](https://click.palletsprojects.com/en/8.0.x/) (already installed with [`dbt`](https://github.com/dbt-labs/dbt)) and [`typer`](https://typer.tiangolo.com/tutorial/)
+- 📦 **very small**: at ~480 [SLOC](https://en.wikipedia.org/wiki/Source_lines_of_code), you can easily validate it works as advertised
+
+
+## Demo
+The package was presented during [Coalesce](https://coalesce.getdbt.com/),
+the annual dbt conference, as a part of the talk
+[_From 100 spreadsheets to 100 data analysts: the story of dbt at Slido_](https://www.getdbt.com/coalesce-2021/from-spreadsheets-to-data-analysts-the-story-of-dbt-at-slido/).
+Watch a demo in the video below.
+
+[![Demo video](assets/demo.png)](https://youtu.be/YA0yqYSs9BQ?t=936)
+
+## Installation
+
+```
+pip install dbt-coverage
+```
+
+## Usage
+
+`dbt-coverage` comes with two basic commands: `compute` and `compare`. The
+documentation for the individual commands can be shown by using the `--help`
+option.
+
+### Compute
+
+Compute coverage from `target/catalog.json` and `target/manifest.json` files
+found in a dbt project, e.g.
+[jaffle_shop](https://github.com/dbt-labs/jaffle_shop). 
+
+To choose between documentation and test coverage, pass `doc` or `test` as the CLI argument.
+
+```console
+$ cd jaffle_shop
+$ dbt run  # Materialize models
+$ dbt docs generate  # Generate catalog.json and manifest.json
+$ dbt-coverage compute doc --cov-report coverage-doc.json  # Compute doc coverage, print it and write it to coverage-doc.json file
+
+Coverage report
+=====================================================================
+jaffle_shop.customers                                  6/7      85.7%
+jaffle_shop.orders                                     9/9     100.0%
+jaffle_shop.raw_customers                              0/3       0.0%
+jaffle_shop.raw_orders                                 0/4       0.0%
+jaffle_shop.raw_payments                               0/4       0.0%
+jaffle_shop.stg_customers                              0/3       0.0%
+jaffle_shop.stg_orders                                 0/4       0.0%
+jaffle_shop.stg_payments                               0/4       0.0%
+=====================================================================
+Total                                                 15/38     39.5%
+
+$ dbt-coverage compute test --cov-report coverage-test.json  # Compute test coverage, print it and write it to coverage-test.json file
+
+Coverage report
+=====================================================================
+jaffle_shop.customers                                  1/7      14.3%
+jaffle_shop.orders                                     8/9      88.9%
+jaffle_shop.raw_customers                              0/3       0.0%
+jaffle_shop.raw_orders                                 0/4       0.0%
+jaffle_shop.raw_payments                               0/4       0.0%
+jaffle_shop.stg_customers                              1/3      33.3%
+jaffle_shop.stg_orders                                 2/4      50.0%
+jaffle_shop.stg_payments                               2/4      50.0%
+=====================================================================
+Total                                                 14/38     36.8%
+```
+
+#### Filtering model paths with `--model-path-filter`
+
+You can also choose a subset of tables to compare using one or multiple `--model-path-filter` options.
+
+```console
+$ cd jaffle_shop
+$ dbt run  # Materialize models
+$ dbt docs generate  # Generate catalog.json and manifest.json
+$ dbt-coverage compute doc --cov-report coverage-doc.json --model-path-filter models/staging/  # Compute doc coverage for a subset of tables, print it and write it to coverage-doc.json file
+
+Coverage report
+======================================================
+jaffle_shop.stg_customers              0/3       0.0%
+jaffle_shop.stg_orders                 0/4       0.0%
+jaffle_shop.stg_payments               0/4       0.0%
+======================================================
+Total                                  0/11      0.0%
+
+$ dbt-coverage compute doc --cov-report coverage-doc.json --model-path-filter models/orders.sql --model-path-filter models/staging/  # Compute doc coverage for a subset of tables, print it and write it to coverage-doc.json file
+
+Coverage report
+======================================================
+jaffle_shop.orders                     0/9       0.0%
+jaffle_shop.stg_customers              0/3       0.0%
+jaffle_shop.stg_orders                 0/4       0.0%
+jaffle_shop.stg_payments               0/4       0.0%
+======================================================
+Total                                  0/20      0.0%
+```
+
+#### Markdown output with `--cov-format`
+
+You can also choose to print the output in the Markdown table format by specifying the `--cov-format` option.
+This can be especially useful when using `dbt-coverage` in CI/CD pipelines.
+
+```console
+$ cd jaffle_shop
+$ dbt run  # Materialize models
+$ dbt docs generate  # Generate catalog.json and manifest.json
+$ dbt-coverage compute doc --model-path-filter models/staging/ --cov-format markdown
+
+# Coverage report
+| Model | Columns Covered | % |
+|:------|----------------:|:-:|
+| jaffle_shop.stg_customers                         |     0/3     |   0.0% |
+| jaffle_shop.stg_orders                            |     0/4     |   0.0% |
+| jaffle_shop.stg_payments                          |     0/4     |   0.0% |
+| Total                                             |     0/11    |   0.0% |
+```
+
+#### Custom run artifacts path with `--run-artifacts-dir`
+
+To compute the coverages, `dbt-coverage` looks up the artefacts from the `dbt run` execution in the
+`./target/` folder in the current directory. You can specify a custom path via the `--run-artifacts-dir`
+option.
+
+```console
+$ dbt-coverage compute doc --run-artifacts-dir jaffle_shop/target --cov-report coverage-doc.json  # Compute doc coverage from the artefacts located in jaffle_shop/target, print it and write it to coverage-doc.json file
+
+Coverage report
+================================================
+jaffle_shop.customers             0/7       0.0%
+jaffle_shop.orders                0/9       0.0%
+jaffle_shop.raw_customers         0/3       0.0%
+jaffle_shop.raw_orders            0/4       0.0%
+jaffle_shop.raw_payments          0/4       0.0%
+jaffle_shop.stg_customers         0/3       0.0%
+jaffle_shop.stg_orders            0/4       0.0%
+jaffle_shop.stg_payments          0/4       0.0%
+================================================
+Total                             0/38      0.0%
+```
+
+### Compare
+
+Compare two `coverage.json` files generated by the `compute` command. This is
+useful to ensure that the coverage does not drop while making changes to the
+project.
+
+```console
+$ dbt-coverage compare coverage-after.json coverage-before.json
+
+# Coverage delta summary
+              before     after            +/-
+=============================================
+Coverage      39.47%    38.46%         -1.01%
+=============================================
+Tables             8         8          +0/+0
+Columns           38        39          +1/+0
+=============================================
+Hits              15        15          +0/+0
+Misses            23        24          +1/+0
+=============================================
+
+# New misses
+=========================================================================
+Catalog                         15/38   (39.47%)  ->    15/39   (38.46%) 
+=========================================================================
+- jaffle_shop.customers          6/7    (85.71%)  ->     6/8    (75.00%) 
+-- new_col                       -/-       (-)    ->     0/1     (0.00%) 
+=========================================================================
+```
+
+### Combined use-case
+
+```console
+$ cd my-dbt-project
+
+$ dbt run  # Materialize models
+$ dbt docs generate  # Generate catalog.json and manifest.json
+$ dbt-coverage compute doc --cov-report before.json --cov-fail-under 0.5  # Fail if coverage is lower than 50%
+
+# Make changes to the dbt project, e.g. add some columns to the DWH, document some columns, etc.
+
+$ dbt run  # Materialize the changed models
+$ dbt docs generate  # Generate catalog.json and manifest.json
+$ dbt-coverage compute doc --cov-report after.json --cov-fail-compare before.json  # Fail if the current coverage is lower than coverage in before.json
+$ dbt-coverage compare after.json before.json  # Generate a detailed coverage delta report
+```
+
+## Supported `dbt` versions
+
+Different version of `dbt-coverage` support different versions of `dbt`. Here is
+the support matrix.
+
+| `dbt`       | `dbt-coverage` |
+|-------------|----------------|
+| <0.20       | not tested     |
+| 0.20 - 0.21 | 0.1            |
+| 1.0 - 1.3   | 0.2, 0.3       |
+
+## Related packages
+
+- https://github.com/mikaelene/dbt-test-coverage
+- [interrogate](https://interrogate.readthedocs.io/en/latest/) (docs coverage for Python)
+- [coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for Python)
+
+## License
+
+Licensed under the MIT license (see [LICENSE.md](LICENSE.md) file for more
+details).
+
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_large)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,150 +1,151 @@
-# -*- coding: utf-8 -*- from distutils.core import setup packages = \
-['dbt_coverage'] package_data = \ {'': ['*']} install_requires = \
-['typer>=0.4.0,<0.5.0'] entry_points = \ {'console_scripts': ['dbt-coverage =
-dbt_coverage.__init__:app']} setup_kwargs = { 'name': 'dbt-coverage',
-'version': '0.3.2', 'description': 'One-stop-shop for docs and test coverage of
-dbt projects', 'long_description': '# dbt-coverage\n\n[PyPI]\n[Downloads]\n!
-[GitHub last commit](https://img.shields.io/github/last-commit/slidoapp/dbt-
-coverage)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dbt-
-coverage)\n![PyPI - Format](https://img.shields.io/pypi/format/dbt-coverage)\n!
-[dbt versions](https://img.shields.io/badge/dbt-1.0-blue)\n[License:_MIT]\n[!
-[FOSSA Status](https://app.fossa.com/api/projects/
-git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=shield)](https://
-app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
-coverage?ref=badge_shield)\n\n\n_One-stop-shop for docs and test coverage of
-[`dbt`](https://github.com/dbt-labs/dbt) projects._\n\nOptimized for dbt 1.0,
-see [full support matrix](#supported-dbt-versions).\n\n## Why do I need
-something like this?\n\n_**[`dbt-coverage`](https://github.com/slidoapp/dbt-
-coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what [`coverage.py`]
-(https://github.com/nedbat/coveragepy) and [`interrogate`](https://
-interrogate.readthedocs.io/en/latest/) are to Python.**_\n\nIt is a single CLI
-tool which checks your `dbt` project for missing documentation and
-tests.\n\nKeeping documentation and tests close to the actual SQL code that
+Metadata-Version: 2.1 Name: dbt-coverage Version: 0.3.3 Summary: One-stop-shop
+for docs and test coverage of dbt projects Home-page: https://github.com/
+slidoapp/dbt-coverage License: MIT Author: Andrej Å vec Author-email:
+asvec@slido.com Requires-Python: >=3.6,<4.0 Classifier: Development Status :: 4
+- Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
+3.10 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: typer (>=0.4.0,<0.5.0) Project-URL:
+Documentation, https://github.com/slidoapp/dbt-coverage Project-URL:
+Repository, https://github.com/slidoapp/dbt-coverage Description-Content-Type:
+text/markdown # dbt-coverage [PyPI] [Downloads] ![GitHub last commit](https://
+img.shields.io/github/last-commit/slidoapp/dbt-coverage) ![PyPI - Python
+Version](https://img.shields.io/pypi/pyversions/dbt-coverage) ![PyPI - Format]
+(https://img.shields.io/pypi/format/dbt-coverage) ![dbt versions](https://
+img.shields.io/badge/dbt-1.0-blue) [License:_MIT] [![FOSSA Status](https://
+app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
+coverage.svg?type=shield)](https://app.fossa.com/projects/
+git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_shield) _One-stop-shop for
+docs and test coverage of [`dbt`](https://github.com/dbt-labs/dbt) projects._
+Optimized for dbt 1.0, see [full support matrix](#supported-dbt-versions). ##
+Why do I need something like this? _**[`dbt-coverage`](https://github.com/
+slidoapp/dbt-coverage) is to [`dbt`](https://github.com/dbt-labs/dbt) what
+[`coverage.py`](https://github.com/nedbat/coveragepy) and [`interrogate`]
+(https://interrogate.readthedocs.io/en/latest/) are to Python.**_ It is a
+single CLI tool which checks your `dbt` project for missing documentation and
+tests. Keeping documentation and tests close to the actual SQL code that
 generates the final model is one of the best design choices of `dbt`. It
 ensures documentation is actually useful and tests are actually used. But how
 do you make adding those a habit in your [`dbt`](https://github.com/dbt-labs/
-dbt) project?\n\nThat is exactly where `dbt-coverage` comes in. It will\n\n-
-Give you a better sense of the level of documentation and test coverage in your
-project;\n- Help your CI/CD pipeline make sure new changes include
-documentation and tests;\n- Let you quickly assess the documentation and tests
-of a new `dbt` project you get your hands on.\n\nStill not convinced? Here are
-some more features:\n\n- â¨ **zero-config**: just install it and run it, there
-is nothing to set up\n- ð **minimal dependences**: the only dependencies are
-[`click`](https://click.palletsprojects.com/en/8.0.x/) (already installed with
-[`dbt`](https://github.com/dbt-labs/dbt)) and [`typer`](https://
-typer.tiangolo.com/tutorial/)\n- ð¦ **very small**: at ~480 [SLOC](https://
-en.wikipedia.org/wiki/Source_lines_of_code), you can easily validate it works
-as advertised\n\n\n## Demo\nThe package was presented during [Coalesce](https:/
-/coalesce.getdbt.com/),\nthe annual dbt conference, as a part of the talk\n
-[_From 100 spreadsheets to 100 data analysts: the story of dbt at Slido_]
-(https://www.getdbt.com/coalesce-2021/from-spreadsheets-to-data-analysts-the-
-story-of-dbt-at-slido/).\nWatch a demo in the video below.\n\n[![Demo video]
-(assets/demo.png)](https://youtu.be/YA0yqYSs9BQ?t=936)\n\n##
-Installation\n\n```\npip install dbt-coverage\n```\n\n## Usage\n\n`dbt-
-coverage` comes with two basic commands: `compute` and `compare`.
-The\ndocumentation for the individual commands can be shown by using the `--
-help`\noption.\n\n### Compute\n\nCompute coverage from `target/catalog.json`
-and `target/manifest.json` files\nfound in a dbt project, e.g.\n[jaffle_shop]
-(https://github.com/dbt-labs/jaffle_shop). \n\nTo choose between documentation
-and test coverage, pass `doc` or `test` as the CLI argument.\n\n```console\n$
-cd jaffle_shop\n$ dbt run # Materialize models\n$ dbt docs generate # Generate
-catalog.json and manifest.json\n$ dbt-coverage compute doc --cov-report
-coverage-doc.json # Compute doc coverage, print it and write it to coverage-
-doc.json file\n\nCoverage
-report\n=====================================================================\njaffle_shop.customers
-6/7 85.7%\njaffle_shop.orders 9/9 100.0%\njaffle_shop.raw_customers 0/
-3 0.0%\njaffle_shop.raw_orders 0/4 0.0%\njaffle_shop.raw_payments 0/
-4 0.0%\njaffle_shop.stg_customers 0/3 0.0%\njaffle_shop.stg_orders 0/
-4 0.0%\njaffle_shop.stg_payments 0/
-4
-0.0%\n=====================================================================\nTotal
-15/38 39.5%\n\n$ dbt-coverage compute test --cov-report coverage-test.json #
-Compute test coverage, print it and write it to coverage-test.json
-file\n\nCoverage
-report\n=====================================================================\njaffle_shop.customers
-1/7 14.3%\njaffle_shop.orders 8/9 88.9%\njaffle_shop.raw_customers 0/
-3 0.0%\njaffle_shop.raw_orders 0/4 0.0%\njaffle_shop.raw_payments 0/
-4 0.0%\njaffle_shop.stg_customers 1/3 33.3%\njaffle_shop.stg_orders 2/
-4 50.0%\njaffle_shop.stg_payments 2/
-4
-50.0%\n=====================================================================\nTotal
-14/38 36.8%\n```\n\n#### Filtering model paths with `--model-path-
-filter`\n\nYou can also choose a subset of tables to compare using one or
-multiple `--model-path-filter` options.\n\n```console\n$ cd jaffle_shop\n$ dbt
-run # Materialize models\n$ dbt docs generate # Generate catalog.json and
-manifest.json\n$ dbt-coverage compute doc --cov-report coverage-doc.json --
-model-path-filter models/staging/ # Compute doc coverage for a subset of
-tables, print it and write it to coverage-doc.json file\n\nCoverage
-report\n======================================================\njaffle_shop.stg_customers
-0/3 0.0%\njaffle_shop.stg_orders 0/4 0.0%\njaffle_shop.stg_payments 0/
-4 0.0%\n======================================================\nTotal 0/11
-0.0%\n\n$ dbt-coverage compute doc --cov-report coverage-doc.json --model-path-
-filter models/orders.sql --model-path-filter models/staging/ # Compute doc
-coverage for a subset of tables, print it and write it to coverage-doc.json
-file\n\nCoverage
-report\n======================================================\njaffle_shop.orders
-0/9 0.0%\njaffle_shop.stg_customers 0/3 0.0%\njaffle_shop.stg_orders 0/
-4 0.0%\njaffle_shop.stg_payments 0/
-4 0.0%\n======================================================\nTotal 0/20
-0.0%\n```\n\n#### Markdown output with `--cov-format`\n\nYou can also choose to
-print the output in the Markdown table format by specifying the `--cov-format`
-option.\nThis can be especially useful when using `dbt-coverage` in CI/CD
-pipelines.\n\n```console\n$ cd jaffle_shop\n$ dbt run # Materialize models\n$
-dbt docs generate # Generate catalog.json and manifest.json\n$ dbt-coverage
-compute doc --model-path-filter models/staging/ --cov-format markdown\n\n#
-Coverage report\n| Model | Columns Covered | % |\n|:------|----------------:|:
--:|\n| jaffle_shop.stg_customers | 0/3 | 0.0% |\n| jaffle_shop.stg_orders | 0/
-4 | 0.0% |\n| jaffle_shop.stg_payments | 0/4 | 0.0% |\n| Total | 0/11 | 0.0%
-|\n```\n\n#### Custom run artifacts path with `--run-artifacts-dir`\n\nTo
-compute the coverages, `dbt-coverage` looks up the artefacts from the `dbt run`
-execution in the\n`./target/` folder in the current directory. You can specify
-a custom path via the `--run-artifacts-dir`\noption.\n\n```console\n$ dbt-
-coverage compute doc --run-artifacts-dir jaffle_shop/target --cov-report
-coverage-doc.json # Compute doc coverage from the artefacts located in
-jaffle_shop/target, print it and write it to coverage-doc.json file\n\nCoverage
-report\n================================================\njaffle_shop.customers
-0/7 0.0%\njaffle_shop.orders 0/9 0.0%\njaffle_shop.raw_customers 0/
-3 0.0%\njaffle_shop.raw_orders 0/4 0.0%\njaffle_shop.raw_payments 0/
-4 0.0%\njaffle_shop.stg_customers 0/3 0.0%\njaffle_shop.stg_orders 0/
-4 0.0%\njaffle_shop.stg_payments 0/
-4 0.0%\n================================================\nTotal 0/38
-0.0%\n```\n\n### Compare\n\nCompare two `coverage.json` files generated by the
-`compute` command. This is\nuseful to ensure that the coverage does not drop
-while making changes to the\nproject.\n\n```console\n$ dbt-coverage compare
-coverage-after.json coverage-before.json\n\n# Coverage delta summary\n before
-after +/-\n=============================================\nCoverage 39.47%
-38.46% -1.01%\n=============================================\nTables 8 8 +0/
-+0\nColumns 38 39 +1/+0\n=============================================\nHits 15
-15 +0/+0\nMisses 23 24 +1/
-+0\n=============================================\n\n# New
-misses\n=========================================================================\nCatalog
-15/38 (39.47%) -> 15/39 (38.46%)
-\n=========================================================================\n-
-jaffle_shop.customers 6/7 (85.71%) -> 6/8 (75.00%) \n-- new_col -/- (-) -> 0/1
+dbt) project? That is exactly where `dbt-coverage` comes in. It will - Give you
+a better sense of the level of documentation and test coverage in your project;
+- Help your CI/CD pipeline make sure new changes include documentation and
+tests; - Let you quickly assess the documentation and tests of a new `dbt`
+project you get your hands on. Still not convinced? Here are some more
+features: - â¨ **zero-config**: just install it and run it, there is nothing
+to set up - ð **minimal dependences**: the only dependencies are [`click`]
+(https://click.palletsprojects.com/en/8.0.x/) (already installed with [`dbt`]
+(https://github.com/dbt-labs/dbt)) and [`typer`](https://typer.tiangolo.com/
+tutorial/) - ð¦ **very small**: at ~480 [SLOC](https://en.wikipedia.org/wiki/
+Source_lines_of_code), you can easily validate it works as advertised ## Demo
+The package was presented during [Coalesce](https://coalesce.getdbt.com/), the
+annual dbt conference, as a part of the talk [_From 100 spreadsheets to 100
+data analysts: the story of dbt at Slido_](https://www.getdbt.com/coalesce-
+2021/from-spreadsheets-to-data-analysts-the-story-of-dbt-at-slido/). Watch a
+demo in the video below. [![Demo video](assets/demo.png)](https://youtu.be/
+YA0yqYSs9BQ?t=936) ## Installation ``` pip install dbt-coverage ``` ## Usage
+`dbt-coverage` comes with two basic commands: `compute` and `compare`. The
+documentation for the individual commands can be shown by using the `--help`
+option. ### Compute Compute coverage from `target/catalog.json` and `target/
+manifest.json` files found in a dbt project, e.g. [jaffle_shop](https://
+github.com/dbt-labs/jaffle_shop). To choose between documentation and test
+coverage, pass `doc` or `test` as the CLI argument. ```console $ cd jaffle_shop
+$ dbt run # Materialize models $ dbt docs generate # Generate catalog.json and
+manifest.json $ dbt-coverage compute doc --cov-report coverage-doc.json #
+Compute doc coverage, print it and write it to coverage-doc.json file Coverage
+report =====================================================================
+jaffle_shop.customers 6/7 85.7% jaffle_shop.orders 9/9 100.0%
+jaffle_shop.raw_customers 0/3 0.0% jaffle_shop.raw_orders 0/4 0.0%
+jaffle_shop.raw_payments 0/4 0.0% jaffle_shop.stg_customers 0/3 0.0%
+jaffle_shop.stg_orders 0/4 0.0% jaffle_shop.stg_payments 0/4 0.0%
+===================================================================== Total 15/
+38 39.5% $ dbt-coverage compute test --cov-report coverage-test.json # Compute
+test coverage, print it and write it to coverage-test.json file Coverage report
+=====================================================================
+jaffle_shop.customers 1/7 14.3% jaffle_shop.orders 8/9 88.9%
+jaffle_shop.raw_customers 0/3 0.0% jaffle_shop.raw_orders 0/4 0.0%
+jaffle_shop.raw_payments 0/4 0.0% jaffle_shop.stg_customers 1/3 33.3%
+jaffle_shop.stg_orders 2/4 50.0% jaffle_shop.stg_payments 2/4 50.0%
+===================================================================== Total 14/
+38 36.8% ``` #### Filtering model paths with `--model-path-filter` You can also
+choose a subset of tables to compare using one or multiple `--model-path-
+filter` options. ```console $ cd jaffle_shop $ dbt run # Materialize models $
+dbt docs generate # Generate catalog.json and manifest.json $ dbt-coverage
+compute doc --cov-report coverage-doc.json --model-path-filter models/staging/
+# Compute doc coverage for a subset of tables, print it and write it to
+coverage-doc.json file Coverage report
+======================================================
+jaffle_shop.stg_customers 0/3 0.0% jaffle_shop.stg_orders 0/4 0.0%
+jaffle_shop.stg_payments 0/4 0.0%
+====================================================== Total 0/11 0.0% $ dbt-
+coverage compute doc --cov-report coverage-doc.json --model-path-filter models/
+orders.sql --model-path-filter models/staging/ # Compute doc coverage for a
+subset of tables, print it and write it to coverage-doc.json file Coverage
+report ======================================================
+jaffle_shop.orders 0/9 0.0% jaffle_shop.stg_customers 0/3 0.0%
+jaffle_shop.stg_orders 0/4 0.0% jaffle_shop.stg_payments 0/4 0.0%
+====================================================== Total 0/20 0.0% ``` ####
+Markdown output with `--cov-format` You can also choose to print the output in
+the Markdown table format by specifying the `--cov-format` option. This can be
+especially useful when using `dbt-coverage` in CI/CD pipelines. ```console $ cd
+jaffle_shop $ dbt run # Materialize models $ dbt docs generate # Generate
+catalog.json and manifest.json $ dbt-coverage compute doc --model-path-filter
+models/staging/ --cov-format markdown # Coverage report | Model | Columns
+Covered | % | |:------|----------------:|:-:| | jaffle_shop.stg_customers | 0/
+3 | 0.0% | | jaffle_shop.stg_orders | 0/4 | 0.0% | | jaffle_shop.stg_payments |
+0/4 | 0.0% | | Total | 0/11 | 0.0% | ``` #### Custom run artifacts path with `-
+-run-artifacts-dir` To compute the coverages, `dbt-coverage` looks up the
+artefacts from the `dbt run` execution in the `./target/` folder in the current
+directory. You can specify a custom path via the `--run-artifacts-dir` option.
+```console $ dbt-coverage compute doc --run-artifacts-dir jaffle_shop/target --
+cov-report coverage-doc.json # Compute doc coverage from the artefacts located
+in jaffle_shop/target, print it and write it to coverage-doc.json file Coverage
+report ================================================ jaffle_shop.customers
+0/7 0.0% jaffle_shop.orders 0/9 0.0% jaffle_shop.raw_customers 0/3 0.0%
+jaffle_shop.raw_orders 0/4 0.0% jaffle_shop.raw_payments 0/4 0.0%
+jaffle_shop.stg_customers 0/3 0.0% jaffle_shop.stg_orders 0/4 0.0%
+jaffle_shop.stg_payments 0/4 0.0%
+================================================ Total 0/38 0.0% ``` ###
+Compare Compare two `coverage.json` files generated by the `compute` command.
+This is useful to ensure that the coverage does not drop while making changes
+to the project. ```console $ dbt-coverage compare coverage-after.json coverage-
+before.json # Coverage delta summary before after +/
+- ============================================= Coverage 39.47% 38.46% -1.01%
+============================================= Tables 8 8 +0/+0 Columns 38 39
++1/+0 ============================================= Hits 15 15 +0/+0 Misses 23
+24 +1/+0 ============================================= # New misses
+=========================================================================
+Catalog 15/38 (39.47%) -> 15/39 (38.46%)
+========================================================================= -
+jaffle_shop.customers 6/7 (85.71%) -> 6/8 (75.00%) -- new_col -/- (-) -> 0/1
 (0.00%)
-\n=========================================================================\n```\n\n###
-Combined use-case\n\n```console\n$ cd my-dbt-project\n\n$ dbt run # Materialize
-models\n$ dbt docs generate # Generate catalog.json and manifest.json\n$ dbt-
+========================================================================= ```
+### Combined use-case ```console $ cd my-dbt-project $ dbt run # Materialize
+models $ dbt docs generate # Generate catalog.json and manifest.json $ dbt-
 coverage compute doc --cov-report before.json --cov-fail-under 0.5 # Fail if
-coverage is lower than 50%\n\n# Make changes to the dbt project, e.g. add some
-columns to the DWH, document some columns, etc.\n\n$ dbt run # Materialize the
-changed models\n$ dbt docs generate # Generate catalog.json and
-manifest.json\n$ dbt-coverage compute doc --cov-report after.json --cov-fail-
-compare before.json # Fail if the current coverage is lower than coverage in
-before.json\n$ dbt-coverage compare after.json before.json # Generate a
-detailed coverage delta report\n```\n\n## Supported `dbt` versions\n\nDifferent
-version of `dbt-coverage` support different versions of `dbt`. Here is\nthe
-support matrix.\n\n| `dbt` | `dbt-coverage` |\n|-------------|----------------
-|\n| <0.20 | not tested |\n| 0.20 - 0.21 | 0.1 |\n| 1.0 - 1.3 | 0.2, 0.3
-|\n\n## Related packages\n\n- https://github.com/mikaelene/dbt-test-coverage\n-
-[interrogate](https://interrogate.readthedocs.io/en/latest/) (docs coverage for
-Python)\n- [coverage.py](https://github.com/nedbat/coveragepy) (execution
-coverage for Python)\n\n## License\n\nLicensed under the MIT license (see
-[LICENSE.md](LICENSE.md) file for more\ndetails).\n\n[![FOSSA Status](https://
-app.fossa.com/api/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
-coverage.svg?type=large)](https://app.fossa.com/projects/
-git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage?ref=badge_large)\n', 'author':
-'Andrej Å vec', 'author_email': 'asvec@slido.com', 'url': 'https://github.com/
-slidoapp/dbt-coverage', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.6,<4.0', } setup(**setup_kwargs)
+coverage is lower than 50% # Make changes to the dbt project, e.g. add some
+columns to the DWH, document some columns, etc. $ dbt run # Materialize the
+changed models $ dbt docs generate # Generate catalog.json and manifest.json $
+dbt-coverage compute doc --cov-report after.json --cov-fail-compare before.json
+# Fail if the current coverage is lower than coverage in before.json $ dbt-
+coverage compare after.json before.json # Generate a detailed coverage delta
+report ``` ## Supported `dbt` versions Different version of `dbt-coverage`
+support different versions of `dbt`. Here is the support matrix. | `dbt` |
+`dbt-coverage` | |-------------|----------------| | <0.20 | not tested | | 0.20
+- 0.21 | 0.1 | | 1.0 - 1.3 | 0.2, 0.3 | ## Related packages - https://
+github.com/mikaelene/dbt-test-coverage - [interrogate](https://
+interrogate.readthedocs.io/en/latest/) (docs coverage for Python) -
+[coverage.py](https://github.com/nedbat/coveragepy) (execution coverage for
+Python) ## License Licensed under the MIT license (see [LICENSE.md](LICENSE.md)
+file for more details). [![FOSSA Status](https://app.fossa.com/api/projects/
+git%2Bgithub.com%2Fslidoapp%2Fdbt-coverage.svg?type=large)](https://
+app.fossa.com/projects/git%2Bgithub.com%2Fslidoapp%2Fdbt-
+coverage?ref=badge_large)
```

