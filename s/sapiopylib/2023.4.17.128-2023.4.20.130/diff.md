# Comparing `tmp/sapiopylib-2023.4.17.128.tar.gz` & `tmp/sapiopylib-2023.4.20.130.tar.gz`

## Comparing `sapiopylib-2023.4.17.128.tar` & `sapiopylib-2023.4.20.130.tar`

### file list

```diff
@@ -1,84 +1,92 @@
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/INSTALL.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/sapio_input_config.py
--rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/sapio_input_data.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/sapio_native_tools.py
--rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/AccessionService.py
--rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/CustomReportService.py
--rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/DashboardManager.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataMgmtService.py
--rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataRecordManagerService.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataTypeService.py
--rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/ELNService.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/PicklistService.py
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/User.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/WebhookService.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/__init__.py
--rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/CustomReport.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecord.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordPaging.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DateRange.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/Picklist.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/SapioAccessType.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/Sort.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/TableColumn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/__init__.py
--rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/ChartData.py
--rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
--rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/__init__.py
--rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataType.py
--rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
--rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
--rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/__init__.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
--rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
--rw-r--r--   0        0        0    21404 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/__init__.py
--rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
--rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
--rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/DataRecordUtil.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/DataTypeCacheManager.py
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/FormBuilder.py
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/FoundationAccessioning.py
--rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/MultiMap.py
--rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/ProtocolUtils.py
--rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/Protocols.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/SapioDateUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/__init__.py
--rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
--rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
--rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/PlatingUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/__init__.py
--rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
--rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
--rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
--rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
--rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/tests/__init__.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/.gitignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/LICENSE
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/README.md
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/pyproject.toml
--rw-r--r--   0        0        0     5878 2020-02-02 00:00:00.000000 sapiopylib-2023.4.17.128/PKG-INFO
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/INSTALL.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_config.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_data.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/sapio_native_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/__init__.py
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/PyCspFieldMap.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/__init__.py
+-rw-r--r--   0        0        0    36589 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspData.py
+-rw-r--r--   0        0        0     9592 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/PlotlyCspEnums.py
+-rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/SapioPyPlotly.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/csp/data/plotly/__init__.py
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/jarvis/JarvisDashboardWebhookContext.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/AccessionService.py
+-rw-r--r--   0        0        0     9903 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/CustomReportService.py
+-rw-r--r--   0        0        0     2677 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DashboardManager.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataMgmtService.py
+-rw-r--r--   0        0        0    41157 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataRecordManagerService.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataTypeService.py
+-rw-r--r--   0        0        0    17191 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/ELNService.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/PicklistService.py
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/User.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/WebhookService.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/__init__.py
+-rw-r--r--   0        0        0    17982 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/CustomReport.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecord.py
+-rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py
+-rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordPaging.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DateRange.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Picklist.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/SapioAccessType.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Sort.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/TableColumn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/__init__.py
+-rw-r--r--   0        0        0    12264 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/ChartData.py
+-rw-r--r--   0        0        0    25151 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py
+-rw-r--r--   0        0        0    18867 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/__init__.py
+-rw-r--r--   0        0        0     7511 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataType.py
+-rw-r--r--   0        0        0    57676 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py
+-rw-r--r--   0        0        0    55185 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/__init__.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperiment.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py
+-rw-r--r--   0        0        0    24595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py
+-rw-r--r--   0        0        0    21409 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/__init__.py
+-rw-r--r--   0        0        0    14259 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py
+-rw-r--r--   0        0        0    10905 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/__init__.py
+-rw-r--r--   0        0        0    13336 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/VeloxRules.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookContext.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookResult.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/__init__.py
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataRecordUtil.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataTypeCacheManager.py
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FormBuilder.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FoundationAccessioning.py
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/MultiMap.py
+-rw-r--r--   0        0        0    14844 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/ProtocolUtils.py
+-rw-r--r--   0        0        0    16327 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/Protocols.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/SapioDateUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/__init__.py
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py
+-rw-r--r--   0        0        0    23324 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/PlatingUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/__init__.py
+-rw-r--r--   0        0        0    25528 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py
+-rw-r--r--   0        0        0    45312 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py
+-rw-r--r--   0        0        0     2493 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py
+-rw-r--r--   0        0        0    11950 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/tests/__init__.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/LICENSE
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/README.md
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/pyproject.toml
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 sapiopylib-2023.4.20.130/PKG-INFO
```

