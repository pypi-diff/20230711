# Comparing `tmp/hstaxe-1.0.4.tar.gz` & `tmp/hstaxe-1.0.5.tar.gz`

## Comparing `hstaxe-1.0.4.tar` & `hstaxe-1.0.5.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/Makefile.am
--rwxr-xr-x   0        0        0    47386 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/autogen.sh
--rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/configure.ac
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/Makefile.am
--rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_AF2PET.c
--rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_BE.c
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_CHECK.c
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DIRIMAGE.c
--rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DRZ2PET.c
--rw-r--r--   0        0        0    21905 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_DRZPREP.c
--rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FILET.c
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FILET2.c
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FRIGEN.c
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_FRINGECORR.c
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_GOL2AF.c
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_GPS.c
--rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_INTPIXCORR.c
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_NICBACK.c
--rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PET2SPC.c
--rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETCONT.c
--rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETFF.c
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_PETIPC.c
--rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_SCALEBCK.c
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_SEX2GOL.c
--rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_STAMPS.c
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_TEST.c
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_TFIT.c
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_errors.c
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_errors.h
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_grism.h
--rw-r--r--   0        0        0    59634 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_utils.c
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aXe_utils.h
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_check.c
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_check.h
--rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_conf.c
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/aper_conf.h
--rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/crossdisp_utils.c
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/crossdisp_utils.h
--rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/dirimage_model.c
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/dirimage_model.h
--rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/disp_conf.c
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/disp_conf.h
--rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drizzle_utils.c
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drizzle_utils.h
--rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drz2pet_utils.c
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/drz2pet_utils.h
--rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_conf.c
--rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_conf.h
--rw-r--r--   0        0        0    36951 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_model.c
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_model.h
--rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_utils.c
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/fringe_utils.h
--rw-r--r--   0        0        0    19909 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inima_utils.c
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inima_utils.h
--rw-r--r--   0        0        0    36861 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inout_aper.c
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/inout_aper.h
--rw-r--r--   0        0        0    40593 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/ipixcorr_utils.c
--rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/ipixcorr_utils.h
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lm_eval.c
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lm_eval.h
--rw-r--r--   0        0        0    40331 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lmmin.c
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/lmmin.h
--rw-r--r--   0        0        0    66123 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/model_utils.c
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/model_utils.h
--rw-r--r--   0        0        0    16948 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/nicback_utils.c
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/nicback_utils.h
--rw-r--r--   0        0        0    19499 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/scaleback_utils.c
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/scaleback_utils.h
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_CD.c
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_CD.h
--rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_FITScards.c
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_FITScards.h
--rw-r--r--   0        0        0    53062 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_back.c
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_back.h
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_cfg.c
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_cfg.h
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_driz.c
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_driz.h
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_extract.c
--rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_flatfield.c
--rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_flatfield.h
--rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_fluxcube.c
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_fluxcube.h
--rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_model.c
--rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_model.h
--rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_optimum.c
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_optimum.h
--rw-r--r--   0        0        0    38085 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_resp.c
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_resp.h
--rw-r--r--   0        0        0    68507 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_sex.c
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_sex.h
--rw-r--r--   0        0        0    45638 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_spc.c
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_spc.h
--rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_trace_functions.c
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_trace_functions.h
--rw-r--r--   0        0        0    31304 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_utils.c
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_utils.h
--rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_wl_calib.c
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spc_wl_calib.h
--rw-r--r--   0        0        0    31020 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_PET.c
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_PET.h
--rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_binning.c
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_binning.h
--rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_fitting.c
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_fitting.h
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_is_in.c
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_is_in.h
--rw-r--r--   0        0        0    35494 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_output.c
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_output.h
--rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pathlength.c
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pathlength.h
--rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pgp.c
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_pgp.h
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_sect.c
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/spce_sect.h
--rw-r--r--   0        0        0    19457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/specmodel_utils.c
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/specmodel_utils.h
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/test_aper_check.c
--rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trace_conf.c
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trace_conf.h
--rw-r--r--   0        0        0    40360 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trfit_utils.c
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 hstaxe-1.0.4/cextern/src/trfit_utils.h
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/_version.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axeException.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axeerror.py
--rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/config.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/utils.py
--rw-r--r--   0        0        0    37795 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/WCSdata.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/__init__.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/axesim_verify.py
--rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/axesimtasks.py
--rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/imagemaker.py
--rw-r--r--   0        0        0    27371 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/interpolator.py
--rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/modspeclist.py
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/realworld.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/templateimages.py
--rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesim/templatespectra.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/__init__.py
--rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axecommands.py
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axeinputs.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axeiol.py
--rw-r--r--   0        0        0    63246 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axelowlev.py
--rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axepreptor.py
--rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axesingextr.py
--rw-r--r--   0        0        0    30236 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/axetasks.py
--rw-r--r--   0        0        0    46451 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/configfile.py
--rw-r--r--   0        0        0    25435 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/dither.py
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/dppdumps.py
--rw-r--r--   0        0        0    59736 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/drizzleobjects.py
--rwxr-xr-x   0        0        0    34257 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/fcubeobjs.py
--rw-r--r--   0        0        0     8263 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/imagemaker.py
--rw-r--r--   0        0        0    25721 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/inputchecks.py
--rw-r--r--   0        0        0    15477 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/iolmaking.py
--rw-r--r--   0        0        0    18555 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/mefobjects.py
--rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/nlincoeffs.py
--rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/axesrc/pysex2gol.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/coveragerc
--rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_acs_cookbook.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_cookbook.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/run_cookbook_part2.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_af2pet.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_axecore.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_axeprep.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_be.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_gol2af.py
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_iolprep.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_pet2spc.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_petcont.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_petff.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_scalebck.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_sex2gol.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hstaxe/tests/test_stamps.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 hstaxe-1.0.4/.gitignore
--rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 hstaxe-1.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 hstaxe-1.0.4/README.md
--rwxr-xr-x   0        0        0     6331 2020-02-02 00:00:00.000000 hstaxe-1.0.4/hatch_build.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hstaxe-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 hstaxe-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/Makefile.am
+-rwxr-xr-x   0        0        0    47386 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/autogen.sh
+-rw-r--r--   0        0        0     4086 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/configure.ac
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/Makefile.am
+-rw-r--r--   0        0        0    13666 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_AF2PET.c
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_BE.c
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_CHECK.c
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_DIRIMAGE.c
+-rw-r--r--   0        0        0    12938 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_DRZ2PET.c
+-rw-r--r--   0        0        0    21905 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_DRZPREP.c
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_FILET.c
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_FILET2.c
+-rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_FRIGEN.c
+-rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_FRINGECORR.c
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_GOL2AF.c
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_GPS.c
+-rw-r--r--   0        0        0    12125 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_INTPIXCORR.c
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_NICBACK.c
+-rw-r--r--   0        0        0    22007 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_PET2SPC.c
+-rw-r--r--   0        0        0     8865 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_PETCONT.c
+-rw-r--r--   0        0        0     6982 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_PETFF.c
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_PETIPC.c
+-rw-r--r--   0        0        0     4505 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_SCALEBCK.c
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_SEX2GOL.c
+-rw-r--r--   0        0        0    11132 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_STAMPS.c
+-rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_TEST.c
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_TFIT.c
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_errors.c
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_errors.h
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_grism.h
+-rw-r--r--   0        0        0    59634 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_utils.c
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aXe_utils.h
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aper_check.c
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aper_check.h
+-rw-r--r--   0        0        0    17573 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aper_conf.c
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/aper_conf.h
+-rw-r--r--   0        0        0    17300 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/crossdisp_utils.c
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/crossdisp_utils.h
+-rw-r--r--   0        0        0    12100 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/dirimage_model.c
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/dirimage_model.h
+-rw-r--r--   0        0        0    15253 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/disp_conf.c
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/disp_conf.h
+-rw-r--r--   0        0        0    23363 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/drizzle_utils.c
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/drizzle_utils.h
+-rw-r--r--   0        0        0    13393 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/drz2pet_utils.c
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/drz2pet_utils.h
+-rw-r--r--   0        0        0    28363 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_conf.c
+-rw-r--r--   0        0        0     4092 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_conf.h
+-rw-r--r--   0        0        0    36951 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_model.c
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_model.h
+-rw-r--r--   0        0        0    17807 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_utils.c
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/fringe_utils.h
+-rw-r--r--   0        0        0    19909 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/inima_utils.c
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/inima_utils.h
+-rw-r--r--   0        0        0    36861 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/inout_aper.c
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/inout_aper.h
+-rw-r--r--   0        0        0    40593 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/ipixcorr_utils.c
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/ipixcorr_utils.h
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/lm_eval.c
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/lm_eval.h
+-rw-r--r--   0        0        0    40331 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/lmmin.c
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/lmmin.h
+-rw-r--r--   0        0        0    66123 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/model_utils.c
+-rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/model_utils.h
+-rw-r--r--   0        0        0    16948 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/nicback_utils.c
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/nicback_utils.h
+-rw-r--r--   0        0        0    19499 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/scaleback_utils.c
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/scaleback_utils.h
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_CD.c
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_CD.h
+-rw-r--r--   0        0        0    26558 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_FITScards.c
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_FITScards.h
+-rw-r--r--   0        0        0    53062 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_back.c
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_back.h
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_cfg.c
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_cfg.h
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_driz.c
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_driz.h
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_extract.c
+-rw-r--r--   0        0        0    13647 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_flatfield.c
+-rw-r--r--   0        0        0     2886 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_flatfield.h
+-rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_fluxcube.c
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_fluxcube.h
+-rw-r--r--   0        0        0    61035 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_model.c
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_model.h
+-rw-r--r--   0        0        0    17812 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_optimum.c
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_optimum.h
+-rw-r--r--   0        0        0    38085 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_resp.c
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_resp.h
+-rw-r--r--   0        0        0    68507 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_sex.c
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_sex.h
+-rw-r--r--   0        0        0    45638 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_spc.c
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_spc.h
+-rw-r--r--   0        0        0     8398 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_trace_functions.c
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_trace_functions.h
+-rw-r--r--   0        0        0    31304 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_utils.c
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_utils.h
+-rw-r--r--   0        0        0     8358 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_wl_calib.c
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spc_wl_calib.h
+-rw-r--r--   0        0        0    31020 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_PET.c
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_PET.h
+-rw-r--r--   0        0        0    19966 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_binning.c
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_binning.h
+-rw-r--r--   0        0        0    15394 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_fitting.c
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_fitting.h
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_is_in.c
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_is_in.h
+-rw-r--r--   0        0        0    35494 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_output.c
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_output.h
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_pathlength.c
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_pathlength.h
+-rw-r--r--   0        0        0     5442 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_pgp.c
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_pgp.h
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_sect.c
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/spce_sect.h
+-rw-r--r--   0        0        0    19457 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/specmodel_utils.c
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/specmodel_utils.h
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/test_aper_check.c
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/trace_conf.c
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/trace_conf.h
+-rw-r--r--   0        0        0    40360 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/trfit_utils.c
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 hstaxe-1.0.5/cextern/src/trfit_utils.h
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/_version.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axeException.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axeerror.py
+-rw-r--r--   0        0        0    11529 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/config.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/utils.py
+-rw-r--r--   0        0        0    37795 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/WCSdata.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/__init__.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/axesim_verify.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/axesimtasks.py
+-rw-r--r--   0        0        0     8187 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/imagemaker.py
+-rw-r--r--   0        0        0    27371 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/interpolator.py
+-rw-r--r--   0        0        0    12873 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/modspeclist.py
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/realworld.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/templateimages.py
+-rw-r--r--   0        0        0    17457 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesim/templatespectra.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/__init__.py
+-rw-r--r--   0        0        0    16190 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axecommands.py
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axeinputs.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axeiol.py
+-rw-r--r--   0        0        0    63246 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axelowlev.py
+-rw-r--r--   0        0        0    22432 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axepreptor.py
+-rw-r--r--   0        0        0     8556 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axesingextr.py
+-rw-r--r--   0        0        0    30236 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/axetasks.py
+-rw-r--r--   0        0        0    46451 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/configfile.py
+-rw-r--r--   0        0        0    25435 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/dither.py
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/dppdumps.py
+-rw-r--r--   0        0        0    59736 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/drizzleobjects.py
+-rwxr-xr-x   0        0        0    34257 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/fcubeobjs.py
+-rw-r--r--   0        0        0     8263 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/imagemaker.py
+-rw-r--r--   0        0        0    25721 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/inputchecks.py
+-rw-r--r--   0        0        0    15477 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/iolmaking.py
+-rw-r--r--   0        0        0    18555 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/mefobjects.py
+-rw-r--r--   0        0        0     5741 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/nlincoeffs.py
+-rw-r--r--   0        0        0    14443 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/axesrc/pysex2gol.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/coveragerc
+-rwxr-xr-x   0        0        0     4014 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/run_acs_cookbook.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/run_cookbook.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/run_cookbook_part2.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_af2pet.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_axecore.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_axeprep.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_be.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_gol2af.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_iolprep.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_pet2spc.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_petcont.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_petff.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_scalebck.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_sex2gol.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hstaxe/tests/test_stamps.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 hstaxe-1.0.5/.gitignore
+-rw-r--r--   0        0        0    36800 2020-02-02 00:00:00.000000 hstaxe-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 hstaxe-1.0.5/README.md
+-rwxr-xr-x   0        0        0     6331 2020-02-02 00:00:00.000000 hstaxe-1.0.5/hatch_build.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hstaxe-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 hstaxe-1.0.5/PKG-INFO
```

### Comparing `hstaxe-1.0.4/cextern/autogen.sh` & `hstaxe-1.0.5/cextern/autogen.sh`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/configure.ac` & `hstaxe-1.0.5/cextern/configure.ac`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/Makefile.am` & `hstaxe-1.0.5/cextern/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_AF2PET.c` & `hstaxe-1.0.5/cextern/src/aXe_AF2PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_BE.c` & `hstaxe-1.0.5/cextern/src/aXe_BE.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_CHECK.c` & `hstaxe-1.0.5/cextern/src/aXe_CHECK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_DIRIMAGE.c` & `hstaxe-1.0.5/cextern/src/aXe_DIRIMAGE.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_DRZ2PET.c` & `hstaxe-1.0.5/cextern/src/aXe_DRZ2PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_DRZPREP.c` & `hstaxe-1.0.5/cextern/src/aXe_DRZPREP.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_FILET.c` & `hstaxe-1.0.5/cextern/src/aXe_FILET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_FILET2.c` & `hstaxe-1.0.5/cextern/src/aXe_FILET2.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_FRIGEN.c` & `hstaxe-1.0.5/cextern/src/aXe_FRIGEN.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_FRINGECORR.c` & `hstaxe-1.0.5/cextern/src/aXe_FRINGECORR.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_GOL2AF.c` & `hstaxe-1.0.5/cextern/src/aXe_GOL2AF.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_GPS.c` & `hstaxe-1.0.5/cextern/src/aXe_GPS.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_INTPIXCORR.c` & `hstaxe-1.0.5/cextern/src/aXe_INTPIXCORR.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_NICBACK.c` & `hstaxe-1.0.5/cextern/src/aXe_NICBACK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_PET2SPC.c` & `hstaxe-1.0.5/cextern/src/aXe_PET2SPC.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_PETCONT.c` & `hstaxe-1.0.5/cextern/src/aXe_PETCONT.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_PETFF.c` & `hstaxe-1.0.5/cextern/src/aXe_PETFF.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_PETIPC.c` & `hstaxe-1.0.5/cextern/src/aXe_PETIPC.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_SCALEBCK.c` & `hstaxe-1.0.5/cextern/src/aXe_SCALEBCK.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_SEX2GOL.c` & `hstaxe-1.0.5/cextern/src/aXe_SEX2GOL.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_STAMPS.c` & `hstaxe-1.0.5/cextern/src/aXe_STAMPS.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_TEST.c` & `hstaxe-1.0.5/cextern/src/aXe_TEST.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_TFIT.c` & `hstaxe-1.0.5/cextern/src/aXe_TFIT.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_errors.c` & `hstaxe-1.0.5/cextern/src/aXe_errors.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_grism.h` & `hstaxe-1.0.5/cextern/src/aXe_grism.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_utils.c` & `hstaxe-1.0.5/cextern/src/aXe_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aXe_utils.h` & `hstaxe-1.0.5/cextern/src/aXe_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aper_check.c` & `hstaxe-1.0.5/cextern/src/aper_check.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aper_conf.c` & `hstaxe-1.0.5/cextern/src/aper_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/aper_conf.h` & `hstaxe-1.0.5/cextern/src/aper_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/crossdisp_utils.c` & `hstaxe-1.0.5/cextern/src/crossdisp_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/crossdisp_utils.h` & `hstaxe-1.0.5/cextern/src/crossdisp_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/dirimage_model.c` & `hstaxe-1.0.5/cextern/src/dirimage_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/dirimage_model.h` & `hstaxe-1.0.5/cextern/src/dirimage_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/disp_conf.c` & `hstaxe-1.0.5/cextern/src/disp_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/disp_conf.h` & `hstaxe-1.0.5/cextern/src/disp_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/drizzle_utils.c` & `hstaxe-1.0.5/cextern/src/drizzle_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/drizzle_utils.h` & `hstaxe-1.0.5/cextern/src/drizzle_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/drz2pet_utils.c` & `hstaxe-1.0.5/cextern/src/drz2pet_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/drz2pet_utils.h` & `hstaxe-1.0.5/cextern/src/drz2pet_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_conf.c` & `hstaxe-1.0.5/cextern/src/fringe_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_conf.h` & `hstaxe-1.0.5/cextern/src/fringe_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_model.c` & `hstaxe-1.0.5/cextern/src/fringe_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_model.h` & `hstaxe-1.0.5/cextern/src/fringe_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_utils.c` & `hstaxe-1.0.5/cextern/src/fringe_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/fringe_utils.h` & `hstaxe-1.0.5/cextern/src/fringe_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/inima_utils.c` & `hstaxe-1.0.5/cextern/src/inima_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/inima_utils.h` & `hstaxe-1.0.5/cextern/src/inima_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/inout_aper.c` & `hstaxe-1.0.5/cextern/src/inout_aper.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/inout_aper.h` & `hstaxe-1.0.5/cextern/src/inout_aper.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/ipixcorr_utils.c` & `hstaxe-1.0.5/cextern/src/ipixcorr_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/ipixcorr_utils.h` & `hstaxe-1.0.5/cextern/src/ipixcorr_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/lm_eval.c` & `hstaxe-1.0.5/cextern/src/lm_eval.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/lm_eval.h` & `hstaxe-1.0.5/cextern/src/lm_eval.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/lmmin.c` & `hstaxe-1.0.5/cextern/src/lmmin.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/lmmin.h` & `hstaxe-1.0.5/cextern/src/lmmin.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/model_utils.c` & `hstaxe-1.0.5/cextern/src/model_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/model_utils.h` & `hstaxe-1.0.5/cextern/src/model_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/nicback_utils.c` & `hstaxe-1.0.5/cextern/src/nicback_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/nicback_utils.h` & `hstaxe-1.0.5/cextern/src/nicback_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/scaleback_utils.c` & `hstaxe-1.0.5/cextern/src/scaleback_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/scaleback_utils.h` & `hstaxe-1.0.5/cextern/src/scaleback_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_CD.c` & `hstaxe-1.0.5/cextern/src/spc_CD.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_CD.h` & `hstaxe-1.0.5/cextern/src/spc_CD.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_FITScards.c` & `hstaxe-1.0.5/cextern/src/spc_FITScards.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_FITScards.h` & `hstaxe-1.0.5/cextern/src/spc_FITScards.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_back.c` & `hstaxe-1.0.5/cextern/src/spc_back.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_back.h` & `hstaxe-1.0.5/cextern/src/spc_back.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_cfg.c` & `hstaxe-1.0.5/cextern/src/spc_cfg.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_cfg.h` & `hstaxe-1.0.5/cextern/src/spc_cfg.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_driz.c` & `hstaxe-1.0.5/cextern/src/spc_driz.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_extract.c` & `hstaxe-1.0.5/cextern/src/spc_extract.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_flatfield.c` & `hstaxe-1.0.5/cextern/src/spc_flatfield.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_flatfield.h` & `hstaxe-1.0.5/cextern/src/spc_flatfield.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_fluxcube.c` & `hstaxe-1.0.5/cextern/src/spc_fluxcube.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_fluxcube.h` & `hstaxe-1.0.5/cextern/src/spc_fluxcube.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_model.c` & `hstaxe-1.0.5/cextern/src/spc_model.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_model.h` & `hstaxe-1.0.5/cextern/src/spc_model.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_optimum.c` & `hstaxe-1.0.5/cextern/src/spc_optimum.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_optimum.h` & `hstaxe-1.0.5/cextern/src/spc_optimum.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_resp.c` & `hstaxe-1.0.5/cextern/src/spc_resp.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_resp.h` & `hstaxe-1.0.5/cextern/src/spc_resp.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_sex.c` & `hstaxe-1.0.5/cextern/src/spc_sex.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_sex.h` & `hstaxe-1.0.5/cextern/src/spc_sex.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_spc.c` & `hstaxe-1.0.5/cextern/src/spc_spc.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_spc.h` & `hstaxe-1.0.5/cextern/src/spc_spc.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_trace_functions.c` & `hstaxe-1.0.5/cextern/src/spc_trace_functions.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_trace_functions.h` & `hstaxe-1.0.5/cextern/src/spc_trace_functions.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_utils.c` & `hstaxe-1.0.5/cextern/src/spc_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_utils.h` & `hstaxe-1.0.5/cextern/src/spc_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_wl_calib.c` & `hstaxe-1.0.5/cextern/src/spc_wl_calib.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spc_wl_calib.h` & `hstaxe-1.0.5/cextern/src/spc_wl_calib.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_PET.c` & `hstaxe-1.0.5/cextern/src/spce_PET.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_PET.h` & `hstaxe-1.0.5/cextern/src/spce_PET.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_binning.c` & `hstaxe-1.0.5/cextern/src/spce_binning.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_binning.h` & `hstaxe-1.0.5/cextern/src/spce_binning.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_fitting.c` & `hstaxe-1.0.5/cextern/src/spce_fitting.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_fitting.h` & `hstaxe-1.0.5/cextern/src/spce_fitting.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_is_in.c` & `hstaxe-1.0.5/cextern/src/spce_is_in.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_is_in.h` & `hstaxe-1.0.5/cextern/src/spce_is_in.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_output.c` & `hstaxe-1.0.5/cextern/src/spce_output.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_output.h` & `hstaxe-1.0.5/cextern/src/spce_output.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_pathlength.c` & `hstaxe-1.0.5/cextern/src/spce_pathlength.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_pgp.c` & `hstaxe-1.0.5/cextern/src/spce_pgp.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_pgp.h` & `hstaxe-1.0.5/cextern/src/spce_pgp.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_sect.c` & `hstaxe-1.0.5/cextern/src/spce_sect.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/spce_sect.h` & `hstaxe-1.0.5/cextern/src/spce_sect.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/specmodel_utils.c` & `hstaxe-1.0.5/cextern/src/specmodel_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/specmodel_utils.h` & `hstaxe-1.0.5/cextern/src/specmodel_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/test_aper_check.c` & `hstaxe-1.0.5/cextern/src/test_aper_check.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/trace_conf.c` & `hstaxe-1.0.5/cextern/src/trace_conf.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/trace_conf.h` & `hstaxe-1.0.5/cextern/src/trace_conf.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/trfit_utils.c` & `hstaxe-1.0.5/cextern/src/trfit_utils.c`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/cextern/src/trfit_utils.h` & `hstaxe-1.0.5/cextern/src/trfit_utils.h`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axeException.py` & `hstaxe-1.0.5/hstaxe/axeException.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axeerror.py` & `hstaxe-1.0.5/hstaxe/axeerror.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/config.py` & `hstaxe-1.0.5/hstaxe/config.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/utils.py` & `hstaxe-1.0.5/hstaxe/utils.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/WCSdata.py` & `hstaxe-1.0.5/hstaxe/axesim/WCSdata.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/axesim_verify.py` & `hstaxe-1.0.5/hstaxe/axesim/axesim_verify.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/axesimtasks.py` & `hstaxe-1.0.5/hstaxe/axesim/axesimtasks.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/imagemaker.py` & `hstaxe-1.0.5/hstaxe/axesim/imagemaker.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/interpolator.py` & `hstaxe-1.0.5/hstaxe/axesim/interpolator.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/modspeclist.py` & `hstaxe-1.0.5/hstaxe/axesim/modspeclist.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/realworld.py` & `hstaxe-1.0.5/hstaxe/axesim/realworld.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/templateimages.py` & `hstaxe-1.0.5/hstaxe/axesim/templateimages.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesim/templatespectra.py` & `hstaxe-1.0.5/hstaxe/axesim/templatespectra.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axecommands.py` & `hstaxe-1.0.5/hstaxe/axesrc/axecommands.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axeinputs.py` & `hstaxe-1.0.5/hstaxe/axesrc/axeinputs.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axeiol.py` & `hstaxe-1.0.5/hstaxe/axesrc/axeiol.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axelowlev.py` & `hstaxe-1.0.5/hstaxe/axesrc/axelowlev.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axepreptor.py` & `hstaxe-1.0.5/hstaxe/axesrc/axepreptor.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axesingextr.py` & `hstaxe-1.0.5/hstaxe/axesrc/axesingextr.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/axetasks.py` & `hstaxe-1.0.5/hstaxe/axesrc/axetasks.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/configfile.py` & `hstaxe-1.0.5/hstaxe/axesrc/configfile.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/dither.py` & `hstaxe-1.0.5/hstaxe/axesrc/dither.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/dppdumps.py` & `hstaxe-1.0.5/hstaxe/axesrc/dppdumps.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/drizzleobjects.py` & `hstaxe-1.0.5/hstaxe/axesrc/drizzleobjects.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/fcubeobjs.py` & `hstaxe-1.0.5/hstaxe/axesrc/fcubeobjs.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/imagemaker.py` & `hstaxe-1.0.5/hstaxe/axesrc/imagemaker.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/inputchecks.py` & `hstaxe-1.0.5/hstaxe/axesrc/inputchecks.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         return is_prism
 
     def _force_dirim(self):
         # go over all inputs
         for one_input in self.axe_inputs:
 
             # check whether there is a direct image
