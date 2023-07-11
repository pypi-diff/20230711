# Comparing `tmp/cmsis_stream-1.4.0-py3-none-any.whl.zip` & `tmp/cmsis_stream-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 80185 bytes, number of entries: 67
+Zip file size: 81120 bytes, number of entries: 67
 -rw-rw-rw-  2.0 fat      298 b- defN 23-May-11 12:29 cmsis_stream/__init__.py
 -rw-rw-rw-  2.0 fat      546 b- defN 23-Jun-02 06:34 cmsis_stream/cmsis_stream.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/__init__.py
 -rw-rw-rw-  2.0 fat     7448 b- defN 23-May-11 12:29 cmsis_stream/cg/types.py
 -rw-rw-rw-  2.0 fat     1925 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/CFFT.py
 -rw-rw-rw-  2.0 fat     1990 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/Duplicate.py
 -rw-rw-rw-  2.0 fat     1930 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/ICFFT.py
@@ -22,48 +22,48 @@
 -rw-rw-rw-  2.0 fat      871 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/VHTCGSTATIC.py
 -rw-rw-rw-  2.0 fat     2029 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSink.py
 -rw-rw-rw-  2.0 fat     2092 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/WavSource.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/__init__.py
 -rw-rw-rw-  2.0 fat     4018 b- defN 23-May-11 12:29 cmsis_stream/cg/nodes/host/message.py
 -rw-rw-rw-  2.0 fat      118 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/__init__.py
 -rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-02 05:41 cmsis_stream/cg/scheduler/args.py
--rw-rw-rw-  2.0 fat     3018 b- defN 23-Jun-02 05:04 cmsis_stream/cg/scheduler/ccode.py
--rw-rw-rw-  2.0 fat     6665 b- defN 23-Jun-06 08:34 cmsis_stream/cg/scheduler/config.py
+-rw-rw-rw-  2.0 fat     3762 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/ccode.py
+-rw-rw-rw-  2.0 fat     7077 b- defN 23-Jul-11 06:04 cmsis_stream/cg/scheduler/config.py
 -rw-rw-rw-  2.0 fat    41853 b- defN 23-Jun-09 07:44 cmsis_stream/cg/scheduler/description.py
 -rw-rw-rw-  2.0 fat    10849 b- defN 23-Jun-09 12:50 cmsis_stream/cg/scheduler/graphviz.py
--rw-rw-rw-  2.0 fat    37754 b- defN 23-Jun-12 08:33 cmsis_stream/cg/scheduler/node.py
--rw-rw-rw-  2.0 fat     1796 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/pythoncode.py
--rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-05 09:45 cmsis_stream/cg/scheduler/standard.py
+-rw-rw-rw-  2.0 fat    38334 b- defN 23-Jul-11 12:02 cmsis_stream/cg/scheduler/node.py
+-rw-rw-rw-  2.0 fat     1864 b- defN 23-Jul-11 05:59 cmsis_stream/cg/scheduler/pythoncode.py
+-rw-rw-rw-  2.0 fat     7540 b- defN 23-Jul-11 06:29 cmsis_stream/cg/scheduler/standard.py
 -rw-rw-rw-  2.0 fat      188 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt
 -rw-rw-rw-  2.0 fat      192 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.linux
 -rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-02 06:56 cmsis_stream/cg/scheduler/example/Makefile.mac
 -rw-rw-rw-  2.0 fat      369 b- defN 23-Jun-02 06:57 cmsis_stream/cg/scheduler/example/Makefile.windows
 -rw-rw-rw-  2.0 fat      566 b- defN 23-Jun-06 06:05 cmsis_stream/cg/scheduler/example/README.md
 -rw-rw-rw-  2.0 fat      826 b- defN 23-Jun-02 06:47 cmsis_stream/cg/scheduler/example/main_board.c
 -rw-rw-rw-  2.0 fat      212 b- defN 23-Jun-02 06:51 cmsis_stream/cg/scheduler/example/run.bat
 -rw-rw-rw-  2.0 fat      589 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple.cproject.yml
 -rw-rw-rw-  2.0 fat     1416 b- defN 23-Jun-02 07:20 cmsis_stream/cg/scheduler/example/simple_ac6.csolution.yml
 -rw-rw-rw-  2.0 fat     2178 b- defN 23-Jun-02 06:48 cmsis_stream/cg/scheduler/example/start_project_appnodes.h
 -rw-rw-rw-  2.0 fat       73 b- defN 23-Jun-02 06:10 cmsis_stream/cg/scheduler/example/start_project_custom.h
 -rw-rw-rw-  2.0 fat     1798 b- defN 23-Jun-02 06:26 cmsis_stream/cg/scheduler/example/start_project_graph.py
 -rw-rw-rw-  2.0 fat      197 b- defN 23-Jun-02 06:05 cmsis_stream/cg/scheduler/example/start_project_main.c
 -rw-rw-rw-  2.0 fat      860 b- defN 23-May-11 12:29 cmsis_stream/cg/scheduler/example/vht.clayer.yml
