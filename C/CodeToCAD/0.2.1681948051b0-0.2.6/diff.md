# Comparing `tmp/CodeToCAD-0.2.1681948051b0.tar.gz` & `tmp/CodeToCAD-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodeToCAD-0.2.1681948051b0.tar", last modified: Thu Apr 20 03:27:12 2023, max compression
+gzip compressed data, was "CodeToCAD-0.2.6.tar", last modified: Tue Mar 14 18:44:06 2023, max compression
```

## Comparing `CodeToCAD-0.2.1681948051b0.tar` & `CodeToCAD-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-04-20 03:27:12.272077 CodeToCAD-0.2.1681948051b0/
-drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-04-20 03:27:12.270700 CodeToCAD-0.2.1681948051b0/CodeToCAD/
--rw-r--r--   0 shehab     (501) staff       (20)    53089 2023-04-19 23:47:55.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD/CodeToCADInterface.py
--rw-r--r--   0 shehab     (501) staff       (20)    23939 2023-04-19 23:47:55.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD/CodeToCADProvider.py
--rw-r--r--   0 shehab     (501) staff       (20)    33354 2023-04-19 23:47:55.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD/TestCodeToCADProvider.py
--rw-r--r--   0 shehab     (501) staff       (20)     4039 2023-03-14 20:56:36.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD/__init__.py
--rw-r--r--   0 shehab     (501) staff       (20)    29692 2023-03-20 17:37:47.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD/utilities.py
-drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-04-20 03:27:12.271633 CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/
--rw-r--r--   0 shehab     (501) staff       (20)     6322 2023-04-20 03:27:12.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/PKG-INFO
--rw-r--r--   0 shehab     (501) staff       (20)      301 2023-04-20 03:27:12.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/SOURCES.txt
--rw-r--r--   0 shehab     (501) staff       (20)        1 2023-04-20 03:27:12.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/dependency_links.txt
--rw-r--r--   0 shehab     (501) staff       (20)       10 2023-04-20 03:27:12.000000 CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/top_level.txt
--rw-r--r--   0 shehab     (501) staff       (20)    32473 2022-06-17 17:22:57.000000 CodeToCAD-0.2.1681948051b0/LICENSE
--rw-r--r--   0 shehab     (501) staff       (20)     6322 2023-04-20 03:27:12.271937 CodeToCAD-0.2.1681948051b0/PKG-INFO
--rw-r--r--   0 shehab     (501) staff       (20)     5778 2023-04-19 23:47:55.000000 CodeToCAD-0.2.1681948051b0/README.md
--rw-r--r--   0 shehab     (501) staff       (20)       38 2023-04-20 03:27:12.272123 CodeToCAD-0.2.1681948051b0/setup.cfg
--rw-r--r--   0 shehab     (501) staff       (20)      934 2023-04-20 03:27:09.000000 CodeToCAD-0.2.1681948051b0/setup.py
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.653009 CodeToCAD-0.2.6/
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.651149 CodeToCAD-0.2.6/CodeToCAD/
+-rw-r--r--   0 shehab     (501) staff       (20)    52877 2023-03-14 17:49:23.000000 CodeToCAD-0.2.6/CodeToCAD/CodeToCADInterface.py
+-rw-r--r--   0 shehab     (501) staff       (20)    24176 2023-03-14 17:49:32.000000 CodeToCAD-0.2.6/CodeToCAD/CodeToCADProvider.py
+-rw-r--r--   0 shehab     (501) staff       (20)    33120 2023-03-14 17:49:27.000000 CodeToCAD-0.2.6/CodeToCAD/TestCodeToCADProvider.py
+-rw-r--r--   0 shehab     (501) staff       (20)     4039 2023-03-14 17:57:05.000000 CodeToCAD-0.2.6/CodeToCAD/__init__.py
+-rw-r--r--   0 shehab     (501) staff       (20)    27428 2023-03-10 02:21:17.000000 CodeToCAD-0.2.6/CodeToCAD/utilities.py
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.652343 CodeToCAD-0.2.6/CodeToCAD.egg-info/
+-rw-r--r--   0 shehab     (501) staff       (20)     5776 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/PKG-INFO
+-rw-r--r--   0 shehab     (501) staff       (20)      301 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/SOURCES.txt
+-rw-r--r--   0 shehab     (501) staff       (20)        1 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/dependency_links.txt
+-rw-r--r--   0 shehab     (501) staff       (20)       10 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/top_level.txt
+-rw-r--r--   0 shehab     (501) staff       (20)    32473 2022-06-17 17:22:57.000000 CodeToCAD-0.2.6/LICENSE
+-rw-r--r--   0 shehab     (501) staff       (20)     5776 2023-03-14 18:44:06.652783 CodeToCAD-0.2.6/PKG-INFO
+-rw-r--r--   0 shehab     (501) staff       (20)     5242 2023-03-14 18:42:58.000000 CodeToCAD-0.2.6/README.md
+-rw-r--r--   0 shehab     (501) staff       (20)       38 2023-03-14 18:44:06.653087 CodeToCAD-0.2.6/setup.cfg
+-rw-r--r--   0 shehab     (501) staff       (20)      785 2023-03-14 18:44:05.000000 CodeToCAD-0.2.6/setup.py
```

### Comparing `CodeToCAD-0.2.1681948051b0/CodeToCAD/CodeToCADInterface.py` & `CodeToCAD-0.2.6/CodeToCAD/CodeToCADInterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# THIS IS AN AUTO-GENERATE FILE.
+# THIS IS AN AUTO-GENERATE FILE. 
 # DO NOT EDIT MANUALLY.
 # Please run development/capabilitiesJsonToPython/capabilitiesToPy.sh to generate this file.
 
 from abc import ABCMeta, abstractmethod
 from typing import Optional, TypeAlias, Union
 
