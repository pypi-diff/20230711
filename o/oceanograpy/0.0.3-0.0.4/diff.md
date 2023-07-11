# Comparing `tmp/oceanograpy-0.0.3.tar.gz` & `tmp/oceanograpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanograpy-0.0.3.tar", last modified: Sun Jul  9 03:11:48 2023, max compression
+gzip compressed data, was "oceanograpy-0.0.4.tar", last modified: Tue Jul 11 14:40:40 2023, max compression
```

## Comparing `oceanograpy-0.0.3.tar` & `oceanograpy-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:48.850725 oceanograpy-0.0.3/
--rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      782 2023-07-09 03:11:48.850725 oceanograpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:48.840727 oceanograpy-0.0.3/oceanograpy/
--rw-rw-rw-   0        0        0      215 2023-07-09 03:11:06.000000 oceanograpy-0.0.3/oceanograpy/__init__.py
--rw-rw-rw-   0        0        0    16665 2023-07-09 02:14:07.000000 oceanograpy-0.0.3/oceanograpy/adcp_plot_tools.py
--rw-rw-rw-   0        0        0     1644 2023-07-09 02:31:28.000000 oceanograpy-0.0.3/oceanograpy/example.py
--rw-rw-rw-   0        0        0     2797 2023-07-09 03:07:43.000000 oceanograpy-0.0.3/oceanograpy/frma.py
--rw-rw-rw-   0        0        0     9289 2023-07-09 02:24:41.000000 oceanograpy-0.0.3/oceanograpy/matplotlib_dhi.py
--rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.3/oceanograpy/processing_tools.py
--rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.3/oceanograpy/seabird_ctd.py
--rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.3/oceanograpy/workhorse_adcp.py
-drwxrwxrwx   0        0        0        0 2023-07-09 03:11:48.849725 oceanograpy-0.0.3/oceanograpy.egg-info/
--rw-rw-rw-   0        0        0      782 2023-07-09 03:11:48.000000 oceanograpy-0.0.3/oceanograpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-09 03:11:48.000000 oceanograpy-0.0.3/oceanograpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 03:11:48.000000 oceanograpy-0.0.3/oceanograpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-09 03:11:48.000000 oceanograpy-0.0.3/oceanograpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 03:11:48.850725 oceanograpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-07-08 03:44:30.000000 oceanograpy-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-07-07 18:08:28.000000 oceanograpy-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      782 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-07-08 03:43:29.000000 oceanograpy-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.938737 oceanograpy-0.0.4/oceanograpy/
+-rw-rw-rw-   0        0        0      215 2023-07-09 03:11:06.000000 oceanograpy-0.0.4/oceanograpy/__init__.py
+-rw-rw-rw-   0        0        0    24745 2023-07-11 00:32:09.000000 oceanograpy-0.0.4/oceanograpy/adcp_plot_tools.py
+-rw-rw-rw-   0        0        0     2166 2023-07-11 00:30:41.000000 oceanograpy-0.0.4/oceanograpy/example.py
+-rw-rw-rw-   0        0        0     2797 2023-07-09 03:07:43.000000 oceanograpy-0.0.4/oceanograpy/frma.py
+-rw-rw-rw-   0        0        0     5339 2023-07-10 23:50:52.000000 oceanograpy-0.0.4/oceanograpy/matplotlib_dhi.py
+-rw-rw-rw-   0        0        0     4375 2023-07-08 03:16:35.000000 oceanograpy-0.0.4/oceanograpy/processing_tools.py
+-rw-rw-rw-   0        0        0    24857 2023-07-08 03:22:23.000000 oceanograpy-0.0.4/oceanograpy/seabird_ctd.py
+-rw-rw-rw-   0        0        0    67612 2023-07-08 17:53:37.000000 oceanograpy-0.0.4/oceanograpy/workhorse_adcp.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:40:40.959720 oceanograpy-0.0.4/oceanograpy.egg-info/
+-rw-rw-rw-   0        0        0      782 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 14:40:40.000000 oceanograpy-0.0.4/oceanograpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      102 2023-07-08 00:06:28.000000 oceanograpy-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:40:40.961719 oceanograpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-07-11 14:35:48.000000 oceanograpy-0.0.4/setup.py
```

### Comparing `oceanograpy-0.0.3/LICENSE` & `oceanograpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.3/PKG-INFO` & `oceanograpy-0.0.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.3/oceanograpy/adcp_plot_tools.py` & `oceanograpy-0.0.4/oceanograpy/adcp_plot_tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import numpy as np
 import os 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib.collections import LineCollection
-
+import matplotlib.ticker as mticker
 
 from matplotlib_dhi import *
 from matplotlib_dhi import subplots
 def import_multiple_pd0(paths,labels):
     '''
     reads multiple Workhorse ADCP files from a list of filepaths
 
@@ -18,34 +18,103 @@
     paths : list
         list containing paths to each .pd0 file
     labels : TYPE
         DESCRIPTION.
 
     Returns
     -------
-    ADCP_data : dict
+    adcp_file : dict
         Dictionary with keys specified by labels.
 
     '''
