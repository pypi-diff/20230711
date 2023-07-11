# Comparing `tmp/calsim-0.0.7.tar.gz` & `tmp/calsim-0.0.8.tar.gz`

## Comparing `calsim-0.0.7.tar` & `calsim-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,24 @@
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/__init__.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/__init__.py
--rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/control.py
--rwxr-xr-x   0        0        0     4852 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/controller.py
--rwxr-xr-x   0        0        0    17318 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/dynamics.py
--rwxr-xr-x   0        0        0     6118 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/environment.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/exceptions.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/manipulator.py
--rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/run_simulation.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/sim_utils.py
--rwxr-xr-x   0        0        0     4475 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/state_estimation.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/tests.py
--rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/transforms.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/core/twist.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.7/src/CalSim/tests/test_double_pend.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.7/tests/test_double_pend.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.7/tests/test_simulation_simple.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.7/LICENSE
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 calsim-0.0.7/README.md
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 calsim-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/__init__.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/__init__.py
+-rw-r--r--   0        0        0    12292 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/control.py
+-rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/controller.py
+-rw-r--r--   0        0        0    11246 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/depth_cam.py
+-rwxr-xr-x   0        0        0    23005 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/dynamics.py
+-rwxr-xr-x   0        0        0     6118 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/environment.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/exceptions.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/manipulator.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/obstacle.py
+-rwxr-xr-x   0        0        0      440 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/run_simulation.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/sim_utils.py
+-rwxr-xr-x   0        0        0     7878 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/state_estimation.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/tests.py
+-rw-r--r--   0        0        0     6795 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/transforms.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/core/twist.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/tests/test_double_pend.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 calsim-0.0.8/src/CalSim/tests/test_planar_qrotor.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 calsim-0.0.8/tests/test_double_pend.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 calsim-0.0.8/tests/test_simulation_simple.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 calsim-0.0.8/LICENSE
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 calsim-0.0.8/README.md
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 calsim-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 calsim-0.0.8/PKG-INFO
```

### Comparing `calsim-0.0.7/src/CalSim/core/control.py` & `calsim-0.0.8/src/CalSim/core/control.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/core/controller.py` & `calsim-0.0.8/src/CalSim/core/controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,17 +37,45 @@
     def get_input(self):
         """
         Retrieves input stored in class parameter
         Returns:
             self._u: most recent input stored in class paramter
         """
         return self._u
+    
+class FFController(Controller):
+    """
+    Class for a simple feedforward controller.
+    """
+    def __init__(self, observer, lyapunovBarrierList = None, trajectory = None, uBounds = None):
+        """
+        Init function for a ff controller
+        Args:
+            observer (Observer): state observer object
+            ff (NumPy Array): constant feedforward input to send to system
+            lyapunov (List of LyapunovBarrier): list of LyapunovBarrier objects
+            trajectory (Trajectory): trajectory for the controller to track (could just be a constant point!)
+            uBounds ((Dynamics.singleInputDimn x 2) numpy array): minimum and maximum input values to the system
+        """
+        self.ff = np.array([[9.81*0.92, 0]]).T
+        super().__init__(observer, lyapunovBarrierList, trajectory, uBounds)
+    
+    def eval_input(self, t):
+        """
+        Solve for and return control input
+        Inputs:
+            t (float): time in simulation
+        Returns:
+            u ((Dynamics.singleInputDimn x 1)): input vector, as determined by controller
+        """
+        self._u = self.ff
+        return self._u
 
 class ControllerManager(Controller):
-    def __init__(self, observerManager, barrierManager, trajectoryManager, lidarManager, ControlType):
+    def __init__(self, observerManager, ControlType, barrierManager = None, trajectoryManager = None, lidarManager = None):
         """
         Managerial class that points to N controller instances for the system. Interfaces
         directly with the overall system dynamics object.
         Args:
             observerManager (ObserverManager)
             barrierManager (BarrierManager)
             trajectoryManager (TrajectoryManager)
```

### Comparing `calsim-0.0.7/src/CalSim/core/dynamics.py` & `calsim-0.0.8/src/CalSim/core/dynamics.py`

 * *Files 19% similar despite different names*

```diff
@@ -173,23 +173,72 @@
                 axs[i+self.singleStateDimn].grid()
         
         axs[self.singleStateDimn + self.singleInputDimn - 1].set(xlabel = xlabel)
         legendList = ["Agent " + str(i) for i in range(self.N)]
         plt.legend(legendList)
         plt.show()
     
-    def show_animation(self, xData, uData, tData):
+    def show_animation(self, xData, uData, tData, axis_lims, labels, anim_point, anim_line = None, animate = True):
         """
         Function to play animations specific to this dynamic system.
         Args:
