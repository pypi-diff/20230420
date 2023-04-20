# Comparing `tmp/BioSeqTools-0.2.0.tar.gz` & `tmp/BioSeqTools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BioSeqTools-0.2.0.tar", last modified: Mon Jul 18 08:22:43 2022, max compression
+gzip compressed data, was "BioSeqTools-0.3.0.tar", last modified: Thu Apr 20 02:21:27 2023, max compression
```

## Comparing `BioSeqTools-0.2.0.tar` & `BioSeqTools-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1808 2022-07-18 08:14:22.000000 BioSeqTools-0.2.0/.gitignore
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      419 2022-07-18 08:22:42.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      341 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/SOURCES.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2022-07-18 08:22:42.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/dependency_links.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       53 2022-07-18 08:22:42.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/entry_points.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2022-07-18 08:22:42.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/requires.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       12 2022-07-18 08:22:42.000000 BioSeqTools-0.2.0/BioSeqTools.egg-info/top_level.txt
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2022-07-18 08:14:22.000000 BioSeqTools-0.2.0/LICENSE
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      419 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/PKG-INFO
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      111 2022-07-18 08:20:29.000000 BioSeqTools-0.2.0/README.md
-drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/bioseqtools/
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2022-07-18 08:14:22.000000 BioSeqTools-0.2.0/bioseqtools/__init__.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    19668 2022-07-18 08:16:44.000000 BioSeqTools-0.2.0/bioseqtools/cli.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    47371 2022-07-18 08:14:22.000000 BioSeqTools-0.2.0/bioseqtools/pipelines.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      300 2022-07-18 08:17:29.000000 BioSeqTools-0.2.0/bioseqtools/versions.py
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2022-07-18 08:22:43.000000 BioSeqTools-0.2.0/setup.cfg
--rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      801 2022-07-18 08:16:29.000000 BioSeqTools-0.2.0/setup.py
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      455 2023-04-20 02:21:26.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      330 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        1 2023-04-20 02:21:26.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       53 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/entry_points.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       66 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/requires.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       12 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/BioSeqTools.egg-info/top_level.txt
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)     1066 2022-07-18 08:14:22.000000 BioSeqTools-0.3.0/LICENSE
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      455 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/PKG-INFO
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      111 2022-07-18 08:20:29.000000 BioSeqTools-0.3.0/README.md
+drwxrwxr-x   0 xuyuxing  (1003) xuyuxing  (1003)        0 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/bioseqtools/
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)        0 2022-07-18 08:14:22.000000 BioSeqTools-0.3.0/bioseqtools/__init__.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    19668 2022-07-18 08:16:44.000000 BioSeqTools-0.3.0/bioseqtools/cli.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)    45793 2023-01-27 13:30:33.000000 BioSeqTools-0.3.0/bioseqtools/pipelines.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      415 2023-01-27 13:31:21.000000 BioSeqTools-0.3.0/bioseqtools/versions.py
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)       38 2023-04-20 02:21:27.000000 BioSeqTools-0.3.0/setup.cfg
+-rw-rw-r--   0 xuyuxing  (1003) xuyuxing  (1003)      801 2022-07-18 08:16:29.000000 BioSeqTools-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `BioSeqTools-0.2.0/LICENSE` & `BioSeqTools-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BioSeqTools-0.2.0/bioseqtools/cli.py` & `BioSeqTools-0.3.0/bioseqtools/cli.py`

 * *Files identical despite different names*

### Comparing `BioSeqTools-0.2.0/bioseqtools/pipelines.py` & `BioSeqTools-0.3.0/bioseqtools/pipelines.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,27 +172,14 @@
             F1.write(">%s\n%s" % (record.seqname_short(), record.seq))
         else:
             print(">%s\n%s" % (record.seqname_short(), record.seq))
     if output_file is not None:
         F1.close()
 
 