-from CodeToCAD.utilities import (Angle, Axis, BoundaryBox, CurveTypes, Dimension, Dimensions, LengthUnit, Point)
+from CodeToCAD.utilities import (Angle, Axis, BoundaryBox, CurveTypes, Dimension,
+                            Dimensions, LengthUnit, Point)
 
 FloatOrItsStringValue: TypeAlias = Union[str, float]
 IntOrFloat: TypeAlias = Union[int, float]
 MaterialOrItsName: TypeAlias = Union[str, 'Material']
 PartOrItsName: TypeAlias = Union[str, 'Part']
 EntityOrItsName: TypeAlias = Union[str, 'Entity']
 LandmarkOrItsName: TypeAlias = Union[str, 'Landmark']
@@ -18,36 +19,25 @@
 AngleOrItsFloatOrStringValue: TypeAlias = Union[str,float, Angle]
 EntityOrItsNameOrLandmark: TypeAlias = Union[str, 'Entity', 'Landmark']
 PointOrListOfFloatOrItsStringValue: TypeAlias = Union[str, list[FloatOrItsStringValue], Point]
 LengthUnitOrItsName: TypeAlias = Union[str,LengthUnit]
 
 class Entity(metaclass=ABCMeta):
     '''Capabilities shared between Parts, Sketches and Landmarks.'''
