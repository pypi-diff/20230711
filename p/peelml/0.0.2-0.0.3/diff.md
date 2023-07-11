# Comparing `tmp/peelml-0.0.2.tar.gz` & `tmp/peelml-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peelml-0.0.2.tar", max compression
+gzip compressed data, was "peelml-0.0.3.tar", max compression
```

## Comparing `peelml-0.0.2.tar` & `peelml-0.0.3.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    11357 2023-07-10 23:20:55.559708 peelml-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1471 2023-07-10 23:20:55.559872 peelml-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.559964 peelml-0.0.2/peelml/__init__.py
--rw-r--r--   0        0        0     2720 2023-07-10 23:20:55.560126 peelml-0.0.2/peelml/cli.py
--rw-r--r--   0        0        0      141 2023-07-10 23:20:55.560265 peelml-0.0.2/peelml/client/.gitignore
--rw-r--r--   0        0        0       43 2023-07-10 23:20:55.560334 peelml-0.0.2/peelml/client/.npmrc
--rw-r--r--   0        0        0      944 2023-07-10 23:20:55.560416 peelml-0.0.2/peelml/client/README.md
--rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.560841 peelml-0.0.2/peelml/client/build/_app/immutable/assets/0.fd99616d.css
--rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.560933 peelml-0.0.2/peelml/client/build/_app/immutable/assets/5.8f04d108.css
--rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561002 peelml-0.0.2/peelml/client/build/_app/immutable/assets/6.98c9af80.css
--rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561142 peelml-0.0.2/peelml/client/build/_app/immutable/assets/7.6f6c636b.css
--rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561359 peelml-0.0.2/peelml/client/build/_app/immutable/assets/8.a14237ec.css
--rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561420 peelml-0.0.2/peelml/client/build/_app/immutable/assets/9.6d9bf5de.css
--rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.561495 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css
--rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561552 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6d9bf5de.css
--rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561616 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css
--rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.561787 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.8f04d108.css
--rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561861 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.98c9af80.css
--rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561967 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.a14237ec.css
--rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.562041 peelml-0.0.2/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0      806 2023-07-10 23:20:55.562102 peelml-0.0.2/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg
--rw-r--r--   0        0        0     3654 2023-07-11 04:05:51.112457 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js
--rw-r--r--   0        0        0       27 2023-07-10 23:20:55.562274 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0    14062 2023-07-11 04:05:51.112735 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.463cc238.js
--rw-r--r--   0        0        0      825 2023-07-11 04:05:51.112841 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.562534 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/logo.be2f9f40.js
--rw-r--r--   0        0        0     2458 2023-07-11 04:05:51.112970 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js
--rw-r--r--   0        0        0     1985 2023-07-11 04:05:51.113089 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/store.4903bc61.js
--rw-r--r--   0        0        0    20948 2023-07-10 23:20:55.563135 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js
--rw-r--r--   0        0        0     8932 2023-07-11 04:05:51.113263 peelml-0.0.2/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js
--rw-r--r--   0        0        0    24059 2023-07-11 04:05:51.113479 peelml-0.0.2/peelml/client/build/_app/immutable/entry/start.c3258ab5.js
--rw-r--r--   0        0        0     6466 2023-07-11 04:05:51.113663 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js
--rw-r--r--   0        0        0      981 2023-07-11 04:05:51.113784 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js
--rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114000 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/10.758b2886.js
--rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114067 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/11.758b2886.js
--rw-r--r--   0        0        0     1322 2023-07-11 04:05:51.114128 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js
--rw-r--r--   0        0        0      996 2023-07-11 04:05:51.114190 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js
--rw-r--r--   0        0        0     1319 2023-07-11 04:05:51.114243 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/14.2e678f15.js
--rw-r--r--   0        0        0     2707 2023-07-11 04:05:51.114504 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js
--rw-r--r--   0        0        0     3447 2023-07-11 04:05:51.114577 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js
--rw-r--r--   0        0        0     2771 2023-07-11 04:05:51.114638 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js
--rw-r--r--   0        0        0     4787 2023-07-11 04:05:51.114706 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/4.177858de.js
--rw-r--r--   0        0        0     6007 2023-07-11 04:05:51.114829 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js
--rw-r--r--   0        0        0   102790 2023-07-11 04:05:51.115307 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js
--rw-r--r--   0        0        0   692826 2023-07-11 04:05:51.117880 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/7.cba8d470.js
--rw-r--r--   0        0        0    39619 2023-07-11 04:05:51.118162 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js
--rw-r--r--   0        0        0      996 2023-07-11 04:05:51.118279 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/9.21929747.js
--rw-r--r--   0        0        0       27 2023-07-11 04:05:51.118441 peelml-0.0.2/peelml/client/build/_app/version.json
--rw-r--r--   0        0        0     2358 2023-07-10 23:20:55.568686 peelml-0.0.2/peelml/client/build/about.html
--rw-r--r--   0        0        0     1706 2023-07-10 23:20:55.568764 peelml-0.0.2/peelml/client/build/addbook.html
--rw-r--r--   0        0        0     3338 2023-07-10 23:20:55.568846 peelml-0.0.2/peelml/client/build/chatbot.html
--rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.569035 peelml-0.0.2/peelml/client/build/favicon.png
--rw-r--r--   0        0        0     1033 2023-07-11 04:05:51.118659 peelml-0.0.2/peelml/client/build/index.html
--rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569264 peelml-0.0.2/peelml/client/build/process copy.html
--rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569330 peelml-0.0.2/peelml/client/build/process.html
--rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569403 peelml-0.0.2/peelml/client/build/randomnumber.html
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.569463 peelml-0.0.2/peelml/client/build/robots.txt
--rw-r--r--   0        0        0     1927 2023-07-10 23:20:55.569530 peelml-0.0.2/peelml/client/build/upload.html
--rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569585 peelml-0.0.2/peelml/client/build/uploadOld.html
--rw-r--r--   0        0        0     1876 2023-07-10 23:20:55.569651 peelml-0.0.2/peelml/client/build/uploadTest.html
--rw-r--r--   0        0        0    66757 2023-07-10 23:20:55.570129 peelml-0.0.2/peelml/client/package-lock.json
--rw-r--r--   0        0        0      793 2023-07-10 23:20:55.570207 peelml-0.0.2/peelml/client/package.json
--rw-r--r--   0        0        0       80 2023-07-10 23:20:55.570261 peelml-0.0.2/peelml/client/postcss.config.js
--rw-r--r--   0        0        0       58 2023-07-10 23:20:55.570341 peelml-0.0.2/peelml/client/src/app.css
--rw-r--r--   0        0        0      329 2023-07-10 23:20:55.570398 peelml-0.0.2/peelml/client/src/app.html
--rw-r--r--   0        0        0      251 2023-07-10 23:20:55.570539 peelml-0.0.2/peelml/client/src/lib/UI/Card.svelte
--rw-r--r--   0        0        0      493 2023-07-10 23:20:55.570636 peelml-0.0.2/peelml/client/src/lib/components/AddBookForm.svelte
--rw-r--r--   0        0        0     4214 2023-07-10 23:20:55.570732 peelml-0.0.2/peelml/client/src/lib/components/Charts/Bubble.svelte
--rw-r--r--   0        0        0      420 2023-07-10 23:20:55.570998 peelml-0.0.2/peelml/client/src/lib/components/Charts/Tooltip.svelte
--rw-r--r--   0        0        0     1219 2023-07-10 23:20:55.571096 peelml-0.0.2/peelml/client/src/lib/components/ChatMessage.svelte
--rw-r--r--   0        0        0     7938 2023-07-10 23:20:55.571379 peelml-0.0.2/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte
--rw-r--r--   0        0        0      381 2023-07-10 23:20:55.571560 peelml-0.0.2/peelml/client/src/lib/components/Embedding/data/projection.js
--rw-r--r--   0        0        0      542 2023-07-10 23:20:55.571457 peelml-0.0.2/peelml/client/src/lib/components/Embedding/data.js
--rw-r--r--   0        0        0      801 2023-07-10 23:20:55.571753 peelml-0.0.2/peelml/client/src/lib/components/Embedding/sequences.js
--rw-r--r--   0        0        0     2075 2023-07-10 23:20:55.571820 peelml-0.0.2/peelml/client/src/lib/components/IndexFiles.svelte
--rw-r--r--   0        0        0      235 2023-07-10 23:20:55.571882 peelml-0.0.2/peelml/client/src/lib/components/Modal.svelte
--rw-r--r--   0        0        0     2219 2023-07-10 23:20:55.571944 peelml-0.0.2/peelml/client/src/lib/components/UploadFiles.svelte
--rw-r--r--   0        0        0      935 2023-07-10 23:20:55.571999 peelml-0.0.2/peelml/client/src/lib/components/UploadTest.svelte
--rw-r--r--   0        0        0     1945 2023-07-10 23:20:55.572100 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte
--rw-r--r--   0        0        0     1909 2023-07-10 23:20:55.572162 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte
--rw-r--r--   0        0        0     7958 2023-07-10 23:20:55.572255 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/Table.svelte
--rw-r--r--   0        0        0     3898 2023-07-10 23:20:55.572453 peelml-0.0.2/peelml/client/src/lib/feedback/ColumnChart.svelte
--rw-r--r--   0        0        0     3888 2023-07-10 23:20:55.572621 peelml-0.0.2/peelml/client/src/lib/feedback/HistogramAnswer.svelte
--rw-r--r--   0        0        0     3873 2023-07-10 23:20:55.572774 peelml-0.0.2/peelml/client/src/lib/feedback/HistogramQuestion.svelte
--rw-r--r--   0        0        0     4967 2023-07-10 23:20:55.572931 peelml-0.0.2/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte
--rw-r--r--   0        0        0     2685 2023-07-10 23:20:55.573089 peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte
--rw-r--r--   0        0        0     2619 2023-07-10 23:20:55.573242 peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardPercentage.svelte
--rw-r--r--   0        0        0     1381 2023-07-10 23:20:55.573380 peelml-0.0.2/peelml/client/src/lib/feedback/QACard.svelte
--rw-r--r--   0        0        0      991 2023-07-10 23:20:55.573495 peelml-0.0.2/peelml/client/src/lib/feedback/QATable.svelte
--rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.573622 peelml-0.0.2/peelml/client/src/lib/images/github.svg
--rw-r--r--   0        0        0      806 2023-07-10 23:20:55.573699 peelml-0.0.2/peelml/client/src/lib/images/logo.svg
--rw-r--r--   0        0        0     1892 2023-07-10 23:20:55.573768 peelml-0.0.2/peelml/client/src/lib/images/svelte-logo.svg
--rw-r--r--   0        0        0   360807 2023-07-10 23:20:55.576100 peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.png
--rw-r--r--   0        0        0   115470 2023-07-10 23:20:55.576232 peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.webp
--rw-r--r--   0        0        0      653 2023-07-10 23:20:55.576502 peelml-0.0.2/peelml/client/src/routes/+layout.svelte
--rw-r--r--   0        0        0      148 2023-07-10 23:20:55.576561 peelml-0.0.2/peelml/client/src/routes/+page.js
--rw-r--r--   0        0        0     1038 2023-07-10 23:20:55.576614 peelml-0.0.2/peelml/client/src/routes/+page.svelte
--rw-r--r--   0        0        0     1972 2023-07-10 23:20:55.576667 peelml-0.0.2/peelml/client/src/routes/Counter.svelte
--rw-r--r--   0        0        0     1152 2023-07-10 23:20:55.576719 peelml-0.0.2/peelml/client/src/routes/Header.svelte
--rw-r--r--   0        0        0     2163 2023-07-10 23:20:55.576775 peelml-0.0.2/peelml/client/src/routes/Sidemenu.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576854 peelml-0.0.2/peelml/client/src/routes/about/+page.js
--rw-r--r--   0        0        0      895 2023-07-10 23:20:55.576912 peelml-0.0.2/peelml/client/src/routes/about/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576992 peelml-0.0.2/peelml/client/src/routes/addbook/+page.js
--rw-r--r--   0        0        0      683 2023-07-10 23:20:55.577049 peelml-0.0.2/peelml/client/src/routes/addbook/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.577118 peelml-0.0.2/peelml/client/src/routes/chatbot/+page.js
--rw-r--r--   0        0        0     8031 2023-07-11 04:05:51.118959 peelml-0.0.2/peelml/client/src/routes/chatbot/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577313 peelml-0.0.2/peelml/client/src/routes/data/+page.js
--rw-r--r--   0        0        0     3645 2023-07-10 23:20:55.577504 peelml-0.0.2/peelml/client/src/routes/data/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577571 peelml-0.0.2/peelml/client/src/routes/embeddings/+page.js
--rw-r--r--   0        0        0      133 2023-07-10 23:20:55.577635 peelml-0.0.2/peelml/client/src/routes/embeddings/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577709 peelml-0.0.2/peelml/client/src/routes/feedback/+page.js
--rw-r--r--   0        0        0     2923 2023-07-10 23:20:55.577847 peelml-0.0.2/peelml/client/src/routes/feedback/+page.svelte
--rw-r--r--   0        0        0      322 2023-07-10 23:20:55.577941 peelml-0.0.2/peelml/client/src/routes/index/+page.js
--rw-r--r--   0        0        0     1867 2023-07-10 23:20:55.578011 peelml-0.0.2/peelml/client/src/routes/index/+page.svelte
--rw-r--r--   0        0        0     6814 2023-07-10 23:20:55.578093 peelml-0.0.2/peelml/client/src/routes/normalize.css
--rw-r--r--   0        0        0     1061 2023-07-10 23:20:55.578154 peelml-0.0.2/peelml/client/src/routes/oldpage.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578436 peelml-0.0.2/peelml/client/src/routes/process/+page.js
--rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578510 peelml-0.0.2/peelml/client/src/routes/process/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578255 peelml-0.0.2/peelml/client/src/routes/process copy/+page.js
--rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578323 peelml-0.0.2/peelml/client/src/routes/process copy/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578620 peelml-0.0.2/peelml/client/src/routes/randomnumber/+page.js
--rw-r--r--   0        0        0      369 2023-07-10 23:20:55.578707 peelml-0.0.2/peelml/client/src/routes/randomnumber/+page.svelte
--rw-r--r--   0        0        0     9118 2023-07-10 23:20:55.578806 peelml-0.0.2/peelml/client/src/routes/styles.css
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578911 peelml-0.0.2/peelml/client/src/routes/upload/+page.js
--rw-r--r--   0        0        0     1621 2023-07-10 23:20:55.578988 peelml-0.0.2/peelml/client/src/routes/upload/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579092 peelml-0.0.2/peelml/client/src/routes/uploadOld/+page.js
--rw-r--r--   0        0        0      366 2023-07-10 23:20:55.579159 peelml-0.0.2/peelml/client/src/routes/uploadOld/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579256 peelml-0.0.2/peelml/client/src/routes/uploadTest/+page.js
--rw-r--r--   0        0        0      241 2023-07-10 23:20:55.579319 peelml-0.0.2/peelml/client/src/routes/uploadTest/+page.svelte
--rw-r--r--   0        0        0     8569 2023-07-10 23:20:55.579487 peelml-0.0.2/peelml/client/src/store.js
--rw-r--r--   0        0        0     1641 2023-07-10 23:20:55.579561 peelml-0.0.2/peelml/client/src/utils.js
--rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.579678 peelml-0.0.2/peelml/client/static/favicon.png
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.579741 peelml-0.0.2/peelml/client/static/robots.txt
--rw-r--r--   0        0        0      144 2023-07-10 23:20:55.579808 peelml-0.0.2/peelml/client/svelte.config.js
--rw-r--r--   0        0        0      242 2023-07-10 23:20:55.579875 peelml-0.0.2/peelml/client/tailwind.config.cjs
--rw-r--r--   0        0        0      364 2023-07-10 23:20:55.579949 peelml-0.0.2/peelml/client/vite.config.js
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580015 peelml-0.0.2/peelml/duck/__init__.py
--rw-r--r--   0        0        0     1430 2023-07-10 23:20:55.580108 peelml-0.0.2/peelml/duck/answer_table.py
--rw-r--r--   0        0        0     3963 2023-07-10 23:20:55.580231 peelml-0.0.2/peelml/duck/preference_table.py
--rw-r--r--   0        0        0     1452 2023-07-10 23:20:55.580323 peelml-0.0.2/peelml/duck/question_table.py
--rw-r--r--   0        0        0     1895 2023-07-10 23:20:55.580436 peelml-0.0.2/peelml/duck/ranking_table.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580514 peelml-0.0.2/peelml/llm/__init__.py
--rw-r--r--   0        0        0      253 2023-07-10 23:20:55.580601 peelml-0.0.2/peelml/llm/abs_llm.py
--rw-r--r--   0        0        0      123 2023-07-10 23:20:55.580667 peelml-0.0.2/peelml/llm/constants.py
--rw-r--r--   0        0        0     1094 2023-07-10 23:20:55.580784 peelml-0.0.2/peelml/llm/embedding_factory.py
--rw-r--r--   0        0        0     1105 2023-07-10 23:20:55.580901 peelml-0.0.2/peelml/llm/llama_cpp.py
--rw-r--r--   0        0        0      895 2023-07-10 23:20:55.581016 peelml-0.0.2/peelml/llm/model_factory.py
--rw-r--r--   0        0        0      935 2023-07-10 23:20:55.581137 peelml-0.0.2/peelml/llm/openai.py
--rw-r--r--   0        0        0     1989 2023-07-10 23:20:55.581256 peelml-0.0.2/peelml/llm/sagemaker.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581335 peelml-0.0.2/peelml/model/__init__.py
--rw-r--r--   0        0        0     3298 2023-07-10 23:20:55.581431 peelml-0.0.2/peelml/model/sagemaker.py
--rw-r--r--   0        0        0    12796 2023-07-11 04:11:21.634754 peelml-0.0.2/peelml/server.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581661 peelml-0.0.2/peelml/vectordb/__init__.py
--rw-r--r--   0        0        0     3096 2023-07-10 23:20:55.581906 peelml-0.0.2/peelml/vectordb/abs_vectordb.py
--rw-r--r--   0        0        0     1520 2023-07-10 23:20:55.582037 peelml-0.0.2/peelml/vectordb/chroma.py
--rw-r--r--   0        0        0       72 2023-07-10 23:20:55.582106 peelml-0.0.2/peelml/vectordb/constants.py
--rw-r--r--   0        0        0      878 2023-07-10 23:20:55.582223 peelml-0.0.2/peelml/vectordb/vectordb_factory.py
--rw-r--r--   0        0        0      990 2023-07-11 04:25:56.182782 peelml-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 peelml-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 23:20:55.559708 peelml-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1471 2023-07-10 23:20:55.559872 peelml-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.559964 peelml-0.0.3/peelml/__init__.py
+-rw-r--r--   0        0        0     2720 2023-07-10 23:20:55.560126 peelml-0.0.3/peelml/cli.py
+-rw-r--r--   0        0        0      141 2023-07-10 23:20:55.560265 peelml-0.0.3/peelml/client/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-10 23:20:55.560334 peelml-0.0.3/peelml/client/.npmrc
+-rw-r--r--   0        0        0      944 2023-07-10 23:20:55.560416 peelml-0.0.3/peelml/client/README.md
+-rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.560841 peelml-0.0.3/peelml/client/build/_app/immutable/assets/0.fd99616d.css
+-rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.560933 peelml-0.0.3/peelml/client/build/_app/immutable/assets/5.8f04d108.css
+-rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561002 peelml-0.0.3/peelml/client/build/_app/immutable/assets/6.98c9af80.css
+-rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561142 peelml-0.0.3/peelml/client/build/_app/immutable/assets/7.6f6c636b.css
+-rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561359 peelml-0.0.3/peelml/client/build/_app/immutable/assets/8.a14237ec.css
+-rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561420 peelml-0.0.3/peelml/client/build/_app/immutable/assets/9.6d9bf5de.css
+-rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.561495 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css
+-rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561552 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.6d9bf5de.css
+-rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561616 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css
+-rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.561787 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.8f04d108.css
+-rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561861 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.98c9af80.css
+-rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561967 peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.a14237ec.css
+-rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.562041 peelml-0.0.3/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0      806 2023-07-10 23:20:55.562102 peelml-0.0.3/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg
+-rw-r--r--   0        0        0     3654 2023-07-11 04:05:51.112457 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js
+-rw-r--r--   0        0        0       27 2023-07-10 23:20:55.562274 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0    14062 2023-07-11 04:05:51.112735 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/index.463cc238.js
+-rw-r--r--   0        0        0      825 2023-07-11 04:05:51.112841 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.562534 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/logo.be2f9f40.js
+-rw-r--r--   0        0        0     2458 2023-07-11 04:05:51.112970 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js
+-rw-r--r--   0        0        0     1985 2023-07-11 04:05:51.113089 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/store.4903bc61.js
+-rw-r--r--   0        0        0    20948 2023-07-10 23:20:55.563135 peelml-0.0.3/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js
+-rw-r--r--   0        0        0     8932 2023-07-11 04:05:51.113263 peelml-0.0.3/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js
+-rw-r--r--   0        0        0    24059 2023-07-11 04:05:51.113479 peelml-0.0.3/peelml/client/build/_app/immutable/entry/start.c3258ab5.js
+-rw-r--r--   0        0        0     6466 2023-07-11 04:05:51.113663 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js
+-rw-r--r--   0        0        0      981 2023-07-11 04:05:51.113784 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js
+-rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114000 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/10.758b2886.js
+-rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114067 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/11.758b2886.js
+-rw-r--r--   0        0        0     1322 2023-07-11 04:05:51.114128 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js
+-rw-r--r--   0        0        0      996 2023-07-11 04:05:51.114190 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js
+-rw-r--r--   0        0        0     1319 2023-07-11 04:05:51.114243 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/14.2e678f15.js
+-rw-r--r--   0        0        0     2707 2023-07-11 04:05:51.114504 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js
+-rw-r--r--   0        0        0     3447 2023-07-11 04:05:51.114577 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js
+-rw-r--r--   0        0        0     2771 2023-07-11 04:05:51.114638 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js
+-rw-r--r--   0        0        0     4787 2023-07-11 04:05:51.114706 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/4.177858de.js
+-rw-r--r--   0        0        0     6007 2023-07-11 04:05:51.114829 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js
+-rw-r--r--   0        0        0   102790 2023-07-11 04:05:51.115307 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js
+-rw-r--r--   0        0        0   692826 2023-07-11 04:05:51.117880 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/7.cba8d470.js
+-rw-r--r--   0        0        0    39619 2023-07-11 04:05:51.118162 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js
+-rw-r--r--   0        0        0      996 2023-07-11 04:05:51.118279 peelml-0.0.3/peelml/client/build/_app/immutable/nodes/9.21929747.js
+-rw-r--r--   0        0        0       27 2023-07-11 04:05:51.118441 peelml-0.0.3/peelml/client/build/_app/version.json
+-rw-r--r--   0        0        0     2358 2023-07-10 23:20:55.568686 peelml-0.0.3/peelml/client/build/about.html
+-rw-r--r--   0        0        0     1706 2023-07-10 23:20:55.568764 peelml-0.0.3/peelml/client/build/addbook.html
+-rw-r--r--   0        0        0     3338 2023-07-10 23:20:55.568846 peelml-0.0.3/peelml/client/build/chatbot.html
+-rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.569035 peelml-0.0.3/peelml/client/build/favicon.png
+-rw-r--r--   0        0        0     1033 2023-07-11 04:05:51.118659 peelml-0.0.3/peelml/client/build/index.html
+-rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569264 peelml-0.0.3/peelml/client/build/process copy.html
+-rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569330 peelml-0.0.3/peelml/client/build/process.html
+-rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569403 peelml-0.0.3/peelml/client/build/randomnumber.html
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.569463 peelml-0.0.3/peelml/client/build/robots.txt
+-rw-r--r--   0        0        0     1927 2023-07-10 23:20:55.569530 peelml-0.0.3/peelml/client/build/upload.html
+-rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569585 peelml-0.0.3/peelml/client/build/uploadOld.html
+-rw-r--r--   0        0        0     1876 2023-07-10 23:20:55.569651 peelml-0.0.3/peelml/client/build/uploadTest.html
+-rw-r--r--   0        0        0    66757 2023-07-10 23:20:55.570129 peelml-0.0.3/peelml/client/package-lock.json
+-rw-r--r--   0        0        0      793 2023-07-10 23:20:55.570207 peelml-0.0.3/peelml/client/package.json
+-rw-r--r--   0        0        0       80 2023-07-10 23:20:55.570261 peelml-0.0.3/peelml/client/postcss.config.js
+-rw-r--r--   0        0        0       58 2023-07-10 23:20:55.570341 peelml-0.0.3/peelml/client/src/app.css
+-rw-r--r--   0        0        0      329 2023-07-10 23:20:55.570398 peelml-0.0.3/peelml/client/src/app.html
+-rw-r--r--   0        0        0      251 2023-07-10 23:20:55.570539 peelml-0.0.3/peelml/client/src/lib/UI/Card.svelte
+-rw-r--r--   0        0        0      493 2023-07-10 23:20:55.570636 peelml-0.0.3/peelml/client/src/lib/components/AddBookForm.svelte
+-rw-r--r--   0        0        0     4214 2023-07-10 23:20:55.570732 peelml-0.0.3/peelml/client/src/lib/components/Charts/Bubble.svelte
+-rw-r--r--   0        0        0      420 2023-07-10 23:20:55.570998 peelml-0.0.3/peelml/client/src/lib/components/Charts/Tooltip.svelte
+-rw-r--r--   0        0        0     1219 2023-07-10 23:20:55.571096 peelml-0.0.3/peelml/client/src/lib/components/ChatMessage.svelte
+-rw-r--r--   0        0        0     7938 2023-07-10 23:20:55.571379 peelml-0.0.3/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte
+-rw-r--r--   0        0        0      381 2023-07-10 23:20:55.571560 peelml-0.0.3/peelml/client/src/lib/components/Embedding/data/projection.js
+-rw-r--r--   0        0        0      542 2023-07-10 23:20:55.571457 peelml-0.0.3/peelml/client/src/lib/components/Embedding/data.js
+-rw-r--r--   0        0        0      801 2023-07-10 23:20:55.571753 peelml-0.0.3/peelml/client/src/lib/components/Embedding/sequences.js
+-rw-r--r--   0        0        0     2075 2023-07-10 23:20:55.571820 peelml-0.0.3/peelml/client/src/lib/components/IndexFiles.svelte
+-rw-r--r--   0        0        0      235 2023-07-10 23:20:55.571882 peelml-0.0.3/peelml/client/src/lib/components/Modal.svelte
+-rw-r--r--   0        0        0     2219 2023-07-10 23:20:55.571944 peelml-0.0.3/peelml/client/src/lib/components/UploadFiles.svelte
+-rw-r--r--   0        0        0      935 2023-07-10 23:20:55.571999 peelml-0.0.3/peelml/client/src/lib/components/UploadTest.svelte
+-rw-r--r--   0        0        0     1945 2023-07-10 23:20:55.572100 peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte
+-rw-r--r--   0        0        0     1909 2023-07-10 23:20:55.572162 peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte
+-rw-r--r--   0        0        0     7958 2023-07-10 23:20:55.572255 peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/Table.svelte
+-rw-r--r--   0        0        0     3898 2023-07-10 23:20:55.572453 peelml-0.0.3/peelml/client/src/lib/feedback/ColumnChart.svelte
+-rw-r--r--   0        0        0     3888 2023-07-10 23:20:55.572621 peelml-0.0.3/peelml/client/src/lib/feedback/HistogramAnswer.svelte
+-rw-r--r--   0        0        0     3873 2023-07-10 23:20:55.572774 peelml-0.0.3/peelml/client/src/lib/feedback/HistogramQuestion.svelte
+-rw-r--r--   0        0        0     4967 2023-07-10 23:20:55.572931 peelml-0.0.3/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte
+-rw-r--r--   0        0        0     2685 2023-07-10 23:20:55.573089 peelml-0.0.3/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte
+-rw-r--r--   0        0        0     2619 2023-07-10 23:20:55.573242 peelml-0.0.3/peelml/client/src/lib/feedback/MetricCardPercentage.svelte
+-rw-r--r--   0        0        0     1381 2023-07-10 23:20:55.573380 peelml-0.0.3/peelml/client/src/lib/feedback/QACard.svelte
+-rw-r--r--   0        0        0      991 2023-07-10 23:20:55.573495 peelml-0.0.3/peelml/client/src/lib/feedback/QATable.svelte
+-rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.573622 peelml-0.0.3/peelml/client/src/lib/images/github.svg
+-rw-r--r--   0        0        0      806 2023-07-10 23:20:55.573699 peelml-0.0.3/peelml/client/src/lib/images/logo.svg
+-rw-r--r--   0        0        0     1892 2023-07-10 23:20:55.573768 peelml-0.0.3/peelml/client/src/lib/images/svelte-logo.svg
+-rw-r--r--   0        0        0   360807 2023-07-10 23:20:55.576100 peelml-0.0.3/peelml/client/src/lib/images/svelte-welcome.png
+-rw-r--r--   0        0        0   115470 2023-07-10 23:20:55.576232 peelml-0.0.3/peelml/client/src/lib/images/svelte-welcome.webp
+-rw-r--r--   0        0        0      653 2023-07-10 23:20:55.576502 peelml-0.0.3/peelml/client/src/routes/+layout.svelte
+-rw-r--r--   0        0        0      148 2023-07-10 23:20:55.576561 peelml-0.0.3/peelml/client/src/routes/+page.js
+-rw-r--r--   0        0        0     1038 2023-07-10 23:20:55.576614 peelml-0.0.3/peelml/client/src/routes/+page.svelte
+-rw-r--r--   0        0        0     1972 2023-07-10 23:20:55.576667 peelml-0.0.3/peelml/client/src/routes/Counter.svelte
+-rw-r--r--   0        0        0     1152 2023-07-10 23:20:55.576719 peelml-0.0.3/peelml/client/src/routes/Header.svelte
+-rw-r--r--   0        0        0     2163 2023-07-10 23:20:55.576775 peelml-0.0.3/peelml/client/src/routes/Sidemenu.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576854 peelml-0.0.3/peelml/client/src/routes/about/+page.js
+-rw-r--r--   0        0        0      895 2023-07-10 23:20:55.576912 peelml-0.0.3/peelml/client/src/routes/about/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576992 peelml-0.0.3/peelml/client/src/routes/addbook/+page.js
+-rw-r--r--   0        0        0      683 2023-07-10 23:20:55.577049 peelml-0.0.3/peelml/client/src/routes/addbook/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.577118 peelml-0.0.3/peelml/client/src/routes/chatbot/+page.js
+-rw-r--r--   0        0        0     8031 2023-07-11 04:05:51.118959 peelml-0.0.3/peelml/client/src/routes/chatbot/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577313 peelml-0.0.3/peelml/client/src/routes/data/+page.js
+-rw-r--r--   0        0        0     3645 2023-07-10 23:20:55.577504 peelml-0.0.3/peelml/client/src/routes/data/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577571 peelml-0.0.3/peelml/client/src/routes/embeddings/+page.js
+-rw-r--r--   0        0        0      133 2023-07-10 23:20:55.577635 peelml-0.0.3/peelml/client/src/routes/embeddings/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577709 peelml-0.0.3/peelml/client/src/routes/feedback/+page.js
+-rw-r--r--   0        0        0     2923 2023-07-10 23:20:55.577847 peelml-0.0.3/peelml/client/src/routes/feedback/+page.svelte
+-rw-r--r--   0        0        0      322 2023-07-10 23:20:55.577941 peelml-0.0.3/peelml/client/src/routes/index/+page.js
+-rw-r--r--   0        0        0     1867 2023-07-10 23:20:55.578011 peelml-0.0.3/peelml/client/src/routes/index/+page.svelte
+-rw-r--r--   0        0        0     6814 2023-07-10 23:20:55.578093 peelml-0.0.3/peelml/client/src/routes/normalize.css
+-rw-r--r--   0        0        0     1061 2023-07-10 23:20:55.578154 peelml-0.0.3/peelml/client/src/routes/oldpage.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578436 peelml-0.0.3/peelml/client/src/routes/process/+page.js
+-rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578510 peelml-0.0.3/peelml/client/src/routes/process/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578255 peelml-0.0.3/peelml/client/src/routes/process copy/+page.js
+-rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578323 peelml-0.0.3/peelml/client/src/routes/process copy/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578620 peelml-0.0.3/peelml/client/src/routes/randomnumber/+page.js
+-rw-r--r--   0        0        0      369 2023-07-10 23:20:55.578707 peelml-0.0.3/peelml/client/src/routes/randomnumber/+page.svelte
+-rw-r--r--   0        0        0     9118 2023-07-10 23:20:55.578806 peelml-0.0.3/peelml/client/src/routes/styles.css
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578911 peelml-0.0.3/peelml/client/src/routes/upload/+page.js
+-rw-r--r--   0        0        0     1621 2023-07-10 23:20:55.578988 peelml-0.0.3/peelml/client/src/routes/upload/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579092 peelml-0.0.3/peelml/client/src/routes/uploadOld/+page.js
+-rw-r--r--   0        0        0      366 2023-07-10 23:20:55.579159 peelml-0.0.3/peelml/client/src/routes/uploadOld/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579256 peelml-0.0.3/peelml/client/src/routes/uploadTest/+page.js
+-rw-r--r--   0        0        0      241 2023-07-10 23:20:55.579319 peelml-0.0.3/peelml/client/src/routes/uploadTest/+page.svelte
+-rw-r--r--   0        0        0     8569 2023-07-10 23:20:55.579487 peelml-0.0.3/peelml/client/src/store.js
+-rw-r--r--   0        0        0     1641 2023-07-10 23:20:55.579561 peelml-0.0.3/peelml/client/src/utils.js
+-rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.579678 peelml-0.0.3/peelml/client/static/favicon.png
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.579741 peelml-0.0.3/peelml/client/static/robots.txt
+-rw-r--r--   0        0        0      144 2023-07-10 23:20:55.579808 peelml-0.0.3/peelml/client/svelte.config.js
+-rw-r--r--   0        0        0      242 2023-07-10 23:20:55.579875 peelml-0.0.3/peelml/client/tailwind.config.cjs
+-rw-r--r--   0        0        0      364 2023-07-10 23:20:55.579949 peelml-0.0.3/peelml/client/vite.config.js
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580015 peelml-0.0.3/peelml/duck/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-10 23:20:55.580108 peelml-0.0.3/peelml/duck/answer_table.py
+-rw-r--r--   0        0        0     3963 2023-07-10 23:20:55.580231 peelml-0.0.3/peelml/duck/preference_table.py
+-rw-r--r--   0        0        0     1452 2023-07-10 23:20:55.580323 peelml-0.0.3/peelml/duck/question_table.py
+-rw-r--r--   0        0        0     1895 2023-07-10 23:20:55.580436 peelml-0.0.3/peelml/duck/ranking_table.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580514 peelml-0.0.3/peelml/llm/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-10 23:20:55.580601 peelml-0.0.3/peelml/llm/abs_llm.py
+-rw-r--r--   0        0        0      123 2023-07-10 23:20:55.580667 peelml-0.0.3/peelml/llm/constants.py
+-rw-r--r--   0        0        0     1094 2023-07-10 23:20:55.580784 peelml-0.0.3/peelml/llm/embedding_factory.py
+-rw-r--r--   0        0        0     1105 2023-07-10 23:20:55.580901 peelml-0.0.3/peelml/llm/llama_cpp.py
+-rw-r--r--   0        0        0      895 2023-07-10 23:20:55.581016 peelml-0.0.3/peelml/llm/model_factory.py
+-rw-r--r--   0        0        0      935 2023-07-10 23:20:55.581137 peelml-0.0.3/peelml/llm/openai.py
+-rw-r--r--   0        0        0     1989 2023-07-10 23:20:55.581256 peelml-0.0.3/peelml/llm/sagemaker.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581335 peelml-0.0.3/peelml/model/__init__.py
+-rw-r--r--   0        0        0     3298 2023-07-10 23:20:55.581431 peelml-0.0.3/peelml/model/sagemaker.py
+-rw-r--r--   0        0        0    12745 2023-07-11 04:40:55.247164 peelml-0.0.3/peelml/server.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581661 peelml-0.0.3/peelml/vectordb/__init__.py
+-rw-r--r--   0        0        0     3096 2023-07-10 23:20:55.581906 peelml-0.0.3/peelml/vectordb/abs_vectordb.py
+-rw-r--r--   0        0        0     1520 2023-07-10 23:20:55.582037 peelml-0.0.3/peelml/vectordb/chroma.py
+-rw-r--r--   0        0        0       72 2023-07-10 23:20:55.582106 peelml-0.0.3/peelml/vectordb/constants.py
+-rw-r--r--   0        0        0      878 2023-07-10 23:20:55.582223 peelml-0.0.3/peelml/vectordb/vectordb_factory.py
+-rw-r--r--   0        0        0      990 2023-07-11 04:38:23.352043 peelml-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 peelml-0.0.3/PKG-INFO
```

### Comparing `peelml-0.0.2/LICENSE.txt` & `peelml-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/README.md` & `peelml-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/cli.py` & `peelml-0.0.3/peelml/cli.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/README.md` & `peelml-0.0.3/peelml/client/README.md`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/0.fd99616d.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/0.fd99616d.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/5.8f04d108.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/5.8f04d108.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/6.98c9af80.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/6.98c9af80.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/7.6f6c636b.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/7.6f6c636b.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/8.a14237ec.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/8.a14237ec.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.8f04d108.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.8f04d108.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.98c9af80.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.98c9af80.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.a14237ec.css` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/_page.a14237ec.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg` & `peelml-0.0.3/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.463cc238.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/index.463cc238.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/store.4903bc61.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/store.4903bc61.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/entry/start.c3258ab5.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/entry/start.c3258ab5.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/10.758b2886.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/10.758b2886.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/11.758b2886.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/11.758b2886.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/14.2e678f15.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/14.2e678f15.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/4.177858de.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/4.177858de.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/7.cba8d470.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/7.cba8d470.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/9.21929747.js` & `peelml-0.0.3/peelml/client/build/_app/immutable/nodes/9.21929747.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/about.html` & `peelml-0.0.3/peelml/client/build/about.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/addbook.html` & `peelml-0.0.3/peelml/client/build/addbook.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/chatbot.html` & `peelml-0.0.3/peelml/client/build/chatbot.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/favicon.png` & `peelml-0.0.3/peelml/client/build/favicon.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/index.html` & `peelml-0.0.3/peelml/client/build/index.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/process copy.html` & `peelml-0.0.3/peelml/client/build/process copy.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/process.html` & `peelml-0.0.3/peelml/client/build/process.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/randomnumber.html` & `peelml-0.0.3/peelml/client/build/randomnumber.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/upload.html` & `peelml-0.0.3/peelml/client/build/upload.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/uploadOld.html` & `peelml-0.0.3/peelml/client/build/uploadOld.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/build/uploadTest.html` & `peelml-0.0.3/peelml/client/build/uploadTest.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/package-lock.json` & `peelml-0.0.3/peelml/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/package.json` & `peelml-0.0.3/peelml/client/package.json`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/Charts/Bubble.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/Charts/Bubble.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/ChatMessage.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/ChatMessage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/Embedding/data.js` & `peelml-0.0.3/peelml/client/src/lib/components/Embedding/data.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/Embedding/sequences.js` & `peelml-0.0.3/peelml/client/src/lib/components/Embedding/sequences.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/IndexFiles.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/IndexFiles.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/UploadFiles.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/UploadFiles.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/UploadTest.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/UploadTest.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/Table.svelte` & `peelml-0.0.3/peelml/client/src/lib/components/tanstackTable/Table.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/ColumnChart.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/ColumnChart.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/HistogramAnswer.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/HistogramAnswer.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/HistogramQuestion.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/HistogramQuestion.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardPercentage.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/MetricCardPercentage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/QACard.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/QACard.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/feedback/QATable.svelte` & `peelml-0.0.3/peelml/client/src/lib/feedback/QATable.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/images/github.svg` & `peelml-0.0.3/peelml/client/src/lib/images/github.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/images/logo.svg` & `peelml-0.0.3/peelml/client/src/lib/images/logo.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/images/svelte-logo.svg` & `peelml-0.0.3/peelml/client/src/lib/images/svelte-logo.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.png` & `peelml-0.0.3/peelml/client/src/lib/images/svelte-welcome.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.webp` & `peelml-0.0.3/peelml/client/src/lib/images/svelte-welcome.webp`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/+layout.svelte` & `peelml-0.0.3/peelml/client/src/routes/+layout.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/Counter.svelte` & `peelml-0.0.3/peelml/client/src/routes/Counter.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/Header.svelte` & `peelml-0.0.3/peelml/client/src/routes/Header.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/Sidemenu.svelte` & `peelml-0.0.3/peelml/client/src/routes/Sidemenu.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/about/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/about/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/addbook/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/addbook/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/chatbot/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/chatbot/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/data/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/data/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/feedback/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/feedback/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/index/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/index/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/normalize.css` & `peelml-0.0.3/peelml/client/src/routes/normalize.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/oldpage.svelte` & `peelml-0.0.3/peelml/client/src/routes/oldpage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/process/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/process/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/process copy/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/process copy/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/styles.css` & `peelml-0.0.3/peelml/client/src/routes/styles.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/routes/upload/+page.svelte` & `peelml-0.0.3/peelml/client/src/routes/upload/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/store.js` & `peelml-0.0.3/peelml/client/src/store.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/src/utils.js` & `peelml-0.0.3/peelml/client/src/utils.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/client/static/favicon.png` & `peelml-0.0.3/peelml/client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/duck/answer_table.py` & `peelml-0.0.3/peelml/duck/answer_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/duck/preference_table.py` & `peelml-0.0.3/peelml/duck/preference_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/duck/question_table.py` & `peelml-0.0.3/peelml/duck/question_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/duck/ranking_table.py` & `peelml-0.0.3/peelml/duck/ranking_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/llm/embedding_factory.py` & `peelml-0.0.3/peelml/llm/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/llm/llama_cpp.py` & `peelml-0.0.3/peelml/llm/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/llm/model_factory.py` & `peelml-0.0.3/peelml/llm/model_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/llm/openai.py` & `peelml-0.0.3/peelml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/llm/sagemaker.py` & `peelml-0.0.3/peelml/llm/sagemaker.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/model/sagemaker.py` & `peelml-0.0.3/peelml/model/sagemaker.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/server.py` & `peelml-0.0.3/peelml/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,13 +411,13 @@
     # upate doc path, vector db path, and openai api key #
     ######################################################
     cwd = os.getcwd()
     print(f"[server]: the current path is {cwd}")
     os.environ["DOC_PATH"] = os.path.join(cwd, "peelml/docs")
     os.environ["VECTORDB_PATH"] = os.path.join(cwd, "peelml/db")
     os.environ["DUCKDB_PATH"] = os.path.join(cwd, "peelml/db/duck")