-            if one_input['DIRIM'] is None:
+            if one_input['dirim'] is None:
                 # error and out
                 err_msg = ("{0:s}: The grism image: {1:s} does NOT have an "
                            "associated direct image!"
                            .format(self.taskname,
                                    config_util.getDATA(one_input['grisim'])))
                 raise aXeError(err_msg)
```

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/iolmaking.py` & `hstaxe-1.0.5/hstaxe/axesrc/iolmaking.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/mefobjects.py` & `hstaxe-1.0.5/hstaxe/axesrc/mefobjects.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/nlincoeffs.py` & `hstaxe-1.0.5/hstaxe/axesrc/nlincoeffs.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/axesrc/pysex2gol.py` & `hstaxe-1.0.5/hstaxe/axesrc/pysex2gol.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/coveragerc` & `hstaxe-1.0.5/hstaxe/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/run_acs_cookbook.py` & `hstaxe-1.0.5/hstaxe/tests/run_acs_cookbook.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/run_cookbook.py` & `hstaxe-1.0.5/hstaxe/tests/run_cookbook.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/run_cookbook_part2.py` & `hstaxe-1.0.5/hstaxe/tests/run_cookbook_part2.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_af2pet.py` & `hstaxe-1.0.5/hstaxe/tests/test_af2pet.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_axecore.py` & `hstaxe-1.0.5/hstaxe/tests/test_axecore.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_axeprep.py` & `hstaxe-1.0.5/hstaxe/tests/test_axeprep.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_be.py` & `hstaxe-1.0.5/hstaxe/tests/test_be.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_gol2af.py` & `hstaxe-1.0.5/hstaxe/tests/test_gol2af.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_iolprep.py` & `hstaxe-1.0.5/hstaxe/tests/test_iolprep.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_pet2spc.py` & `hstaxe-1.0.5/hstaxe/tests/test_pet2spc.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_petcont.py` & `hstaxe-1.0.5/hstaxe/tests/test_petcont.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_petff.py` & `hstaxe-1.0.5/hstaxe/tests/test_petff.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_scalebck.py` & `hstaxe-1.0.5/hstaxe/tests/test_scalebck.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_sex2gol.py` & `hstaxe-1.0.5/hstaxe/tests/test_sex2gol.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hstaxe/tests/test_stamps.py` & `hstaxe-1.0.5/hstaxe/tests/test_stamps.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/.gitignore` & `hstaxe-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/LICENSE.txt` & `hstaxe-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/README.md` & `hstaxe-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/hatch_build.py` & `hstaxe-1.0.5/hatch_build.py`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/pyproject.toml` & `hstaxe-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hstaxe-1.0.4/PKG-INFO` & `hstaxe-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstaxe
-Version: 1.0.4
+Version: 1.0.5
 Summary: Spectral extraction tools for Hubble Space Telescope Grisms
 Project-URL: Homepage, https://github.com/spacetelescope/hstaxe
 Author-email: hstaxe and aXe developers <help@stsci.edu>
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

