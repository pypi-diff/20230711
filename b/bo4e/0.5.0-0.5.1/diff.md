# Comparing `tmp/bo4e-0.5.0.tar.gz` & `tmp/bo4e-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo4e-0.5.0.tar", last modified: Mon Jul  3 11:38:36 2023, max compression
+gzip compressed data, was "bo4e-0.5.1.tar", last modified: Tue Jul 11 11:24:15 2023, max compression
```

## Comparing `bo4e-0.5.0.tar` & `bo4e-0.5.1.tar`

### file list

```diff
@@ -1,447 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-03 11:38:22.000000 bo4e-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 11:38:22.000000 bo4e-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-03 11:38:22.000000 bo4e-0.5.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 11:38:22.000000 bo4e-0.5.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 11:38:22.000000 bo4e-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 11:38:22.000000 bo4e-0.5.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 11:38:22.000000 bo4e-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-03 11:38:22.000000 bo4e-0.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 11:38:22.000000 bo4e-0.5.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:22.000000 bo4e-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 11:38:36.862871 bo4e-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-03 11:38:22.000000 bo4e-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.822870 bo4e-0.5.0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.bo.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.com.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.enum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/test_uml.py
--rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/uml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.822870 bo4e-0.5.0/json_schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.826870 bo4e-0.5.0/json_schemas/bo/
--rw-r--r--   0 runner    (1001) docker     (123)    52157 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Angebot.json
--rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Ansprechpartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Ausschreibung.json
--rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Buendelvertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Energiemenge.json
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Fremdkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Geschaeftsobjekt.json
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Geschaeftspartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Kosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Lastgang.json
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/LastgangKompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)    24945 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Marktlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Marktteilnehmer.json
--rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Messlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Netznutzungsrechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Preisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    39186 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattDienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)    39843 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattHardware.json
--rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattKonzessionsabgabe.json
--rw-r--r--   0 runner    (1001) docker     (123)    39860 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattMessung.json
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattNetznutzung.json
--rw-r--r--   0 runner    (1001) docker     (123)    36100 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Rechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Region.json
--rw-r--r--   0 runner    (1001) docker     (123)    61951 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Regionaltarif.json
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Standorteigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)    59198 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarif.json
--rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)    44628 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)    56245 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifpreisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26552 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Vertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Zaehler.json
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Zeitreihe.json
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/_LastgangBody.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.830870 bo4e-0.5.0/json_schemas/com/
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Adresse.json
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsvariante.json
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagRegional.json
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Ausschreibungsdetail.json
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Ausschreibungslos.json
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Betrag.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/COM.json
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Dienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Energieherkunft.json
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Energiemix.json
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/ExterneReferenz.json
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Fremdkostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Fremdkostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geokoordinaten.json
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geraet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geraeteeigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Hardware.json
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Katasteradresse.json
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Kostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Kostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/KriteriumWert.json
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/MarktgebietInfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Menge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Messlokationszuordnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/PositionsAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Rechnungsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionaleGueltigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalePreisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalePreisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionaleTarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalerAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Regionskriterium.json
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Rufnummer.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Sigmoidparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenAllgemein.json
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenGas.json
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenStrom.json
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Steuerbetrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tagesvektor.json
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifberechnungsparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifeinschraenkung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifpreis.json
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/TarifpreispositionProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/TarifpreisstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Unterschrift.json
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Verbrauch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Vertragskonditionen.json
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Vertragsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zaehlwerk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitintervall.json
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitraum.json
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitreihenwert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitreihenwertkompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zustaendigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-03 11:38:22.000000 bo4e-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 11:38:22.000000 bo4e-0.5.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 11:38:22.000000 bo4e-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-03 11:38:36.862871 bo4e-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 11:38:22.000000 bo4e-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.814869 bo4e-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e/bo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/zeitreihe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.842871 bo4e-0.5.0/src/bo4e/com/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/com.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/externereferenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/rufnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zustaendigkeit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.850871 bo4e-0.5.0/src/bo4e/enum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/anrede.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/artikelid.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/botyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/energierichtung.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geraetemerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kontaktart.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundentyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/landescode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/marktrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messart.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/netzebene.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/nnrechnungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/nnrechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/oekolabel.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preismodell.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preisstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rufnummernart.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/sparte.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifart.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tariftyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/themengebiet.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/titel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsform.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zeiteinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.850871 bo4e-0.5.0/src/bo4e/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/serialization_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_bypassing_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.814869 bo4e-0.5.0/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/tests/test_data/test_data_adresse/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_externe_referenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kriteriumswert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_lastgangkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_messung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-03 11:38:22.000000 bo4e-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.660151 bo4e-0.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-11 11:24:01.000000 bo4e-0.5.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-11 11:24:01.000000 bo4e-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-11 11:24:01.000000 bo4e-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-11 11:24:01.000000 bo4e-0.5.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-11 11:24:01.000000 bo4e-0.5.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-11 11:24:01.000000 bo4e-0.5.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-11 11:24:01.000000 bo4e-0.5.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 11:24:01.000000 bo4e-0.5.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-11 11:24:01.000000 bo4e-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-11 11:24:01.000000 bo4e-0.5.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:24:01.000000 bo4e-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-11 11:24:15.660151 bo4e-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-11 11:24:01.000000 bo4e-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.628151 bo4e-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.628151 bo4e-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/_static/bo4e-python-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.628151 bo4e-0.5.1/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/api/bo4e.bo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/api/bo4e.com.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/api/bo4e.enum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/api/bo4e.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/test_uml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28380 2023-07-11 11:24:01.000000 bo4e-0.5.1/docs/uml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.628151 bo4e-0.5.1/json_schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.632151 bo4e-0.5.1/json_schemas/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)    52157 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Angebot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Ansprechpartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Ausschreibung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Buendelvertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Energiemenge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Fremdkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Geschaeftsobjekt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Geschaeftspartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Kosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Lastgang.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/LastgangKompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24945 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Marktlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Marktteilnehmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Messlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Netznutzungsrechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Preisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39186 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/PreisblattDienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39843 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/PreisblattHardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/PreisblattKonzessionsabgabe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39860 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/PreisblattMessung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/PreisblattNetznutzung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36100 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Rechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Region.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61951 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Regionaltarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Standorteigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59198 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Tarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Tarifinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44628 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Tarifkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56245 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Tarifpreisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26552 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Vertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Zaehler.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/Zeitreihe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/bo/_LastgangBody.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.636151 bo4e-0.5.1/json_schemas/com/
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Adresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Angebotsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Angebotsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Angebotsvariante.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/AufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/AufAbschlagProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/AufAbschlagRegional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/AufAbschlagstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Ausschreibungsdetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Ausschreibungslos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Betrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/COM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Dienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Energieherkunft.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Energiemix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/ExterneReferenz.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Fremdkostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Fremdkostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Geokoordinaten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Geraet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Geraeteeigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Hardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Katasteradresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Kostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Kostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/KriteriumWert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/MarktgebietInfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Menge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Messlokationszuordnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/PositionsAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Preis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Preisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Preisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Preisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Rechnungsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/RegionaleGueltigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/RegionalePreisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/RegionalePreisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/RegionaleTarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/RegionalerAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Regionskriterium.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Rufnummer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Sigmoidparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/StandorteigenschaftenAllgemein.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/StandorteigenschaftenGas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/StandorteigenschaftenStrom.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Steuerbetrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Tagesvektor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Tarifberechnungsparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Tarifeinschraenkung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Tarifpreis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Tarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/TarifpreispositionProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/TarifpreisstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Unterschrift.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Verbrauch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Vertragskonditionen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Vertragsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zaehlwerk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zeitintervall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zeitraum.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zeitreihenwert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zeitreihenwertkompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/com/Zustaendigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-11 11:24:01.000000 bo4e-0.5.1/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-11 11:24:01.000000 bo4e-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 11:24:01.000000 bo4e-0.5.1/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-11 11:24:01.000000 bo4e-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-11 11:24:15.660151 bo4e-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 11:24:01.000000 bo4e-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.636151 bo4e-0.5.1/src/bo4e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.640151 bo4e-0.5.1/src/bo4e/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/bo/zeitreihe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.644151 bo4e-0.5.1/src/bo4e/com/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/externereferenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/rufnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/com/zustaendigkeit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.652151 bo4e-0.5.1/src/bo4e/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/anrede.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/artikelid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/botyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/geraetemerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/landescode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/messart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/netzebene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/nnrechnungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/nnrechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/preismodell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/preistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/rufnummernart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/sparte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tarifart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/titel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/enum/zeiteinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.652151 bo4e-0.5.1/src/bo4e/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-11 11:24:01.000000 bo4e-0.5.1/src/bo4e/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.636151 bo4e-0.5.1/src/bo4e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13420 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 11:24:15.000000 bo4e-0.5.1/src/bo4e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.660151 bo4e-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/serialization_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_bypassing_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.624151 bo4e-0.5.1/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:24:15.660151 bo4e-0.5.1/tests/test_data/test_data_adresse/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_externe_referenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_kriteriumswert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_lastgangkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9738 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblatt_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblatt_messung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zeitreihe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/test_zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 11:24:01.000000 bo4e-0.5.1/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-11 11:24:01.000000 bo4e-0.5.1/tox.ini
```

### Comparing `bo4e-0.5.0/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-0.5.1/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-0.5.1/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/dependabot.yml` & `bo4e-0.5.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/codeql-analysis.yml` & `bo4e-0.5.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/coverage.yml` & `bo4e-0.5.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/docs.yml` & `bo4e-0.5.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/formatting.yml` & `bo4e-0.5.1/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/linting.yml` & `bo4e-0.5.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/python-publish.yml` & `bo4e-0.5.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.github/workflows/tests.yml` & `bo4e-0.5.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.gitignore` & `bo4e-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.pre-commit-config.yaml` & `bo4e-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.pylintrc` & `bo4e-0.5.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/.readthedocs.yaml` & `bo4e-0.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/CONTRIBUTING.md` & `bo4e-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/LICENSE.rst` & `bo4e-0.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/PKG-INFO` & `bo4e-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.5.0/README.rst` & `bo4e-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/Makefile` & `bo4e-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/_static/bo4e-python-favicon.png` & `bo4e-0.5.1/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/_static/bo4e-python-favicon.svg` & `bo4e-0.5.1/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/_static/bo4e-python-logo.png` & `bo4e-0.5.1/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/_static/bo4e-python-logo.svg` & `bo4e-0.5.1/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/api/bo4e.bo.rst` & `bo4e-0.5.1/docs/api/bo4e.bo.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/api/bo4e.com.rst` & `bo4e-0.5.1/docs/api/bo4e.com.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/api/bo4e.enum.rst` & `bo4e-0.5.1/docs/api/bo4e.enum.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/conf.py` & `bo4e-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/index.rst` & `bo4e-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/requirements.txt` & `bo4e-0.5.1/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/docs/uml.py` & `bo4e-0.5.1/docs/uml.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 import os
 import pkgutil
 import re
 import shlex
 import subprocess
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Type, cast
+from types import NoneType
+from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast, get_args
 
-import networkx as nx  # type: ignore[import]
-import requests  # type: ignore[import]
-from pydantic._internal._model_construction import ModelMetaclass
+import networkx as nx
+import requests
+from annotated_types import Len, MaxLen, MinLen
+from pydantic import BaseModel
 from pydantic._internal._repr import display_as_type
 from pydantic.fields import FieldInfo
+from typeguard import TypeCheckError, check_type
 
 
 # pylint: disable=too-few-public-methods
 class _Package:
     """
     Encapsulates scope and color options into a class to make linter and type checker happier
     """
@@ -98,27 +101,27 @@
             """
             This method is designed to be assigned as hash function for dictionaries. In this case specifically used for
             `**kwargs` in `get_node_str` and `get_edge_str` for caching purposes. See those functions for more
             information.
             """
             return hash(json.dumps(self, sort_keys=True))
 
-    def add_class(self, node: str, cls: ModelMetaclass) -> None:
+    def add_class(self, node: str, cls: type[BaseModel]) -> None:
         """
-        Adds a class to the UML-Network. It copies the __fields__ dictionary because it will possibly be mutated when
+        Adds a class to the UML-Network. It copies the model_fields dictionary because it will possibly be mutated when
         adding superclasses to the network.
         """
         super().add_node(
             node,
             cls=cls,
             fields={
                 field_name: {"model_field": model_field, "card": None}
-                for field_name, model_field in cls.__fields__.items()
+                for field_name, model_field in cls.model_fields.items()
             }
-            if hasattr(cls, "__fields__")
+            if hasattr(cls, "model_fields")
             else {},
         )
 
     def add_extension(self, node1: str, node2: str) -> None:
         """
         Adds an extension-relation: node1 🠒 node2. All fields of the superclass will be removed in node1 to improve
         clarity.
@@ -218,41 +221,15 @@
     @staticmethod
     def model_field_str(model_field: FieldInfo, card: Optional[Cardinality] = None) -> str:
         """
         Parse the type of the ModelField to a printable string. Copied from
         pydantic._internal._repr.display_as_type
         https://github.com/pydantic/pydantic/blob/58ae1ef77a4bf4276aaa6214aaaaf59455f5e587/pydantic/_internal/_repr.py#L85
         """
-        result_str = display_as_type(model_field.annotation)
-        # todo: check if this is still necessary
-        # https://github.com/bo4e/BO4E-python/issues/478
-        # have to do this since display_as_type(self.outer_type_) is different (and wrong) on python 3.6
-        # if model_field.shape in MAPPING_LIKE_SHAPES:
-        #    result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
-        # elif model_field.shape == SHAPE_TUPLE:
-        #    result_str = "Tuple[" + ", ".join(
-        #        display_as_type(
-        #            sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
-        #        )
-        #    )
-        #    result_str += "]"
-        # elif model_field.shape == SHAPE_GENERIC:
-        #    assert model_field.sub_fields
-        #    result_str = (
-        #        f"{display_as_type(model_field.type_)}["
-        #        f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
-        #    )
-        # elif model_field.shape not in (SHAPE_SINGLETON, SHAPE_LIST):
-        #    result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
-        #
-        # if is_constrained_str(model_field):
-        #    if isinstance(model_field.outer_type_.regex, Pattern):
-        #        result_str = f"str<{model_field.outer_type_.regex.pattern}>"
-        #    elif isinstance(model_field.outer_type_.regex, str):
-        #        result_str = f"str<{model_field.outer_type_.regex}>"
+        result_str = display_as_type(get_referenced_inner_type(model_field.annotation))
         assert card is not None
         return f"{result_str} [{_UMLNetworkABC.get_cardinality_string(card)}]"
 
     @staticmethod
     def _remove_last_package_name(namespace: str) -> str:
         """
         E.g. `_remove_last_package_name('bo4e.bo.angebot.Angebot')` -> `bo4e.bo.Angebot`. The only use of this function