--rw-rw-rw-  2.0 fat    16526 b- defN 23-Jun-12 11:34 cmsis_stream/cg/scheduler/templates/GenericNodes.h
--rw-rw-rw-  2.0 fat     2006 b- defN 23-Jun-12 11:34 cmsis_stream/cg/scheduler/templates/cg_status.h
+-rw-rw-rw-  2.0 fat    16526 b- defN 23-Jul-11 12:29 cmsis_stream/cg/scheduler/templates/GenericNodes.h
+-rw-rw-rw-  2.0 fat     2006 b- defN 23-Jul-11 12:29 cmsis_stream/cg/scheduler/templates/cg_status.h
 -rw-rw-rw-  2.0 fat      434 b- defN 23-Jun-12 07:09 cmsis_stream/cg/scheduler/templates/cmsis.cpp
 -rw-rw-rw-  2.0 fat      287 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsis.py
 -rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-12 06:56 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp
 -rw-rw-rw-  2.0 fat     1232 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.cpp
--rw-rw-rw-  2.0 fat     1111 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/code.h
+-rw-rw-rw-  2.0 fat     1584 b- defN 23-Jul-11 06:54 cmsis_stream/cg/scheduler/templates/code.h
 -rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-02 07:49 cmsis_stream/cg/scheduler/templates/code.py
--rw-rw-rw-  2.0 fat     3305 b- defN 23-Jun-12 05:32 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
--rw-rw-rw-  2.0 fat     4482 b- defN 23-Jun-02 05:31 cmsis_stream/cg/scheduler/templates/commonc.cpp
+-rw-rw-rw-  2.0 fat     3316 b- defN 23-Jul-11 11:52 cmsis_stream/cg/scheduler/templates/codeSwitch.cpp
+-rw-rw-rw-  2.0 fat     5659 b- defN 23-Jul-11 06:54 cmsis_stream/cg/scheduler/templates/commonc.cpp
 -rw-rw-rw-  2.0 fat     1427 b- defN 23-Jun-12 05:39 cmsis_stream/cg/scheduler/templates/defineConfig.h
 -rw-rw-rw-  2.0 fat     7826 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/dot_template.dot
 -rw-rw-rw-  2.0 fat     7555 b- defN 23-Jun-09 12:52 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
--rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     4046 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       59 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     6473 b- defN 23-Jun-12 11:34 cmsis_stream-1.4.0.dist-info/RECORD
-67 files, 242775 bytes uncompressed, 69603 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4252 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       59 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     6473 b- defN 23-Jul-11 12:30 cmsis_stream-1.5.0.dist-info/RECORD
+67 files, 246463 bytes uncompressed, 70538 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -177,26 +177,26 @@
 
 Filename: cmsis_stream/cg/scheduler/templates/dot_template.dot
 Comment: 
 
 Filename: cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/LICENSE.txt
+Filename: cmsis_stream-1.5.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/METADATA
+Filename: cmsis_stream-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/WHEEL
+Filename: cmsis_stream-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/entry_points.txt
+Filename: cmsis_stream-1.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/top_level.txt
+Filename: cmsis_stream-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cmsis_stream-1.4.0.dist-info/RECORD
+Filename: cmsis_stream-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cmsis_stream/cg/scheduler/ccode.py