-def extract_longest_isofrom_from_gene_in_trinity(trinity_output):
-    longest_dict = {}
-    for record in sb.read_fasta_big(trinity_output):
-        cluster_id, gene_id, isoform_id = re.match(r'^(\S+c\d+)_(g\d+)_(i\d+)$',
-                                                   record.seqname_short()).groups()
-        gene_name = cluster_id + "_" + gene_id
-        if not gene_name in longest_dict:
-            longest_dict[gene_name] = record
-        elif len(longest_dict[gene_name].seq) < len(record.seq):
-            longest_dict[gene_name] = record
-    return longest_dict
-
-
 def split_fasta(input_file, output_dir, outpre, contig_model=False, unit_num=None, file_size=None):
     mkdir(output_dir, True)
 
     record_dict = sb.read_fasta_by_faidx(input_file)
     if contig_model:
         for i in record_dict:
             record_tmp = record_dict[i]
@@ -209,15 +196,16 @@
             num_used = num_used + 1
             F1.write(">%s\n%s\n" % (record.seqname, record.seq))
             all_used += 1
             if num_used >= unit_num:
                 F1.close()
                 file_num = file_num + 1
                 if all_used < len(record_dict):
-                    F1 = open(output_dir + "/%s%d.fa" % (outpre, file_num), 'w')
+                    F1 = open(output_dir + "/%s%d.fa" %
+                              (outpre, file_num), 'w')
                 num_used = 0
 
         try:
             F1.close()
         except:
             pass
 
@@ -569,43 +557,14 @@
     elif ID_list:
         ID_list = ID_list.split(",")
 
     found_num, want_num = sb.ExtractNr(db_fasta_file, tuple(
         ID_list), output_file, short_name=long_name)
     print("%d records found in %d queries" % (found_num, want_num))
 
-# TrinityGene
-
-
-def TrinityGene_main(args):
-    Trinity_output = args.Trinity_output
-    Trinity_gene = args.Trinity_gene
-    output = extract_longest_isofrom_from_gene_in_trinity(Trinity_output)
-    with open(Trinity_gene, "w") as f:
-        for i in output:
-            i = output[i]
-            i.wrap(60)
-            f.write(">%s\n%s" % (i.seqname, i.seq))
-
-# GenerateTrinityGeneTransMap
-
-
-def GenerateTrinityGeneTransMap_main(args):
-    Trinity_output = args.Trinity_output
-    Trinity_gene = args.gene_map_file
-    with open(Trinity_output, 'r') as f:
-        with open(Trinity_gene, 'w') as w:
-            for each_line in f:
-                each_line = each_line.strip()
-                record_head = re.match(r"^>", each_line)
-                if record_head:
-                    seqname = re.sub(r'^>', '', each_line)
-                    name_short = re.search('^(\S+)', seqname).group(1)
-                    gene_name = re.sub(r'\_i\d+$', '', name_short)
-                    w.write("%s\t%s\n" % (gene_name, name_short))
 
 # SeqLength
 
 
 def SeqLength_main(args):
     seq_file = args.seq_file
     output_file = args.output_file
@@ -1049,14 +1008,15 @@
 
                 if sb.sequence_entropy(sub_seq, 3) > args.entropy_threshold:
 
                     f.write(">%s\n%s\n" % (sub_seq_name, sub_seq))
 
 # ReGetContig
 
+
 def contig_range(SeqRecord_input):
     sequence = str(SeqRecord_input.seq)
 
     num = 1
     n_site = []
     for i in sequence:
         if i != "N":
@@ -1069,20 +1029,21 @@
     num = 0
     for contig_range_tmp in contig_range_output:
         qualifiers = {
             "source": "ReGetContig",
             "ID": "%s_%d" % (SeqRecord_input.id, num)
         }
         top_feature = SeqFeature(FeatureLocation(contig_range_tmp[0] - 1, contig_range_tmp[1]),
-                                    type="contig", qualifiers=qualifiers)
+                                 type="contig", qualifiers=qualifiers)
         SeqRecord_input.features.append(top_feature)
         num = num + 1
 
     return SeqRecord_input
 
+
 def ReGetContig_main(args):
     """
     class abc():
         pass
 
     args=abc()
```

### Comparing `BioSeqTools-0.2.0/setup.py` & `BioSeqTools-0.3.0/setup.py`

 * *Files identical despite different names*