-    ADCP_data = {}
+    adcp_file = {}
     for p,path in enumerate(paths):
         label = labels[p]
         #path = row['Relative Data Location'].strip('\n').strip() # path to the ADCP data, strip formatting characters and spaces
         
         try:
-            ADCP_data[label] = WorkhorseADCP.WorkhorseADCP(path)
+            adcp_file[label] = WorkhorseADCP.WorkhorseADCP(path)
         except: 
             print(f'Cound not read {path}')        
-    return ADCP_data
+    return adcp_file
+#%%
 
+def metadata_table(adcp_file,**kwargs):
+## Add a table with metadata 
 
-#%% plot echo intensites
-def echo_intensity_plot(adcp_file,**kwargs):#plot_by = 'bin',start_bin = None,end_bin = None,start_ensemble = None,end_ensemble = None,title = None):
+    fig,ax = subplots(for_production = True, figheight = 5, figwidth = 5)
+    
+    row_labels = ['File',
+                  'Instrument S/N',
+                  'Beam Facing',
+                  'Instrument Depth (m)',
+                  'Instrument HAB (m)',
+                  'Frequency',
+                  '# Bins',
+                  'First Date',
+                  'Last Date',
+                  'Elapsed Time (hr)',
+                  'First Good Bin',
+                  'Last Good Bin',]
+    
+    try:
+        beam_dir = adcp_file.beam_facing
+        sysfreq  = adcp_file.ensemble_data[0]['SYSTEM CONFIGURATION']['FREQUENCY']
+    except:
+        beam_dir = 'unknown'
+        sysfreq  = 'unknown'
+    
+    cell_text = [adcp_file.filepath.split(os.sep)[-1],
+                 str(adcp_file.ensemble_data[0]['FIXED LEADER']['INSTRUMENT SERIAL NUMBER']),
+                 str(beam_dir),
+                 str(adcp_file.instrument_depth),
+                 str(adcp_file.instrument_HAB),
+                 str(sysfreq),
+                 str(adcp_file.n_bins),
+                 adcp_file.ensemble_times[0].strftime('%d-%b-%y %H:%M:%S'),
+                 adcp_file.ensemble_times[-1].strftime('%d-%b-%y %H:%M:%S'),
+                 str(round((adcp_file.ensemble_times[-1]- adcp_file.ensemble_times[0]).total_seconds()/60/60,2)),
+                 'nan',
+                 'nan',]
+    
+    
+
+
+    def left_justify_list(x):
+        # left jsutify a list of strings so that they all have the same length
+        x = cell_text 
+        max_len = max([len(i) for i in x])
+        
+        for i in range(len(x)):
+            x[i] = x[i].ljust(max_len)
+        return x
+        
+    
+    cell_text = [[i] for i in left_justify_list(cell_text)]    
+    # pad each string on the right to have length 
+    
+    
+    table = ax.table(cellText = cell_text,
+                        rowLabels = row_labels,
+                        rowLoc = 'left',
+                        cellLoc = 'left',
+                        bbox = [0.6,00,.4,1],alpha = 0.4)
+    
+    table.set_fontsize(9)
+            
+    ax.axis('off')
+    ax.grid(False)
+    ax.set_title("File Metadata",pad = 15)
+    
+    return fig,ax
+#%%
+
+def error_velocity_plot(adcp_file,**kwargs):#plot_by = 'bin',start_bin = None,end_bin = None,start_ensemble = None,end_ensemble = None,title = None):
     """
-    Generate a fencegate plot of echo intensities 
+    Generate a fencegate plot of error velocity
 
     Parameters
     ----------
     adcp_file : object
         WorkhorseADCP object.
     plot_by : str
         y-axes plot method ('bin','depth').
@@ -85,134 +154,390 @@
     else: end_ensemble = adcp_file.n_ensembles   
     
     if kwargs.get('title'): title = kwargs.get('title')
     else: title = adcp_file.filepath.split(os.sep)[-1]
     
     
     nbins = (end_bin - start_bin)
-    echo_intensity = adcp_file.get_ensemble_array(beam_number = 0, field_name = 'ECHO INTENSITY')[start_bin:end_bin,start_ensemble:end_ensemble]
+    u,v,z,du,dv,dz,errv = adcp_file.get_velocity()
+    errv = errv.T[start_bin:end_bin,start_ensemble:end_ensemble]
     #echo_intensity = adcp_file.get_ensemble_array(beam_number = 0, field_name = 'CORRELATION MAGNITUDE')[start_bin:end_bin,start_ensemble:end_ensemble]
     ensemble_times = adcp_file.get_ensemble_datetimes()[start_ensemble:end_ensemble]
     
 
     subplot_titles = []
-    fig,ax = subplots(nrow = 1, ncol = 2, figheight = 4, figwidth = 16, width_ratios = [4,1])
+    fig,ax = subplots( figheight = 2.5, figwidth = 10.5, width_ratios = [1])
     
 
     ## format the ADCP data axes (left)
-    topax = ax[0].twiny()
-    ax[0].set_title(title)
+    topax = ax.twiny()
+    ax.set_title(title)
     
     
     # set plot params based on instrument configuration 
 
     
     
     # set plotting extents in vertical direction
     if plot_by == 'bin':
         ylims = [start_bin,end_bin]
-        ax[0].set_ylabel('Bin')
+        ax.set_ylabel('Bin')
     elif plot_by == 'depth':
         bin_depths = adcp_file.get_bin_midpoints_depth()
         ylims = [bin_depths[start_bin],bin_depths[end_bin]]
-        ax[0].set_ylabel('Depth')
+        ax.set_ylabel('Depth')
     elif plot_by == 'HAB':
         bin_heights = adcp_file.get_bin_midpoints_HAB()
         ylims = [bin_heights[start_bin],bin_heights[end_bin]]
-        ax[0].set_ylabel('Height Above Bed')
+        ax.set_ylabel('Height Above Bed')
     else: 
         print('Invalid plot_by parameter')
     
     
     # set plotting extents in horizontal direction
     xlims = mdates.date2num(ensemble_times) # list of elegible xlimits 
     if adcp_file.beam_facing == 'UP':
         extent = [xlims[0],xlims[-1],ylims[0],ylims[1]]
     else:
-        echo_intensity = np.flipud(echo_intensity)
+        errv = np.flipud(errv)
         extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
         
         
-    cmap = plt.cm.Spectral_r
-    im = ax[0].imshow(echo_intensity, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
-    cbar = fig.colorbar(im, ax=ax[0],orientation="vertical",location = 'left',fraction=0.046)
-    cbar.set_label('Echo Intensity', rotation=90,fontsize= 8)
+    cmap = plt.cm.magma
+    im = ax.imshow(errv, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto',norm=mpl.colors.LogNorm())#vmin=-1, vmax=2))# vmin = 0, vmax = np.nanmax(errv))
+    cbar = fig.colorbar(im, ax=ax,orientation="vertical",location = 'right',fraction=0.046)
+    cbar.set_label('Error Velocity (m/s)', rotation=90,fontsize= 12)
+    
+    
+    ax.xaxis.set_major_locator(mticker.FixedLocator(ax.get_xticks()))
+    ax.xaxis.set_major_formatter(mdates.DateFormatter('%H:%M %d%b%y '))
+    topax.set_xlim(start_ensemble,end_ensemble)
+    ax.set_xlabel('Ensemble')
+    ax.grid(alpha = 0.1)
+    ax.set_xticklabels(ax.get_xticklabels(), rotation = -10, ha = 'left')
     
     
+    
+
+    
+    return fig,ax
+
+#%%
+def four_beam_flood_plot(adcp_file,**kwargs):#plot_by = 'bin',start_bin = None,end_bin = None,start_ensemble = None,end_ensemble = None,title = None):
+    """
+    Generate a flooded color plots of correlation magnitude
 
