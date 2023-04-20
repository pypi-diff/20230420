# Comparing `tmp/MatAn-0.1.4-py3-none-any.whl.zip` & `tmp/MatAn-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 18590 bytes, number of entries: 8
--rw-r--r--  2.0 unx    16575 b- defN 23-Apr-18 08:42 matan/__init__.py
+Zip file size: 18594 bytes, number of entries: 8
+-rw-r--r--  2.0 unx    17024 b- defN 23-Apr-20 06:16 matan/__init__.py
 -rw-r--r--  2.0 unx      107 b- defN 23-Apr-18 08:30 misc/__init__.py
 -rw-r--r--  2.0 unx     2363 b- defN 23-Apr-18 08:30 properties/__init__.py
--rw-r--r--  2.0 unx    34670 b- defN 23-Apr-18 19:34 MatAn-0.1.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     1194 b- defN 23-Apr-18 19:34 MatAn-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 19:34 MatAn-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-18 19:34 MatAn-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      603 b- defN 23-Apr-18 19:34 MatAn-0.1.4.dist-info/RECORD
-8 files, 55626 bytes uncompressed, 17552 bytes compressed:  68.4%
+-rw-r--r--  2.0 unx    34670 b- defN 23-Apr-20 15:17 MatAn-0.1.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1194 b- defN 23-Apr-20 15:17 MatAn-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 15:17 MatAn-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Apr-20 15:17 MatAn-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      603 b- defN 23-Apr-20 15:17 MatAn-0.1.5.dist-info/RECORD
+8 files, 56075 bytes uncompressed, 17556 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: misc/__init__.py
 Comment: 
 
 Filename: properties/__init__.py
 Comment: 
 
-Filename: MatAn-0.1.4.dist-info/LICENSE
+Filename: MatAn-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: MatAn-0.1.4.dist-info/METADATA
+Filename: MatAn-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: MatAn-0.1.4.dist-info/WHEEL
+Filename: MatAn-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: MatAn-0.1.4.dist-info/top_level.txt
+Filename: MatAn-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: MatAn-0.1.4.dist-info/RECORD
+Filename: MatAn-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matan/__init__.py

```diff
@@ -104,16 +104,18 @@
         self.eng_values=engineering_values(name=name,
                                            force_units=force_units,
                                            lenght_units=lenght_units,
                                            thickness=thickness,
                                            width=width
                                            )
         self.real_values=real_values_class(name=name,
-            thickness=thickness,
-            width=width)
+                                           thickness=thickness,
+                                           width=width,
+                                           force_units=force_units,
+                                           lenght_units=lenght_units,)
         
         if stress_array is None and strain_array is None:
             if elongation_array is None and force_array is None:
                 raise ValueError("None of elongation/force or stress/strain arrays are defined!")
             elif thickness is None:
                 raise ValueError("Thickness is not defined!")
             elif width is None:
@@ -177,15 +179,15 @@
             self.thickness=thickness,
             self.width=width
             self.stress, self.strain=None,None
         def calculate(self,
                       thickness:float,
                       width:float,
                       elongation_array,
-                      force_array
+                      force_array,
                       ):
             """Calculates the engineering stress and strain
 
             This method is used to calculate engineering stress and strain from height
 
             Parameters
             ----------
@@ -222,15 +224,15 @@
                                                   self.strain)
             
             self.at_break=self.calculate_at_break(self.strain,
                                                   self.stress)
             
             self.yield_strength=self.calculate_yield_strength(self.stress,
                                                               self.strain)
-            
+            self.tensile_modulus=self.calculate_tensile_modulus()
 
         class calculate_strength:
             def __init__(self,strain: np.array,stress:np.array):
                 """Strenght is according to ISO-527-1 first maximum local value
 
                 Parameters
                 ----------
@@ -273,15 +275,15 @@
             """
             def __init__(self,stress, strain):
                 at_break=properties.at_break(stress, strain)
                 self.stress=at_break.stress
                 self.strain=at_break.strain
 
 
-        def tensile_modulus(self,
+        def calculate_tensile_modulus(self,
                                     plot=True,
                                     r2=True,
                                     output=True,
                                     lower_limit=0.05,
                                     upper_limit=0.25
                                     ):
             """            Tensile, or Young's modulus is the slope of strain/stress curve, between strains equals to 0.05 and 0.25 percent according to DIN ISO 527-1
@@ -313,17 +315,17 @@
                 label=rf"Young's modulus {int(E.tensile_modulus)} $\left[\frac{{{self.force_units}}}{{{self.lenght_units}^2}}\right]$"
                 if r2:
                     label+="\n"+rf"$R^{{{2}}}={E.r2}$"
                 plt.plot(E.module_strain,
                          E.module_stress,
                          label=label
                          )
-            self.tensile_modulus = E.tensile_modulus
             if output:
                 print(f"Tensile modulus is equal to {int(E.tensile_modulus)} [{self.force_units}/{self.lenght_units}^2]")
+                return   E.tensile_modulus
 
                 
         def set(self,
                 engineering_stress: Union[list, np.array] =None,
                 engineering_strain:Union[list, np.array] =None,
                 # TODO: gives TypeError: only size-1 arrays can be converted to Python scalars while using numpy array
                 # TODO: gives KeyKerrr None
@@ -373,22 +375,28 @@
             plt.xlabel(f"Strain [{self.lenght_units}]")
             plt.legend()
             if show:
                 plt.show()
 
 class real_values_class(engineering_values):
 
-        def __init__(self, name,thickness, width):
-            # self.force_units=force_units
-            # self.lenght_units=lenght_units
-            # if lenght_units=="%" or lenght_units=="percent":
-            #     self.percent_strain=True
-            # else:
-            #     self.percent_strain=False
+        def __init__(self, name,
+                     thickness,
+                     width,
+                     force_units,
+                     lenght_units,
+                     ):
+            self.force_units=force_units
+            self.lenght_units=lenght_units
+            if lenght_units=="%" or lenght_units=="percent":
+                self.percent_strain=True
+            else:
+                self.percent_strain=False
 
+    
             engineering_values.__init__(self,
                                         name=name,
                                         thickness=thickness,
                                         width=width
                                         )
             self.name=name + " [real]"
             width=self.width
@@ -418,15 +426,16 @@
                                                   self.strain)
             
             self.at_break=self.calculate_at_break(self.strain,
                                                   self.stress)
             
             self.yield_strength=self.calculate_yield_strength(self.stress,
                                                               self.strain)
-            
+            self.tensile_modulus=self.calculate_tensile_modulus()            
+
 
 
         # def plot(self, show: bool=False):
         #     plt.plot(self.strain,self.stress, label=self.name)
         #     plt.title("real")
             
         #     plt.legend()
```