@@ -278,16 +255,16 @@
             f'class "[[{LINK_URI_BASE}/api/bo4e.{node.split(".")[1]}.html#{node}'
             f' {node.split(".")[-1]}]]\\n<size:10>{".".join(node.split(".")[0:-1])}" as {node.split(".")[-1]}'
         )
         if detailed:
             cls_str += " {\n"
             for field_dict in self.nodes[node]["fields"].values():
                 model_field: FieldInfo = field_dict["model_field"]
-                assert model_field.annotation is not None
-                type_modl_namespace = f"{model_field.annotation.__module__}.{model_field.annotation.__name__}"
+                model_field_inner_type = get_referenced_inner_type(model_field.annotation)
+                type_modl_namespace = f"{model_field_inner_type.__module__}.{model_field_inner_type.__name__}"
                 if type_modl_namespace in self[node]:
                     # Skip the fields which will appear as references in the graph
                     continue
                 type_str = _UMLNetworkABC.model_field_str(model_field, field_dict["card"])
                 if model_field.is_required():
                     cls_str += f"\t{model_field.alias} : {type_str}\n"
                 else:
@@ -444,66 +421,82 @@
         with open(file_path / file_name, "w+", encoding="utf-8") as uml_file:
             uml_file.write(file_content)
             path_list.append(file_path / file_name)
 
     return path_list
 
 
-def model_field_str(model_field: FieldInfo) -> str:
-    """
-    Parse the type of the ModelField to a printable string. Copied from pydantic.field.ModelField._type_display()
-    """
-    result_str = display_as_type(model_field.annotation)
-    # todo: check if this is still necessary
-    # https://github.com/bo4e/BO4E-python/issues/478
-    # have to do this since display_as_type(self.outer_type_) is different (and wrong) on python 3.6
-    # if model_field.shape in MAPPING_LIKE_SHAPES:
-    #    result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
-    # elif model_field.shape == SHAPE_TUPLE:
-    #    result_str = "Tuple[" + ", ".join(
-    #        display_as_type(
-    #            sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
-    #        )
-    #    )
-    #    result_str += "]"
-    # elif model_field.shape == SHAPE_GENERIC:
-    #    assert model_field.sub_fields
-    #    result_str = (
-    #        f"{display_as_type(model_field.type_)}["
-    #        f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
-    #    )
-    # elif model_field.shape != SHAPE_SINGLETON:
-    #    result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
-    # if model_field.allow_none and (model_field.shape != SHAPE_SINGLETON or not model_field.sub_fields):
-    #    result_str = f"Optional[{result_str}]"
-    return result_str
-
-
 def get_cardinality(model_field: FieldInfo) -> Cardinality:
     """
     Determines the cardinality of a field. This field can either contain a reference to another node in the graph or
     be of another arbitrary type.
     """
-    type_str = model_field_str(model_field)
     card1: str = "1"
     card2: str = "1"
-    if type_str.startswith("Optional["):
+    try:
+        check_type(None, model_field.annotation)
+        # The field can be None
         card1 = "0"
-    if type_str.startswith("List[") or type_str.startswith("Optional[List["):
+    except TypeCheckError:
+        pass
+    try:
+        check_type([], model_field.annotation)
+        # The field can be a list
         card1 = "0"
         card2 = "*"
-        # todo: re-add min_length / max_length interpretation
-        # https://github.com/bo4e/BO4E-python/issues/477
-        # if hasattr(model_field.outer_type_, "max_items") and model_field.outer_type_.max_items:
-        #    card2 = str(model_field.outer_type_.max_items)
-        # if hasattr(model_field.outer_type_, "min_items") and model_field.outer_type_.min_items:
-        #    card1 = str(model_field.outer_type_.min_items)
+        for metadate in model_field.metadata:
+            # min-length and max-length are stored as entries in the metadata list
+            if isinstance(metadate, MinLen):
+                card1 = str(metadate.min_length)
+            elif isinstance(metadate, MaxLen):
+                card2 = str(metadate.max_length)
+            elif isinstance(metadate, Len):
+                card1 = str(metadate.min_length)
+                if metadate.max_length is not None:
+                    card2 = str(metadate.max_length)
+    except TypeCheckError:
+        pass
     return card1, card2
 
 
+def get_referenced_inner_type(type_annotation: Any) -> Any:
+    """
+    Returns the inner type of a list or optional type annotation.
+    Should also handle nested types like Optional[List[...]].
+    If the type annotation is not a list or optional type, the type annotation itself is returned.
+    """
+    while True:
+        if not hasattr(type_annotation, "__origin__"):
+            return type_annotation
+        # pylint: disable=protected-access
+        if type_annotation.__origin__ is Union and type_annotation._name == "Optional":
+            # Optional is internally a Union with None. We want to ignore the None type.
+            generic_alias_args = get_args(type_annotation)
+            generic_alias_args = tuple(
+                generic_alias_arg for generic_alias_arg in generic_alias_args if generic_alias_arg is not NoneType
+            )
+        elif type_annotation.__origin__ is list:
+            generic_alias_args = get_args(type_annotation)
+        elif hasattr(type_annotation, "__metadata__"):
+            # This is Annotated[...]
+            generic_alias_args = (type_annotation.__origin__,)
+        else:
+            return type_annotation
+        if len(generic_alias_args) > 1:
+            raise TypeError(
+                f"Could not determine inner type of {type_annotation}: Too many generic alias args {generic_alias_args}"
+            )
+        if len(generic_alias_args) == 0:
+            raise TypeError(
+                f"Could not determine inner type of {type_annotation}: "
+                f"Undefined generic alias args {generic_alias_args}"
+            )
+        type_annotation = generic_alias_args[0]
+
+
 def build_network(module_dir: Path, parser: Type[_UMLNetworkABC]) -> Tuple[_UMLNetworkABC, List[str]]:
     """
     Build a network of the relationships of all classes found in bo4e packages defined by `pkgs` and all classes
     referenced by any class in these packages. Referenced classes will be added only if `regex_incl_network` matches and
     `regex_excl_network` does not match the namespace name of the respective class (e.g. `bo4e.bo.angebot.Angebot`).
     """
     uml_network = parser()
@@ -524,46 +517,47 @@
                 namespaces_to_parse.append(modl_namespace)
                 if not uml_network.has_node(modl_namespace):
                     _recursive_add_class(cls, modl_namespace, uml_network)
     return uml_network, namespaces_to_parse
 
 
 def _recursive_add_class(
-    cls_cur: ModelMetaclass,
+    cls_cur: type[BaseModel],
     modl_namespace: str,
     uml_network: _UMLNetworkABC,
 ) -> None:
     """
     Add the specified class `cls_cur` to the `uml_network` and recursively add all classes found in fields and
     bases including all matching `regex_incl_network` but excluding all matching 'regex_excl_network'. If both regex
     are conflicting, the respective class will not be added.
     """
     uml_network.add_class(modl_namespace, cls=cls_cur)
     # ------ add base classes to the network which pass `regex_incl_network` and `regex_excl_network` ------------------
     for parent in cls_cur.__bases__:
         type_modl_namespace = f"{parent.__module__}.{parent.__name__}"
         if re.match(regex_incl_network, type_modl_namespace) and not re.match(regex_excl_network, type_modl_namespace):
             if not uml_network.has_node(type_modl_namespace):
-                _recursive_add_class(cast(ModelMetaclass, parent), type_modl_namespace, uml_network)
+                _recursive_add_class(cast(type[BaseModel], parent), type_modl_namespace, uml_network)
             uml_network.add_extension(
                 modl_namespace,
                 type_modl_namespace,
             )
     # ------------------------------------------------------------------------------------------------------------------
     # ------ determine references in fields which pass `regex_incl_network` and `regex_excl_network` -------------------
     for field_dict in uml_network.nodes[modl_namespace]["fields"].values():
         model_field: FieldInfo = field_dict["model_field"]
+        model_inner_type = get_referenced_inner_type(model_field.annotation)
         # Add cardinality information to the field
         field_card = get_cardinality(model_field)
         field_dict["card"] = field_card
         assert model_field.annotation is not None
-        type_modl_namespace = f"{model_field.annotation.__module__}.{model_field.annotation.__name__}"
+        type_modl_namespace = f"{model_inner_type.__module__}.{model_inner_type.__name__}"
         if re.match(regex_incl_network, type_modl_namespace) and not re.match(regex_excl_network, type_modl_namespace):
             if not uml_network.has_node(type_modl_namespace):