```diff
@@ -26,14 +26,27 @@
 # limitations under the License.
 ############################################
 from jinja2 import Environment, PackageLoader, select_autoescape
 import os.path
 import pathlib
 from .config import *
 
+def mkNodeIdentifications(config,sched):
+   idents=[]
+   nb = 0
+   for n in sched.nodes:
+      if n.identified:
+         name = f"{config.prefix.upper()}{n.nodeName.upper()}_ID"
+         n.identificationName = name
+         idents.append((name,nb))
+         nb = nb + 1
+
+   return(idents)
+
+
 def gencode(sched,directory,config):
 
 
     env = Environment(
        loader=PackageLoader("cmsis_stream.cg.scheduler"),
        autoescape=select_autoescape(),
        trim_blocks=True
@@ -46,14 +59,20 @@
        config.cOptionalArgs = f",\n{spc}".join(config.cOptionalArgs)
 
     # Asychronous implies code array and switchCase
     if config.asynchronous:
        config.switchCase = True
        config.memoryOptimization = False
 
+    identifiedNodes = []
+    if config.nodeIdentification:
+       config.heapAllocation = True
+       r = mkNodeIdentifications(config,sched)
+       identifiedNodes = r
+
     if config.switchCase:
        ctemplate = env.get_template("codeSwitch.cpp")
        nb = 0
        for s in sched.schedule:
          schedDescription = schedDescription + ("%d," % sched.nodes[s].codeID)
          nb = nb + 1
          if nb == 40:
@@ -64,28 +83,37 @@
     htemplate = env.get_template("code.h")
 
 
     cfile=os.path.join(directory,"%s.cpp" % config.schedulerCFileName)
     hfile=os.path.join(directory,"%s.h" % config.schedulerCFileName)
 
     nbFifos = len(sched._graph._allFIFOs)
-    
+
+    schedSwitchDataType = "uint16_t"
+    if len(sched.schedule) <=255:
+       schedSwitchDataType = "uint8_t"
+
     with open(cfile,"w") as f:
          print(ctemplate.render(fifos=sched._graph._allFIFOs,
             nbFifos=nbFifos,
             nbNodes=len(sched.nodes),
             nodes=sched.nodes,
             schedule=sched.schedule,
             schedLen=len(sched.schedule),
+            schedSwitchDataType=schedSwitchDataType,
             config=config,
             sched=sched,
-            schedDescription=schedDescription
+            schedDescription=schedDescription,
+            identifiedNodes=identifiedNodes
             ),file=f)
 
     with open(hfile,"w") as f:
          print(htemplate.render(fifos=sched._graph._allFIFOs,
             nbFifos=nbFifos,
             nodes=sched.nodes,
             schedule=sched.schedule,
             config=config,
-            sched=sched
-            ),file=f)
+            sched=sched,
+            identifiedNodes=identifiedNodes
+            ),file=f)
+
+
```

## cmsis_stream/cg/scheduler/config.py

```diff
@@ -142,14 +142,22 @@
 
         # Default asynchronous more for pure functions 
         # like CMSIS-DSP
         self.asyncDefaultSkip = True
 
         self.heapAllocation = False
 
+        # When true, create a new C++ header only
+        # with an array allowing to access the identified
+        # nodes (identified is a node creation option true by default)
+        # Macros are also generated to give indexes into this array
+        # It implies heapAllocation true because nodes
+        # must be available before the scheduler is started.
+        self.nodeIdentification = False
+
 
        
     @property
     def debug(self):
         return (self.debugLimit > 0)
```

## cmsis_stream/cg/scheduler/node.py