-
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @abstractmethod
-    def createFromFile(self, filePath:str, fileType:Optional[str]=None
-    ):
-        '''
-        Adds geometry to a part from a file. If the part does not exist, this will create it.
-        '''
-        
-        print("createFromFile is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
     def isExists(self
     ) -> bool:
         '''
         Check if an entity exists
         '''
         
         print("isExists is called in an abstract method. Please override this method.")
@@ -436,16 +426,27 @@
         '''
         
         print("getLandmark is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 class Part(Entity,metaclass=ABCMeta):
     '''Create and manipulate 3D shapes.'''
-
     
+    
+
+    @abstractmethod
+    def createFromFile(self, filePath:str, fileType:Optional[str]=None
+    ):
+        '''
+        Adds geometry to a part from a file. If the part does not exist, this will create it.
+        '''
+        
+        print("createFromFile is called in an abstract method. Please override this method.")
+        return self
+        
 
     @abstractmethod
     def createCube(self, width:DimensionOrItsFloatOrStringValue, length:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None
     ):
         '''
         Adds cuboid geometry to a part.
         '''
@@ -704,15 +705,15 @@
         '''
         
         print("selectFaceNearLandmark is called in an abstract method. Please override this method.")
         return self
         
 class Sketch(Entity,metaclass=ABCMeta):
     '''Capabilities related to adding, multiplying, and/or modifying a curve.'''
-
+    
     
     name:str
     curveType:Optional['CurveTypes']=None
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, curveType:Optional['CurveTypes']=None, description:Optional[str]=None):
@@ -741,25 +742,14 @@
         '''
         
         print("revolve is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def thicken(self, radius:DimensionOrItsFloatOrStringValue
-    ):
-        '''
-        Uniformly add a wall around a sketch.
-        '''
-        
-        print("thicken is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
     def extrude(self, length:DimensionOrItsFloatOrStringValue
     ) -> 'Part':
         '''
         Extrude a curve by a specified length. Returns a Part type.
         '''
         
         print("extrude is called in an abstract method. Please override this method.")
@@ -928,15 +918,15 @@
         '''
         
         print("createTrapezoid is called in an abstract method. Please override this method.")
         return self
         
 class Landmark(metaclass=ABCMeta):
     '''Landmarks are named positions on an entity.'''
-
+    
     
     name:str
     parentEntity:EntityOrItsName
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, parentEntity:EntityOrItsName, description:Optional[str]=None):
@@ -1056,15 +1046,15 @@
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 class Joint(metaclass=ABCMeta):
     '''Joints define the relationships and constraints between entities.'''
-
+    
     
     entity1:EntityOrItsNameOrLandmark
     entity2:EntityOrItsNameOrLandmark
 
     @abstractmethod
     def __init__(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark):
         self.entity1 = entity1
@@ -1188,15 +1178,15 @@
         '''
         
         print("limitRotationZ is called in an abstract method. Please override this method.")
         return self
         
 class Material(metaclass=ABCMeta):
     '''Materials affect the appearance and simulation properties of the parts.'''
-
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
@@ -1223,15 +1213,15 @@
     ):
         
         print("addImageTexture is called in an abstract method. Please override this method.")
         return self
         
 class Animation(metaclass=ABCMeta):
     '''Camera, lighting, rendering, animation related functionality.'''
-
+    
     
 
     @abstractmethod
     def __init__(self):
         pass
 
     @staticmethod
@@ -1253,15 +1243,15 @@
     ):
         
         print("createKeyFrameRotation is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 class Light(metaclass=ABCMeta):
     
-
+    
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
@@ -1402,15 +1392,15 @@
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 class Camera(metaclass=ABCMeta):
     
-
+    
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
@@ -1535,15 +1525,15 @@
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 class Scene(metaclass=ABCMeta):
     '''Scene, camera, lighting, rendering, animation, simulation and GUI related functionality.'''
-
+    
     
     name:Optional[str]=None
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:Optional[str]=None, description:Optional[str]=None):
         self.name = name
@@ -1662,15 +1652,15 @@
         '''
         
         print("setBackgroundImage is called in an abstract method. Please override this method.")
         return self
         
 class Analytics(metaclass=ABCMeta):
     '''Tools for collecting data about the entities and scene.'''
-
+    
     
 
     @abstractmethod
     def __init__(self):
         pass
 
     @abstractmethod
