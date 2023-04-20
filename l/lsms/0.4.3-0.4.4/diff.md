# Comparing `tmp/lsms-0.4.3-py2.py3-none-any.whl.zip` & `tmp/lsms-0.4.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7200 bytes, number of entries: 9
--rw-rw----  2.0 unx      121 b- defN 23-Mar-14 23:04 lsms/__init__.py
--rw-rw----  2.0 unx      838 b- defN 23-Mar-14 23:05 lsms/dta_concordance.py
--rw-rw----  2.0 unx      633 b- defN 23-Mar-14 23:05 lsms/from_dta.py
--rw-rw----  2.0 unx    21406 b- defN 23-Mar-14 23:05 lsms/tools.py
--rw-rw----  2.0 unx      282 b- defN 23-Mar-14 23:05 lsms-0.4.3.dist-info/LICENSE.txt
--rw-rw----  2.0 unx      396 b- defN 23-Mar-14 23:05 lsms-0.4.3.dist-info/METADATA
--rw-rw----  2.0 unx      110 b- defN 23-Mar-14 23:05 lsms-0.4.3.dist-info/WHEEL
--rw-rw----  2.0 unx        5 b- defN 23-Mar-14 23:05 lsms-0.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      667 b- defN 23-Mar-14 23:05 lsms-0.4.3.dist-info/RECORD
-9 files, 24458 bytes uncompressed, 6062 bytes compressed:  75.2%
+Zip file size: 7304 bytes, number of entries: 9
+-rw-rw----  2.0 unx      121 b- defN 23-Apr-20 02:21 lsms/__init__.py
+-rw-rw----  2.0 unx      838 b- defN 23-Apr-20 02:21 lsms/dta_concordance.py
+-rw-rw----  2.0 unx      633 b- defN 23-Apr-20 02:21 lsms/from_dta.py
+-rw-rw----  2.0 unx    21813 b- defN 23-Apr-20 02:21 lsms/tools.py
+-rw-rw----  2.0 unx      282 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/LICENSE.txt
+-rw-rw----  2.0 unx      396 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/METADATA
+-rw-rw----  2.0 unx      110 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/WHEEL
+-rw-rw----  2.0 unx        5 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      667 b- defN 23-Apr-20 02:21 lsms-0.4.4.dist-info/RECORD
+9 files, 24865 bytes uncompressed, 6166 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: lsms/from_dta.py
 Comment: 
 
 Filename: lsms/tools.py
 Comment: 
 
-Filename: lsms-0.4.3.dist-info/LICENSE.txt
+Filename: lsms-0.4.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lsms-0.4.3.dist-info/METADATA
+Filename: lsms-0.4.4.dist-info/METADATA
 Comment: 
 
-Filename: lsms-0.4.3.dist-info/WHEEL
+Filename: lsms-0.4.4.dist-info/WHEEL
 Comment: 
 
-Filename: lsms-0.4.3.dist-info/top_level.txt
+Filename: lsms-0.4.4.dist-info/top_level.txt
 Comment: 
 
-Filename: lsms-0.4.3.dist-info/RECORD
+Filename: lsms-0.4.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lsms/__init__.py

```diff
@@ -1,5 +1,5 @@
 from . import tools
 from . dta_concordance import dta_concordance
 from . from_dta import from_dta
 
-__version__ = '0.4.3'
+__version__ = '0.4.4'
```

## lsms/tools.py