-    ax[0].xaxis.set_major_formatter(mdates.DateFormatter('%H:%M %d%b%y '))
+    Parameters
+    ----------
+    adcp_file : object
+        WorkhorseADCP object.
+    plot_by : str
+        y-axes plot method ('bin','depth').
+    start_bin : int
+        First bin to plot. (use zero based index)
+    end_bin : int
+        Last bin to plot.(use zero based index)
+    start_ensemble : int
+        First ensemble to plot.(use zero based index)
+    end_ensemble : int
+        Last ensemble to plot.(use zero based index)
+    title : str
+        plot axes title.
+
+    Returns
+    -------
+    fig,ax
+        matplotlib figure and axes objects
+
+    """
+    
+    # if adcp_file.ensemble_data[0]['COORDINATE SYSTEM'] != 'BEAM COORDINATES':
+    #     print('Plot feature only implemented for BEAM coordinates')
+
+
+    if kwargs.get('plot_by'):plot_by = kwargs.get('plot_by')
+    else: plot_by = 'bin'
+    
+    if kwargs.get('start_bin'): start_bin = kwargs.get('start_bin')
+    else: start_bin = 0
+    
+    if kwargs.get('end_bin'): end_bin = kwargs.get('end_bin')
+    else: end_bin = adcp_file.n_bins
+    
+
+    if kwargs.get('start_ensemble'): start_ensemble = kwargs.get('start_ensemble')
+    else: start_ensemble = 0
+    
+    if kwargs.get('end_ensemble'): end_ensemble = kwargs.get('end_ensemble')
+    else: end_ensemble = adcp_file.n_ensembles   
+    
+    if kwargs.get('title'): title = kwargs.get('title')
+    else: title = adcp_file.filepath.split(os.sep)[-1]
+    
+    
+    nbins = (end_bin - start_bin)
+
+    if kwargs.get('field'): field = kwargs.get('field')
+    else: field = 'ECHO INTENSITY'
+    
+
+    x1 = adcp_file.get_ensemble_array(field_name = field, beam_number = 0)[start_bin:end_bin,start_ensemble:end_ensemble]
+    x2 = adcp_file.get_ensemble_array(field_name = field, beam_number = 1)[start_bin:end_bin,start_ensemble:end_ensemble]
+    x3 = adcp_file.get_ensemble_array(field_name = field, beam_number = 2)[start_bin:end_bin,start_ensemble:end_ensemble]
+    x4 = adcp_file.get_ensemble_array(field_name = field, beam_number = 3)[start_bin:end_bin,start_ensemble:end_ensemble]
+    
+    
+    #echo_intensity = adcp_file.get_ensemble_array(beam_number = 0, field_name = 'CORRELATION MAGNITUDE')[start_bin:end_bin,start_ensemble:end_ensemble]
+    ensemble_times = adcp_file.get_ensemble_datetimes()[start_ensemble:end_ensemble]
+    
+
+    subplot_titles = []
+    fig,ax = subplots(nrow = 4, ncol = 1, figheight = 8, figwidth = 10.5, width_ratios = [1])
+    
+
+    ## format the ADCP data axes (left)
+    topax = ax[0].twiny()
     topax.set_xlim(start_ensemble,end_ensemble)
-    ax[0].set_xlabel('Ensemble')
-    ax[0].grid(alpha = 0.1)
-    ax[0].set_xticklabels(ax[0].get_xticklabels(), rotation = -30, ha = 'left')
+    ax[0].set_title(field)
     
+    fig.suptitle(title, fontsize = 16)
     
+
+    # set plot params based on instrument configuration 
+
+    def set_axes_labels(axs,ylabel):
+        # function to set the ylabel on a list of axes objects 
+        for ax in axs:
+            ax.set_ylabel(ylabel)
+            
+        return axs
+            
     
-    ## Add a table with metadata 
     
-    row_labels = ['File',
-                  'Instrument S/N',
-                  'Beam Facing',
-                  'Instrument Depth (m)',
-                  'Instrument HAB (m)',
-                  'Frequency',
-                  'First\Last Ensemble',
-                  'First Date',
-                  'Last Date',
-                  'Elapsed Time (hr)',
-                  'Start Bin',
-                  'End Bin',]
+    # set plotting extents in vertical direction
+    if plot_by == 'bin':
+        ylims = [start_bin,end_bin]
+        set_axes_labels(ax,'Bin')
+    elif plot_by == 'depth':
+        bin_depths = adcp_file.get_bin_midpoints_depth()
+        ylims = [bin_depths[start_bin],bin_depths[end_bin]]
+        set_axes_labels(ax,'Depth')
+    elif plot_by == 'HAB':
+        bin_heights = adcp_file.get_bin_midpoints_HAB()
+        ylims = [bin_heights[start_bin],bin_heights[end_bin]]
+        set_axes_labels(ax,'Height Above Bed')
+
+    else: 
+        print('Invalid plot_by parameter')
+        
+        
+        
     
-    try:
-        beam_dir = adcp_file.beam_facing
-        sysfreq  = adcp_file.ensemble_data[0]['SYSTEM CONFIGURATION']['FREQUENCY']
-    except:
-        beam_dir = 'unknown'
-        sysfreq  = 'unknown'
     
-    cell_text = [adcp_file.filepath.split(os.sep)[-1],
-                 str(adcp_file.ensemble_data[0]['FIXED LEADER']['INSTRUMENT SERIAL NUMBER']),
-                 str(beam_dir),
-                 str(adcp_file.instrument_depth),
-                 str(adcp_file.instrument_HAB),
-                 str(sysfreq),
-                 str(start_ensemble)+' - '+str(end_ensemble),
-                 ensemble_times[0].strftime('%d-%b-%y %H:%M:%S'),
-                 ensemble_times[-1].strftime('%d-%b-%y %H:%M:%S'),
-                 str(round((ensemble_times[-1]- ensemble_times[0]).total_seconds()/60/60,2)),
-                 str(start_bin),
-                 str(end_bin),]
+    def get_plot_extent(X):
+        """
+        
+
+        Parameters
+        ----------
+        X : numpy array
+            Input array (ensemble data).
+
+        Returns
+        -------
+        X : numpy array
+            Possibly rotated input array (ensemble data) - to match the sensor orientation.
+            
+        extent : list
+            bounding box for the plotted image.
+
+        """
+   
+    
+        # set plotting extents in horizontal direction
+        xlims = mdates.date2num(ensemble_times) # list of elegible xlimits 
+        if adcp_file.beam_facing == 'UP':
+            extent = [xlims[0],xlims[-1],ylims[0],ylims[1]]
+        else:
+            X = np.flipud(X)
+            extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
+        return X,extent
+        
     
+    cmaps = {'PERCENT GOOD': plt.cm.bone,
+             'ECHO INTENSITY': plt.cm.Spectral_r,
+             'CORRELATION MAGNITUDE': plt.cm.twilight_shifted}
+    cmap = cmaps[field]
     
     
-    def left_justify_list(x):
-        # left jsutify a list of strings so that they all have the same length
-        x = cell_text 
-        max_len = max([len(i) for i in x])
+    vmin = np.nanmin([x1,x2,x3,x4])
+    vmax = np.nanmax([x1,x2,x3,x4])
+    print(vmin)
+    
+    x1,extent = get_plot_extent(x1)
+    im = ax[0].imshow(x1, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
+    
+    x2,extent = get_plot_extent(x2)
+    im = ax[1].imshow(x2, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
+    
+    x3,extent = get_plot_extent(x3)
+    im = ax[2].imshow(x3, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
+    
+    x4,extent = get_plot_extent(x4)
+    im = ax[3].imshow(x4, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
+    
+
+    
+    for i,axes in enumerate(ax):# modify subplot apperance 
+        # set colorbar 
+        cbar = fig.colorbar(im, ax=axes,orientation="vertical",location = 'right',fraction=0.046)
+        cbar.set_label(f'Beam {i+1}', rotation=90,fontsize= 8)
         
-        for i in range(len(x)):
-            x[i] = x[i].ljust(max_len)
-        return x
+        axes.xaxis.set_major_locator(mticker.FixedLocator(axes.get_xticks()))
+        axes.xaxis.set_major_formatter(mdates.DateFormatter('%H:%M %d%b%y '))
+        axes.grid(alpha = 0.1)
+        axes.set_xticklabels(axes.get_xticklabels(), rotation = 0, ha = 'center')
         
+        #axes.text(.5,.5,f'PG{i+1}',transform = ax. transAxes)
+        #axes.text(0.5, 0.5, 'matplotlib')#, horizontalalignment='center',verticalalignment='center', transform=ax.transAxes)
+        #path_effects=[mpl_path_effects.Stroke(linewidth=.25, foreground="black",alpha = .75)] 
+        #axes.text(.025,.8,f'Percent Good {i}',transform = axes.transAxes, fontsize = 8, color = 'white',path_effects = path_effects)
+    ax[-1].set_xlabel('Ensemble')
     
-    cell_text = [[i] for i in left_justify_list(cell_text)]    
-    # pad each string on the right to have length 
     
+
     
-    table = ax[1].table(cellText = cell_text,
-                        rowLabels = row_labels,
-                        rowLoc = 'left',
-                        cellLoc = 'left',
-                        bbox = [0.35,0,.95,1],alpha = 0.4)
+    return fig,ax
+
+
+
+#%%
+def single_beam_flood_plot(adcp_file,**kwargs):#plot_by = 'bin',start_bin = None,end_bin = None,start_ensemble = None,end_ensemble = None,title = None):
+    """
+    Generate a fencegate plot of ensemble data
+
+    Parameters
+    ----------
+    adcp_file : object
+        WorkhorseADCP object.
+    plot_by : str
+        y-axes plot method ('bin','depth').
+    start_bin : int
+        First bin to plot. (use zero based index)
+    end_bin : int
+        Last bin to plot.(use zero based index)
+    start_ensemble : int
+        First ensemble to plot.(use zero based index)
+    end_ensemble : int
+        Last ensemble to plot.(use zero based index)
+    title : str
+        plot axes title.
+
+    Returns
+    -------
+    fig,ax
+        matplotlib figure and axes objects
+
+    """
+
+
+    if kwargs.get('plot_by'):plot_by = kwargs.get('plot_by')
+    else: plot_by = 'bin'
     
-    table.set_fontsize(9)
-            
-    ax[1].axis('off')
-    ax[1].grid(False)
-    ax[1].set_title("File Metadata",pad = 15)
+    if kwargs.get('start_bin'): start_bin = kwargs.get('start_bin')
+    else: start_bin = 0
+    
+    if kwargs.get('end_bin'): end_bin = kwargs.get('end_bin')
+    else: end_bin = adcp_file.n_bins
+
+    if kwargs.get('start_ensemble'): start_ensemble = kwargs.get('start_ensemble')
+    else: start_ensemble = 0
+    
+    if kwargs.get('end_ensemble'): end_ensemble = kwargs.get('end_ensemble')
+    else: end_ensemble = adcp_file.n_ensembles   
+    
+    if kwargs.get('title'): title = kwargs.get('title')
+    else: title = adcp_file.filepath.split(os.sep)[-1]
+    
+    if kwargs.get('field'): field = kwargs.get('field')
+    else: field = 'ECHO INTENSITY'
+    
+    if kwargs.get('beam'): beam = kwargs.get('beam')
+    else: beam = 0
+    
+    if beam == 'average': beam = 0 
+    
+    
+    nbins = (end_bin - start_bin)
+    x = adcp_file.get_ensemble_array(beam_number = 0, field_name = field)[start_bin:end_bin,start_ensemble:end_ensemble]
+    #echo_intensity = adcp_file.get_ensemble_array(beam_number = 0, field_name = 'CORRELATION MAGNITUDE')[start_bin:end_bin,start_ensemble:end_ensemble]
+    ensemble_times = adcp_file.get_ensemble_datetimes()[start_ensemble:end_ensemble]
+    
+
+    subplot_titles = []
+    fig,ax = subplots( figheight = 2.5, figwidth = 10.5, width_ratios = [1])
+    
+
+    ## format the ADCP data axes (left)
+    topax = ax.twiny()
+    ax.set_title(title)
+    
+    
+    # set plot params based on instrument configuration 
+
+    
+    
+    # set plotting extents in vertical direction
+    if plot_by == 'bin':
+        ylims = [start_bin,end_bin]
+        ax.set_ylabel('Bin')
+    elif plot_by == 'depth':
+        bin_depths = adcp_file.get_bin_midpoints_depth()
+        ylims = [bin_depths[start_bin],bin_depths[end_bin]]
+        ax.set_ylabel('Depth')
+    elif plot_by == 'HAB':
+        bin_heights = adcp_file.get_bin_midpoints_HAB()
+        ylims = [bin_heights[start_bin],bin_heights[end_bin]]
+        ax.set_ylabel('Height Above Bed')
+    else: 
+        print('Invalid plot_by parameter')
+    
+    
+    # set plotting extents in horizontal direction
+    xlims = mdates.date2num(ensemble_times) # list of elegible xlimits 
+    if adcp_file.beam_facing == 'UP':
+        extent = [xlims[0],xlims[-1],ylims[0],ylims[1]]
+    else:
+        x = np.flipud(x)
+        extent = [xlims[0],xlims[-1],ylims[1],ylims[0]]
+        
+        
+    cmaps = {'PERCENT GOOD': plt.cm.bone,
+             'ECHO INTENSITY': plt.cm.Spectral_r,
+             'CORRELATION MAGNITUDE': plt.cm.twilight_shifted}
+    cmap = cmaps[field]
+    
+    im = ax.imshow(x, origin = 'lower', extent = extent, cmap = cmap, aspect = 'auto')
+    cbar = fig.colorbar(im, ax=ax,orientation="vertical",location = 'right',fraction=0.046)
+    
+    if beam == 0:
+        cbar_label = f'{field}\n BEAM AVERAGE' 
+    else:
+        cbar_label = f'{field}\n BEAM {beam}' 
+    cbar.set_label(cbar_label, rotation=90,fontsize= 9)
+    
+    
+    ax.xaxis.set_major_locator(mticker.FixedLocator(ax.get_xticks()))
+    ax.xaxis.set_major_formatter(mdates.DateFormatter('%H:%M %d%b%y '))
+    topax.set_xlim(start_ensemble,end_ensemble)
+    ax.set_xlabel('Ensemble')
+    ax.grid(alpha = 0.1)
+    ax.set_xticklabels(ax.get_xticklabels(), rotation = 0, ha = 'left')
+    
+
     
     return fig,ax
 
 
 #%%
 def progressive_vector_plot(adcp_file,**kwargs):
     """