```

### Comparing `CodeToCAD-0.2.1681948051b0/CodeToCAD/TestCodeToCADProvider.py` & `CodeToCAD-0.2.6/CodeToCAD/TestCodeToCADProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,14 @@
         # inject provider?
         super().setUp()
 
 class TestEntity(TestProviderCase):
     
     
     @unittest.skip
-    def test_createFromFile(self):
-        instance = Part("name","description")
-
-        value = instance.createFromFile("filePath","fileType")
-
-        
-        assert value.isExists(), "Create method failed."
-        
-    @unittest.skip
     def test_isExists(self):
         instance = Part("name","description")
 
         value = instance.isExists("")
 
         
         assert value, "Get method failed."
@@ -346,14 +337,23 @@
 
         
         assert value, "Get method failed."
         
 class TestPart(TestProviderCase):
     
     @unittest.skip
+    def test_createFromFile(self):
+        instance = Part("")
+
+        value = instance.createFromFile("filePath","fileType")
+
+        
+        assert value.isExists(), "Create method failed."
+        
+    @unittest.skip
     def test_createCube(self):
         instance = Part("")
 
         value = instance.createCube("width","length","height","keywordArguments")
 
         
         assert value.isExists(), "Create method failed."
@@ -577,23 +577,14 @@
 
         value = instance.revolve("angle","aboutEntityOrLandmark","axis")
 
         
         assert value, "Modify method failed."
         
     @unittest.skip
-    def test_thicken(self):
-        instance = Sketch("name","curveType","description")
-
-        value = instance.thicken("radius")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
     def test_extrude(self):
         instance = Sketch("name","curveType","description")
 
         value = instance.extrude("length")
 
         
         assert value, "Get method failed."
```

### Comparing `CodeToCAD-0.2.1681948051b0/CodeToCAD/__init__.py` & `CodeToCAD-0.2.6/CodeToCAD/__init__.py`

 * *Files identical despite different names*

### Comparing `CodeToCAD-0.2.1681948051b0/CodeToCAD/utilities.py` & `CodeToCAD-0.2.6/CodeToCAD/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             "d": AngleUnit.DEGREES
         }
 
         fromString: str = name.lower().replace("(s)", "")
 
         parsedUnit: Optional[AngleUnit] = aliases[fromString] if fromString in aliases else None
 
-        assert parsedUnit is not None, f"Could not parse unit {fromString}"
+        assert parsedUnit != None, f"Could not parse unit {fromString}"
 
         return parsedUnit
 
 
 class Angle():
 
     def toRadians(self) -> 'Angle':
@@ -261,15 +261,15 @@
 
     if type(angleString) == str:
         angleString = angleString.replace(" ", "").lower()
         angleString = re.search('[A-Za-z]+$', angleString)
 
         unitInString = AngleUnit.fromString(
             angleString[0]) if angleString else None
-        if unitInString is not None and angleString is not None:
+        if unitInString != None and angleString != None:
             defaultUnit = unitInString
             if len(angleString[0]) == len(anglesList[-1]):
                 anglesList.pop()
 
     parsedAngles = []
     for angle in anglesList:
         parsedAngles.append(Angle.fromString(angle, defaultUnit))
@@ -322,15 +322,15 @@
             "mi": LengthUnit.mi
         }
 
         fromString: str = name.lower().replace("(s)", "")
 
         parsedUnit: LengthUnit | None = aliases[fromString] if fromString in aliases else None
 
-        assert parsedUnit is not None, f"Could not parse unit {fromString}"
+        assert parsedUnit != None, f"Could not parse unit {fromString}"
 
         return parsedUnit
 
 
 class Axis(EquittableEnum):
     X = 0
     Y = 1
@@ -471,31 +471,31 @@
     def __str__(self) -> str:
         return f"{self.value}{' '+self.unit.name if self.unit else ''}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def convertToUnit(self, targetUnit: LengthUnit) -> 'Dimension':