```diff
@@ -224,15 +224,15 @@
      def arg(self):
         return(self._name)
 
 class BaseNode:
     """Root class for all Nodes of a dataflow graph.
        To define a new kind of node, inherit from this class"""
 
-    def __init__(self,name):
+    def __init__(self,name,identified=True):
         """Create a new kind of Node.
 
         name :: The name of the node which is used as
         a C variable in final code"""
         self._nodeName = name
         self._nodeID = name
         self._inputs={}
@@ -253,14 +253,16 @@
         self._positionInCycle = 0
 
         self.sortedNodeID = 0
         # Updated during toplogical sorts to find the current
         # sinks of the truncated graph
         self.nbOutputsForTopologicalSort = 0
 
+        self._identified = identified
+
     def __getattr__(self,name):
         """Present inputs / outputs as attributes"""
         if name in self._inputs:
            return(self._inputs[name])
         if name in self._outputs:
            return(self._outputs[name])
         raise AttributeError
@@ -269,14 +271,22 @@
         """Present inputs / outputs as keys"""
         if name in self._inputs:
            return(self._inputs[name])
         if name in self._outputs:
            return(self._outputs[name])
         raise IndexError 
 
+    @property
+    def identified(self):
+        return self._identified
+
+    @identified.setter
+    def identified(self, value):
+        self._identified = value
+    
     # For cyclo static scheduling we need to compute
     # the cycle period for this node based upon the
     # period of the IOs 
     def computeCyclePeriod(self):
         allLengths = []
         for k in self._inputs:
             allLengths.append(self._inputs[k].cyclePeriod)
@@ -624,16 +634,16 @@
         return max(len(self._inputs.keys()),len(self._outputs.keys()))
     
     
 
 class GenericSink(BaseNode):
     """A sink in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         self._isPureNode = False
     
     @property
     def isPureNode(self):
         return self._isPureNode
 
     @property
@@ -643,16 +653,16 @@
     def addInput(self,name,theType,theLength):
         self._inputs[name]=Input(self,name,theType,theLength)
 
 
 class GenericSource(BaseNode):
     """A source in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         self._isPureNode = False
     
     @property
     def isPureNode(self):
         return self._isPureNode
 
     @property
@@ -661,16 +671,16 @@
 
     def addOutput(self,name,theType,theLength):
         self._outputs[name]=Output(self,name,theType,theLength)
 
 class GenericNode(BaseNode):
     """A source in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         # Pure node is for instance a 
         # CMSIS-DSP function.
         # It is not packaged into an object
         # and the code is generated directly
         self._isPureNode = False
     
     @property
@@ -686,16 +696,16 @@
 
     def addOutput(self,name,theType,theLength):
         self._outputs[name]=Output(self,name,theType,theLength)
 
 class GenericToManyNode(BaseNode):
     """A source in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         # Pure node is for instance a 
         # CMSIS-DSP function.
         # It is not packaged into an object
         # and the code is generated directly
         self._isPureNode = False
     
     @property
@@ -753,16 +763,16 @@
         ios.append("%s,%d" % (self._outputType.ctype,nbOut))
         return("".join(joinit(ios,",")))
 
 
 class GenericFromManyNode(BaseNode):
     """A source in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         # Pure node is for instance a 
         # CMSIS-DSP function.
         # It is not packaged into an object
         # and the code is generated directly
         self._isPureNode = False
     
     @property
@@ -822,16 +832,16 @@
 
 
         return("".join(joinit(ios,",")))
 
 class GenericManyToManyNode(BaseNode):
     """A source in the dataflow graph""" 
 
-    def __init__(self,name):
-        BaseNode.__init__(self,name)
+    def __init__(self,name,identified=True):
+        BaseNode.__init__(self,name,identified=identified)
         # Pure node is for instance a 
         # CMSIS-DSP function.
         # It is not packaged into an object
         # and the code is generated directly
         self._isPureNode = False
     
     @property
@@ -997,24 +1007,28 @@
 
     PYTEMPLATE = ENV.get_template("cmsis.py")
 
     def __init__(self,funcname,argsDesc):
         if not (funcname in GenericFunction.NODEID):
             GenericFunction.NODEID[funcname]=1 
 
-        GenericNode.__init__(self,"%s%d" % (funcname,GenericFunction.NODEID[funcname]))
+        GenericNode.__init__(self,"%s%d" % (funcname,GenericFunction.NODEID[funcname]),identified=False)
 
         self._hasState = False
         #self._length = length 
         self._nodeName = funcname
         self._isPureNode = True
         self._argsDesc = argsDesc
 
         GenericFunction.NODEID[funcname]=GenericFunction.NODEID[funcname]+1
 
+    @BaseNode.identified.setter
+    def identified(self, value):
+        self._identified = False
+
     @property
     def realInputs(self):
         return self._realInputs
     
     @property
     def realOutputs(self):
         return self._realOutputs
```

## cmsis_stream/cg/scheduler/pythoncode.py

```diff
@@ -36,14 +36,16 @@
        trim_blocks=True
     )
     
     template = env.get_template("code.py")
 
     cfile=os.path.join(directory,"%s.py" % config.schedulerPythonFileName)
 
+    if config.identification:
+       config.heapAllocation = True
 
     with open(cfile,"w") as f:
          nbFifos = len(sched._graph._allFIFOs)
          print(template.render(fifos=sched._graph._allFIFOs,
             nbFifos=nbFifos,
             nodes=sched.nodes,
             schedule=sched.schedule,
```

## cmsis_stream/cg/scheduler/standard.py

```diff
@@ -155,15 +155,15 @@
 # As consequence, the formatting of the arguments in the
 # generated code must be modified.
 # The template only use one arguments covering all the list
 # And finally the arguments naming is following alphabetical
 # order
 class Duplicate(GenericToManyNode):
     def __init__(self,name,theType,inLength,nb,className="Duplicate"):
-        GenericToManyNode.__init__(self,name)
+        GenericToManyNode.__init__(self,name,identified=False)
 
         self._className = className
 
         self.addInput("i",theType,inLength)
         self.addManyOutput(theType,inLength,nb)
 
     # Naming of output from index
```