-                _recursive_add_class(model_field.annotation, type_modl_namespace, uml_network)  # type:ignore[arg-type]
+                _recursive_add_class(model_inner_type, type_modl_namespace, uml_network)
 
             uml_network.add_association(
                 modl_namespace,
                 type_modl_namespace,
                 through_field=model_field,
                 card1=None,
                 card2=field_card,
@@ -579,15 +573,15 @@
     url = "https://kroki.io"
     for root, _, files in os.walk(input_dir):
         for file in files:
             with open(os.path.join(root, file), "r", encoding="utf-8") as uml_file:
                 answer = requests.post(
                     url,
                     json={"diagram_source": uml_file.read(), "diagram_type": "plantuml", "output_format": "svg"},
-                    timeout=5,
+                    timeout=15,
                 )
                 subdir = root[len(str(input_dir)) + 1 :]
                 os.makedirs(output_dir / subdir, exist_ok=True)
                 with open(output_dir / subdir / re.sub(r"\.puml$", ".svg", file), "w+", encoding="utf-8") as svg_file:
                     svg_file.write(answer.text)
```

### Comparing `bo4e-0.5.0/json_schemas/bo/Angebot.json` & `bo4e-0.5.1/json_schemas/bo/Angebot.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Ansprechpartner.json` & `bo4e-0.5.1/json_schemas/bo/Ansprechpartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Ausschreibung.json` & `bo4e-0.5.1/json_schemas/bo/Ausschreibung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Buendelvertrag.json` & `bo4e-0.5.1/json_schemas/bo/Buendelvertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Energiemenge.json` & `bo4e-0.5.1/json_schemas/bo/Energiemenge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Fremdkosten.json` & `bo4e-0.5.1/json_schemas/bo/Fremdkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Geschaeftsobjekt.json` & `bo4e-0.5.1/json_schemas/bo/Geschaeftsobjekt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Geschaeftspartner.json` & `bo4e-0.5.1/json_schemas/bo/Geschaeftspartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Kosten.json` & `bo4e-0.5.1/json_schemas/bo/Kosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Lastgang.json` & `bo4e-0.5.1/json_schemas/bo/Lastgang.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/LastgangKompakt.json` & `bo4e-0.5.1/json_schemas/bo/LastgangKompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Marktlokation.json` & `bo4e-0.5.1/json_schemas/bo/Marktlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Marktteilnehmer.json` & `bo4e-0.5.1/json_schemas/bo/Marktteilnehmer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Messlokation.json` & `bo4e-0.5.1/json_schemas/bo/Messlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Netznutzungsrechnung.json` & `bo4e-0.5.1/json_schemas/bo/Netznutzungsrechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Preisblatt.json` & `bo4e-0.5.1/json_schemas/bo/Preisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/PreisblattDienstleistung.json` & `bo4e-0.5.1/json_schemas/bo/PreisblattDienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/PreisblattHardware.json` & `bo4e-0.5.1/json_schemas/bo/PreisblattHardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/PreisblattKonzessionsabgabe.json` & `bo4e-0.5.1/json_schemas/bo/PreisblattKonzessionsabgabe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/PreisblattMessung.json` & `bo4e-0.5.1/json_schemas/bo/PreisblattMessung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/PreisblattNetznutzung.json` & `bo4e-0.5.1/json_schemas/bo/PreisblattNetznutzung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Rechnung.json` & `bo4e-0.5.1/json_schemas/bo/Rechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Region.json` & `bo4e-0.5.1/json_schemas/bo/Region.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Regionaltarif.json` & `bo4e-0.5.1/json_schemas/bo/Regionaltarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Standorteigenschaften.json` & `bo4e-0.5.1/json_schemas/bo/Standorteigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Tarif.json` & `bo4e-0.5.1/json_schemas/bo/Tarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Tarifinfo.json` & `bo4e-0.5.1/json_schemas/bo/Tarifinfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Tarifkosten.json` & `bo4e-0.5.1/json_schemas/bo/Tarifkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Tarifpreisblatt.json` & `bo4e-0.5.1/json_schemas/bo/Tarifpreisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Vertrag.json` & `bo4e-0.5.1/json_schemas/bo/Vertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Zaehler.json` & `bo4e-0.5.1/json_schemas/bo/Zaehler.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/Zeitreihe.json` & `bo4e-0.5.1/json_schemas/bo/Zeitreihe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/bo/_LastgangBody.json` & `bo4e-0.5.1/json_schemas/bo/_LastgangBody.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Adresse.json` & `bo4e-0.5.1/json_schemas/com/Adresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Angebotsposition.json` & `bo4e-0.5.1/json_schemas/com/Angebotsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Angebotsteil.json` & `bo4e-0.5.1/json_schemas/com/Angebotsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Angebotsvariante.json` & `bo4e-0.5.1/json_schemas/com/Angebotsvariante.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/AufAbschlag.json` & `bo4e-0.5.1/json_schemas/com/AufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/AufAbschlagProOrt.json` & `bo4e-0.5.1/json_schemas/com/AufAbschlagProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/AufAbschlagRegional.json` & `bo4e-0.5.1/json_schemas/com/AufAbschlagRegional.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/AufAbschlagstaffelProOrt.json` & `bo4e-0.5.1/json_schemas/com/AufAbschlagstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Ausschreibungsdetail.json` & `bo4e-0.5.1/json_schemas/com/Ausschreibungsdetail.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Ausschreibungslos.json` & `bo4e-0.5.1/json_schemas/com/Ausschreibungslos.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Betrag.json` & `bo4e-0.5.1/json_schemas/com/Betrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Dienstleistung.json` & `bo4e-0.5.1/json_schemas/com/Dienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Energieherkunft.json` & `bo4e-0.5.1/json_schemas/com/Energieherkunft.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Energiemix.json` & `bo4e-0.5.1/json_schemas/com/Energiemix.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/ExterneReferenz.json` & `bo4e-0.5.1/json_schemas/com/ExterneReferenz.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Fremdkostenblock.json` & `bo4e-0.5.1/json_schemas/com/Fremdkostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Fremdkostenposition.json` & `bo4e-0.5.1/json_schemas/com/Fremdkostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Geokoordinaten.json` & `bo4e-0.5.1/json_schemas/com/Geokoordinaten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Geraet.json` & `bo4e-0.5.1/json_schemas/com/Geraet.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Geraeteeigenschaften.json` & `bo4e-0.5.1/json_schemas/com/Geraeteeigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Hardware.json` & `bo4e-0.5.1/json_schemas/com/Hardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Katasteradresse.json` & `bo4e-0.5.1/json_schemas/com/Katasteradresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Kostenblock.json` & `bo4e-0.5.1/json_schemas/com/Kostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Kostenposition.json` & `bo4e-0.5.1/json_schemas/com/Kostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/KriteriumWert.json` & `bo4e-0.5.1/json_schemas/com/KriteriumWert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/MarktgebietInfo.json` & `bo4e-0.5.1/json_schemas/com/MarktgebietInfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Menge.json` & `bo4e-0.5.1/json_schemas/com/Menge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Messlokationszuordnung.json` & `bo4e-0.5.1/json_schemas/com/Messlokationszuordnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/PositionsAufAbschlag.json` & `bo4e-0.5.1/json_schemas/com/PositionsAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Preis.json` & `bo4e-0.5.1/json_schemas/com/Preis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Preisgarantie.json` & `bo4e-0.5.1/json_schemas/com/Preisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Preisposition.json` & `bo4e-0.5.1/json_schemas/com/Preisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Preisstaffel.json` & `bo4e-0.5.1/json_schemas/com/Preisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Rechnungsposition.json` & `bo4e-0.5.1/json_schemas/com/Rechnungsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/RegionaleGueltigkeit.json` & `bo4e-0.5.1/json_schemas/com/RegionaleGueltigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/RegionalePreisgarantie.json` & `bo4e-0.5.1/json_schemas/com/RegionalePreisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/RegionalePreisstaffel.json` & `bo4e-0.5.1/json_schemas/com/RegionalePreisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/RegionaleTarifpreisposition.json` & `bo4e-0.5.1/json_schemas/com/RegionaleTarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/RegionalerAufAbschlag.json` & `bo4e-0.5.1/json_schemas/com/RegionalerAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Regionskriterium.json` & `bo4e-0.5.1/json_schemas/com/Regionskriterium.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Rufnummer.json` & `bo4e-0.5.1/json_schemas/com/Rufnummer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Sigmoidparameter.json` & `bo4e-0.5.1/json_schemas/com/Sigmoidparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenAllgemein.json` & `bo4e-0.5.1/json_schemas/com/StandorteigenschaftenAllgemein.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenGas.json` & `bo4e-0.5.1/json_schemas/com/StandorteigenschaftenGas.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenStrom.json` & `bo4e-0.5.1/json_schemas/com/StandorteigenschaftenStrom.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Steuerbetrag.json` & `bo4e-0.5.1/json_schemas/com/Steuerbetrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Tagesvektor.json` & `bo4e-0.5.1/json_schemas/com/Tagesvektor.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Tarifberechnungsparameter.json` & `bo4e-0.5.1/json_schemas/com/Tarifberechnungsparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Tarifeinschraenkung.json` & `bo4e-0.5.1/json_schemas/com/Tarifeinschraenkung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Tarifpreis.json` & `bo4e-0.5.1/json_schemas/com/Tarifpreis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Tarifpreisposition.json` & `bo4e-0.5.1/json_schemas/com/Tarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/TarifpreispositionProOrt.json` & `bo4e-0.5.1/json_schemas/com/TarifpreispositionProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/TarifpreisstaffelProOrt.json` & `bo4e-0.5.1/json_schemas/com/TarifpreisstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Unterschrift.json` & `bo4e-0.5.1/json_schemas/com/Unterschrift.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Verbrauch.json` & `bo4e-0.5.1/json_schemas/com/Verbrauch.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Vertragskonditionen.json` & `bo4e-0.5.1/json_schemas/com/Vertragskonditionen.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Vertragsteil.json` & `bo4e-0.5.1/json_schemas/com/Vertragsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zaehlwerk.json` & `bo4e-0.5.1/json_schemas/com/Zaehlwerk.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zeitintervall.json` & `bo4e-0.5.1/json_schemas/com/Zeitintervall.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zeitraum.json` & `bo4e-0.5.1/json_schemas/com/Zeitraum.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zeitreihenwert.json` & `bo4e-0.5.1/json_schemas/com/Zeitreihenwert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zeitreihenwertkompakt.json` & `bo4e-0.5.1/json_schemas/com/Zeitreihenwertkompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/com/Zustaendigkeit.json` & `bo4e-0.5.1/json_schemas/com/Zustaendigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/json_schemas/generate_json_schemas.py` & `bo4e-0.5.1/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/pyproject.toml` & `bo4e-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/setup.cfg` & `bo4e-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/angebot.py` & `bo4e-0.5.1/src/bo4e/bo/angebot.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Contains Angebot class and corresponding marshmallow schema for de-/serialization
 """
 
 from datetime import datetime
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist, constr
+from annotated_types import Len
+from pydantic import Field
 
 from bo4e.bo.ansprechpartner import Ansprechpartner
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.angebotsvariante import Angebotsvariante
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.sparte import Sparte
@@ -34,25 +35,25 @@
 
 
     """
 
     bo_typ: BoTyp = BoTyp.ANGEBOT
     # required attributes
     #: Eindeutige Nummer des Angebotes
-    angebotsnummer: constr(strict=True, pattern=r"^\d+$")  # type: ignore[valid-type]
+    angebotsnummer: Annotated[str, Field(strict=True, pattern=r"^\d+$")]
     #: Erstellungsdatum des Angebots
     angebotsdatum: datetime
     #: Sparte, für die das Angebot abgegeben wird (Strom/Gas)
     sparte: Sparte
     #: Ersteller des Angebots
     angebotsgeber: Geschaeftspartner
     #: Empfänger des Angebots
     angebotsnehmer: Geschaeftspartner
 
-    varianten: conlist(Angebotsvariante, min_length=1)  # type: ignore[valid-type]
+    varianten: Annotated[list[Angebotsvariante], Len(1)]
     """ Eine oder mehrere Varianten des Angebots mit den Angebotsteilen;
     Ein Angebot besteht mindestens aus einer Variante."""
 
     # optional attributes
     anfragereferenz: Optional[str] = None
     """	Referenz auf eine Anfrage oder Ausschreibung;
     Kann dem Empfänger des Angebotes bei Zuordnung des Angebotes zur Anfrage bzw. Ausschreibung helfen."""
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/ansprechpartner.py` & `bo4e-0.5.1/src/bo4e/bo/ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/ausschreibung.py` & `bo4e-0.5.1/src/bo4e/bo/ausschreibung.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Ausschreibung class and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.ausschreibungslos import Ausschreibungslos
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.ausschreibungsportal import Ausschreibungsportal
 from bo4e.enum.ausschreibungsstatus import Ausschreibungsstatus
@@ -56,14 +56,14 @@
     """
     bindefrist: Zeitraum
     """
     Diese Komponente wird zur Abbildung von Zeiträumen in Form von Dauern oder der Angabe von Start und Ende verwendet.
     Es muss daher entweder eine Dauer oder ein Zeitraum in Form von Start und Ende angegeben sein
     """
     #: Die einzelnen Lose, aus denen sich die Ausschreibung zusammensetzt
-    lose: conlist(Ausschreibungslos, min_length=1)  # type: ignore[valid-type]
+    lose: Annotated[list[Ausschreibungslos], Len(1)]
 
     # optional attributes
     #: Aufzählung der unterstützten Ausschreibungsportale
     ausschreibungportal: Optional[Ausschreibungsportal] = None
     #: Internetseite, auf der die Ausschreibung veröffentlicht wurde (falls vorhanden)
     webseite: Optional[str] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/buendelvertrag.py` & `bo4e-0.5.1/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/energiemenge.py` & `bo4e-0.5.1/src/bo4e/bo/energiemenge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains Energiemenge class
 and corresponding marshmallow schema for de-/serialization
 """
+from typing import Annotated
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.verbrauch import Verbrauch
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.lokationstyp import Lokationstyp
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Energiemenge(Geschaeftsobjekt):
     """
     Abbildung von Mengen, die Lokationen zugeordnet sind
 
     .. raw:: html
 
@@ -31,9 +33,9 @@
     #: Eindeutige Nummer der Marktlokation bzw. der Messlokation, zu der die Energiemenge gehört
     lokations_id: str
     # todo: add validator such that only mess- or marktlokations IDs are accepted + cross check with lokationstyp
     #: Gibt an, ob es sich um eine Markt- oder Messlokation handelt
     lokationstyp: Lokationstyp
 
     #: Gibt den Verbrauch in einer Zeiteinheit an
-    energieverbrauch: conlist(Verbrauch, min_length=1)  # type: ignore[valid-type]
+    energieverbrauch: Annotated[list[Verbrauch], Len(1)]
     # there are no optional attributes
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/fremdkosten.py` & `bo4e-0.5.1/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-0.5.1/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=missing-module-docstring
 from decimal import Decimal
 from typing import List, Optional
 
 from humps.main import camelize
 
 # pylint: disable=no-name-in-module
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from bo4e.com.externereferenz import ExterneReferenz
 from bo4e.enum.botyp import BoTyp
 
 # pylint: disable=too-few-public-methods
 
 
@@ -32,17 +32,20 @@
     bo_typ: BoTyp = BoTyp.GESCHAEFTSOBJEKT  #: Der Typ des Geschäftsobjektes
     # bo_typ is used as discriminator f.e. for databases or deserialization
 
     # optional attributes
     externe_referenzen: Optional[List[ExterneReferenz]] = []
 
     #: Hier können IDs anderer Systeme hinterlegt werden (z.B. eine SAP-GP-Nummer oder eine GUID)
-    # pylint:disable=duplicate-code
-    class Config:
-        """
-        basic configuration for pydantic's behaviour
-        """
-
-        alias_generator = camelize
-        populate_by_name = True
-        extra = "allow"
-        json_encoders = {Decimal: str}
+    # pylint: disable=duplicate-code
+    model_config = ConfigDict(
+        alias_generator=camelize,
+        populate_by_name=True,
+        extra="allow",
+        # json_encoders is deprecated, but there is no easy-to-use alternative. The best way would be to create
+        # an annotated version of Decimal, but you would have to use it everywhere in the pydantic models.
+        # See this issue for more info: https://github.com/pydantic/pydantic/issues/6375
+        json_encoders={Decimal: str},  # type: ignore[typeddict-unknown-key]
+    )
+    """
+    basic configuration for pydantic's behaviour
+    """
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/geschaeftspartner.py` & `bo4e-0.5.1/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/kosten.py` & `bo4e-0.5.1/src/bo4e/bo/kosten.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """
 Contains Kosten class and corresponding marshmallow schema for de-/serialization
 """
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-many-instance-attributes, too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.betrag import Betrag
 from bo4e.com.kostenblock import Kostenblock
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.kostenklasse import Kostenklasse
 
+# pylint: disable=too-many-instance-attributes, too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Kosten(Geschaeftsobjekt):
     """
     Dieses BO wird zur Übertagung von hierarchischen Kostenstrukturen verwendet.
     Die Kosten werden dabei in Kostenblöcke und diese wiederum in Kostenpositionen strukturiert.
 
     .. raw:: html
@@ -32,12 +33,12 @@
     # required attributes
     bo_typ: BoTyp = BoTyp.KOSTEN
     #: Klasse der Kosten, beispielsweise Fremdkosten
     kostenklasse: Kostenklasse
     #: Für diesen Zeitraum wurden die Kosten ermittelt
     gueltigkeit: Zeitraum
     #: In Kostenblöcken werden Kostenpositionen zusammengefasst. Beispiele: Netzkosten, Umlagen, Steuern etc
-    kostenbloecke: conlist(Kostenblock, min_length=1)  # type: ignore[valid-type]
+    kostenbloecke: Annotated[list[Kostenblock], Len(1)]
 
     # optional attributes
     #: Die Gesamtsumme über alle Kostenblöcke und -positionen
     summe_kosten: Optional[List[Betrag]] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/lastgang.py` & `bo4e-0.5.1/src/bo4e/bo/lastgang.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Contains Lastgang and LastgangKompakt class
 and corresponding marshmallow schema for de-/serialization
 """
-from typing import List, Optional
+from typing import Annotated, List, Optional
+
+from annotated_types import Len
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from pydantic import conlist, constr
+from pydantic import constr
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.tagesvektor import Tagesvektor
 from bo4e.com.zeitintervall import Zeitintervall
 from bo4e.com.zeitreihenwert import Zeitreihenwert
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.mengeneinheit import Mengeneinheit
@@ -85,8 +87,8 @@
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.LASTGANG
 
     #: Die im Lastgang enthaltenen Messwerte
-    werte: conlist(Zeitreihenwert, min_length=1)  # type: ignore[valid-type]
+    werte: Annotated[list[Zeitreihenwert], Len(1)]
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/marktlokation.py` & `bo4e-0.5.1/src/bo4e/bo/marktlokation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 from typing import Optional
 
 # pylint: disable=no-name-in-module
-from pydantic import conlist, field_validator
+from pydantic import field_validator
 from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.adresse import Adresse
 from bo4e.com.geokoordinaten import Geokoordinaten
 from bo4e.com.katasteradresse import Katasteradresse
@@ -111,15 +111,15 @@
     """
     katasterinformation: Optional[Katasteradresse] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
-    kundengruppen: Optional[conlist(Kundentyp, min_length=0)] = None  # type: ignore[valid-type]
+    kundengruppen: Optional[list[Kundentyp]] = None
     #: Kundengruppen der Marktlokation
 
     # pylint:disable=unused-argument, no-self-argument
     @field_validator("katasterinformation")
     def validate_address_info(
         cls, katasterinformation: Optional[Katasteradresse], validation_info: ValidationInfo
     ) -> Optional[Katasteradresse]:
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/marktteilnehmer.py` & `bo4e-0.5.1/src/bo4e/bo/marktteilnehmer.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Contains Marktteilnehmer class
 and corresponding marshmallow schema for de-/serialization
 """
 
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import constr
+from pydantic import Field
 
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.marktrolle import Marktrolle
 from bo4e.enum.rollencodetyp import Rollencodetyp
 from bo4e.enum.sparte import Sparte
 
@@ -31,15 +31,15 @@
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.MARKTTEILNEHMER
     #: Gibt im Klartext die Bezeichnung der Marktrolle an
     marktrolle: Marktrolle
     #: Gibt die Codenummer der Marktrolle an
-    rollencodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
+    rollencodenummer: Annotated[str, Field(strict=True, pattern=r"^\d{13}$")]
     #: Gibt den Typ des Codes an
     rollencodetyp: Rollencodetyp
     #: Sparte des Marktteilnehmers, z.B. Gas oder Strom
     sparte: Sparte
 
     # optional attributes
     #: Die 1:1-Kommunikationsadresse des Marktteilnehmers; Diese wird in der Marktkommunikation verwendet.
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/messlokation.py` & `bo4e-0.5.1/src/bo4e/bo/messlokation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
 Contains Messlokation class
 and corresponding marshmallow schema for de-/serialization
 """
 import re
-from typing import Any, Dict, List, Optional
+from typing import Annotated, List, Optional
 
 from iso3166 import countries
-
-# Structure of a Messlokations-ID
-# Ländercode nach DIN ISO 3166 (2 Stellen)
-# Verteilnetzbetreiber (6 Stellen)
-# Postleitzahl (5 Stellen)
-# Zählpunktnummer (20 Stellen alphanumerisch)
-# source: https://de.wikipedia.org/wiki/Z%C3%A4hlpunkt#Struktur_der_Z%C3%A4hlpunktbezeichnung
-from pydantic import validator
+from pydantic import Field, field_validator, model_validator
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.zaehler import Zaehler
 from bo4e.com.adresse import Adresse
 from bo4e.com.dienstleistung import Dienstleistung
 from bo4e.com.geokoordinaten import Geokoordinaten
 from bo4e.com.hardware import Hardware
 from bo4e.com.katasteradresse import Katasteradresse
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.netzebene import Netzebene
 from bo4e.enum.sparte import Sparte
 
+# Structure of a Messlokations-ID
+# Ländercode nach DIN ISO 3166 (2 Stellen)
+# Verteilnetzbetreiber (6 Stellen)
+# Postleitzahl (5 Stellen)
+# Zählpunktnummer (20 Stellen alphanumerisch)
+# source: https://de.wikipedia.org/wiki/Z%C3%A4hlpunkt#Struktur_der_Z%C3%A4hlpunktbezeichnung
+
 _melo_id_pattern = re.compile(r"^[A-Z]{2}\d{6}\d{5}[A-Z\d]{20}$")
 
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 class Messlokation(Geschaeftsobjekt):
@@ -44,15 +44,15 @@
         `Messlokation JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Messlokation.json>`_
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.MESSLOKATION
     #: Die Messlokations-Identifikation; Das ist die frühere Zählpunktbezeichnung
-    messlokations_id: str
+    messlokations_id: Annotated[str, Field(pattern=_melo_id_pattern.pattern)]
     #: Sparte der Messlokation, z.B. Gas oder Strom
     sparte: Sparte
 
     # optional attributes
     #: Spannungsebene der Messung
     netzebene_messung: Optional[Netzebene] = None
     #: Die Nummer des Messgebietes in der ene't-Datenbank
@@ -90,49 +90,38 @@
     katasterinformation: Optional[Katasteradresse] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
     # pylint: disable=unused-argument, no-self-argument
-    @validator("messlokations_id")
-    def _validate_messlokations_id(cls, messlokations_id: str) -> str:
-        if not messlokations_id:
-            raise ValueError("The messlokations_id must not be empty.")
-        if not _melo_id_pattern.match(messlokations_id):
-            raise ValueError(f"The messlokations_id '{messlokations_id}' does not match {_melo_id_pattern.pattern}")
+    @field_validator("messlokations_id", mode="after")
+    @classmethod
+    def _validate_messlokations_id_country_code(cls, messlokations_id: str) -> str:
+        # The regex pattern in the annotated type above already checks for the correct format
         if not messlokations_id[0:2] in countries:
             raise ValueError(f"The country code '{messlokations_id[0:2]}' is not a valid country code")
         return messlokations_id
 
     # pylint: disable=no-self-argument
-    @validator("katasterinformation")
-    def validate_address_info(
-        cls, katasterinformation: Optional[Katasteradresse], values: Dict[str, Any]
-    ) -> Optional[Katasteradresse]:
+    @model_validator(mode="after")  # type:ignore[arg-type]
+    @classmethod
+    def validate_address_info(cls, model: "Messlokation") -> "Messlokation":
         """Checks that if an address is given, that there is only one valid address given"""
         all_address_attributes = [
-            values["messadresse"],
-            values["geoadresse"],
-            katasterinformation,
+            model.messadresse,
+            model.geoadresse,
+            model.katasterinformation,
         ]
         amount_of_given_address_infos = len([i for i in all_address_attributes if i is not None])
         if amount_of_given_address_infos > 1:
             raise ValueError("More than one address information is given.")
-        return katasterinformation
+        return model
 
     # pylint: disable=no-self-argument
-    @validator("grundzustaendiger_msbim_codenr")
-    def validate_grundzustaendiger_x_codenr(
-        cls, grundzustaendiger_msbim_codenr: Optional[str], values: Dict[str, Any]
-    ) -> Optional[str]:
+    @model_validator(mode="after")  # type:ignore[arg-type]
+    @classmethod
+    def validate_grundzustaendiger_x_codenr(cls, model: "Messlokation") -> "Messlokation":
         """Checks that if a codenr is given, that there is only one valid codenr given."""
-        all_grundzustaendiger_x_codenr_attributes = [
-            values["grundzustaendiger_msb_codenr"],
-            grundzustaendiger_msbim_codenr,
-        ]
-        amount_of_given_grundzustaendiger_x_codenr = len(
-            [i for i in all_grundzustaendiger_x_codenr_attributes if i is not None]
-        )
-        if amount_of_given_grundzustaendiger_x_codenr > 1:
+        if model.grundzustaendiger_msb_codenr is not None and model.grundzustaendiger_msbim_codenr is not None:
             raise ValueError("More than one codenr is given.")
-        return grundzustaendiger_msbim_codenr
+        return model
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/netznutzungsrechnung.py` & `bo4e-0.5.1/src/bo4e/bo/netznutzungsrechnung.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains Netznutzungsrechnung class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import constr
+from pydantic import Field
 
 from bo4e.bo.rechnung import Rechnung
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.nnrechnungsart import NNRechnungsart
 from bo4e.enum.nnrechnungstyp import NNRechnungstyp
 from bo4e.enum.sparte import Sparte
 
@@ -28,20 +28,20 @@
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.NETZNUTZUNGSRECHNUNG
     #: Sparte (Strom, Gas ...) für die die Rechnung ausgestellt ist
     sparte: Sparte
-    absendercodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
+    absendercodenummer: Annotated[str, Field(strict=True, pattern=r"^\d{13}$")]
     """
     Die Rollencodenummer des Absenders (siehe :class:`Marktteilnehmer`).
     Über die Nummer können weitere Informationen zum Marktteilnehmer ermittelt werden.
     """
-    empfaengercodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
+    empfaengercodenummer: Annotated[str, Field(strict=True, pattern=r"^\d{13}$")]
     """
     Die Rollencodenummer des Empfängers (siehe :class:`Marktteilnehmer`).
     Über die Nummer können weitere Informationen zum Marktteilnehmer ermittelt werden.
     """
     #: Aus der INVOIC entnommen
     nnrechnungsart: NNRechnungsart
     #: Aus der INVOIC entnommen
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblatt.py` & `bo4e-0.5.1/src/bo4e/bo/preisblatt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Preisblatt class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.marktteilnehmer import Marktteilnehmer
 from bo4e.com.preisposition import Preisposition
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.preisstatus import Preisstatus
@@ -43,11 +43,11 @@
     #: Preisblatt gilt für angegebene Sparte
     sparte: Sparte
     #: Merkmal, das anzeigt, ob es sich um vorläufige oder endgültige Preise handelt
     preisstatus: Preisstatus
     #: Der Zeitraum für den der Preis festgelegt ist
     gueltigkeit: Zeitraum
     #: Die einzelnen Positionen, die mit dem Preisblatt abgerechnet werden können. Z.B. Arbeitspreis, Grundpreis etc
-    preispositionen: conlist(Preisposition, min_length=1)  # type: ignore[valid-type]
+    preispositionen: Annotated[list[Preisposition], Len(1)]
     # optional attributes
     #: Der Netzbetreiber, der die Preise veröffentlicht hat
     herausgeber: Optional[Marktteilnehmer] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-0.5.1/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblatthardware.py` & `bo4e-0.5.1/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-0.5.1/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblattmessung.py` & `bo4e-0.5.1/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-0.5.1/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/rechnung.py` & `bo4e-0.5.1/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/region.py` & `bo4e-0.5.1/src/bo4e/bo/region.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Contains Region class and corresponding marshmallow schema for de-/serialization
 """
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.regionskriterium import Regionskriterium
 from bo4e.enum.botyp import BoTyp
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Region(Geschaeftsobjekt):
     """
     Modellierung einer Region als Menge von Kriterien, die eine Region beschreiben
 
     .. raw:: html
 
@@ -27,12 +28,12 @@
 
     # required attributes
     bo_typ: BoTyp = BoTyp.REGION
     #: Bezeichnung der Region
     bezeichnung: str
 
     #: Positivliste der Kriterien zur Definition der Region
-    positiv_liste: conlist(Regionskriterium, min_length=1)  # type: ignore[valid-type]
+    positiv_liste: Annotated[list[Regionskriterium], Len(1)]
 
     # optional attributes
     #: Negativliste der Kriterien zur Definition der Region
     negativ_liste: Optional[List[Regionskriterium]] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/regionaltarif.py` & `bo4e-0.5.1/src/bo4e/bo/regionaltarif.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Contains Regionaltarif class and corresponding marshmallow schema for de-/serialization
 """
 
 from datetime import datetime
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods, empty-docstring
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.tarifinfo import Tarifinfo
 from bo4e.com.regionalepreisgarantie import RegionalePreisgarantie
 from bo4e.com.regionaleraufabschlag import RegionalerAufAbschlag
 from bo4e.com.regionaletarifpreisposition import RegionaleTarifpreisposition
 from bo4e.com.tarifberechnungsparameter import Tarifberechnungsparameter
 from bo4e.com.tarifeinschraenkung import Tarifeinschraenkung
 from bo4e.enum.botyp import BoTyp
 
+# pylint: disable=too-few-public-methods, empty-docstring
+# pylint: disable=no-name-in-module
+
 
 class Regionaltarif(Tarifinfo):
     #: Abbildung eines Tarifs mit regionaler Zuordnung von Preisen und Auf- und Abschlägen.
     """
 
     .. raw:: html
 
@@ -34,15 +35,15 @@
     bo_typ: BoTyp = BoTyp.REGIONALTARIF
     # required attributes
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
     #: Die festgelegten Preise mit regionaler Eingrenzung, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(RegionaleTarifpreisposition, min_length=1)  # type: ignore[valid-type]
+    tarifpreise: Annotated[list[RegionaleTarifpreisposition], Len(1)]
 
     # optional attributes
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
     tarif_auf_abschlaege: Optional[List[RegionalerAufAbschlag]] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
     preisgarantien: Optional[List[RegionalePreisgarantie]] = None
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/standorteigenschaften.py` & `bo4e-0.5.1/src/bo4e/bo/standorteigenschaften.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Standorteigenschaften class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.standorteigenschaftengas import StandorteigenschaftenGas
 from bo4e.com.standorteigenschaftenstrom import StandorteigenschaftenStrom
 from bo4e.enum.botyp import BoTyp
 
 
@@ -27,12 +27,12 @@
         `Standorteigenschaften JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Standorteigenschaften.json>`_
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.STANDORTEIGENSCHAFTEN
     #: Eigenschaften zur Sparte Strom
-    eigenschaften_strom: conlist(StandorteigenschaftenStrom, min_length=1)  # type: ignore[valid-type]
+    eigenschaften_strom: Annotated[list[StandorteigenschaftenStrom], Len(1)]
 
     # optional attributes
     #: Eigenschaften zur Sparte Gas
     eigenschaften_gas: Optional[StandorteigenschaftenGas] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/tarif.py` & `bo4e-0.5.1/src/bo4e/bo/tarif.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Contains Tarif class and corresponding marshmallow schema for de-/serialization
 """
 
 from datetime import datetime
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.tarifinfo import Tarifinfo
 from bo4e.com.aufabschlagregional import AufAbschlagRegional
 from bo4e.com.preisgarantie import Preisgarantie
 from bo4e.com.tarifberechnungsparameter import Tarifberechnungsparameter
 from bo4e.com.tarifeinschraenkung import Tarifeinschraenkung
 from bo4e.com.tarifpreispositionproort import TarifpreispositionProOrt
 from bo4e.enum.botyp import BoTyp
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Tarif(Tarifinfo):
     """
     Abbildung eines Tarifs mit regionaler Zuordnung von Preisen und Auf- und Abschlägen
 
     .. raw:: html
 
@@ -34,15 +35,15 @@
     bo_typ: BoTyp = BoTyp.TARIF
     # required attributes
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
     #: Die festgelegten Preise mit regionaler Eingrenzung z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(TarifpreispositionProOrt, min_length=1)  # type: ignore[valid-type]
+    tarifpreise: Annotated[list[TarifpreispositionProOrt], Len(1)]
 
     # optional attributes
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
     tarif_auf_abschlaege: Optional[List[AufAbschlagRegional]] = None
     # todo: fix inconsistency: RegionalerAufAbschlag vs. AufAbschlagRegional
     # https://github.com/Hochfrequenz/BO4E-python/issues/345
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/tarifinfo.py` & `bo4e-0.5.1/src/bo4e/bo/tarifinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Contains Tarifinfo class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 # pylint: disable=no-name-in-module
 from datetime import datetime
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.marktteilnehmer import Marktteilnehmer
 from bo4e.com.energiemix import Energiemix
 from bo4e.com.vertragskonditionen import Vertragskonditionen
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.botyp import BoTyp
@@ -42,21 +42,21 @@
     #: Name des Tarifs
     bezeichnung: str
     #: Der Name des Marktpartners, der den Tarif anbietet
     anbietername: str
     #: Strom oder Gas, etc.
     sparte: Sparte
     #: Kundentypen für den der Tarif gilt, z.B. Privatkunden
-    kundentypen: conlist(Kundentyp, min_length=1)  # type: ignore[valid-type]
+    kundentypen: Annotated[list[Kundentyp], Len(1)]
     #: Die Art des Tarifes, z.B. Eintarif oder Mehrtarif
     tarifart: Tarifart
     #: Hinweis auf den Tariftyp, z.B. Grundversorgung oder Sondertarif
     tariftyp: Tariftyp
     #: Weitere Merkmale des Tarifs, z.B. Festpreis oder Vorkasse
-    tarifmerkmale: conlist(Tarifmerkmal, min_length=1)  # type: ignore[valid-type]
+    tarifmerkmale: Annotated[list[Tarifmerkmal], Len(1)]
     #: Der Marktteilnehmer (Lieferant), der diesen Tarif anbietet
     anbieter: Marktteilnehmer
 
     # optional attributes
     #: Internetseite auf dem der Tarif zu finden ist
     website: Optional[str] = None
     #: Freitext
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/tarifkosten.py` & `bo4e-0.5.1/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-0.5.1/src/bo4e/bo/tarifpreisblatt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Contains Tarifpreisblatt class and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.tarifinfo import Tarifinfo
 from bo4e.com.aufabschlag import AufAbschlag
 from bo4e.com.preisgarantie import Preisgarantie
 from bo4e.com.tarifberechnungsparameter import Tarifberechnungsparameter
 from bo4e.com.tarifeinschraenkung import Tarifeinschraenkung
 from bo4e.com.tarifpreisposition import Tarifpreisposition
 from bo4e.enum.botyp import BoTyp
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Tarifpreisblatt(Tarifinfo):
     """
     Tarifinformation mit Preisen, Aufschlägen und Berechnungssystematik
 
     .. raw:: html
 
@@ -31,15 +32,15 @@
     """
 
     bo_typ: BoTyp = BoTyp.TARIFPREISBLATT
     # required attributes (additional to those of Tarifinfo)
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Die festgelegten Preise, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(Tarifpreisposition, min_length=1)  # type: ignore[valid-type]
+    tarifpreise: Annotated[list[Tarifpreisposition], Len(1)]
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
 
     # optional attributes
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
     tarifeinschraenkung: Optional[Tarifeinschraenkung] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/vertrag.py` & `bo4e-0.5.1/src/bo4e/bo/vertrag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Contains Vertrag class
 and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=unused-argument
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.unterschrift import Unterschrift
 from bo4e.com.vertragskonditionen import Vertragskonditionen
 from bo4e.com.vertragsteil import Vertragsteil
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.sparte import Sparte
 from bo4e.enum.vertragsart import Vertragsart
 from bo4e.enum.vertragsstatus import Vertragsstatus
 
+# pylint: disable=unused-argument
+# pylint: disable=no-name-in-module
+
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 class Vertrag(Geschaeftsobjekt):
     """
     Modell für die Abbildung von Vertragsbeziehungen;
     Das Objekt dient dazu, alle Arten von Verträgen, die in der Energiewirtschaft Verwendung finden, abzubilden.
@@ -60,15 +61,15 @@
     """
     vertragspartner2: Geschaeftspartner
     """
     Der "zweitgenannte" Vertragspartner.
     In der Regel der Empfänger des Vertrags.
     Beispiel "Vertrag zwischen Vertragspartner 1 und Vertragspartner 2".
     """
-    vertragsteile: conlist(Vertragsteil, min_length=1)  # type: ignore[valid-type]
+    vertragsteile: Annotated[list[Vertragsteil], Len(1)]
     """
     Der Vertragsteil wird dazu verwendet, eine vertragliche Leistung in Bezug zu einer Lokation
     (Markt- oder Messlokation) festzulegen.
     """
 
     # optional attributes
     #: Beschreibung zum Vertrag
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/zaehler.py` & `bo4e-0.5.1/src/bo4e/bo/zaehler.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 from decimal import Decimal
 
 # pylint: disable=unused-argument
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.zaehlwerk import Zaehlwerk
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.sparte import Sparte
 from bo4e.enum.tarifart import Tarifart
@@ -38,15 +38,15 @@
 
     # required attributes
     bo_typ: BoTyp = BoTyp.ZAEHLER
     zaehlernummer: str  #: Nummerierung des Zählers,vergeben durch den Messstellenbetreiber
     sparte: Sparte  #: Strom oder Gas
     zaehlerauspraegung: Zaehlerauspraegung  #: Spezifikation die Richtung des Zählers betreffend
     zaehlertyp: Zaehlertyp  #: Typisierung des Zählers
-    zaehlwerke: conlist(Zaehlwerk, min_length=1)  # type: ignore[valid-type]  #: Die Zählwerke des Zählers
+    zaehlwerke: Annotated[list[Zaehlwerk], Len(1)]
     tarifart: Tarifart  #: Spezifikation bezüglich unterstützter Tarifarten
 
     # optional attributes
     zaehlerkonstante: Optional[Decimal] = None  #: Zählerkonstante auf dem Zähler
     eichung_bis: Optional[datetime] = None  #: Bis zu diesem Datum (exklusiv) ist der Zähler geeicht.
     letzte_eichung: Optional[datetime] = None  #: Zu diesem Datum fand die letzte Eichprüfung des Zählers statt.
     zaehlerhersteller: Optional[Geschaeftspartner] = None  #: Der Hersteller des Zählers
```

### Comparing `bo4e-0.5.0/src/bo4e/bo/zeitreihe.py` & `bo4e-0.5.1/src/bo4e/bo/zeitreihe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains Zeitreihe class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.com.zeitreihenwert import Zeitreihenwert
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.medium import Medium
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.messart import Messart
@@ -41,15 +41,15 @@
     #: Beschreibt die Art der Messung (z.B. aktueller Wert, mittlerer Wert, maximaler Wert)
     messart: Messart
     #: Medium, das gemessen wurde (z.B. Wasser, Dampf, Strom, Gas)
     medium: Medium
     #: Alle Werte in der Tabelle haben die Einheit, die hier angegeben ist
     einheit: Mengeneinheit
     #: Hier liegen jeweils die Werte
-    werte: conlist(Zeitreihenwert, min_length=1)  # type: ignore[valid-type]
+    werte: Annotated[list[Zeitreihenwert], Len(1)]
 
     # optional attributes
     #: Beschreibt die Verwendung der Zeitreihe
     beschreibung: Optional[str] = None
     #: Version der Zeitreihe
     version: Optional[str] = None
     #: Kennzeichnung, wie die Werte entstanden sind, z.B. durch Messung
```

### Comparing `bo4e-0.5.0/src/bo4e/com/adresse.py` & `bo4e-0.5.1/src/bo4e/com/adresse.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains Adresse class
 and corresponding marshmallow schema for de-/serialization
 """
-from typing import Any, Dict, Optional
+from typing import Optional
 
-from pydantic import validator
+from pydantic import model_validator
 
 from bo4e.com.com import COM
 from bo4e.enum.landescode import Landescode
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
@@ -44,29 +44,24 @@
     adresszusatz: Optional[str] = None
     #: Im Falle einer c/o-Adresse steht in diesem Attribut die Anrede. Z.B. "c/o Veronica Hauptmieterin"
     co_ergaenzung: Optional[str] = None
     #: Offizieller ISO-Landescode
     landescode: Landescode = Landescode.DE  # type:ignore
 
     # pylint: disable=no-self-argument
-    @validator("postfach")
-    def strasse_xor_postfach(cls, postfach: Optional[str], values: Dict[str, Any]) -> Optional[str]:
+    @model_validator(mode="after")  # type:ignore[arg-type]
+    @classmethod
+    def strasse_xor_postfach(cls, model: "Adresse") -> "Adresse":
         """
         An address is valid if it contains a postfach XOR (a strasse AND hausnummer).
         This functions checks for these conditions of a valid address.
 
         Nur folgende Angabekombinationen sind (nach der Abfrage) möglich:
         Straße           w   f   f
         Hausnummer       w   f   f
         Postfach         f   w   f
         Postleitzahl     w   w   w
         Ort              w   w   w
         """
-        if (
-            values["strasse"]
-            and values["hausnummer"]
-            and not postfach
-            or not values["strasse"]
-            and not values["hausnummer"]
-        ):
-            return postfach
+        if model.strasse and model.hausnummer and not model.postfach or not model.strasse and not model.hausnummer:
+            return model
         raise ValueError('You have to define either "strasse" and "hausnummer" or "postfach".')
```

### Comparing `bo4e-0.5.0/src/bo4e/com/angebotsposition.py` & `bo4e-0.5.1/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/angebotsteil.py` & `bo4e-0.5.1/src/bo4e/com/angebotsteil.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Contains Angebotsteil class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.bo.marktlokation import Marktlokation
 from bo4e.com.angebotsposition import Angebotsposition
 from bo4e.com.betrag import Betrag
 from bo4e.com.com import COM
 from bo4e.com.menge import Menge
 from bo4e.com.zeitraum import Zeitraum
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Angebotsteil(COM):
     """
     Mit dieser Komponente wird ein Teil einer Angebotsvariante abgebildet.
     Hier werden alle Angebotspositionen aggregiert.
     Angebotsteile werden im einfachsten Fall für eine Marktlokation oder Lieferstellenadresse erzeugt.
     Hier werden die Mengen und Gesamtkosten aller Angebotspositionen zusammengefasst.
@@ -32,15 +33,15 @@
     .. HINT::
         `Angebotsteil JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Angebotsteil.json>`_
 
     """
 
     # required attributes
     #: Einzelne Positionen, die zu diesem Angebotsteil gehören
-    positionen: conlist(Angebotsposition, min_length=1)  # type: ignore[valid-type]
+    positionen: Annotated[list[Angebotsposition], Len(1)]
 
     # optional attributes
     #: Identifizierung eines Subkapitels einer Anfrage, beispielsweise das Los einer Ausschreibung
     anfrage_subreferenz: Optional[str] = None
     lieferstellenangebotsteil: Optional[List[Marktlokation]] = None
     """
     Marktlokationen, für die dieses Angebotsteil gilt, falls vorhanden.
```

### Comparing `bo4e-0.5.0/src/bo4e/com/angebotsvariante.py` & `bo4e-0.5.1/src/bo4e/com/angebotsvariante.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Angebotsvariante and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.angebotsteil import Angebotsteil
 from bo4e.com.betrag import Betrag
 from bo4e.com.com import COM
 from bo4e.com.menge import Menge
 from bo4e.enum.angebotsstatus import Angebotsstatus
 
@@ -35,15 +35,15 @@
 
     #: Datum der Erstellung der Angebotsvariante
     erstellungsdatum: datetime
 
     #: Bis zu diesem Zeitpunkt gilt die Angebotsvariante
     bindefrist: datetime
 
-    teile: conlist(Angebotsteil, min_length=1)  # type: ignore[valid-type]
+    teile: Annotated[list[Angebotsteil], Len(1)]
     """
     Angebotsteile werden im einfachsten Fall für eine Marktlokation oder Lieferstellenadresse erzeugt.
     Hier werden die Mengen und Gesamtkosten aller Angebotspositionen zusammengefasst.
     Eine Variante besteht mindestens aus einem Angebotsteil.
     """
 
     # optional attributes
```

### Comparing `bo4e-0.5.0/src/bo4e/com/aufabschlag.py` & `bo4e-0.5.1/src/bo4e/com/aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/aufabschlagproort.py` & `bo4e-0.5.1/src/bo4e/com/aufabschlagproort.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Contains AufAbschlagProOrt class
 and corresponding marshmallow schema for de-/serialization
 """
+from typing import Annotated
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.aufabschlagstaffelproort import AufAbschlagstaffelProOrt
 from bo4e.com.com import COM
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class AufAbschlagProOrt(COM):
     """
     Mit dieser Komponente können Auf- und Abschläge verschiedener Typen im Zusammenhang
     mit örtlichen Gültigkeiten abgebildet werden.
 
     .. raw:: html
@@ -29,8 +31,8 @@
     #: Die Postleitzahl des Ortes für den der Aufschlag gilt.
     postleitzahl: str
     #: Der Ort für den der Aufschlag gilt.
     ort: str
     #: Die ene't-Netznummer des Netzes in dem der Aufschlag gilt.
     netznr: str
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung.
-    staffeln: conlist(AufAbschlagstaffelProOrt, min_length=1)  # type: ignore[valid-type]
+    staffeln: Annotated[list[AufAbschlagstaffelProOrt], Len(1)]
```

### Comparing `bo4e-0.5.0/src/bo4e/com/aufabschlagregional.py` & `bo4e-0.5.1/src/bo4e/com/aufabschlagregional.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Contains AufAbschlagRegional and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods, too-many-instance-attributes
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.aufabschlagproort import AufAbschlagProOrt
 from bo4e.com.com import COM
 from bo4e.com.energiemix import Energiemix
 from bo4e.com.preisgarantie import Preisgarantie
 from bo4e.com.tarifeinschraenkung import Tarifeinschraenkung
 from bo4e.com.vertragskonditionen import Vertragskonditionen
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.aufabschlagstyp import AufAbschlagstyp
 from bo4e.enum.aufabschlagsziel import AufAbschlagsziel
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
 
+# pylint: disable=too-few-public-methods, too-many-instance-attributes
+# pylint: disable=no-name-in-module
+
 
 # pylint: disable=R0801
 class AufAbschlagRegional(COM):
     """
     Mit dieser Komponente können Auf- und Abschläge verschiedener Typen
     im Zusammenhang mit regionalen Gültigkeiten abgebildet werden.
     Hier sind auch die Auswirkungen auf verschiedene Tarifparameter modelliert,
@@ -37,15 +38,15 @@
 
     """
 
     # required attributess
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: str
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    betraege: conlist(AufAbschlagProOrt, min_length=1)  # type: ignore[valid-type]
+    betraege: Annotated[list[AufAbschlagProOrt], Len(1)]
 
     # optional attributes
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #:Typ des Aufabschlages (z.B. absolut oder prozentual)
     auf_abschlagstyp: Optional[AufAbschlagstyp] = None
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc.
```

### Comparing `bo4e-0.5.0/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-0.5.1/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-0.5.1/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/ausschreibungslos.py` & `bo4e-0.5.1/src/bo4e/com/ausschreibungslos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains Ausschreibungslos class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.ausschreibungsdetail import Ausschreibungsdetail
 from bo4e.com.com import COM
 from bo4e.com.menge import Menge
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.preismodell import Preismodell
 from bo4e.enum.rechnungslegung import Rechnungslegung
@@ -47,15 +47,15 @@
     wunsch_vertragsform: Vertragsform
     #: Name des Lizenzpartners
     betreut_durch: str
     #: Anzahl der Lieferstellen in dieser Ausschreibung
     anzahl_lieferstellen: int
 
     #: Die ausgeschriebenen Lieferstellen
-    lieferstellen: conlist(Ausschreibungsdetail, min_length=1)  # type: ignore[valid-type]
+    lieferstellen: Annotated[list[Ausschreibungsdetail], Len(1)]
 
     #: Zeitraum, für den die in diesem Los enthaltenen Lieferstellen beliefert werden sollen
     lieferzeitraum: Zeitraum
 
     # optional attributes
     #: Bemerkung des Kunden zum Los
     bemerkung: Optional[str] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/com/betrag.py` & `bo4e-0.5.1/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/com.py` & `bo4e-0.5.1/src/bo4e/com/com.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from decimal import Decimal
 from typing import Type, TypeVar
 
 from humps.main import camelize
 
 # pylint: disable=no-name-in-module
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 
 # pylint: disable=too-few-public-methods
 #
 class COM(BaseModel):
     """
     base class for all components
@@ -22,24 +22,27 @@
         <object data="../_static/images/bo4e/com/COM.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `COM JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/COM.json>`_
 
     """
 
-    # pylint:disable=duplicate-code
-    class Config:
-        """
-        basic configuration for pydantic's behaviour
-        """
-
-        alias_generator = camelize
-        populate_by_name = True
-        extra = "allow"
-        json_encoders = {Decimal: str}
+    # pylint: disable=duplicate-code
+    model_config = ConfigDict(
+        alias_generator=camelize,
+        populate_by_name=True,
+        extra="allow",
+        # json_encoders is deprecated, but there is no easy-to-use alternative. The best way would be to create
+        # an annotated version of Decimal, but you would have to use it everywhere in the pydantic models.
+        # See this issue for more info: https://github.com/pydantic/pydantic/issues/6375
+        json_encoders={Decimal: str},  # type: ignore[typeddict-unknown-key]
+    )
+    """
+    basic configuration for pydantic's behaviour
+    """
 
 
 # pylint: disable=invalid-name
 #: Any type derived from COM including those that do not directly inherit from COM
 TCom = TypeVar("TCom", bound=Type[COM])
```

### Comparing `bo4e-0.5.0/src/bo4e/com/dienstleistung.py` & `bo4e-0.5.1/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/energieherkunft.py` & `bo4e-0.5.1/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/energiemix.py` & `bo4e-0.5.1/src/bo4e/com/energiemix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 Contains Energiemix class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods, too-many-instance-attributes
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.energieherkunft import Energieherkunft
 from bo4e.enum.oekolabel import Oekolabel
 from bo4e.enum.oekozertifikat import Oekozertifikat
 from bo4e.enum.sparte import Sparte
 
+# pylint: disable=too-few-public-methods, too-many-instance-attributes
+# pylint: disable=no-name-in-module
+
 
 class Energiemix(COM):
     """
     Zusammensetzung der gelieferten Energie aus den verschiedenen Primärenergieformen.
 
     .. raw:: html
 
@@ -36,15 +37,15 @@
     #: Strom oder Gas etc.
     energieart: Sparte
     #: Bezeichnung des Energiemix
     bezeichnung: str
     #: Jahr, für das der Energiemix gilt
     gueltigkeitsjahr: int
     #: Anteile der jeweiligen Erzeugungsart
-    anteil: conlist(Energieherkunft, min_length=1)  # type: ignore[valid-type]
+    anteil: Annotated[list[Energieherkunft], Len(1)]
 
     # optional attributes
     #: Bemerkung zum Energiemix
     bemerkung: Optional[str] = None
     #: Höhe des erzeugten CO2-Ausstosses in g/kWh
     co2_emission: Optional[Decimal] = None
     #: Höhe des erzeugten Atommülls in g/kWh
```

### Comparing `bo4e-0.5.0/src/bo4e/com/externereferenz.py` & `bo4e-0.5.1/src/bo4e/com/externereferenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/fremdkostenblock.py` & `bo4e-0.5.1/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/fremdkostenposition.py` & `bo4e-0.5.1/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/geokoordinaten.py` & `bo4e-0.5.1/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/geraet.py` & `bo4e-0.5.1/src/bo4e/com/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/geraeteeigenschaften.py` & `bo4e-0.5.1/src/bo4e/com/geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/hardware.py` & `bo4e-0.5.1/src/bo4e/com/hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/katasteradresse.py` & `bo4e-0.5.1/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/kostenblock.py` & `bo4e-0.5.1/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/kostenposition.py` & `bo4e-0.5.1/src/bo4e/com/kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/kriteriumwert.py` & `bo4e-0.5.1/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/marktgebietinfo.py` & `bo4e-0.5.1/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/menge.py` & `bo4e-0.5.1/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/messlokationszuordnung.py` & `bo4e-0.5.1/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/positionsaufabschlag.py` & `bo4e-0.5.1/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/preis.py` & `bo4e-0.5.1/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/preisgarantie.py` & `bo4e-0.5.1/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/preisposition.py` & `bo4e-0.5.1/src/bo4e/com/preisposition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains Preisposition class and corresponding marshmallow schema for de-/serialization
 """
 from decimal import Decimal
 
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.preisstaffel import Preisstaffel
 from bo4e.enum.bdewartikelnummer import BDEWArtikelnummer
 from bo4e.enum.bemessungsgroesse import Bemessungsgroesse
 from bo4e.enum.kalkulationsmethode import Kalkulationsmethode
 from bo4e.enum.leistungstyp import Leistungstyp
@@ -43,15 +43,15 @@
     #: Bezeichnung für die in der Position abgebildete Leistungserbringung
     leistungsbezeichnung: str
     #: Festlegung, mit welcher Preiseinheit abgerechnet wird, z.B. Ct. oder €
     preiseinheit: Waehrungseinheit
     #: Hier wird festgelegt, auf welche Bezugsgrösse sich der Preis bezieht, z.B. kWh oder Stück
     bezugsgroesse: Mengeneinheit
     #: Preisstaffeln, die zu dieser Preisposition gehören
-    preisstaffeln: conlist(Preisstaffel, min_length=1)  # type: ignore[valid-type]
+    preisstaffeln: Annotated[list[Preisstaffel], Len(1)]
 
     # optional attributes
     zeitbasis: Optional[Zeiteinheit] = None
     """
     Die Zeit(dauer) auf die sich der Preis bezieht.
     Z.B. ein Jahr für einen Leistungspreis der in €/kW/Jahr ausgegeben wird
     """
```

### Comparing `bo4e-0.5.0/src/bo4e/com/preisstaffel.py` & `bo4e-0.5.1/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/rechnungsposition.py` & `bo4e-0.5.1/src/bo4e/com/rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-0.5.1/src/bo4e/com/regionalegueltigkeit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 Contains RegionaleGueltigkeit class
 and corresponding marshmallow schema for de-/serialization
 """
+from typing import Annotated
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.kriteriumwert import KriteriumWert
 from bo4e.enum.gueltigkeitstyp import Gueltigkeitstyp
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class RegionaleGueltigkeit(COM):
     """
     Mit dieser Komponente können regionale Gültigkeiten, z.B. für Tarife, Zu- und Abschläge und Preise definiert werden.
 
     .. raw:: html
 
@@ -23,10 +25,10 @@
     .. HINT::
         `RegionaleGueltigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionaleGueltigkeit.json>`_
 
     """
 
     # required attributes
     gueltigkeitstyp: Gueltigkeitstyp  #: Unterscheidung ob Positivliste oder Negativliste übertragen wird
-    kriteriums_werte: conlist(  # type: ignore[valid-type]
-        KriteriumWert, min_length=1
-    )  #: Hier stehen die Kriterien, die die regionale Gültigkeit festlegen
+    kriteriums_werte: Annotated[
+        list[KriteriumWert], Len(1)
+    ]  #: Hier stehen die Kriterien, die die regionale Gültigkeit festlegen
```

### Comparing `bo4e-0.5.0/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-0.5.1/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-0.5.1/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-0.5.1/src/bo4e/com/regionaleraufabschlag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 Contains RegionalerAufAbschlag class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import List, Optional
+from typing import Annotated, List, Optional
 
-# pylint: disable=too-few-public-methods, too-many-instance-attributes
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.energiemix import Energiemix
 from bo4e.com.preisgarantie import Preisgarantie
 from bo4e.com.regionalepreisstaffel import RegionalePreisstaffel
 from bo4e.com.tarifeinschraenkung import Tarifeinschraenkung
 from bo4e.com.vertragskonditionen import Vertragskonditionen
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.aufabschlagstyp import AufAbschlagstyp
 from bo4e.enum.aufabschlagsziel import AufAbschlagsziel
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
 
+# pylint: disable=too-few-public-methods, too-many-instance-attributes
+# pylint: disable=no-name-in-module
+
 
 # pylint: disable=R0801
 class RegionalerAufAbschlag(COM):
     """
     Mit dieser Komponente können Auf- und Abschläge verschiedener Typen im Zusammenhang mit regionalen Gültigkeiten
     abgebildet werden.
     Hier sind auch die Auswirkungen auf verschiedene Tarifparameter modelliert, die sich durch die Auswahl eines Auf-
@@ -38,15 +39,15 @@
     """
 
     # required attributes
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: str
 
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    staffeln: conlist(RegionalePreisstaffel, min_length=1)  # type: ignore[valid-type]
+    staffeln: Annotated[list[RegionalePreisstaffel], Len(1)]
 
     # optional attributes
     #: Beschreibung des Auf-/Abschlags
     beschreibung: Optional[str] = None
 
     #: Typ des Aufabschlages (z.B. absolut oder prozentual)
     auf_abschlagstyp: Optional[AufAbschlagstyp] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-0.5.1/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains RegionaleTarifpreisposition class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.regionalepreisstaffel import RegionalePreisstaffel
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.preistyp import Preistyp
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
 
@@ -33,12 +33,12 @@
     #: Angabe des Preistypes (z.B. Grundpreis)
     preistyp: Preistyp
     #: Einheit des Preises (z.B. EURO)
     einheit: Waehrungseinheit
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
     bezugseinheit: Mengeneinheit
     #: Hier sind die Staffeln mit ihren Preisangaben und regionalen Gültigkeiten definiert
-    preisstaffeln: conlist(RegionalePreisstaffel, min_length=1)  # type: ignore[valid-type]
+    preisstaffeln: Annotated[list[RegionalePreisstaffel], Len(1)]
 
     # optional attributes
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
     mengeneinheitstaffel: Optional[Mengeneinheit] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/com/regionskriterium.py` & `bo4e-0.5.1/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/rufnummer.py` & `bo4e-0.5.1/src/bo4e/com/rufnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/sigmoidparameter.py` & `bo4e-0.5.1/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-0.5.1/src/bo4e/com/standorteigenschaftengas.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Contains StandorteigenschaftenGas class
 and corresponding marshmallow schema for de-/serialization
 """
-from typing import List
+from typing import Annotated, List
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.marktgebietinfo import MarktgebietInfo
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class StandorteigenschaftenGas(COM):
     """
     Standorteigenschaften der Sparte Gas
 
     .. raw:: html
 
@@ -22,9 +23,9 @@
 
     .. HINT::
         `StandorteigenschaftenGas JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/StandorteigenschaftenGas.json>`_
 
     """
 
     # required attributes
-    netzkontonummern: conlist(str, min_length=1, max_length=2)  # type: ignore[valid-type]  #: Netzkontonummern der Gasnetze
+    netzkontonummern: Annotated[list[str], Len(1, 2)]  #: Netzkontonummern der Gasnetze
     marktgebiete: List[MarktgebietInfo]  #: Die Informationen zu Marktgebieten in dem Netz.
```

### Comparing `bo4e-0.5.0/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-0.5.1/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/steuerbetrag.py` & `bo4e-0.5.1/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/tagesvektor.py` & `bo4e-0.5.1/src/bo4e/com/tagesvektor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Contains Tagesvektor class and corresponding marshmallow schema for de-/serialization
 """
 import datetime
+from typing import Annotated
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.zeitreihenwertkompakt import Zeitreihenwertkompakt
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class Tagesvektor(COM):
     """
     Abbildung eines Tagesvektors eines beliebigen äquidistanten Zeitrasters
 
     .. raw:: html
 
@@ -29,12 +31,12 @@
     tag: datetime.datetime
     """
     Der Zeitpunkt ab dem die Werte ermittelt wurden.
     Es kann entweder der Beginn des Strom- oder Gastages verwendet werden.
     Der Zeitpunkt sollte eindeutig sein, d.h. sowohl Datum+Uhrzeit als auch den UTC-Offset spezifizieren.
     """
     # for the validator see also https://github.com/Hochfrequenz/BO4E-python/issues/262
-    werte: conlist(Zeitreihenwertkompakt, min_length=1)  # type: ignore[valid-type]
+    werte: Annotated[list[Zeitreihenwertkompakt], Len(1)]
     """
     Die Werte am angegebenen Tag;
     In Kombination aus Zeitintervall und Tag lassen sich die Zeiten der Werte eindeutig konstruieren.
     """
```

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-0.5.1/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-0.5.1/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifpreis.py` & `bo4e-0.5.1/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifpreisposition.py` & `bo4e-0.5.1/src/bo4e/com/tarifpreisposition.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Tarifpreisposition class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import Annotated, Optional
 
-from pydantic import conlist
+from annotated_types import Len
 
 from bo4e.com.com import COM
 from bo4e.com.preisstaffel import Preisstaffel
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.preistyp import Preistyp
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
 
@@ -33,12 +33,12 @@
     #: Angabe des Preistypes (z.B. Grundpreis)
     preistyp: Preistyp
     #: Einheit des Preises (z.B. EURO)
     einheit: Waehrungseinheit
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
     bezugseinheit: Mengeneinheit
     #: Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: conlist(Preisstaffel, min_length=1)  # type: ignore[valid-type]
+    preisstaffeln: Annotated[list[Preisstaffel], Len(1)]
 
     # optional attributes
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
     mengeneinheitstaffel: Optional[Mengeneinheit] = None
```

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-0.5.1/src/bo4e/com/tarifpreispositionproort.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains TarifpreispositionProOrt class
 and corresponding marshmallow schema for de-/serialization
 """
+from typing import Annotated
 
-# pylint: disable=too-few-public-methods
-# pylint: disable=no-name-in-module
-from pydantic import conlist, constr
+from annotated_types import Len
+from pydantic import Field
 
 from bo4e.com.com import COM
 from bo4e.com.tarifpreisstaffelproort import TarifpreisstaffelProOrt
 
+# pylint: disable=too-few-public-methods
+# pylint: disable=no-name-in-module
+
 
 class TarifpreispositionProOrt(COM):
     """
     Mit dieser Komponente können Tarifpreise verschiedener Typen abgebildet werden
 
     .. raw:: html
 
@@ -22,15 +25,15 @@
     .. HINT::
         `TarifpreispositionProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/TarifpreispositionProOrt.json>`_
 
     """
 
     # required attributes
     #: Postleitzahl des Ortes für den der Preis gilt
-    postleitzahl: constr(strict=True, pattern=r"^\d{5}$")  # type: ignore[valid-type]
+    postleitzahl: Annotated[str, Field(strict=True, pattern=r"^\d{5}$")]
     #: Ort für den der Preis gilt
     ort: str
     #: ene't-Netznummer des Netzes in dem der Preis gilt
     netznr: str
     # Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: conlist(TarifpreisstaffelProOrt, min_length=1)  # type: ignore[valid-type]
+    preisstaffeln: Annotated[list[TarifpreisstaffelProOrt], Len(1)]
     # there are no optional attributes
```

### Comparing `bo4e-0.5.0/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-0.5.1/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/unterschrift.py` & `bo4e-0.5.1/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/verbrauch.py` & `bo4e-0.5.1/src/bo4e/com/verbrauch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Contains Verbrauch and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 from decimal import Decimal
-from typing import Optional
+from typing import Annotated, Optional
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from pydantic import constr, field_validator
+from pydantic import Field, field_validator
 from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.com.com import COM
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.wertermittlungsverfahren import Wertermittlungsverfahren
 from bo4e.validators import OBIS_PATTERN, check_bis_is_later_than_von
 
@@ -29,15 +29,15 @@
 
     """
 
     # required attributes
     #: Gibt an, ob es sich um eine PROGNOSE oder eine MESSUNG handelt
     wertermittlungsverfahren: Wertermittlungsverfahren
     #: Die OBIS-Kennzahl für den Wert, die festlegt, welche Größe mit dem Stand gemeldet wird, z.B. '1-0:
-    obis_kennzahl: constr(strict=True, pattern=OBIS_PATTERN)  # type: ignore[valid-type]  # type: ignore[valid-type]
+    obis_kennzahl: Annotated[str, Field(strict=True, pattern=OBIS_PATTERN)]
     #: Gibt den absoluten Wert der Menge an
     wert: Decimal
     #: Gibt die Einheit zum jeweiligen Wert an
     einheit: Mengeneinheit
 
     # optional attributes
     #: Inklusiver Beginn des Zeitraumes, für den der Verbrauch angegeben wird
```

### Comparing `bo4e-0.5.0/src/bo4e/com/vertragskonditionen.py` & `bo4e-0.5.1/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/vertragsteil.py` & `bo4e-0.5.1/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/zaehlwerk.py` & `bo4e-0.5.1/src/bo4e/com/zaehlwerk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Contains Zaehlwerk class
 and corresponding marshmallow schema for de-/serialization
 """
 from decimal import Decimal
+from typing import Annotated
 
 # pylint: disable=no-name-in-module
 # pylint: disable=no-name-in-module
-from pydantic import constr
+from pydantic import Field
 
 from bo4e.com.com import COM
 from bo4e.enum.energierichtung import Energierichtung
 from bo4e.enum.mengeneinheit import Mengeneinheit
 
 # pylint: disable=too-few-public-methods
 
@@ -28,16 +29,19 @@
 
     """
 
     zaehlwerk_id: str  # Identifikation des Zählwerks (Registers) innerhalb des Zählers.
     # Oftmals eine laufende Nummer hinter der Zählernummer. Z.B. 47110815_1
     bezeichnung: str  # Zusätzliche Bezeichnung, z.B. Zählwerk_Wirkarbeit.
     richtung: Energierichtung  # Die Energierichtung, Einspeisung oder Ausspeisung.
-    obis_kennzahl: constr(  # type: ignore[valid-type]
-        strict=True,
-        pattern=r"(?:(1)-((?:[0-5]?[0-9])|(?:6[0-5])):((?:[1-8]|99))\.((?:6|8|9|29))\.([0-9]{1,2}))|"
-        r"(?:(7)-((?:[0-5]?[0-9])|(?:6[0-5])):(.{1,2})\.(.{1,2})\.([0-9]{1,2}))",
-    )  # Die OBIS-Kennzahl für das Zählwerk, die festlegt, welche auf die gemessene Größe mit dem Stand gemeldet wird.
+    obis_kennzahl: Annotated[
+        str,
+        Field(
+            strict=True,
+            pattern=r"(?:(1)-((?:[0-5]?[0-9])|(?:6[0-5])):((?:[1-8]|99))\.((?:6|8|9|29))\.([0-9]{1,2}))|"
+            r"(?:(7)-((?:[0-5]?[0-9])|(?:6[0-5])):(.{1,2})\.(.{1,2})\.([0-9]{1,2}))",
+        ),
+    ]  # Die OBIS-Kennzahl für das Zählwerk, die festlegt, welche auf die gemessene Größe mit dem Stand gemeldet wird.
     # Nur Zählwerkstände mit dieser OBIS-Kennzahl werden an diesem Zählwerk registriert.
     wandlerfaktor: Decimal  # Mit diesem Faktor wird eine Zählerstandsdifferenz multipliziert, um zum eigentlichen Verbrauch im Zeitraum
     # zu kommen.
     einheit: Mengeneinheit  # Die Einheit der gemessenen Größe, z.B. kWh
```

### Comparing `bo4e-0.5.0/src/bo4e/com/zeitintervall.py` & `bo4e-0.5.1/src/bo4e/com/zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/zeitraum.py` & `bo4e-0.5.1/src/bo4e/com/zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/zeitreihenwert.py` & `bo4e-0.5.1/src/bo4e/com/zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/zeitreihenwertkompakt.py` & `bo4e-0.5.1/src/bo4e/com/zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/com/zustaendigkeit.py` & `bo4e-0.5.1/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/angebotsstatus.py` & `bo4e-0.5.1/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/artikelid.py` & `bo4e-0.5.1/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-0.5.1/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-0.5.1/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-0.5.1/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-0.5.1/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-0.5.1/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/botyp.py` & `bo4e-0.5.1/src/bo4e/enum/botyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-0.5.1/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/erzeugungsart.py` & `bo4e-0.5.1/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/gebiettyp.py` & `bo4e-0.5.1/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/geraetemerkmal.py` & `bo4e-0.5.1/src/bo4e/enum/geraetemerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/geraetetyp.py` & `bo4e-0.5.1/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-0.5.1/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-0.5.1/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/kostenklasse.py` & `bo4e-0.5.1/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/kundengruppe.py` & `bo4e-0.5.1/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/kundengruppeka.py` & `bo4e-0.5.1/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/kundentyp.py` & `bo4e-0.5.1/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/leistungstyp.py` & `bo4e-0.5.1/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/marktrolle.py` & `bo4e-0.5.1/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/mengeneinheit.py` & `bo4e-0.5.1/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/messgroesse.py` & `bo4e-0.5.1/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/messpreistyp.py` & `bo4e-0.5.1/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/messwertstatus.py` & `bo4e-0.5.1/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-0.5.1/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/netzebene.py` & `bo4e-0.5.1/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/nnrechnungstyp.py` & `bo4e-0.5.1/src/bo4e/enum/nnrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/oekolabel.py` & `bo4e-0.5.1/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/oekozertifikat.py` & `bo4e-0.5.1/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/preisgarantietyp.py` & `bo4e-0.5.1/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/preistyp.py` & `bo4e-0.5.1/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/rechnungslegung.py` & `bo4e-0.5.1/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/rechnungsstatus.py` & `bo4e-0.5.1/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/rechnungstyp.py` & `bo4e-0.5.1/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-0.5.1/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/rufnummernart.py` & `bo4e-0.5.1/src/bo4e/enum/rufnummernart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-0.5.1/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-0.5.1/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/tarifmerkmal.py` & `bo4e-0.5.1/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/themengebiet.py` & `bo4e-0.5.1/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/vertragsart.py` & `bo4e-0.5.1/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/vertragsstatus.py` & `bo4e-0.5.1/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/voraussetzungen.py` & `bo4e-0.5.1/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/waehrungscode.py` & `bo4e-0.5.1/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/zaehlertyp.py` & `bo4e-0.5.1/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/enum/zeiteinheit.py` & `bo4e-0.5.1/src/bo4e/enum/zeiteinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/utils/__init__.py` & `bo4e-0.5.1/src/bo4e/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/src/bo4e/validators.py` & `bo4e-0.5.1/src/bo4e/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     """
     Get the checksum of a marktlokations id.
     a) Quersumme aller Ziffern in ungerader Position
     b) Quersumme aller Ziffern auf gerader Position multipliziert mit 2
     c) Summe von a) und b) d) Differenz von c) zum nächsten Vielfachen von 10 (ergibt sich hier 10, wird die
        Prüfziffer 0 genommen
     https://bdew-codes.de/Content/Files/MaLo/2017-04-28-BDEW-Anwendungshilfe-MaLo-ID_Version1.0_FINAL.PDF
-    :param self:
     :return: the checksum as string
     """
     odd_checksum: int = 0
     even_checksum: int = 0
     # start counting at 1 to be consistent with the above description
     # of "even" and "odd" but stop at tenth digit.
     for i in range(1, 11):
```

### Comparing `bo4e-0.5.0/src/bo4e.egg-info/PKG-INFO` & `bo4e-0.5.1/src/bo4e.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.5.0/src/bo4e.egg-info/SOURCES.txt` & `bo4e-0.5.1/src/bo4e.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -416,10 +416,11 @@
 tests/test_vertragsteil.py
 tests/test_zaehler.py
 tests/test_zeitintervall.py
 tests/test_zeitraum.py
 tests/test_zeitreihe.py
 tests/test_zeitreihenwert.py
 tests/test_zeitreihenwertkompakt.py
+tests/utils.py
 tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
 tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
 tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
```

### Comparing `bo4e-0.5.0/tests/serialization_helper.py` & `bo4e-0.5.1/tests/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_adresse.py` & `bo4e-0.5.1/tests/test_adresse.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pytest
 from pydantic import ValidationError
 
 from bo4e.com.adresse import Adresse
 from bo4e.enum import landescode
 from bo4e.enum.landescode import Landescode
+from tests.utils import parse_file
 
 # import pydantic
 
 # can be imported by other tests
 example_adresse = Adresse(
     ort="Grünwald",
     landescode=Landescode.DE,  # type: ignore[attr-defined]
@@ -23,17 +24,16 @@
 class TestAddress:
     def test_serialization_strasse(self) -> None:
         """
         Test serialization with strasse und hausnummer
         and default value of landescode
         """
 
-        address_test_data = Adresse.parse_file(
-            "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json",
-            encoding="utf-8",
+        address_test_data = parse_file(
+            Adresse, "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json"
         )
 
         address_dict = address_test_data.model_dump_json(by_alias=True)
 
         assert "Nördliche Münchner Straße" in address_dict
         assert "27A" in address_dict
         assert "82031" in address_dict
@@ -94,17 +94,16 @@
         deserialized_address = Adresse.model_validate_json(address_json)
 
         assert isinstance(deserialized_address, Adresse)
         assert deserialized_address.ort == "Grünwald"
         assert deserialized_address.postleitzahl == "82031"
 
     def test_serialization_only_required_fields_landescode_AT(self) -> None:
-        address_test_data = Adresse.parse_file(
-            "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json",
-            encoding="utf-8",
+        address_test_data = parse_file(
+            Adresse, "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json"
         )
         address_test_data.landescode = Landescode.AT  # type: ignore[attr-defined]
 
         address_json = address_test_data.model_dump_json(by_alias=True)
         deserialized_address = Adresse.model_validate_json(address_json)
 
         assert deserialized_address.landescode == Landescode.AT  # type: ignore[attr-defined]
@@ -122,15 +121,15 @@
     @pytest.mark.datafiles("./tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json")
     def test_missing_required_attribute(self, datafiles: Path) -> None:
         """
         Test for getting an error message if a required attribute is missing
         """
 
         with pytest.raises(ValidationError) as excinfo:
-            _ = Adresse.parse_file(datafiles / "test_data_adresse_missing_plz.json", encoding="utf-8")
+            _ = parse_file(Adresse, datafiles / "test_data_adresse_missing_plz.json")
 
         assert "postleitzahl" in str(excinfo.value)
 
     @pytest.mark.parametrize(
         "address_test_data, expected",
         [
             pytest.param(
@@ -177,21 +176,15 @@
                 'You have to define either "strasse" and "hausnummer" or "postfach".',
                 id="Postfach and hausnummer",
             ),
         ],
     )
     def test_strasse_xor_postfach(self, address_test_data: Dict[str, Optional[str]], expected: str) -> None:
         with pytest.raises(ValidationError) as excinfo:
-            _ = Adresse(
-                postleitzahl=address_test_data["postleitzahl"],  # type: ignore[arg-type]
-                ort=address_test_data["ort"],  # type: ignore[arg-type]
-                strasse=address_test_data["strasse"],
-                hausnummer=address_test_data["hausnummer"],
-                postfach=address_test_data["postfach"],
-            )
+            _ = Adresse.model_validate(address_test_data)
         assert expected in str(excinfo.value)
 
     def test_serialization_of_non_german_address(self) -> None:
         """
         Minimal working example
         :return:
         """
@@ -204,15 +197,15 @@
         deserialized_address = Adresse.model_validate_json(serialized_address)
         assert deserialized_address.landescode == Landescode.AT  # type: ignore[attr-defined]
 
     @pytest.mark.parametrize(
         "address_json, adresse",
         [
             pytest.param(
-                r"""{"postleitzahl": "12345", 
+                r"""{"postleitzahl": "12345",
                     "ort": "ISS spacestation",
                     "strasse": "Milky Way",
                     "hausnummer": "42",
                     "landescode": "FR",
                     "adresszusatz": "to whom it may concern",
                     "co_ergaenzung": "you will find me",
                     "ortsteil": "Mitte"}""",
```

### Comparing `bo4e-0.5.0/tests/test_angebot.py` & `bo4e-0.5.1/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_angebotsposition.py` & `bo4e-0.5.1/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_angebotsteil.py` & `bo4e-0.5.1/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_angebotsvariante.py` & `bo4e-0.5.1/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_ansprechpartner.py` & `bo4e-0.5.1/tests/test_ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_aufabschlag.py` & `bo4e-0.5.1/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_aufabschlagproort.py` & `bo4e-0.5.1/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_aufabschlagregional.py` & `bo4e-0.5.1/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_aufabschlagstaffelproort.py` & `bo4e-0.5.1/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_ausschreibung.py` & `bo4e-0.5.1/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_ausschreibungsdetail.py` & `bo4e-0.5.1/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_ausschreibungslos.py` & `bo4e-0.5.1/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_betrag.py` & `bo4e-0.5.1/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_buendelvertrag.py` & `bo4e-0.5.1/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_bypassing_validation.py` & `bo4e-0.5.1/tests/test_bypassing_validation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_energieherkunft.py` & `bo4e-0.5.1/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_energiemenge.py` & `bo4e-0.5.1/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_energiemix.py` & `bo4e-0.5.1/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_enums.py` & `bo4e-0.5.1/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_externe_referenz.py` & `bo4e-0.5.1/tests/test_externe_referenz.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,10 +67,10 @@
     def test_extension_data(self) -> None:
         """
         tests the behaviour of the json extension data (`extra="allow"`)
         """
         er = ExterneReferenz(ex_ref_name="foo.bar", ex_ref_wert="12345")
         er_json: Dict[str, Any] = er.model_dump()
         er_json["additional_key"] = "additional_value"
-        deserialized_er: ExterneReferenz = ExterneReferenz.parse_obj(er_json)
+        deserialized_er: ExterneReferenz = ExterneReferenz.model_validate(er_json)
         assert isinstance(deserialized_er, ExterneReferenz)
         assert deserialized_er.additional_key == "additional_value"  # type:ignore[attr-defined]
```

### Comparing `bo4e-0.5.0/tests/test_fremdkosten.py` & `bo4e-0.5.1/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_fremdkostenblock.py` & `bo4e-0.5.1/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_fremdkostenposition.py` & `bo4e-0.5.1/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_geokoordinaten.py` & `bo4e-0.5.1/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_geraet.py` & `bo4e-0.5.1/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_geraeteeigenschaften.py` & `bo4e-0.5.1/tests/test_geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_geschaeftsobjekt.py` & `bo4e-0.5.1/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_geschaeftspartner.py` & `bo4e-0.5.1/tests/test_geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_kosten.py` & `bo4e-0.5.1/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_kostenblock.py` & `bo4e-0.5.1/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_kostenposition.py` & `bo4e-0.5.1/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_kriteriumswert.py` & `bo4e-0.5.1/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_lastgang.py` & `bo4e-0.5.1/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_lastgangkompakt.py` & `bo4e-0.5.1/tests/test_lastgangkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_marktlokation.py` & `bo4e-0.5.1/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_marktteilnehmer.py` & `bo4e-0.5.1/tests/test_marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_menge.py` & `bo4e-0.5.1/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_messlokation.py` & `bo4e-0.5.1/tests/test_messlokation.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,10 +222,10 @@
         """
         melo = Messlokation(
             messlokations_id="DE00056266802AO6G56M11SN51G21M24S",
             sparte=Sparte.STROM,
         )
         melo_json: Dict[str, Any] = melo.model_dump()
         melo_json["additional_key"] = "additional_value"
-        deserialized_melo: Messlokation = Messlokation.parse_obj(melo_json)
+        deserialized_melo: Messlokation = Messlokation.model_validate(melo_json)
         assert isinstance(deserialized_melo, Messlokation)
         assert deserialized_melo.additional_key == "additional_value"  # type:ignore[attr-defined]
```

### Comparing `bo4e-0.5.0/tests/test_messlokationszuordnung.py` & `bo4e-0.5.1/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_netznutzungsrechnung.py` & `bo4e-0.5.1/tests/test_netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_positionsaufabschlag.py` & `bo4e-0.5.1/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preis.py` & `bo4e-0.5.1/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblatt.py` & `bo4e-0.5.1/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblatt_dienstleistung.py` & `bo4e-0.5.1/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblatt_hardware.py` & `bo4e-0.5.1/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-0.5.1/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblatt_messung.py` & `bo4e-0.5.1/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisblattnetznutzung.py` & `bo4e-0.5.1/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisgarantie.py` & `bo4e-0.5.1/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisposition.py` & `bo4e-0.5.1/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_preisstaffel.py` & `bo4e-0.5.1/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_rechnung.py` & `bo4e-0.5.1/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_rechnungsposition.py` & `bo4e-0.5.1/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_region.py` & `bo4e-0.5.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionalegueltigkeit.py` & `bo4e-0.5.1/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionalepreisgarantie.py` & `bo4e-0.5.1/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionalepreisstaffel.py` & `bo4e-0.5.1/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionaleraufabschlag.py` & `bo4e-0.5.1/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionaletarifpreisposition.py` & `bo4e-0.5.1/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionaltarif.py` & `bo4e-0.5.1/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_regionskriterium.py` & `bo4e-0.5.1/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_sigmoidparameter.py` & `bo4e-0.5.1/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_standorteigenschaften.py` & `bo4e-0.5.1/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_standorteigenschaftengas.py` & `bo4e-0.5.1/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_standorteigenschaftenstrom.py` & `bo4e-0.5.1/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_steuerbetrag.py` & `bo4e-0.5.1/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tagesvektor.py` & `bo4e-0.5.1/tests/test_tagesvektor.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarif.py` & `bo4e-0.5.1/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifberechnungsparameter.py` & `bo4e-0.5.1/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifeinschraenkung.py` & `bo4e-0.5.1/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifinfo.py` & `bo4e-0.5.1/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifkosten.py` & `bo4e-0.5.1/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifpreis.py` & `bo4e-0.5.1/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifpreisblatt.py` & `bo4e-0.5.1/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifpreisposition.py` & `bo4e-0.5.1/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifpreispositionproort.py` & `bo4e-0.5.1/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_tarifpreisstaffelproort.py` & `bo4e-0.5.1/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_unterschrift.py` & `bo4e-0.5.1/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_verbrauch.py` & `bo4e-0.5.1/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_vertrag.py` & `bo4e-0.5.1/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_vertragskonditionen.py` & `bo4e-0.5.1/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_vertragsteil.py` & `bo4e-0.5.1/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zaehler.py` & `bo4e-0.5.1/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zeitintervall.py` & `bo4e-0.5.1/tests/test_zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zeitraum.py` & `bo4e-0.5.1/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zeitreihe.py` & `bo4e-0.5.1/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zeitreihenwert.py` & `bo4e-0.5.1/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tests/test_zeitreihenwertkompakt.py` & `bo4e-0.5.1/tests/test_zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.5.0/tox.ini` & `bo4e-0.5.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -20,28 +20,30 @@
     dictdiffer
 commands = python -m pytest --basetemp={envtmpdir} {posargs}
 
 
 [testenv:linting]
 deps =
     -rrequirements.txt
+    {[testenv:docs]deps}
     pylint
-    networkx
-    requests
 commands =
     pylint src/bo4e
     pylint docs/uml.py
     pylint json_schemas/generate_json_schemas.py
 
 [testenv:type_check]
 usedevelop = True
 # the type_check environment checks the type hints using mypy
 deps =
     -rrequirements.txt
+    {[testenv:docs]deps}
     mypy
+    types-requests
+    networkx-stubs
     pytest
 commands =
     mypy --show-error-codes src/bo4e
     mypy --show-error-codes tests
     mypy --show-error-codes docs/uml.py
     mypy --show-error-codes json_schemas/generate_json_schemas.py
     # add single files (ending with .py) or packages here
@@ -81,14 +83,15 @@
 [testenv:docs]
 deps =
     -rrequirements.txt
     Sphinx
     sphinx_rtd_theme
     networkx
     requests
+    typeguard
 commands =
     sphinx-build -W -b html -d {envtmpdir}/doctrees docs {envtmpdir}/html
     sphinx-build -n -T -W -b doctest -d {envtmpdir}/doctrees docs docs/_build/html
     python -m doctest README.rst
 
 
 [testenv:bo4e-from-pip]
```