```diff
@@ -91,15 +91,15 @@
         varnames.update({units:'units'})
 
     df.rename(columns=varnames,inplace=True)
 
     try:
         if df['HHID'].iloc[0].split('.')[-1]=='0':  # String representation of a float?
             df['HHID']=df['HHID'].apply(lambda x: '%d' % int(float(x)))
-    except ValueError:
+    except (ValueError,AttributeError):
         pass
     try:
         df['itmcd']=df['itmcd'].astype(float)
         originalShape=df.shape
         df=df.loc[~np.isnan(df['itmcd']),:]
         if df.shape!=originalShape:
             warn("Warning: %d missing item codes dropped" % (originalShape[0]-df.shape[0]))
@@ -367,15 +367,17 @@
     x=x.unstack()
 
     x.replace(np.NaN,0,inplace=True)
 
     return x,defaultdict(int,{v:k for k,v in itemlabels.items()})
 
 
-def get_household_roster(fn,sex='sex',sex_converter=None,age='age',age_converter=None,months_spent='months_spent',HHID='HHID',months_converter=None, convert_categoricals=True,Age_ints=None,fn_type='stata'):
+def get_household_roster(fn,sex='sex',sex_converter=None,age='age',age_converter=None,months_spent='months_spent',HHID='HHID',months_converter=None,
+wave=None, region=None,
+convert_categoricals=True,Age_ints=None,fn_type='stata'):
     if fn_type in ['stata','dta']:
         if type(fn)==list:
             files=[f for f in set(fn)]
             df=from_dta(files.pop(), convert_categoricals=convert_categoricals)
             for f in files:
                 current_df=from_dta(f, convert_categoricals=convert_categoricals)
                 df=pd.merge(df,current_df)
@@ -403,16 +405,19 @@
 
     if type(HHID)==list:
         df['HHID']=df[HHID[0]].apply(lambda x: unicode(x))
         for itm in HHID[1:]:
             df['HHID']=df['HHID']+'-'+df[itm].apply(lambda x: unicode(x))
         HHID = 'HHID'
 
-    df=df.loc[:,[v for v in [HHID, sex, age, months_spent] if v in df.columns.tolist()]]
-    df.rename(columns={HHID:'HHID',sex:'sex',age:'age',months_spent:'months_spent'},inplace=True)
+    fulldf = df.copy()
+    df=df.loc[:,[v for v in [HHID, sex, age, months_spent, wave, region] if v in df.columns.tolist()]]
+    df.rename(columns={HHID:'HHID',sex:'sex',age:'age',
+                       months_spent:'months_spent',
+                       wave:'wave',region:'region'},inplace=True)
 
     if months_converter is not None:
         df['months_spent']=df['months_spent'].apply(months_converter)
 
     if sex_converter is not None:
         df['sex']=df['sex'].apply(sex_converter)
 
@@ -428,15 +433,15 @@
     df['men']=((df['sex']=='m') & (df['age']>=18))
     df['women']=((df['sex']=='f') & (df['age']>=18))
 
     if Age_ints is None:
         Age_ints = ((0,1),(1,5),(5,10),(10,15),(15,20),(20,30),(30,50),(50,60),(60,100))
 
     # Aggregate household members
-    valvars = ['HHID','girls','boys','men','women']
+    valvars = list(set(['HHID','girls','boys','men','women','wave','region']).intersection(df.columns))
     for ages in Age_ints:
         agestr = list(ages)
         agestr[1] = agestr[1]-1
         agestr = tuple(agestr)
         df['Males %02d-%02d' % agestr] = ((df['sex']=='m') & (df['age'] < ages[1]) & (df['age'] >= ages[0]))
         df['Females %02d-%02d' % agestr] = ((df['sex']=='f') & (df['age'] < ages[1]) & (df['age'] >= ages[0]))
         valvars.append('Males %02d-%02d' % agestr)
@@ -444,19 +449,24 @@
 
     try:
         if df['HHID'].iloc[0].split('.')[-1]=='0':  # String representation of a float?
             df['HHID']=df['HHID'].apply(lambda x: '%d' % int(float(x)))
     except (ValueError,AttributeError):
         pass
 
+    idxs = ['HHID']
+    if wave is not None:
+        idxs += ['wave']
+    if region is not None:
+        idxs += ['region']
 
     if 'months_spent' in df.columns and df['months_spent'].count()>0:
-        g=df.loc[df['months_spent']>0,valvars].groupby(['HHID']) # Drop members never resident this year
+        g=df.loc[df['months_spent']>0,valvars].groupby(idxs) # Drop members never resident this year
     else:
-        g=df[valvars].groupby(['HHID']) # Aggregate at hh level.
+        g=df[valvars].groupby(idxs) # Aggregate at hh level.
     x=g.sum()
 
     return x
 
 def get_household_variables(fn, HHID, variables, names, converters, convert_categoricals):
     # construct one dataframe from multiple files if necessary
     if type(fn)==list:
@@ -512,15 +522,15 @@
     except ValueError:
         pass
 
     df = df.loc[:, ['HHID']+names]
     df.set_index('HHID', inplace=True)
     return df.loc[:, names]
 
-def get_household_identification_particulars(fn,HHID='HHID',urban='urban',urban_converter=None,region='region',region_converter=None,convert_categoricals=True,wealth_rank=None,wealth_rank_converter=None,happiness=None):
+def get_household_identification_particulars(fn,HHID='HHID',urban='urban',urban_converter=None,region='region',region_converter=None,convert_categoricals=True,wealth_rank=None,wealth_rank_converter=None,happiness=None,wave=None):
 
     if type(fn)==list:
         files=[f for f in set(fn)]
         df=from_dta(files.pop(), convert_categoricals=convert_categoricals)
         for f in files:
             current_df=from_dta(f, convert_categoricals=convert_categoricals)
             df=pd.merge(df,current_df)
@@ -543,23 +553,26 @@
     df['region']=df['region'].apply(lambda s: str(s).lower())
     #df['urban']=df['urban'].apply(lambda s: str(s).lower())=='urban'
     df['urban']=df['urban'].apply(lambda x: x==1)
 
     try:
         if df['HHID'].iloc[0].split('.')[-1]=='0':  # String representation of a float?
             df['HHID']=df['HHID'].apply(lambda x: '%d' % int(float(x)))
-    except ValueError:
+    except (ValueError,AttributeError):
         pass
 
+    columns = ['urban','region']
+    if wave is not None:
+        columns += ['wave']
+        df['wave'] = df[wave]
+
     if wealth_rank is not None:
-        columns=['urban','region','wealth rank','happiness']
+        columns += ['wealth rank','happiness']
         df['wealth rank']=df[wealth_rank].apply(wealth_rank_converter)
         df['happiness']=df[happiness]
-    else:
-        columns=['urban','region']
 
     df=df.loc[:,['HHID']+columns]
     #df=df.drop_duplicates()
 
     df.set_index('HHID',inplace=True)
 
     return df.loc[:,columns]
```