-            x ((sysStateDimn x N) numpy array): history of N states to plot
-            u ((sysInputDimn x N) numpy array): history of N inputs to plot
-            t ((1 x N) numpy array): history of N times associated with x and u
+            xData ((sysStateDimn x N) numpy array): history of N states to plot
+            uData ((sysInputDimn x N) numpy array): history of N inputs to plot
+            tData ((1 x N) numpy array): history of N times associated with x and u
+            axis_lims (Python List, length 4): list of axis limits, ex: [-0.25, 5.25, -0.25, 5.25]
+            labels (Python list, length 3): List of strings ["Xlabel", "Ylabel", "Title"] for plot
+            anim_point (Python function): function to be called at an index i, returns x, y to be animated
+            anim_line (Python function): function to be called at an index i, returns line to be animated
         """
-        pass
+        #Set constant animtion parameters
+        FREQ = 50 #control frequency, same as data update frequency
+        
+        if animate:
+            fig, ax = plt.subplots()
+            # set the axes limits
+            ax.axis(axis_lims)
+            # set equal aspect such that the circle is not shown as ellipse
+            ax.set_aspect("equal")
+
+            # create a set of points in the axes
+            point, = ax.plot([],[], marker="o", linestyle='None')
+
+            #check for anim_line
+            if anim_line is not None:
+                #define the line for the quadrotor
+                line, = ax.plot([], [], 'o-', lw=2)
+
+            def anim_func(i):
+                #Call animate_func to get the x and y to plot
+                x, y = anim_point(i)
+
+                #set the data to points and return points
+                point.set_data(x, y)
+
+                #check for anim_line
+                if anim_line is not None:
+                    #call the line animation function
+                    thisx, thisy = anim_line(i)
+                    #set the data for the line
+                    line.set_data(thisx, thisy)
+
+                    #if we use a line, return line and point
+                    return line, point
+                else:
+                    #if no line is present, just return the point
+                    return point,
+
+            num_frames = xData.shape[1]-1
+
+            anim = animation.FuncAnimation(fig, anim_func, frames=num_frames, interval=1/FREQ*1000, blit=True)
+
+            plt.xlabel(labels[0])
+            plt.ylabel(labels[1])
+            plt.title(labels[2])
+            plt.show()
     
     
 """
 **********************************
 PLACE YOUR DYNAMICS FUNCTIONS HERE
 **********************************
 """
@@ -420,36 +469,127 @@
         Shows the animation and visualization of data for this system.
         Args:
             xData (stateDimn x N Numpy array): state vector history array
             u (inputDimn x N numpy array): input vector history array
             t (1 x N numpy array): time history
             animate (bool, optional): Whether to generate animation or not. Defaults to True.
         """
+        #define animation function to return the x, y points to be animated
+        def anim_point(i):
+            x = []
+            y = []
+            #get the x, y data associated with each turtlebot
+            for j in range(self.N):
+                x.append(xData[3*j, i])
+                y.append(xData[3*j+1, i])
+            return x, y
+    
+        #define axis limits
+        axis_lims = [-0.25, 5.25, -0.25, 5.25]
+
+        #define labels
+        axis_labels = ["X Position (m)", "Y Position (m)", "Positions of Turtlebots in Space"]
+
+        #call the super() animation function
+        super().show_animation(xData, uData, tData, axis_lims, axis_labels, anim_point, anim_line = None, animate = animate)
+
+
+
+class PlanarQrotor(Dynamics):
+    def __init__(self, x0 = np.zeros((8, 1)), m = 0.92, Ixx = 0.0023, l = 0.15, N = 1):
+        """
+        Init function for a Planar quadrotor system.
+        State Vector: X = [x, y, z, theta, x_dot, y_dot, z_dot, theta_dot]
+        Input Vector: U = [F, M]
+        
+        Args:
+            x0 ((8 x 1) NumPy Array): initial state (x, y, z, theta, x_dot, y_dot, z_dot, theta_dot)
+            m (float): mass of quadrotor in kg
+            Ixx (float): moment of inertia about x axis of quadrotor
+            l (float): length of one arm of quadrotor
+            N (int): number of quadrotors
+        """
+        #store physical parameters
+        self._m = m
+        self._Ixx = Ixx
+        self._g = 9.81
+        self._l = l
+
+        #define quadrotor dynamics
+        def quadrotor_dyn(X, U, t):
+            """
+            Returns the derivative of the state vector
+            Args:
+                X (8 x 1 numpy array): current state vector at time t
+                U (2 x 1 numpy array): current input vector at time t
+                t (float): current time with respect to simulation start
+            Returns:
+                xDot: state_dimn x 1 derivative of the state vector
+            """
+            #unpack the input vector
+            F, M = U[0, 0], U[1, 0]
+            F = max(0, F) #Cut off force at zero to prevent negative thrust
+            
+            #unpack the state vector
+            x_dot, y_dot, z_dot = X[4, 0], X[5, 0], X[6, 0] #velocities
+            theta, theta_dot = X[3, 0], X[7, 0] #orientations
+            
+            #calculate the second time derivatives of each
+            x_ddot = 0
+            y_ddot = (-np.sin(theta)*F)/self._m
+            z_ddot = (np.cos(theta)*F - self._m*self._g)/self._m
+            theta_ddot = M/self._Ixx
+            
+            #construct and return state vector        
+            return np.array([[x_dot, y_dot, z_dot, theta_dot, x_ddot, y_ddot, z_ddot, theta_ddot]]).T
+        
+        #call the super init function
+        super().__init__(x0, 8, 2, quadrotor_dyn, N = N)
+
+    def show_plots(self, xData, uData, tData):
+        #Plot each state variable in time
+        stateLabels = ['X Pos (m)', 'Y Pos (m)', 'Z Pos (m)', 'Theta (rad)', 'X Vel (m/s)', 'Y Vel (m/s)', 'Z Vel (m/s)', 'Angular Vel (rad/s)']
+        inputLabels = ['Force (N)', 'Moment (N*m)']
+        super().show_plots(xData, uData, tData, stateLabels, inputLabels)
+        
+    def show_animation(self, xData, uData, tData, animate = True):
+        """
+        Shows the animation and visualization of data for this system.
+        Args:
+            xData (stateDimn x N Numpy array): state vector history array
+            u (inputDimn x N numpy array): input vector history array
+            t (1 x N numpy array): time history
+            animate (bool, optional): Whether to generate animation or not. Defaults to True.
+        """
         #Set constant animtion parameters
         FREQ = 50 #control frequency, same as data update frequency
