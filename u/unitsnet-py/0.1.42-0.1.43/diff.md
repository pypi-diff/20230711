# Comparing `tmp/unitsnet-py-0.1.42.tar.gz` & `tmp/unitsnet-py-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitsnet-py-0.1.42.tar", last modified: Sat Jul  1 18:24:07 2023, max compression
+gzip compressed data, was "unitsnet-py-0.1.43.tar", last modified: Tue Jul 11 13:51:18 2023, max compression
```

## Comparing `unitsnet-py-0.1.42.tar` & `unitsnet-py-0.1.43.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:24:07.623080 unitsnet-py-0.1.42/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 18:23:14.000000 unitsnet-py-0.1.42/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-07-01 18:24:07.623080 unitsnet-py-0.1.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27204 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-01 18:24:01.000000 unitsnet-py-0.1.42/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 18:24:07.623080 unitsnet-py-0.1.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-01 18:24:01.000000 unitsnet-py-0.1.42/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:24:07.607079 unitsnet-py-0.1.42/unitsnet_py/
--rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:24:07.623080 unitsnet-py-0.1.42/unitsnet_py/units/
--rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/amount_of_substance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/amplitude_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/apparent_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/apparent_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/area.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/area_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/area_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/brake_specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/capacitance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/coefficient_of_thermal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/density.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/dynamic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_admittance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_conductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_current_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_current_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_inductance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_dc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_resistivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/electric_surface_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/energy_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/force.py
--rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/force_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-01 18:23:57.000000 unitsnet-py-0.1.42/unitsnet_py/units/force_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/fuel_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/heat_transfer_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/impulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/information.py
--rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/irradiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/jerk.py
--rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/kinematic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/leak_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    50654 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/level.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/linear_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/linear_power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/luminance.py
--rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/luminous_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/luminous_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/magnetic_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/magnetic_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass_fraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/mass_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/molar_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/molar_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/molar_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/molar_mass.py
--rw-r--r--   0 runner    (1001) docker     (123)    19727 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/molarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/permittivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/porous_medium_permeability.py
--rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/power.py
--rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/power_ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (123)    28785 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/pressure_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/ratio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/ratio_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/reactive_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/reactive_power.py
--rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/reciprocal_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/reciprocal_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/relative_humidity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/rotational_acceleration.py
--rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/rotational_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/rotational_stiffness.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/rotational_stiffness_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/specific_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-01 18:23:58.000000 unitsnet-py-0.1.42/unitsnet_py/units/specific_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/specific_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/specific_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/speed.py
--rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/standard_volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/temperature_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/temperature_delta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/temperature_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/thermal_resistance.py
--rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/torque.py
--rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/torque_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/turbidity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/vitamin_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volume_flow_per_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volume_per_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/volumetric_heat_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-01 18:23:59.000000 unitsnet-py-0.1.42/unitsnet_py/units/warping_moment_of_inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 18:24:07.607079 unitsnet-py-0.1.42/unitsnet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27745 2023-07-01 18:24:07.000000 unitsnet-py-0.1.42/unitsnet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-01 18:24:07.000000 unitsnet-py-0.1.42/unitsnet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 18:24:07.000000 unitsnet-py-0.1.42/unitsnet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-01 18:24:07.000000 unitsnet-py-0.1.42/unitsnet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:51:18.411357 unitsnet-py-0.1.43/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 13:50:18.000000 unitsnet-py-0.1.43/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-11 13:51:18.411357 unitsnet-py-0.1.43/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27203 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-11 13:51:11.000000 unitsnet-py-0.1.43/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 13:51:18.411357 unitsnet-py-0.1.43/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-11 13:51:12.000000 unitsnet-py-0.1.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:51:18.395357 unitsnet-py-0.1.43/unitsnet_py/
+-rw-r--r--   0 runner    (1001) docker     (123)    13575 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:51:18.411357 unitsnet-py-0.1.43/unitsnet_py/units/
+-rw-r--r--   0 runner    (1001) docker     (123)    28358 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25910 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24343 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/amount_of_substance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/amplitude_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22523 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/apparent_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/apparent_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24143 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/area_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14055 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/area_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23054 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10849 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/brake_specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/capacitance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/coefficient_of_thermal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14699 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77189 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/dynamic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_admittance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18982 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_conductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14167 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_current_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15935 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_current_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5904 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_inductance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12327 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37281 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_dc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13413 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_resistivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10486 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/electric_surface_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51805 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/energy_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22813 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27351 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/force_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62708 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/force_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19966 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-07-11 13:51:07.000000 unitsnet-py-0.1.43/unitsnet_py/units/fuel_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/heat_transfer_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20955 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26281 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20171 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16967 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/kinematic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/leak_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50654 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6373 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/linear_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42257 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/linear_power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20973 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/luminous_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/luminous_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/magnetic_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/magnetic_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40535 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80144 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48229 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48955 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/mass_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8507 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/molar_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/molar_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/molar_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22032 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/molar_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/molarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/permittivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11926 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/porous_medium_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36732 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69959 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/power_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73652 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34511 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/pressure_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/ratio_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/reactive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/reactive_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/reciprocal_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18523 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/reciprocal_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/relative_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11867 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/rotational_acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24312 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/rotational_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61867 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/rotational_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/rotational_stiffness_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-11 13:51:08.000000 unitsnet-py-0.1.43/unitsnet_py/units/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50352 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/specific_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19629 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/specific_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9371 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/specific_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32699 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/specific_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48511 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20246 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/standard_volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17918 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22040 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/temperature_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/temperature_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11102 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/temperature_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/thermal_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38844 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39573 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/torque_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/turbidity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/vitamin_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71514 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34742 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99718 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8478 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volume_flow_per_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volume_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22169 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/volumetric_heat_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-11 13:51:09.000000 unitsnet-py-0.1.43/unitsnet_py/units/warping_moment_of_inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 13:51:18.395357 unitsnet-py-0.1.43/unitsnet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27744 2023-07-11 13:51:18.000000 unitsnet-py-0.1.43/unitsnet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-11 13:51:18.000000 unitsnet-py-0.1.43/unitsnet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 13:51:18.000000 unitsnet-py-0.1.43/unitsnet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 13:51:18.000000 unitsnet-py-0.1.43/unitsnet_py.egg-info/top_level.txt
```

### Comparing `unitsnet-py-0.1.42/LICENSE` & `unitsnet-py-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/PKG-INFO` & `unitsnet-py-0.1.43/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.42
+Version: 0.1.43
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
@@ -316,15 +316,15 @@
 - **MolarFlow**
     -   *Molar flow is the ratio of the amount of substance change to the time during which the change occurred (value of amount of substance changes per unit time).*
 
 - **MolarMass**
     -   *In chemistry, the molar mass M is a physical property defined as the mass of a given substance (chemical element or chemical compound) divided by the amount of substance.*
 
 - **Molarity**