@@ -261,17 +586,17 @@
     if kwargs.get('end_ensemble'): end_ensemble= kwargs.get('end_ensemble')
     else: end_ensemble = adcp_file.n_ensembles   
     
     if kwargs.get('title'): title = kwargs.get('title')
     else: title = adcp_file.filepath.split(os.sep)[-1]     
     
 
-    print(start_ensemble)
+
     
-    #adcp_file = ADCP_data[ID]
+    #adcp_file = adcp_file[ID]
     # start_ensemble = 0
     # end_ensemble = adcp_file.n_ensembles
     # start_bin = 0
     # end_bin = adcp_file.n_bins-1
     #color_by = 'bin' #velocity'  #bin'#'velocity'#'bin'
     
     
@@ -301,25 +626,25 @@
     
     
     if plot:
         # fig = plt.figure()
         # ax = plt.gca()
         #fig, ax = plt.subplots(1, 2,gridspec_kw={'width_ratios': [3, 1]})
         
-        fig,ax = DHI_subplots(nrow = 1, ncol = 2, figheight = 7, figwidth =9, width_ratios = [3,1])
+        fig,ax = subplots( figheight = 5, figwidth =5.5, width_ratios = [1])
  
-        #ax[0].set_aspect('equal')
-        ax[0].grid(alpha = 0.3)
-        ax[0].set_xlabel('East Distance (m)')
-        ax[0].set_ylabel('North Distance (m)')
-        ax[0].set_title(title)
-        #ax[0].set_aspect('equal',adjustable = 'datalim')
+        #ax.set_aspect('equal')
+        ax.grid(alpha = 0.3)
+        ax.set_xlabel('East Distance (m)')
+        ax.set_ylabel('North Distance (m)')
+        ax.set_title(title)
+        #ax.set_aspect('equal',adjustable = 'datalim')
         
 
-        cbar_shrink = .043#.75
+        cbar_shrink = .046#.75
         global points,segments
         
         if color_by == 'bin':
 
             cmap = plt.cm.Spectral  # define the colormap
             # extract all colors from the .jet map
             cmaplist = [cmap(i) for i in range(cmap.N)]