+        L = self._l #quadrotor arm length
+
+        #define point animation function
+        def anim_point(i):
+            y = xData[1, i]
+            z = xData[2, i]
+            return y, z
         
-        if animate:
-            fig, ax = plt.subplots()
-            # set the axes limits
-            ax.axis([-0.25, 5.25, -0.25, 5.25])
-            # set equal aspect such that the circle is not shown as ellipse
-            ax.set_aspect("equal")
-            # create a set of points in the axes
-            points, = ax.plot([],[], marker="o", linestyle='None')
-            num_frames = xData.shape[1]-1
-                
-            def animate(i):
-                x = []
-                y = []
-                #get the x, y data associated with each turtlebot
-                for j in range(self.N):
-                    x.append(xData[3*j, i])
-                    y.append(xData[3*j+1, i])
-                points.set_data(x, y)
-                return points,
-            
-            anim = animation.FuncAnimation(fig, animate, frames=num_frames, interval=1/FREQ*1000, blit=True)
+        #define line animation function
+        def anim_line(i):
+            y = xData[1, i]
+            z = xData[2, i]
+
+            #draw the quadrotor line body
+            theta = xData[3, i]
+            x1 = y + L*np.cos(theta)
+            x2 = y - L*np.cos(theta)
+            y1 = z + L*np.sin(theta)
+            y2 = z - L*np.sin(theta)
+            thisx = [x1, x2]
+            thisy = [y1, y2]
+            return thisx, thisy
+        
+        #define axis limits
+        axis_lims = [-1, 2.5, 0, 2.5]
+
+        #define plot labels
+        labels = ["Y Position (m)", "Z Position (m)", "Position of Drone in Space"]
 
-            plt.xlabel("X Position (m)")
-            plt.ylabel("Y Position (m)")
-            plt.title("Positions of Turtlebots in Space")
-            plt.show()
+        #call the super animation function
+        super().show_animation(xData, uData, tData, axis_lims, labels, anim_point, anim_line, animate = animate)
```

### Comparing `calsim-0.0.7/src/CalSim/core/environment.py` & `calsim-0.0.8/src/CalSim/core/environment.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/core/manipulator.py` & `calsim-0.0.8/src/CalSim/core/manipulator.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/core/sim_utils.py` & `calsim-0.0.8/src/CalSim/core/sim_utils.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/core/transforms.py` & `calsim-0.0.8/src/CalSim/core/transforms.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/core/twist.py` & `calsim-0.0.8/src/CalSim/core/twist.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/src/CalSim/tests/test_double_pend.py` & `calsim-0.0.8/src/CalSim/tests/test_double_pend.py`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/LICENSE` & `calsim-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `calsim-0.0.7/pyproject.toml` & `calsim-0.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "CalSim"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Massimiliano de Sa", email="mz.desa@berkeley.edu" },
 ]
 description = "Simulator package for Berkeley robotics course."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