-        assert self.unit is not None, f"Current dimension does not have a unit."
+        assert self.unit != None, f"Current dimension does not have a unit."
         targetUnit = LengthUnit.fromString(targetUnit) if not isinstance(
             targetUnit, LengthUnit) else targetUnit
         assert isinstance(
             targetUnit, LengthUnit), f"Could not convert to unit {targetUnit}"
 
         newDimension = Dimension(
             self.value * (self.unit.value/targetUnit.value),
             targetUnit
         )
         return newDimension
 
     def arithmeticPrecheckAndUnitConversion(self, other) -> 'Dimension':
-        assert other is not None, "Right-hand value cannot be None."
+        assert other != None, "Right-hand value cannot be None."
         if not isinstance(other, Dimension):
             other = Dimension.fromString(other)
-        if other.unit is not None and self.unit is not None and other.unit != self.unit:
+        if other.unit != None and other.unit != self.unit:
             other = other.convertToUnit(self.unit)
         return other
 
     def __add__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
         return Dimension(self.value + other.value, self.unit)
 
@@ -595,20 +595,17 @@
         if unitInString:
             value = fromString[0:-1*len(unitInString)]
             unitInString = LengthUnit.fromString(unitInString)
             unit = unitInString or unit
 
         # if min,max,center is used, try to parse those words into their respective values.
         if isReservedWordInString(value):
-            assert boundaryAxis is not None, "min,max,center keywords used, but boundaryAxis is not known."
+            assert boundaryAxis != None, "min,max,center keywords used, but boundaryAxis is not known."
             if unit == None:
                 unit = boundaryAxis.unit
-
-            assert unit, "Could not determine the unit to convert the boundary axis."
-
             value = replaceMinMaxCenterWithRespectiveValue(
                 value, boundaryAxis, unit)
 
         assert len(value) > 0, f"Dimension value cannot be empty."
 
         # Make sure our value only contains math operations and numbers as a weak safety check before passing it to `eval`
         assert re.match(
@@ -633,110 +630,60 @@
         return [self.x, self.y, self.z]
 
     @classmethod
     def fromList(cls, pointList: list[Dimension]):
         assert len(pointList) == 3, "Point list must contain three Dimensions."
         return cls(pointList[0], pointList[1], pointList[2])
 
-    def arithmeticPrecheckAndUnitConversion(self, other) -> 'Point':
-        assert other is not None, "Right-hand value cannot be None."
-
-        if not isinstance(other, (int, float, str, Dimension, list, Point)):
-            raise TypeError(
-                "Only int/float, Dimension, or Dimension String, or a list of those types is allowed.")
-
-        if isinstance(other, (int, float)):
-            return Point(Dimension(other), Dimension(other), Dimension(other))
-
-        x = Dimension(0)
-        y = Dimension(0)
-        z = Dimension(0)
-
-        if isinstance(other, list):
-            [x, y, z] = getDimensionListFromStringList(other)
-
-        if isinstance(other, str):
-            if "," in other:
-                [x, y, z] = getDimensionListFromStringList(other)
-            else:
-                other = Dimension.fromString(other)
-
-        if isinstance(other, Dimension):
-            x = other
-            y = other
-            z = other
-
-        if isinstance(other, Point):
-            x = other.x
-            y = other.y
-            z = other.z
-
-        if x.unit is not None and self.x.unit is not None and x.unit != self.x.unit:
-            x: Dimension = x.convertToUnit(self.x.unit)
-        if y.unit is not None and self.y.unit is not None and y.unit != self.y.unit:
-            y: Dimension = y.convertToUnit(self.y.unit)
-        if z.unit is not None and self.z.unit is not None and z.unit != self.z.unit:
-            z: Dimension = z.convertToUnit(self.z.unit)
-        return Point(x, y, z)
-
     def __eq__(self, other) -> bool:
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         return self.x == other.x and self.y == other.y and self.z == other.z
 
     def __add__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x + other.x
         y = self.y + other.y
         z = self.z + other.z
         return Point(x, y, z)
 
     def __sub__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x - other.x
         y = self.y - other.y
         z = self.z - other.z
         return Point(x, y, z)
 
     def __mul__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x * other.x
         y = self.y * other.y
         z = self.z * other.z
         return Point(x, y, z)
 
     def __truediv__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x / other.x
         y = self.y / other.y
         z = self.z / other.z
         return Point(x, y, z)
 
     def __floordiv__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x // other.x
         y = self.y // other.y
         z = self.z // other.z
         return Point(x, y, z)
 
     def __mod__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x % other.x
         y = self.y % other.y
         z = self.z % other.z
         return Point(x, y, z)
 
-    # def __divmod__(self, other):
-    #     other = self.arithmeticPrecheckAndUnitConversion(other)
-    #     x = divmod(self.x, other.x)
-    #     y = divmod(self.y, other.y)
-    #     z = divmod(self.z, other.z)
-    #     return Point(x, y, z)
+    def __divmod__(self, other):
+        x = divmod(self.x, other.x)
+        y = divmod(self.y, other.y)
+        z = divmod(self.z, other.z)
+        return Point(x, y, z)
 
     def __pow__(self, other, mod=None):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = pow(self.x, other.x)
         y = pow(self.y, other.y)
         z = pow(self.z, other.z)
         return Point(x, y, z)
 
     def __abs__(self):
         x = abs(self.x)
@@ -925,21 +872,21 @@
                       ), "Only a list of strings is allowed."
 
     parsedDimensions = []
 
     defaultUnit = None
 
     unitInString = getUnitInString(dimensions[-1])