@@ -330,40 +655,40 @@
             cmap = mpl.colors.LinearSegmentedColormap.from_list(
                 'Custom cmap', cmaplist, cmap.N)
             
             # define the bins and normalize
             bounds = np.linspace(0, nbins, nbins+1)
             norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
             for b in range(nbins):
-                #ax[0].plot(pu[:,b],pv[:,b], label = f'Bin {start_bin+b}')#, c = cmap(b), norm = norm)#,color = colors[s],alpha = 0.6)
+                #ax.plot(pu[:,b],pv[:,b], label = f'Bin {start_bin+b}')#, c = cmap(b), norm = norm)#,color = colors[s],alpha = 0.6)
     
                 points = np.array((pu[:-1,b], pv[:-1,b])).T.reshape(-1, 1, 2)
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
                 #norm = plt.Normalize(0, adcp_file.n_bins,1)
                 lines = LineCollection(segments, cmap=cmap, norm=norm)
                 lines.set_array(len(points)*[b])
                 lines.set_linewidth(1)
-                line = ax[0].add_collection(lines)           
-            cbar = fig.colorbar(line, ax=ax[0],orientation="horizontal", pad=.2, fraction=cbar_shrink)
-            cbar.set_label('Bin Number', rotation=0)
+                line = ax.add_collection(lines)           
+            cbar = fig.colorbar(line, ax=ax,orientation="vertical")
+            cbar.set_label('Bin Number', rotation=270, labelpad = 10, fontsize = 12)
     
     
         elif color_by == 'velocity':
             cmap = plt.cm.jet
             for b in range(nbins):
                 points = np.array((pu[:-1,b], pv[1:,b])).T.reshape(-1, 1, 2)
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
                 norm = plt.Normalize(0, np.quantile(xy_speed[~np.isnan(xy_speed)],0.99))
                 lines = LineCollection(segments, cmap=cmap, norm=norm)
                 lines.set_array(xy_speed[:,b])
                 lines.set_linewidth(1)