## cmsis_stream/cg/scheduler/templates/code.h

```diff
@@ -6,16 +6,16 @@
 The support classes and code is covered by CMSIS-DSP license.
 
 */
 
 #ifndef _{{config.schedulerCFileName |replace(".h","")|upper()}}_H_ 
 #define _{{config.schedulerCFileName |replace(".h","")|upper()}}_H_
 
-{% macro optionalargs() -%}
-{% if config.cOptionalArgs %},{{config.cOptionalArgs}}{% endif %}
+{% macro optionalargs(first) -%}
+{% if config.cOptionalArgs %}{% if not first %},{% endif %}{{config.cOptionalArgs}}{% endif %}
 {% endmacro -%}
 
 {% if config.CAPI -%}
 #ifdef   __cplusplus
 extern "C"
 {
 #endif
@@ -28,19 +28,32 @@
 
 #define Evt_Scheduler   EventID (EventLevelAPI,   EvtSched, 0x00)
 #define Evt_Node        EventID (EventLevelAPI,   EvtSched, 0x01)
 #define Evt_Error       EventID (EventLevelError,   EvtSched, 0x02)
 
 {% endif %}
 
+{% if config.nodeIdentification %}
+#define {{config.prefix | upper}}NB_IDENTIFIED_NODES {{identifiedNodes|length}}
+{% for node in identifiedNodes %}
+#define {{node[0]}} {{node[1]}}
+{% endfor %}
+
+{% if config.CAPI -%}
+extern void *get_{{config.schedName}}_node(int32_t nodeID);
+{% else %}
+extern NodeBase *get_node_{{config.schedName}}(int32_t nodeID);
+{% endif %}
+{% endif %}
+
 {% if config.heapAllocation %}
-extern int init_{{config.schedName}}();
-extern void free_{{config.schedName}}();
+extern int init_{{config.schedName}}({{optionalargs(True)}});
+extern void free_{{config.schedName}}({{optionalargs(True)}});
 {% endif %}
-extern uint32_t {{config.schedName}}(int *error{{optionalargs()}});
+extern uint32_t {{config.schedName}}(int *error{{optionalargs(False)}});
 
 {% if config.CAPI -%}
 #ifdef   __cplusplus
 }
 #endif
 {% endif %}
```

## cmsis_stream/cg/scheduler/templates/codeSwitch.cpp

```diff
@@ -2,15 +2,15 @@
 
 {% block schedArray %}
 /*
 
 Description of the scheduling. 
 
 */
-static unsigned int schedule[{{schedLen}}]=
+static {{schedSwitchDataType}} schedule[{{schedLen}}]=
 { 
 {{schedDescription}}
 };
 {% endblock %}
 
 {% block scheduleLoop %}
     CG_BEFORE_SCHEDULE;
```

## cmsis_stream/cg/scheduler/templates/commonc.cpp