### Comparing `sapiopylib-2023.4.17.128/INSTALL.md` & `sapiopylib-2023.4.20.130/INSTALL.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/sapio_input_data.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/sapio_input_data.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/sapio_native_tools.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/sapio_native_tools.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/AccessionService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/AccessionService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/CustomReportService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/CustomReportService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/DashboardManager.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DashboardManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataMgmtService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataMgmtService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataRecordManagerService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataRecordManagerService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/DataTypeService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/DataTypeService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/ELNService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/ELNService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/PicklistService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/PicklistService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/User.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/User.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/WebhookService.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/WebhookService.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/CustomReport.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/CustomReport.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecord.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecord.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordBatchUpdate.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordPaging.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DataRecordSideLinkPaging.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/DateRange.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/DateRange.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/Picklist.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Picklist.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/Sort.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/Sort.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/TableColumn.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/TableColumn.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/ChartData.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/ChartData.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/chartdata/DashboardSeries.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataType.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeComponent.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeDescriptors.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/DataTypeLayout.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/FieldDefinition.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/datatype/TemporaryDataType.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ElnExperiment.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperiment.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ElnExperimentRole.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntry.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/ExperimentEntryCriteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         if self.entry_name is not None:
             ret['experimentEntryName'] = self.entry_name
         if self.dependency_set is not None:
             ret['dependencySet'] = self.dependency_set
         if self.related_entry_set is not None:
             ret['relatedEntrySet'] = self.related_entry_set
         if self.entry_status is not None:
-            ret['entryStatus'] = self.entry_status
+            ret['entryStatus'] = self.entry_status.name
         if self.order is not None:
             ret['order'] = self.order
         if self.description is not None:
             ret['description'] = self.description
         if self.requires_grabber_plugin is not None:
             ret['requiresGrabberPlugin'] = self.requires_grabber_plugin
         if self.is_initialization_required is not None:
```

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/eln/SapioELNEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/ReportBuilderEntryContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/reportbuilder/VeloxReportBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackRequest.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/ClientCallbackResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/VeloxRules.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/VeloxRules.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookContext.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookContext.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookDirective.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookEnums.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/pojo/webhook/WebhookResult.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/pojo/webhook/WebhookResult.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/DataRecordUtil.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataRecordUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/DataTypeCacheManager.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/DataTypeCacheManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/FormBuilder.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FormBuilder.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/FoundationAccessioning.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/FoundationAccessioning.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/MultiMap.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/MultiMap.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/ProtocolUtils.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/ProtocolUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/Protocols.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/Protocols.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/SapioDateUtils.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/SapioDateUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlating.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/MultiLayerPlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/plates/PlatingUtils.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/plates/PlatingUtils.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/PyRecordModel.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEventBus.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelEvents.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelManager.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelUtil.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RecordModelWrapper.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py` & `sapiopylib-2023.4.20.130/src/sapiopylib/rest/utils/recordmodel/RelationshipPath.py`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/LICENSE` & `sapiopylib-2023.4.20.130/LICENSE`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/README.md` & `sapiopylib-2023.4.20.130/README.md`

 * *Files identical despite different names*

### Comparing `sapiopylib-2023.4.17.128/pyproject.toml` & `sapiopylib-2023.4.20.130/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sapiopylib"
-version='2023.04.17.128'
+version='2023.04.20.130'
 authors = [
     { name="Yechen Qiao", email="yqiao@sapiosciences.com" },
 ]
 description = "Official Sapio Informatics Platform Python API"
 license = "MPL-2.0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    'requests>=2.28.1', 'pandas>=1.3.0', 'flask>=2.2.0', 'buslane>=0.0.5'
+    'requests>=2.28.1', 'pandas>=1.3.0', 'flask>=2.2.0', 'buslane>=0.0.5', 'plotly>=5.14.0', 'kaleido>=0.2.0'
 ]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: Healthcare Industry",
     "Programming Language :: Python :: 3.7",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Software Development :: Libraries :: Python Modules",
-    'Development Status :: 5 - Production/Stable',
+    'Development Status :: 4 - Beta',
 ]
 homepage = "https://www.sapiosciences.com/"
 keywords = ["lims", "eln", "rest", "sapio"]
 
 [project.urls]
 "Homepage" = "https://github.com/sapiosciences"
 "Bug Tracker" = "https://github.com/sapiosciences/sapio-py-tutorials/issues"
```

### Comparing `sapiopylib-2023.4.17.128/PKG-INFO` & `sapiopylib-2023.4.20.130/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: sapiopylib
-Version: 2023.4.17.128
+Version: 2023.4.20.130
 Summary: Official Sapio Informatics Platform Python API
 Project-URL: Homepage, https://github.com/sapiosciences
 Project-URL: Bug Tracker, https://github.com/sapiosciences/sapio-py-tutorials/issues
 Author-email: Yechen Qiao <yqiao@sapiosciences.com>
 License-Expression: MPL-2.0
 License-File: LICENSE
 Keywords: eln,lims,rest,sapio
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Requires-Dist: buslane>=0.0.5
 Requires-Dist: flask>=2.2.0
+Requires-Dist: kaleido>=0.2.0
 Requires-Dist: pandas>=1.3.0
+Requires-Dist: plotly>=5.14.0
 Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 
 # sapiopylib: Official Sapio Informatics Platform Python API
 
 <div align="center">
```