## Comparing `lsms-0.4.3.dist-info/RECORD` & `lsms-0.4.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-lsms/__init__.py,sha256=TLgAM6AIxfibipbPVbpcVjsimLbSSoXNWpAFjW61XC8,121
+lsms/__init__.py,sha256=dw5tDmXoDpZDcS8JbIbimsUnKmLihVBA5gDfcGxcc6c,121
 lsms/dta_concordance.py,sha256=MIruKRn1IqVgXdUGf4X4MJ65Pmw-POwctVTpKohozDg,838
 lsms/from_dta.py,sha256=QQgP8ftl-DOM1llg3gcGTJmyFJgOGWIfiKhIvst2aDg,633
-lsms/tools.py,sha256=dZghVoSupfYkGSyaMGNiKcqosS1vKrMF_X_KtPqsCG0,21406
-lsms-0.4.3.dist-info/LICENSE.txt,sha256=qImFXcRJwxIHS80FE7uOx6FhmLY8apd4Y12aR54QU7w,282
-lsms-0.4.3.dist-info/METADATA,sha256=bnDd3HXjmt4E0XfJH5q6K0wGsxab_unEKOnSvCs-GmE,396
-lsms-0.4.3.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-lsms-0.4.3.dist-info/top_level.txt,sha256=kOSV2CMw4OoSMw9rYGFItmsQDWDXpO3GzeVBTj020lc,5
-lsms-0.4.3.dist-info/RECORD,,
+lsms/tools.py,sha256=BW-7yrz4249mJB5Dr0GRi7vUj_ohurfZXmNU05_DPCY,21813
+lsms-0.4.4.dist-info/LICENSE.txt,sha256=qImFXcRJwxIHS80FE7uOx6FhmLY8apd4Y12aR54QU7w,282
+lsms-0.4.4.dist-info/METADATA,sha256=uWkZYZUn3coMS957iZZqw8m3gkn6JhJYJB7ZYInFMO8,396
+lsms-0.4.4.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+lsms-0.4.4.dist-info/top_level.txt,sha256=kOSV2CMw4OoSMw9rYGFItmsQDWDXpO3GzeVBTj020lc,5
+lsms-0.4.4.dist-info/RECORD,,
```