-                line = ax[0].add_collection(lines)
+                line = ax.add_collection(lines)
                 #break
-            cbar = fig.colorbar(line, ax=ax[0],orientation="horizontal", pad=.2, fraction = cbar_shrink)
-            cbar.set_label('Velocity (m/s) ', rotation=0)
+            cbar = fig.colorbar(line, ax=ax,orientation="vertical")
+            cbar.set_label('Velocity (m/s) ', rotation=270, labelpad = 10, fontsize = 12)
             
         elif color_by == 'month':
             cmap = plt.cm.get_cmap('tab20b', 12)
             def gen_interval(x):
                 x = x.isoweekday()
                 return x
             vgen_interval = np.vectorize(gen_interval)
@@ -371,104 +696,37 @@
             for b in range(nbins):
                 points = np.array((pu[:-1,b], pv[1:,b])).T.reshape(-1, 1, 2)
                 segments = np.concatenate([points[:-1], points[1:]], axis=1)
                 norm = plt.Normalize(1,12)
                 lines = LineCollection(segments, cmap=cmap, norm=norm)
                 lines.set_array(months)
                 lines.set_linewidth(1)
-                line = ax[0].add_collection(lines)
+                line = ax.add_collection(lines)
                 #break
-            cbar = fig.colorbar(line, ax=ax[0],orientation="horizontal", pad=.2, fraction = cbar_shrink)
-            cbar.set_label('Month of Year', rotation=0)        
+            cbar = fig.colorbar(line, ax=ax,orientation="vertical")
+            cbar.set_label('Month of Year', rotation=270, labelpad = 10, fontsize = 12)        
             
             
         else:
             print(r'Invalid plot mode {color_by}')
     
         #set axes limits 
         xrange = 1.1*(np.nanmax(abs(pu)))
         yrange = 1.1*(np.nanmax(abs(pv)))
         
         rng = max(xrange,yrange)
         #print([np.nanmax(pu),xrange])
         # ax.set_xbound([-xrange,xrange])
         # ax.set_ybound([-yrange,yrange])
         