```diff
@@ -26,25 +26,38 @@
 {% endif %}
 
 {% include "defineConfig.h" %}
 
 
 CG_AFTER_INCLUDES
 
-{% macro optionalargs() -%}
-{% if config.cOptionalArgs %},{{config.cOptionalArgs}}{% endif %}
+{% macro optionalargs(first) -%}
+{% if config.cOptionalArgs %}{% if not first %},{% endif %}{{config.cOptionalArgs}}{% endif %}
 {% endmacro -%}
 
 {% macro async() -%}
 {% if config.asynchronous %}1{% else %}0{% endif %}
 {% endmacro %}
 
 {% block schedArray %}
 {% endblock %}
 
+{% if config.nodeIdentification %}
+/***********
+
+Node identification
+
+************/
+{% if config.CAPI -%}
+static void * identifiedNodes[{{config.prefix | upper}}NB_IDENTIFIED_NODES]={0};
+{% else %}
+static NodeBase * identifiedNodes[{{config.prefix | upper}}NB_IDENTIFIED_NODES]={0};
+{% endif %}
+{% endif %}
+
 CG_BEFORE_FIFO_BUFFERS
 /***********
 
 FIFO buffers
 
 ************/
 {% for fifo in fifos %}
@@ -75,15 +88,34 @@
 
 CG_BEFORE_BUFFER
 static fifos_t fifos={0};
 
 CG_BEFORE_BUFFER
 static nodes_t nodes={0};
 
-int init_{{config.schedName}}()
+{% if config.nodeIdentification %}
+{% if config.CAPI -%}
+void *get_{{config.schedName}}_node(int32_t nodeID)
+{% else %}
+NodeBase *get_node_{{config.schedName}}(int32_t nodeID)
+{% endif %}
+{
+    if (nodeID >= {{config.prefix | upper}}NB_IDENTIFIED_NODES)
+    {
+        return(NULL);
+    }
+    if (nodeID < 0)
+    {
+        return(NULL);
+    }
+    return(identifiedNodes[nodeID]);
+}
+{% endif %}
+
+int init_{{config.schedName}}({{optionalargs(True)}})
 {
     CG_BEFORE_FIFO_INIT;
 {% for id in range(nbFifos) %}
 {% if fifos[id].hasDelay %}
     fifos.fifo{{id}} = new {{fifos[id].fifoClass}}<{{fifos[id].theType.ctype}},FIFOSIZE{{id}},{{fifos[id].isArrayAsInt}},{{async()}}>({{config.prefix}}buf{{fifos[id].buffer._bufferID}},{{fifos[id].delay}});
     if (fifos.fifo{{id}}==NULL)
     {
@@ -102,22 +134,32 @@
 {% for node in nodes %}
 {% if node.hasState %}
     nodes.{{node.nodeName}} = new {{node.typeName}}<{{node.ioTemplate()}}>({{node.args}});
     if (nodes.{{node.nodeName}}==NULL)
     {
         return(CG_MEMORY_ALLOCATION_FAILURE);
     }
+{% if config.nodeIdentification -%}
+{% if node.identified -%}
+{% if config.CAPI %}
+    identifiedNodes[{{node.identificationName}}]=(void*)nodes.{{node.nodeName}};
+{% else %}
+    identifiedNodes[{{node.identificationName}}]=nodes.{{node.nodeName}};
+{% endif %}
+    nodes.{{node.nodeName}}->setID({{node.identificationName}});
+{% endif %}
+{% endif %}
 {% endif %}
 {% endfor %}
 
     return(CG_SUCCESS);
 
 }
 
-void free_{{config.schedName}}()
+void free_{{config.schedName}}({{optionalargs(True)}})
 {
 {% for id in range(nbFifos) %}
     if (fifos.fifo{{id}}!=NULL)
     {
        delete fifos.fifo{{id}};
     }
 {% endfor %}
@@ -131,15 +173,15 @@
 {% endif %}
 {% endfor %}
 }
 
 {% endif %}
 
 CG_BEFORE_SCHEDULER_FUNCTION
-uint32_t {{config.schedName}}(int *error{{optionalargs()}})
+uint32_t {{config.schedName}}(int *error{{optionalargs(False)}})
 {
     int cgStaticError=0;
     uint32_t nbSchedule=0;
 {% if config.debug %}
     int32_t debugCounter={{config.debugLimit}};
 {% endif %}
```

## Comparing `cmsis_stream-1.4.0.dist-info/LICENSE.txt` & `cmsis_stream-1.5.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cmsis_stream-1.4.0.dist-info/METADATA` & `cmsis_stream-1.5.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmsis-stream
-Version: 1.4.0
+Version: 1.5.0
 Summary: CMSIS-Stream graph description
 Home-page: https://github.com/ARM-software/CMSIS-Stream
 Author: Copyright (C) 2010-2023 ARM Limited or its affiliates. All rights reserved.
 Author-email: christophe.favergeon@arm.com
 License: License :: OSI Approved :: Apache Software License
 Project-URL: Bug Reports, https://github.com/ARM-software/CMSIS-Stream/issues
 Project-URL: Source, https://github.com/ARM-software/CMSIS-Stream
@@ -41,14 +41,19 @@
 
 * Define new compute nodes
 * Connect them into a dataflow graph to process streams
 * Generate a C scheduler to run the graph on your target
 
 # Change history
 
+## Version 1.5.0:
+
+* Corrections to the heap mode
+* Added possibility to identify and access nodes from the outside of the scheduler (it implies the heap mode). See documentation for more information
+
 ## Version 1.4.0:
 
 * Possibility to customize the style of the graph pictures (colors, fonts ...)
 * Graph picture can now also be generated before schedule computation (useful to debug an incorrect graph before trying to compute a schedule)
 * Possibility to use more **pure** C functions in the graph. The `GenericFunction` node can now easily be used to plug more kind of C functions without having to write a C++ wrapper
 * `Dsp` node has been removed. Instead use the `Unary`, `Binary` or the more flexible `GenericFunction` node