-    if unitInString is not None:
+    if unitInString != None:
         defaultUnit = LengthUnit.fromString(unitInString)
         if len(unitInString) == len(dimensions[-1].replace(" ", "").lower()):
             dimensions.pop()
 
     for index, dimension in enumerate(dimensions):
-        if boundingBox is not None and index < 3:
+        if boundingBox != None and index < 3:
             boundaryAxis = getattr(boundingBox, "xyz"[index])
             parsedDimensions.append(Dimension.fromString(
                 dimension, defaultUnit, boundaryAxis))
             continue
 
         parsedDimensions.append(
             Dimension.fromString(dimension, defaultUnit, None))
```

### Comparing `CodeToCAD-0.2.1681948051b0/CodeToCAD.egg-info/PKG-INFO` & `CodeToCAD-0.2.6/CodeToCAD.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeToCAD
-Version: 0.2.1681948051b0
+Version: 0.2.6
 Summary: 3D modeling automation in your favorite modeling software.
 Home-page: https://github.com/CodeToCAD/CodeToCAD
 Author: CodeToCAD
 Author-email: shehab@codethatdown.com
 License: GPL v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,21 +16,19 @@
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
 Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -39,33 +37,33 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/import_file_in_blender.png)
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
@@ -115,15 +113,15 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
 ### Contributing
```

### Comparing `CodeToCAD-0.2.1681948051b0/LICENSE` & `CodeToCAD-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CodeToCAD-0.2.1681948051b0/PKG-INFO` & `CodeToCAD-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeToCAD
-Version: 0.2.1681948051b0
+Version: 0.2.6
 Summary: 3D modeling automation in your favorite modeling software.
 Home-page: https://github.com/CodeToCAD/CodeToCAD
 Author: CodeToCAD
 Author-email: shehab@codethatdown.com
 License: GPL v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,21 +16,19 @@
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
 Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -39,33 +37,33 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/import_file_in_blender.png)
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
@@ -115,15 +113,15 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
 ### Contributing
```

### Comparing `CodeToCAD-0.2.1681948051b0/README.md` & `CodeToCAD-0.2.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
 Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -24,33 +22,33 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/import_file_in_blender.png)
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/documentation/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
@@ -100,18 +98,18 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
 ### Contributing
 
 If you would like to contribute to the project, please feel free to submit a PR. 
 
-Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
+Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
```