-        ax[0].set_xlim(-rng,rng)
-        ax[0].set_ylim(-rng,rng)
+        ax.set_xlim(-rng,rng)
+        ax.set_ylim(-rng,rng)
     
-        ax[0].set_aspect('equal')
-        ## Add a table with metadata 
-        
-        row_labels = ['File',
-                      'Instrument S/N',
-                      'Beam Facing',
-                      'Frequency',
-                      'First\Last Ensemble',
-                      'First Date',
-                      'Last Date',
-                      'Elapsed Time (hr)',
-                      'Start Bin',
-                      'End Bin',
-                      'Mean Speed (m/s)',
-                      'StD Speed (m/s)',]
-        try:
-            beam_dir = adcp_file.beam_facing
-            sysfreq  = adcp_file.ensemble_data[0]['SYSTEM CONFIGURATION']['FREQUENCY']
-        except:
-            beam_dir = 'unknown'
-            sysfreq  = 'unknown'
-               
-        cell_text = [adcp_file.filepath.split(os.sep)[-1],
-                     str(adcp_file.ensemble_data[0]['FIXED LEADER']['INSTRUMENT SERIAL NUMBER']),
-                     beam_dir,
-                     sysfreq,
-                     str(start_ensemble)+' - '+str(end_ensemble),
-                     ensemble_times[0].strftime('%d-%b-%y %H:%M:%S'),
-                     ensemble_times[-1].strftime('%d-%b-%y %H:%M:%S'),
-                     str((ensemble_times[-1]- ensemble_times[0]).total_seconds()/60/60),
-                     str(start_bin),
-                     str(end_bin),
-                     str(round(np.nanmean(xy_speed),1)),
-                     str(round(np.nanstd(xy_speed),1))]
-        
-        
-        
-        def left_justify_list(x):
-            # left jsutify a list of strings so that they all have the same length
-            x = cell_text 
-            max_len = max([len(i) for i in x])
-            
-            for i in range(len(x)):
-                x[i] = x[i].ljust(max_len)
-            return x
-            
-        
-        cell_text = [[i] for i in left_justify_list(cell_text)]    
-        # pad each string on the right to have length 
-        
-        
-        table = ax[1].table(cellText = cell_text,
-                            rowLabels = row_labels,
-                            rowLoc = 'left',
-                            cellLoc = 'left',
-                            bbox = [0.4,0.5,1,.5],alpha = 0.4)
-        
-        table.set_fontsize(9)
-                
-        ax[1].axis('off')
-        ax[1].grid(False)
-        ax[1].set_title("File Metadata")
-        
-    # progressive_vector_plot(ADCP_data[ID],
-    #                         color_by = 'velocity',
-    #                         start_bin = start_bin,
-    #                         end_bin = end_bin,
-    #                         start_ensemble = start_ensemble,
-    #                         end_ensemble = end_ensemble)
+        ax.set_aspect('equal')
+
     return fig,ax
 #%%