## Comparing `MatAn-0.1.4.dist-info/LICENSE` & `MatAn-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `MatAn-0.1.4.dist-info/METADATA` & `MatAn-0.1.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MatAn
-Version: 0.1.4
+Version: 0.1.5
 Summary: Material analysis package to plot or extract properties like tensile modulus etc. 
 Home-page: https://codeberg.org/309631/matan
 Author: Igor Cudnik
 Author-email: igor.cudnik@student.put.poznan.pl
 License: GPLv3
 Keywords: material analysis,ISO 527,ISO 527-1,polymers analysis
 Classifier: Development Status :: 3 - Alpha
@@ -14,11 +14,11 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
 Requires-Dist: matplotlib
+Requires-Dist: numpy
 
 Python package was created to calculate the stress, strains, tensile modulus, and other properties from force and elongation data from a machine. For now, it includes only polymer tests according to the ISO-527-1 standard, but in the future, other standards should be included.
```

## Comparing `MatAn-0.1.4.dist-info/RECORD` & `MatAn-0.1.5.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-matan/__init__.py,sha256=w24dFPwec7WN5qvHqkQNxN78K2v3fTrFmZuot5Q1LXM,16575
+matan/__init__.py,sha256=rDBigQe7kZDEwpdB_6DzpOUAKvUrWmLcXFY_abGmkH0,17024
 misc/__init__.py,sha256=S4SweLuIAeWI1arT-Lwzy4ifxc8Ettq7RvbJVuLIFnc,107
 properties/__init__.py,sha256=zyx81mL3DxiY38oSdHf8H4_2K_X4Qy1PtUkM0vWFbsk,2363
-MatAn-0.1.4.dist-info/LICENSE,sha256=tqi_Y64slbCqJW7ndGgNe9GPIfRX2nVGb3YQs7FqzE4,34670
-MatAn-0.1.4.dist-info/METADATA,sha256=t5tYoPyHnE3L8KO_upePSKZITqoV9ubvkRRyci0XkBA,1194
-MatAn-0.1.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-MatAn-0.1.4.dist-info/top_level.txt,sha256=w-JKsP40rv98l3aspw7sJg6CBr_vifDhX3EyG_RP9Xs,22
-MatAn-0.1.4.dist-info/RECORD,,
+MatAn-0.1.5.dist-info/LICENSE,sha256=tqi_Y64slbCqJW7ndGgNe9GPIfRX2nVGb3YQs7FqzE4,34670
+MatAn-0.1.5.dist-info/METADATA,sha256=qrEyuDC0x8zOd07sz37HNxO948JpDUeBzxdoWgWybMs,1194
+MatAn-0.1.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+MatAn-0.1.5.dist-info/top_level.txt,sha256=w-JKsP40rv98l3aspw7sJg6CBr_vifDhX3EyG_RP9Xs,22
+MatAn-0.1.5.dist-info/RECORD,,
```