-    os.environ["OPENAI_API_KEY"] = "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"
+    os.environ["OPENAI_API_KEY"] = ""
     app.config["vectordb"] = "chroma"
     app.config["model"] = "openai"
     if os.environ["OPENAI_API_KEY"] == "":
         raise ValueError("OPENAI_API_KEY is not set")
     app.run(port=5000, debug=True)
```

### Comparing `peelml-0.0.2/peelml/vectordb/abs_vectordb.py` & `peelml-0.0.3/peelml/vectordb/abs_vectordb.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/vectordb/chroma.py` & `peelml-0.0.3/peelml/vectordb/chroma.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/peelml/vectordb/vectordb_factory.py` & `peelml-0.0.3/peelml/vectordb/vectordb_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.2/pyproject.toml` & `peelml-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peelml"
-version = "0.0.2"
+version = "0.0.3"
 description = "Peel away the pain of ml deployment"
 authors = ["Rachel Hu <goldpiggy@berkeley.edu>"]
 maintainers = [
     "Jared Wilber <jdwlbr@gmail.com>",
     "Rachel Hu <goldpiggy@berkeley.edu>"
     ]
 readme = "README.md"
```

### Comparing `peelml-0.0.2/PKG-INFO` & `peelml-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peelml
-Version: 0.0.2
+Version: 0.0.3
 Summary: Peel away the pain of ml deployment
 Author: Rachel Hu
 Author-email: goldpiggy@berkeley.edu
 Maintainer: Jared Wilber
 Maintainer-email: jdwlbr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