```

### Comparing `oceanograpy-0.0.3/oceanograpy/example.py` & `oceanograpy-0.0.4/oceanograpy/example.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,36 +7,68 @@
 
 from workhorse_adcp import workhorse_adcp as wh_adcp 
 from seabird_ctd import seabird_ctd as sb_ctd 
 import processing_tools as ptools 
 from matplotlib_dhi import subplots 
 import adcp_plot_tools
 
+import matplotlib.pyplot as plt
+import matplotlib as mpl
 
 pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Config\ROV_ADCP_20161_PT3.txt'
 adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\ROV\Island Pride HD14\ADCP\Raw\ADCP_24142_600kHz\ROV_ADCP_12102022\_RDI_005.000'
 
 
 
-# pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Config_File\FBCT02_P3_TEST_17112022.txt'
-# adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Raw\FBCT2_Full_Download_17112022\FBCT2000.000'
+pt3_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Config_File\FBCT02_P3_TEST_17112022.txt'
+adcp_filepath = r'\\USDEN1-STOR.DHI.DK\Projects\41806287\41806287 NORI-D Data\Data\Fixed Stations\02_Fixed_Bottom_Current_Turbidity\02_FBCT2\01_ADCP_600kHz-24144\Raw\FBCT2_Full_Download_17112022\FBCT2000.000'
 
 
 adcp_data = wh_adcp(filepath = adcp_filepath, PT3_filepath = pt3_filepath, verbose = 1)
 
 
 
 #%%
 
 import adcp_plot_tools
 import processing_tools as ptools
-#adcp_plot_tools.progressive_vector_plot(adcp_data)#, color_by , start_bin, end_bin, start_ensemble, end_ensemble, title)
+from matplotlib_dhi import subplots
 
-#adcp_plot_tools.echo_intensity_plot(adcp_data)
+import os
+
+
+adcp_plot_tools.progressive_vector_plot(adcp_data)#, color_by , start_bin, end_bin, start_ensemble, end_ensemble, title)
+fig,ax = adcp_plot_tools.error_velocity_plot(adcp_data)
+
+fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'ECHO INTENSITY')
+fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'CORRELATION MAGNITUDE')
+fig,ax = adcp_plot_tools.four_beam_flood_plot(adcp_data,field = 'PERCENT GOOD')
+
+fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'ECHO INTENSITY')
+fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'CORRELATION MAGNITUDE')
+fig,ax = adcp_plot_tools.single_beam_flood_plot(adcp_data,field = 'PERCENT GOOD')
+#fig,ax = adcp_plot_tools.metadata_table(adcp_data)
+
+
+
+
+
+
+
+#%% correlation magnitude plots 
+
+
+
+#%% Auto QAQC
+
+
+
+
+
+
+
+
+#%% Add position data 
 
 
-from matplotlib_dhi import subplots
 
 
-fig,axs = subplots()
-adcp_plot_tools.echo_intensity_plot(adcp_data)#, start_ensemble = 250, end_ensemble = 1000)
-adcp_plot_tools.progressive_vector_plot(adcp_data)#, color_by , start_bin, end_bin, start_ensemble, end_ensemble, title)
```

### Comparing `oceanograpy-0.0.3/oceanograpy/frma.py` & `oceanograpy-0.0.4/oceanograpy/frma.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.3/oceanograpy/processing_tools.py` & `oceanograpy-0.0.4/oceanograpy/processing_tools.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.3/oceanograpy/seabird_ctd.py` & `oceanograpy-0.0.4/oceanograpy/seabird_ctd.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.3/oceanograpy/workhorse_adcp.py` & `oceanograpy-0.0.4/oceanograpy/workhorse_adcp.py`

 * *Files identical despite different names*

### Comparing `oceanograpy-0.0.3/oceanograpy.egg-info/PKG-INFO` & `oceanograpy-0.0.4/oceanograpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanograpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Toolbox for importing and plotting ADCP and CTD data
 Home-page:  
 Author: Andy Banks
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `oceanograpy-0.0.3/setup.py` & `oceanograpy-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oceanograpy",
-    version="0.0.3",
+    version="0.0.4",
     author="Andy Banks",
     author_email="",
     description="Toolbox for importing and plotting ADCP and CTD data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url=" ",
     packages=["oceanograpy"],
```