```

## Comparing `cmsis_stream-1.4.0.dist-info/RECORD` & `cmsis_stream-1.5.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 cmsis_stream/cg/nodes/host/VHTCGSTATIC.py,sha256=zNXVzkZZROzGwHBq62uzFuAVIummPwMcxW0JhpaI-88,871
 cmsis_stream/cg/nodes/host/WavSink.py,sha256=ldo5e9wjaIp0Ef6GvRgZIICuuk3H1V7B-hn1et6S7Wo,2029
 cmsis_stream/cg/nodes/host/WavSource.py,sha256=KywcbHsrCqrAQD6HuZaxOxVj_ekYDYIgzx_6Nh2R4Gk,2092
 cmsis_stream/cg/nodes/host/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cmsis_stream/cg/nodes/host/message.py,sha256=e2hto5-Ly08sUCKN8F94qH3O3lAxcGGIGBLkf6cLJCY,4018
 cmsis_stream/cg/scheduler/__init__.py,sha256=-GMWFk8b3LpReDjD7yHF_SLrFDu5PRZuxN1RbjkY6nk,118
 cmsis_stream/cg/scheduler/args.py,sha256=mepFm7CJa2wnB-21a-h1FrufP5KtI78l_B3HNb87ayk,1691
-cmsis_stream/cg/scheduler/ccode.py,sha256=f57rHk2gtgkikywW_ZEkdXlibV4wnHbOQ5vi0fHRcME,3018
-cmsis_stream/cg/scheduler/config.py,sha256=J3W01wi-DO32EVKsgQ5ztUeNMBl0fDk2cXuOzySMM30,6665
+cmsis_stream/cg/scheduler/ccode.py,sha256=NBv9eqec1TdyhRcn2-ZwBb7sVeIc4SwmS5rOStt0HoY,3762
+cmsis_stream/cg/scheduler/config.py,sha256=SOSgp7rDFccmVEjikyodwUczN9hfdeJAKFQnTmu6E_w,7077
 cmsis_stream/cg/scheduler/description.py,sha256=FPLRFTxk3mGduq2_hLPxNiL5MNzpFDzl-Nk1ivyyBVk,41853
 cmsis_stream/cg/scheduler/graphviz.py,sha256=TwiDslHOJlek2otwA_5sspTWaf_trLV4QMthpv6fzM4,10849
-cmsis_stream/cg/scheduler/node.py,sha256=RqSxM0EHSUUkrBu9wEMByEGbGgW2QA_jMXm5kAT4d9A,37754
-cmsis_stream/cg/scheduler/pythoncode.py,sha256=bDtCVYvgtLO_wpl33HlyyAEZtfyW6wHyANQsdPvdlBA,1796
-cmsis_stream/cg/scheduler/standard.py,sha256=VngMlAxV9n8HNPX50KDD_OLQvaTI4Q7iz_mxjRgHEWU,7523
+cmsis_stream/cg/scheduler/node.py,sha256=b_tO27sp1gphHM710mwRrHsOW8aezwxzJHDY_cSsR3s,38334
+cmsis_stream/cg/scheduler/pythoncode.py,sha256=48KAT64uzM5z8S2QoqkZPZLCUnk3TpOIPjhUGEbnyA4,1864
+cmsis_stream/cg/scheduler/standard.py,sha256=LFenG7Da-TBzzp_Pl2BKAzJj3li9WFLNOJF4xwnkoY4,7540
 cmsis_stream/cg/scheduler/example/ARMCM55_FP_MVE_config.txt,sha256=Yn4YtMgyACdeesvFcPkP1xZ9Q8rIEarIAIrJeQNn3sw,188
 cmsis_stream/cg/scheduler/example/Makefile.linux,sha256=4x9Z6tbRIswUvBQuTuD9t0Co-DCwEGevAnaMc3CC5NU,192
 cmsis_stream/cg/scheduler/example/Makefile.mac,sha256=-2ldN02pnOEKwS1QqxY9-97qnUse6MEDZO9Ru1CkplQ,267
 cmsis_stream/cg/scheduler/example/Makefile.windows,sha256=p6ic8tdH0H0Fm6A8-877JIvIqgnhaScSjUKNSgB7Wb8,369
 cmsis_stream/cg/scheduler/example/README.md,sha256=_o0nMzYUELDms9o9Gh__4fuOTYqUAwabijVBSHkqsiA,566
 cmsis_stream/cg/scheduler/example/main_board.c,sha256=DJCtYtjQimSzK2OeN4c38qAFKVSmK5pc1FCE8m8KwgU,826
 cmsis_stream/cg/scheduler/example/run.bat,sha256=kYGYp4pNuKJFiWPqQyBoT0u7MXzuth6iTZ7CTBZVfDg,212