-    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume. *
+    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume.*
 
 - **Permeability**
     -   *In electromagnetism, permeability is the measure of the ability of a material to support the formation of a magnetic field within itself.*
 
 - **Permittivity**
     -   *In electromagnetism, permittivity is the measure of resistance that is encountered when forming an electric field in a particular medium.*
```

### Comparing `unitsnet-py-0.1.42/README.md` & `unitsnet-py-0.1.43/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 - **MolarFlow**
     -   *Molar flow is the ratio of the amount of substance change to the time during which the change occurred (value of amount of substance changes per unit time).*
 
 - **MolarMass**
     -   *In chemistry, the molar mass M is a physical property defined as the mass of a given substance (chemical element or chemical compound) divided by the amount of substance.*
 
 - **Molarity**
-    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume. *
+    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume.*
 
 - **Permeability**
     -   *In electromagnetism, permeability is the measure of the ability of a material to support the formation of a magnetic field within itself.*
 
 - **Permittivity**
     -   *In electromagnetism, permittivity is the measure of resistance that is encountered when forming an electric field in a particular medium.*
```

### Comparing `unitsnet-py-0.1.42/pyproject.toml` & `unitsnet-py-0.1.43/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unitsnet_py"
-version = "0.1.42"
+version = "0.1.43"
 description = "A better way to hold unit variables and easily convert to the destination unit"
 repository = "https://github.com/haimkastner/unitsnet-py"
 authors = ["Haim Kastner <haim.kastner@gmail.com>"]
 maintainers = [
     "Haim Kastner <haim.kastner@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `unitsnet-py-0.1.42/setup.py` & `unitsnet-py-0.1.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['unitsnet_py', 'unitsnet_py.units']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unitsnet-py',
-    'version': '0.1.42',
+    'version': '0.1.43',
     'keywords': 'conversion, units-of-measure, units, quantities, unit-converter, converter, unit, measure, measures, measurement, measurements',
     'description': 'A better way to hold unit variables and easily convert to the destination unit',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Haim Kastner',
     'author_email': 'haim.kastner@gmail.com',
     'maintainer': 'Haim Kastner',
```

### Comparing `unitsnet-py-0.1.42/unitsnet_py/__init__.py` & `unitsnet-py-0.1.43/unitsnet_py/__init__.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py` & `unitsnet-py-0.1.43/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/acceleration.py` & `unitsnet-py-0.1.43/unitsnet_py/units/acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/amount_of_substance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/amount_of_substance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/amplitude_ratio.py` & `unitsnet-py-0.1.43/unitsnet_py/units/amplitude_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/angle.py` & `unitsnet-py-0.1.43/unitsnet_py/units/angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/apparent_energy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/apparent_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/apparent_power.py` & `unitsnet-py-0.1.43/unitsnet_py/units/apparent_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/area.py` & `unitsnet-py-0.1.43/unitsnet_py/units/area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/area_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/area_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/area_moment_of_inertia.py` & `unitsnet-py-0.1.43/unitsnet_py/units/area_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/bit_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/bit_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/brake_specific_fuel_consumption.py` & `unitsnet-py-0.1.43/unitsnet_py/units/brake_specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/capacitance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/capacitance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/coefficient_of_thermal_expansion.py` & `unitsnet-py-0.1.43/unitsnet_py/units/coefficient_of_thermal_expansion.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/compressibility.py` & `unitsnet-py-0.1.43/unitsnet_py/units/compressibility.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/duration.py` & `unitsnet-py-0.1.43/unitsnet_py/units/duration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/dynamic_viscosity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/dynamic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_admittance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_admittance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_charge.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_charge.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_charge_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_conductance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_conductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_conductivity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_current.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_current.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_current_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_current_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_current_gradient.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_current_gradient.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,14 +9,19 @@
         """
         
         AmperePerSecond = 'ampere_per_second'
         """
             
         """
         
+        AmperePerMinute = 'ampere_per_minute'
+        """
+            
+        """
+        
         AmperePerMillisecond = 'ampere_per_millisecond'
         """
             
         """
         
         AmperePerMicrosecond = 'ampere_per_microsecond'
         """
@@ -24,14 +29,24 @@
         """
         
         AmperePerNanosecond = 'ampere_per_nanosecond'
         """
             
         """
         
+        MilliamperePerSecond = 'milliampere_per_second'
+        """
+            
+        """
+        
+        MilliamperePerMinute = 'milliampere_per_minute'
+        """
+            
+        """
+        
 
 class ElectricCurrentGradient:
     """
     In electromagnetism, the current gradient describes how the current changes in time.
 
     Args:
         value (float): The value.
@@ -40,53 +55,77 @@
     def __init__(self, value: float, from_unit: ElectricCurrentGradientUnits = ElectricCurrentGradientUnits.AmperePerSecond):
         if math.isnan(value):
             raise ValueError('Invalid unit: value is NaN')
         self.__value = self.__convert_to_base(value, from_unit)
         
         self.__amperes_per_second = None
         
+        self.__amperes_per_minute = None
+        
         self.__amperes_per_millisecond = None
         
         self.__amperes_per_microsecond = None
         
         self.__amperes_per_nanosecond = None
         
+        self.__milliamperes_per_second = None
+        
+        self.__milliamperes_per_minute = None
+        
 
     def __convert_from_base(self, from_unit: ElectricCurrentGradientUnits) -> float:
         value = self.__value
         
         if from_unit == ElectricCurrentGradientUnits.AmperePerSecond:
             return (value)
         
+        if from_unit == ElectricCurrentGradientUnits.AmperePerMinute:
+            return (value * 60)
+        
         if from_unit == ElectricCurrentGradientUnits.AmperePerMillisecond:
             return (value / 1e3)
         
         if from_unit == ElectricCurrentGradientUnits.AmperePerMicrosecond:
             return (value / 1e6)
         
         if from_unit == ElectricCurrentGradientUnits.AmperePerNanosecond:
             return (value / 1e9)
         
+        if from_unit == ElectricCurrentGradientUnits.MilliamperePerSecond:
+            return ((value) / 0.001)
+        
+        if from_unit == ElectricCurrentGradientUnits.MilliamperePerMinute:
+            return ((value * 60) / 0.001)
+        
         return None
 
 
     def __convert_to_base(self, value: float, to_unit: ElectricCurrentGradientUnits) -> float:
         
         if to_unit == ElectricCurrentGradientUnits.AmperePerSecond:
             return (value)
         
+        if to_unit == ElectricCurrentGradientUnits.AmperePerMinute:
+            return (value / 60)
+        
         if to_unit == ElectricCurrentGradientUnits.AmperePerMillisecond:
             return (value * 1e3)
         
         if to_unit == ElectricCurrentGradientUnits.AmperePerMicrosecond:
             return (value * 1e6)
         
         if to_unit == ElectricCurrentGradientUnits.AmperePerNanosecond:
             return (value * 1e9)
         
+        if to_unit == ElectricCurrentGradientUnits.MilliamperePerSecond:
+            return ((value) * 0.001)
+        
+        if to_unit == ElectricCurrentGradientUnits.MilliamperePerMinute:
+            return ((value / 60) * 0.001)
+        
         return None
 
 
     @property
     def base_value(self) -> float:
         return self.__value
 
@@ -103,14 +142,29 @@
         :return: A new instance of ElectricCurrentGradient.
         :rtype: ElectricCurrentGradient
         """
         return ElectricCurrentGradient(amperes_per_second, ElectricCurrentGradientUnits.AmperePerSecond)
 
     
     @staticmethod
+    def from_amperes_per_minute(amperes_per_minute: float):
+        """
+        Create a new instance of ElectricCurrentGradient from a value in amperes_per_minute.
+
+        
+
+        :param meters: The ElectricCurrentGradient value in amperes_per_minute.
+        :type amperes_per_minute: float
+        :return: A new instance of ElectricCurrentGradient.
+        :rtype: ElectricCurrentGradient
+        """
+        return ElectricCurrentGradient(amperes_per_minute, ElectricCurrentGradientUnits.AmperePerMinute)
+
+    
+    @staticmethod
     def from_amperes_per_millisecond(amperes_per_millisecond: float):
         """
         Create a new instance of ElectricCurrentGradient from a value in amperes_per_millisecond.
 
         
 
         :param meters: The ElectricCurrentGradient value in amperes_per_millisecond.
@@ -147,26 +201,67 @@
         :type amperes_per_nanosecond: float
         :return: A new instance of ElectricCurrentGradient.
         :rtype: ElectricCurrentGradient
         """
         return ElectricCurrentGradient(amperes_per_nanosecond, ElectricCurrentGradientUnits.AmperePerNanosecond)
 
     
+    @staticmethod
+    def from_milliamperes_per_second(milliamperes_per_second: float):
+        """
+        Create a new instance of ElectricCurrentGradient from a value in milliamperes_per_second.
+
+        
+
+        :param meters: The ElectricCurrentGradient value in milliamperes_per_second.
+        :type milliamperes_per_second: float
+        :return: A new instance of ElectricCurrentGradient.
+        :rtype: ElectricCurrentGradient
+        """
+        return ElectricCurrentGradient(milliamperes_per_second, ElectricCurrentGradientUnits.MilliamperePerSecond)
+
+    
+    @staticmethod
+    def from_milliamperes_per_minute(milliamperes_per_minute: float):
+        """
+        Create a new instance of ElectricCurrentGradient from a value in milliamperes_per_minute.
+
+        
+
+        :param meters: The ElectricCurrentGradient value in milliamperes_per_minute.
+        :type milliamperes_per_minute: float
+        :return: A new instance of ElectricCurrentGradient.
+        :rtype: ElectricCurrentGradient
+        """
+        return ElectricCurrentGradient(milliamperes_per_minute, ElectricCurrentGradientUnits.MilliamperePerMinute)
+
+    
     @property
     def amperes_per_second(self) -> float:
         """
         
         """
         if self.__amperes_per_second != None:
             return self.__amperes_per_second
         self.__amperes_per_second = self.__convert_from_base(ElectricCurrentGradientUnits.AmperePerSecond)
         return self.__amperes_per_second
 
     
     @property
+    def amperes_per_minute(self) -> float:
+        """
+        
+        """
+        if self.__amperes_per_minute != None:
+            return self.__amperes_per_minute
+        self.__amperes_per_minute = self.__convert_from_base(ElectricCurrentGradientUnits.AmperePerMinute)
+        return self.__amperes_per_minute
+
+    
+    @property
     def amperes_per_millisecond(self) -> float:
         """
         
         """
         if self.__amperes_per_millisecond != None:
             return self.__amperes_per_millisecond
         self.__amperes_per_millisecond = self.__convert_from_base(ElectricCurrentGradientUnits.AmperePerMillisecond)
@@ -191,55 +286,95 @@
         """
         if self.__amperes_per_nanosecond != None:
             return self.__amperes_per_nanosecond
         self.__amperes_per_nanosecond = self.__convert_from_base(ElectricCurrentGradientUnits.AmperePerNanosecond)
         return self.__amperes_per_nanosecond
 
     
+    @property
+    def milliamperes_per_second(self) -> float:
+        """
+        
+        """
+        if self.__milliamperes_per_second != None:
+            return self.__milliamperes_per_second
+        self.__milliamperes_per_second = self.__convert_from_base(ElectricCurrentGradientUnits.MilliamperePerSecond)
+        return self.__milliamperes_per_second
+
+    
+    @property
+    def milliamperes_per_minute(self) -> float:
+        """
+        
+        """
+        if self.__milliamperes_per_minute != None:
+            return self.__milliamperes_per_minute
+        self.__milliamperes_per_minute = self.__convert_from_base(ElectricCurrentGradientUnits.MilliamperePerMinute)
+        return self.__milliamperes_per_minute
+
+    
     def to_string(self, unit: ElectricCurrentGradientUnits = ElectricCurrentGradientUnits.AmperePerSecond) -> string:
         """
         Format the ElectricCurrentGradient to string.
         Note! the default format for ElectricCurrentGradient is AmperePerSecond.
         To specify the unit format set the 'unit' parameter.
         """
         
         if unit == ElectricCurrentGradientUnits.AmperePerSecond:
             return f"""{self.amperes_per_second} A/s"""
         
+        if unit == ElectricCurrentGradientUnits.AmperePerMinute:
+            return f"""{self.amperes_per_minute} A/min"""
+        
         if unit == ElectricCurrentGradientUnits.AmperePerMillisecond:
             return f"""{self.amperes_per_millisecond} A/ms"""
         
         if unit == ElectricCurrentGradientUnits.AmperePerMicrosecond:
             return f"""{self.amperes_per_microsecond} A/μs"""
         
         if unit == ElectricCurrentGradientUnits.AmperePerNanosecond:
             return f"""{self.amperes_per_nanosecond} A/ns"""
         
+        if unit == ElectricCurrentGradientUnits.MilliamperePerSecond:
+            return f"""{self.milliamperes_per_second} """
+        
+        if unit == ElectricCurrentGradientUnits.MilliamperePerMinute:
+            return f"""{self.milliamperes_per_minute} """
+        
         return f'{self.__value}'
 
 
     def get_unit_abbreviation(self, unit_abbreviation: ElectricCurrentGradientUnits = ElectricCurrentGradientUnits.AmperePerSecond) -> string:
         """
         Get ElectricCurrentGradient unit abbreviation.
         Note! the default abbreviation for ElectricCurrentGradient is AmperePerSecond.
         To specify the unit abbreviation set the 'unit_abbreviation' parameter.
         """
         
         if unit_abbreviation == ElectricCurrentGradientUnits.AmperePerSecond:
             return """A/s"""
         
+        if unit_abbreviation == ElectricCurrentGradientUnits.AmperePerMinute:
+            return """A/min"""
+        
         if unit_abbreviation == ElectricCurrentGradientUnits.AmperePerMillisecond:
             return """A/ms"""
         
         if unit_abbreviation == ElectricCurrentGradientUnits.AmperePerMicrosecond:
             return """A/μs"""
         
         if unit_abbreviation == ElectricCurrentGradientUnits.AmperePerNanosecond:
             return """A/ns"""
         
+        if unit_abbreviation == ElectricCurrentGradientUnits.MilliamperePerSecond:
+            return """"""
+        
+        if unit_abbreviation == ElectricCurrentGradientUnits.MilliamperePerMinute:
+            return """"""
+        
 
     def __str__(self):
         return self.to_string()
 
 
     def __add__(self, other):
         if not isinstance(other, ElectricCurrentGradient):
```

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_field.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_inductance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_inductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_potential.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_ac.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_ac.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_change_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_potential_dc.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_potential_dc.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_resistance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_resistivity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_resistivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/electric_surface_charge_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/electric_surface_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/energy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/energy_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/energy_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/entropy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/force.py` & `unitsnet-py-0.1.43/unitsnet_py/units/force.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/force_change_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/force_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/force_per_length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/force_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/frequency.py` & `unitsnet-py-0.1.43/unitsnet_py/units/frequency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/fuel_efficiency.py` & `unitsnet-py-0.1.43/unitsnet_py/units/fuel_efficiency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/heat_flux.py` & `unitsnet-py-0.1.43/unitsnet_py/units/heat_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/heat_transfer_coefficient.py` & `unitsnet-py-0.1.43/unitsnet_py/units/heat_transfer_coefficient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/illuminance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/illuminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/impulse.py` & `unitsnet-py-0.1.43/unitsnet_py/units/impulse.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/information.py` & `unitsnet-py-0.1.43/unitsnet_py/units/information.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/irradiance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/irradiance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/irradiation.py` & `unitsnet-py-0.1.43/unitsnet_py/units/irradiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/jerk.py` & `unitsnet-py-0.1.43/unitsnet_py/units/jerk.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/kinematic_viscosity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/kinematic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/leak_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/leak_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/level.py` & `unitsnet-py-0.1.43/unitsnet_py/units/level.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/linear_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/linear_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/linear_power_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/linear_power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/luminance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/luminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/luminosity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/luminosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/luminous_flux.py` & `unitsnet-py-0.1.43/unitsnet_py/units/luminous_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/luminous_intensity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/luminous_intensity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/magnetic_field.py` & `unitsnet-py-0.1.43/unitsnet_py/units/magnetic_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/magnetic_flux.py` & `unitsnet-py-0.1.43/unitsnet_py/units/magnetic_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/magnetization.py` & `unitsnet-py-0.1.43/unitsnet_py/units/magnetization.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass_concentration.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass_flow.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass_flux.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass_fraction.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass_fraction.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/mass_moment_of_inertia.py` & `unitsnet-py-0.1.43/unitsnet_py/units/mass_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/molar_energy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/molar_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/molar_entropy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/molar_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/molar_flow.py` & `unitsnet-py-0.1.43/unitsnet_py/units/molar_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/molar_mass.py` & `unitsnet-py-0.1.43/unitsnet_py/units/molar_mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/molarity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/molarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         """
             
         """
         
 
 class Molarity:
     """
-    Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume. 
+    Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume.
 
     Args:
         value (float): The value.
         from_unit (MolarityUnits): The Molarity unit to create from, The default unit is MolePerCubicMeter
     """
     def __init__(self, value: float, from_unit: MolarityUnits = MolarityUnits.MolePerCubicMeter):
         if math.isnan(value):
```

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/permeability.py` & `unitsnet-py-0.1.43/unitsnet_py/units/permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/permittivity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/permittivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/porous_medium_permeability.py` & `unitsnet-py-0.1.43/unitsnet_py/units/porous_medium_permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/power.py` & `unitsnet-py-0.1.43/unitsnet_py/units/power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/power_density.py` & `unitsnet-py-0.1.43/unitsnet_py/units/power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/power_ratio.py` & `unitsnet-py-0.1.43/unitsnet_py/units/power_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/pressure.py` & `unitsnet-py-0.1.43/unitsnet_py/units/pressure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/pressure_change_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/pressure_change_rate.py`

 * *Files 15% similar despite different names*

```diff
@@ -34,14 +34,24 @@
         """
         
         PoundForcePerSquareInchPerMinute = 'pound_force_per_square_inch_per_minute'
         """
             
         """
         
+        BarPerSecond = 'bar_per_second'
+        """
+            
+        """
+        
+        BarPerMinute = 'bar_per_minute'
+        """
+            
+        """
+        
         KilopascalPerSecond = 'kilopascal_per_second'
         """
             
         """
         
         MegapascalPerSecond = 'megapascal_per_second'
         """
@@ -74,14 +84,24 @@
         """
         
         MegapoundForcePerSquareInchPerMinute = 'megapound_force_per_square_inch_per_minute'
         """
             
         """
         
+        MillibarPerSecond = 'millibar_per_second'
+        """
+            
+        """
+        
+        MillibarPerMinute = 'millibar_per_minute'
+        """
+            
+        """
+        
 
 class PressureChangeRate:
     """
     Pressure change rate is the ratio of the pressure change to the time during which the change occurred (value of pressure changes per unit time).
 
     Args:
         value (float): The value.
@@ -100,14 +120,18 @@
         
         self.__atmospheres_per_second = None
         
         self.__pounds_force_per_square_inch_per_second = None
         
         self.__pounds_force_per_square_inch_per_minute = None
         
+        self.__bars_per_second = None
+        
+        self.__bars_per_minute = None
+        
         self.__kilopascals_per_second = None
         
         self.__megapascals_per_second = None
         
         self.__kilopascals_per_minute = None
         
         self.__megapascals_per_minute = None
@@ -116,14 +140,18 @@
         
         self.__megapounds_force_per_square_inch_per_second = None
         
         self.__kilopounds_force_per_square_inch_per_minute = None
         
         self.__megapounds_force_per_square_inch_per_minute = None
         
+        self.__millibars_per_second = None
+        
+        self.__millibars_per_minute = None
+        
 
     def __convert_from_base(self, from_unit: PressureChangeRateUnits) -> float:
         value = self.__value
         
         if from_unit == PressureChangeRateUnits.PascalPerSecond:
             return (value)
         
@@ -138,14 +166,20 @@
         
         if from_unit == PressureChangeRateUnits.PoundForcePerSquareInchPerSecond:
             return (value / 6.894757293168361e3)
         
         if from_unit == PressureChangeRateUnits.PoundForcePerSquareInchPerMinute:
             return (value / 6.894757293168361e3 * 60)
         
+        if from_unit == PressureChangeRateUnits.BarPerSecond:
+            return (value / 1e5)
+        
+        if from_unit == PressureChangeRateUnits.BarPerMinute:
+            return (value / 1e5 * 60)
+        
         if from_unit == PressureChangeRateUnits.KilopascalPerSecond:
             return ((value) / 1000.0)
         
         if from_unit == PressureChangeRateUnits.MegapascalPerSecond:
             return ((value) / 1000000.0)
         
         if from_unit == PressureChangeRateUnits.KilopascalPerMinute:
@@ -162,14 +196,20 @@
         
         if from_unit == PressureChangeRateUnits.KilopoundForcePerSquareInchPerMinute:
             return ((value / 6.894757293168361e3 * 60) / 1000.0)
         
         if from_unit == PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute:
             return ((value / 6.894757293168361e3 * 60) / 1000000.0)
         
+        if from_unit == PressureChangeRateUnits.MillibarPerSecond:
+            return ((value / 1e5) / 0.001)
+        
+        if from_unit == PressureChangeRateUnits.MillibarPerMinute:
+            return ((value / 1e5 * 60) / 0.001)
+        
         return None
 
 
     def __convert_to_base(self, value: float, to_unit: PressureChangeRateUnits) -> float:
         
         if to_unit == PressureChangeRateUnits.PascalPerSecond:
             return (value)
@@ -185,14 +225,20 @@
         
         if to_unit == PressureChangeRateUnits.PoundForcePerSquareInchPerSecond:
             return (value * 6.894757293168361e3)
         
         if to_unit == PressureChangeRateUnits.PoundForcePerSquareInchPerMinute:
             return (value * 6.894757293168361e3 / 60)
         
+        if to_unit == PressureChangeRateUnits.BarPerSecond:
+            return (value * 1e5)
+        
+        if to_unit == PressureChangeRateUnits.BarPerMinute:
+            return (value * 1e5 / 60)
+        
         if to_unit == PressureChangeRateUnits.KilopascalPerSecond:
             return ((value) * 1000.0)
         
         if to_unit == PressureChangeRateUnits.MegapascalPerSecond:
             return ((value) * 1000000.0)
         
         if to_unit == PressureChangeRateUnits.KilopascalPerMinute:
@@ -209,14 +255,20 @@
         
         if to_unit == PressureChangeRateUnits.KilopoundForcePerSquareInchPerMinute:
             return ((value * 6.894757293168361e3 / 60) * 1000.0)
         
         if to_unit == PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute:
             return ((value * 6.894757293168361e3 / 60) * 1000000.0)
         
+        if to_unit == PressureChangeRateUnits.MillibarPerSecond:
+            return ((value * 1e5) * 0.001)
+        
+        if to_unit == PressureChangeRateUnits.MillibarPerMinute:
+            return ((value * 1e5 / 60) * 0.001)
+        
         return None
 
 
     @property
     def base_value(self) -> float:
         return self.__value
 
@@ -308,14 +360,44 @@
         :return: A new instance of PressureChangeRate.
         :rtype: PressureChangeRate
         """
         return PressureChangeRate(pounds_force_per_square_inch_per_minute, PressureChangeRateUnits.PoundForcePerSquareInchPerMinute)
 
     
     @staticmethod
+    def from_bars_per_second(bars_per_second: float):
+        """
+        Create a new instance of PressureChangeRate from a value in bars_per_second.
+
+        
+
+        :param meters: The PressureChangeRate value in bars_per_second.
+        :type bars_per_second: float
+        :return: A new instance of PressureChangeRate.
+        :rtype: PressureChangeRate
+        """
+        return PressureChangeRate(bars_per_second, PressureChangeRateUnits.BarPerSecond)
+
+    
+    @staticmethod
+    def from_bars_per_minute(bars_per_minute: float):
+        """
+        Create a new instance of PressureChangeRate from a value in bars_per_minute.
+
+        
+
+        :param meters: The PressureChangeRate value in bars_per_minute.
+        :type bars_per_minute: float
+        :return: A new instance of PressureChangeRate.
+        :rtype: PressureChangeRate
+        """
+        return PressureChangeRate(bars_per_minute, PressureChangeRateUnits.BarPerMinute)
+
+    
+    @staticmethod
     def from_kilopascals_per_second(kilopascals_per_second: float):
         """
         Create a new instance of PressureChangeRate from a value in kilopascals_per_second.
 
         
 
         :param meters: The PressureChangeRate value in kilopascals_per_second.
@@ -427,14 +509,44 @@
         :type megapounds_force_per_square_inch_per_minute: float
         :return: A new instance of PressureChangeRate.
         :rtype: PressureChangeRate
         """
         return PressureChangeRate(megapounds_force_per_square_inch_per_minute, PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute)
 
     
+    @staticmethod
+    def from_millibars_per_second(millibars_per_second: float):
+        """
+        Create a new instance of PressureChangeRate from a value in millibars_per_second.
+
+        
+
+        :param meters: The PressureChangeRate value in millibars_per_second.
+        :type millibars_per_second: float
+        :return: A new instance of PressureChangeRate.
+        :rtype: PressureChangeRate
+        """
+        return PressureChangeRate(millibars_per_second, PressureChangeRateUnits.MillibarPerSecond)
+
+    
+    @staticmethod
+    def from_millibars_per_minute(millibars_per_minute: float):
+        """
+        Create a new instance of PressureChangeRate from a value in millibars_per_minute.
+
+        
+
+        :param meters: The PressureChangeRate value in millibars_per_minute.
+        :type millibars_per_minute: float
+        :return: A new instance of PressureChangeRate.
+        :rtype: PressureChangeRate
+        """
+        return PressureChangeRate(millibars_per_minute, PressureChangeRateUnits.MillibarPerMinute)
+
+    
     @property
     def pascals_per_second(self) -> float:
         """
         
         """
         if self.__pascals_per_second != None:
             return self.__pascals_per_second
@@ -494,14 +606,36 @@
         if self.__pounds_force_per_square_inch_per_minute != None:
             return self.__pounds_force_per_square_inch_per_minute
         self.__pounds_force_per_square_inch_per_minute = self.__convert_from_base(PressureChangeRateUnits.PoundForcePerSquareInchPerMinute)
         return self.__pounds_force_per_square_inch_per_minute
 
     
     @property
+    def bars_per_second(self) -> float:
+        """
+        
+        """
+        if self.__bars_per_second != None:
+            return self.__bars_per_second
+        self.__bars_per_second = self.__convert_from_base(PressureChangeRateUnits.BarPerSecond)
+        return self.__bars_per_second
+
+    
+    @property
+    def bars_per_minute(self) -> float:
+        """
+        
+        """
+        if self.__bars_per_minute != None:
+            return self.__bars_per_minute
+        self.__bars_per_minute = self.__convert_from_base(PressureChangeRateUnits.BarPerMinute)
+        return self.__bars_per_minute
+
+    
+    @property
     def kilopascals_per_second(self) -> float:
         """
         
         """
         if self.__kilopascals_per_second != None:
             return self.__kilopascals_per_second
         self.__kilopascals_per_second = self.__convert_from_base(PressureChangeRateUnits.KilopascalPerSecond)
@@ -581,14 +715,36 @@
         """
         if self.__megapounds_force_per_square_inch_per_minute != None:
             return self.__megapounds_force_per_square_inch_per_minute
         self.__megapounds_force_per_square_inch_per_minute = self.__convert_from_base(PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute)
         return self.__megapounds_force_per_square_inch_per_minute
 
     
+    @property
+    def millibars_per_second(self) -> float:
+        """
+        
+        """
+        if self.__millibars_per_second != None:
+            return self.__millibars_per_second
+        self.__millibars_per_second = self.__convert_from_base(PressureChangeRateUnits.MillibarPerSecond)
+        return self.__millibars_per_second
+
+    
+    @property
+    def millibars_per_minute(self) -> float:
+        """
+        
+        """
+        if self.__millibars_per_minute != None:
+            return self.__millibars_per_minute
+        self.__millibars_per_minute = self.__convert_from_base(PressureChangeRateUnits.MillibarPerMinute)
+        return self.__millibars_per_minute
+
+    
     def to_string(self, unit: PressureChangeRateUnits = PressureChangeRateUnits.PascalPerSecond) -> string:
         """
         Format the PressureChangeRate to string.
         Note! the default format for PressureChangeRate is PascalPerSecond.
         To specify the unit format set the 'unit' parameter.
         """
         
@@ -606,14 +762,20 @@
         
         if unit == PressureChangeRateUnits.PoundForcePerSquareInchPerSecond:
             return f"""{self.pounds_force_per_square_inch_per_second} psi/s"""
         
         if unit == PressureChangeRateUnits.PoundForcePerSquareInchPerMinute:
             return f"""{self.pounds_force_per_square_inch_per_minute} psi/min"""
         
+        if unit == PressureChangeRateUnits.BarPerSecond:
+            return f"""{self.bars_per_second} bar/s"""
+        
+        if unit == PressureChangeRateUnits.BarPerMinute:
+            return f"""{self.bars_per_minute} bar/min"""
+        
         if unit == PressureChangeRateUnits.KilopascalPerSecond:
             return f"""{self.kilopascals_per_second} """
         
         if unit == PressureChangeRateUnits.MegapascalPerSecond:
             return f"""{self.megapascals_per_second} """
         
         if unit == PressureChangeRateUnits.KilopascalPerMinute:
@@ -630,14 +792,20 @@
         
         if unit == PressureChangeRateUnits.KilopoundForcePerSquareInchPerMinute:
             return f"""{self.kilopounds_force_per_square_inch_per_minute} """
         
         if unit == PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute:
             return f"""{self.megapounds_force_per_square_inch_per_minute} """
         
+        if unit == PressureChangeRateUnits.MillibarPerSecond:
+            return f"""{self.millibars_per_second} """
+        
+        if unit == PressureChangeRateUnits.MillibarPerMinute:
+            return f"""{self.millibars_per_minute} """
+        
         return f'{self.__value}'
 
 
     def get_unit_abbreviation(self, unit_abbreviation: PressureChangeRateUnits = PressureChangeRateUnits.PascalPerSecond) -> string:
         """
         Get PressureChangeRate unit abbreviation.
         Note! the default abbreviation for PressureChangeRate is PascalPerSecond.
@@ -658,14 +826,20 @@
         
         if unit_abbreviation == PressureChangeRateUnits.PoundForcePerSquareInchPerSecond:
             return """psi/s"""
         
         if unit_abbreviation == PressureChangeRateUnits.PoundForcePerSquareInchPerMinute:
             return """psi/min"""
         
+        if unit_abbreviation == PressureChangeRateUnits.BarPerSecond:
+            return """bar/s"""
+        
+        if unit_abbreviation == PressureChangeRateUnits.BarPerMinute:
+            return """bar/min"""
+        
         if unit_abbreviation == PressureChangeRateUnits.KilopascalPerSecond:
             return """"""
         
         if unit_abbreviation == PressureChangeRateUnits.MegapascalPerSecond:
             return """"""
         
         if unit_abbreviation == PressureChangeRateUnits.KilopascalPerMinute:
@@ -682,14 +856,20 @@
         
         if unit_abbreviation == PressureChangeRateUnits.KilopoundForcePerSquareInchPerMinute:
             return """"""
         
         if unit_abbreviation == PressureChangeRateUnits.MegapoundForcePerSquareInchPerMinute:
             return """"""
         
+        if unit_abbreviation == PressureChangeRateUnits.MillibarPerSecond:
+            return """"""
+        
+        if unit_abbreviation == PressureChangeRateUnits.MillibarPerMinute:
+            return """"""
+        
 
     def __str__(self):
         return self.to_string()
 
 
     def __add__(self, other):
         if not isinstance(other, PressureChangeRate):
```

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/ratio.py` & `unitsnet-py-0.1.43/unitsnet_py/units/ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/ratio_change_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/ratio_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/reactive_energy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/reactive_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/reactive_power.py` & `unitsnet-py-0.1.43/unitsnet_py/units/reactive_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/reciprocal_area.py` & `unitsnet-py-0.1.43/unitsnet_py/units/reciprocal_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/reciprocal_length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/reciprocal_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/relative_humidity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/relative_humidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/rotational_acceleration.py` & `unitsnet-py-0.1.43/unitsnet_py/units/rotational_acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/rotational_speed.py` & `unitsnet-py-0.1.43/unitsnet_py/units/rotational_speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/rotational_stiffness.py` & `unitsnet-py-0.1.43/unitsnet_py/units/rotational_stiffness.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/rotational_stiffness_per_length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/rotational_stiffness_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/scalar.py` & `unitsnet-py-0.1.43/unitsnet_py/units/scalar.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/solid_angle.py` & `unitsnet-py-0.1.43/unitsnet_py/units/solid_angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/specific_energy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/specific_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/specific_entropy.py` & `unitsnet-py-0.1.43/unitsnet_py/units/specific_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/specific_fuel_consumption.py` & `unitsnet-py-0.1.43/unitsnet_py/units/specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/specific_volume.py` & `unitsnet-py-0.1.43/unitsnet_py/units/specific_volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/specific_weight.py` & `unitsnet-py-0.1.43/unitsnet_py/units/specific_weight.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/speed.py` & `unitsnet-py-0.1.43/unitsnet_py/units/speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/standard_volume_flow.py` & `unitsnet-py-0.1.43/unitsnet_py/units/standard_volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/temperature.py` & `unitsnet-py-0.1.43/unitsnet_py/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/temperature_change_rate.py` & `unitsnet-py-0.1.43/unitsnet_py/units/temperature_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/temperature_delta.py` & `unitsnet-py-0.1.43/unitsnet_py/units/temperature_delta.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/temperature_gradient.py` & `unitsnet-py-0.1.43/unitsnet_py/units/temperature_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/thermal_conductivity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/thermal_resistance.py` & `unitsnet-py-0.1.43/unitsnet_py/units/thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/torque.py` & `unitsnet-py-0.1.43/unitsnet_py/units/torque.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/torque_per_length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/torque_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/turbidity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/turbidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/vitamin_a.py` & `unitsnet-py-0.1.43/unitsnet_py/units/vitamin_a.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volume.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volume_concentration.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volume_flow.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volume_flow_per_area.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volume_flow_per_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volume_per_length.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volume_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/volumetric_heat_capacity.py` & `unitsnet-py-0.1.43/unitsnet_py/units/volumetric_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py/units/warping_moment_of_inertia.py` & `unitsnet-py-0.1.43/unitsnet_py/units/warping_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.42/unitsnet_py.egg-info/PKG-INFO` & `unitsnet-py-0.1.43/unitsnet_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.42
+Version: 0.1.43
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 Keywords: conversion,units-of-measure,units,quantities,unit-converter,converter,unit,measure,measures,measurement,measurements
@@ -316,15 +316,15 @@
 - **MolarFlow**
     -   *Molar flow is the ratio of the amount of substance change to the time during which the change occurred (value of amount of substance changes per unit time).*
 
 - **MolarMass**
     -   *In chemistry, the molar mass M is a physical property defined as the mass of a given substance (chemical element or chemical compound) divided by the amount of substance.*
 
 - **Molarity**
-    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume. *
+    -   *Molar concentration, also called molarity, amount concentration or substance concentration, is a measure of the concentration of a solute in a solution, or of any chemical species, in terms of amount of substance in a given volume.*
 
 - **Permeability**
     -   *In electromagnetism, permeability is the measure of the ability of a material to support the formation of a magnetic field within itself.*
 
 - **Permittivity**
     -   *In electromagnetism, permittivity is the measure of resistance that is encountered when forming an electric field in a particular medium.*
```

### Comparing `unitsnet-py-0.1.42/unitsnet_py.egg-info/SOURCES.txt` & `unitsnet-py-0.1.43/unitsnet_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