@@ -48,20 +48,20 @@
 cmsis_stream/cg/scheduler/example/vht.clayer.yml,sha256=KYF6zwS9iDaoH9iUWGZjuoX880f-Az7-LnQIsaAIRTQ,860
 cmsis_stream/cg/scheduler/templates/GenericNodes.h,sha256=Xs7uGOL8YYvTaWc_L-07t029hiQiN5NqtV7g9V3s-gE,16526
 cmsis_stream/cg/scheduler/templates/cg_status.h,sha256=1ZBdMG2s9FMyTzdvFtxpPIK624-jnfRd_Q2Qxe_MwTM,2006
 cmsis_stream/cg/scheduler/templates/cmsis.cpp,sha256=Fw5MHQqCZt2srXAuJjvXSHS1m-78DGdT4sGHDEQgG28,434
 cmsis_stream/cg/scheduler/templates/cmsis.py,sha256=iC5sSkuZ01iGT0dBfqNPUbMKE86y10-0Gj8fLOfbgi8,287
 cmsis_stream/cg/scheduler/templates/cmsisCheck.cpp,sha256=JMn_nIJiPYSnu7qVKHS8jKEtAjktGpWSyzxg-r2olgw,682
 cmsis_stream/cg/scheduler/templates/code.cpp,sha256=uiJEAmZyGoMq_AqYqZ3aXRyX9L7cRKdkUFazGLc1eP0,1232
-cmsis_stream/cg/scheduler/templates/code.h,sha256=BULWyJn9FAU6laXpg6UjyP5TtHHMCW_3zTccu_EtjKU,1111
+cmsis_stream/cg/scheduler/templates/code.h,sha256=EL-F5iS31gGrFK7WMi5bxWThZyALgmovpqVbOkLMNVw,1584
 cmsis_stream/cg/scheduler/templates/code.py,sha256=eOK6r2DkCD-JftAKAi0K3PxOwidRWtdtal4N8_xC6wk,2199
-cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=aL_bl4hTZ5dtNGKOoLxgqURt6rH6AJt3Sw-61qmFSJs,3305
-cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=nmlbxVoBiujXLYerA056T_GPRL-LZSo0IFcz6BHdTHc,4482
+cmsis_stream/cg/scheduler/templates/codeSwitch.cpp,sha256=QoQiLGGb_AUbeTE2LyaOneAkkfccxl4Ah-K-AbVoh-M,3316
+cmsis_stream/cg/scheduler/templates/commonc.cpp,sha256=r0lKbtH4QL_fhdX43iLeU5nqHA8FkuoCnq7vywtTsR4,5659
 cmsis_stream/cg/scheduler/templates/defineConfig.h,sha256=KoW0i45XF2-Ghcs-snyqlyysT0SfcKVJcStrBotO1gE,1427
 cmsis_stream/cg/scheduler/templates/dot_template.dot,sha256=_4a8oe0kvSDx-Hl1P0aIZMFAOYMpknhGkeOUI8Nqy6g,7826
 cmsis_stream/cg/scheduler/templates/precompute_dot_template.dot,sha256=wLfhZpZS0VHm43dpaQYZBSd8ftd0KdUS_hSo2cSHwLU,7555
-cmsis_stream-1.4.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
-cmsis_stream-1.4.0.dist-info/METADATA,sha256=UakFDEe3RXFSR9baQZ5IMDZ-3I0HbSmJhFQao94fBKM,4046
-cmsis_stream-1.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cmsis_stream-1.4.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
-cmsis_stream-1.4.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
-cmsis_stream-1.4.0.dist-info/RECORD,,
+cmsis_stream-1.5.0.dist-info/LICENSE.txt,sha256=4DukHX-rIHAHaf5BGLq1DYAMt0-ZA1OgXS9f_xwig2M,11558
+cmsis_stream-1.5.0.dist-info/METADATA,sha256=_Bd9BnB8LyHBwH_1baff5VTdPUcHu0YgxYG1qgpQOEg,4252
+cmsis_stream-1.5.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cmsis_stream-1.5.0.dist-info/entry_points.txt,sha256=WOEqwaMTN0K5CT8Yfd-z53mE82xfyzsM16a0eR4Ipds,59
+cmsis_stream-1.5.0.dist-info/top_level.txt,sha256=a7ZhPCd-XkrgWSSuOstN5Jgqe60MV4q7-tWximJBomA,13
+cmsis_stream-1.5.0.dist-info/RECORD,,
```

