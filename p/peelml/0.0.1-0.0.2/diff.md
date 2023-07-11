# Comparing `tmp/peelml-0.0.1.tar.gz` & `tmp/peelml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peelml-0.0.1.tar", max compression
+gzip compressed data, was "peelml-0.0.2.tar", max compression
```

## Comparing `peelml-0.0.1.tar` & `peelml-0.0.2.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0    11357 2023-07-10 23:20:55.559708 peelml-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1471 2023-07-10 23:20:55.559872 peelml-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.559964 peelml-0.0.1/peelml/__init__.py
--rw-r--r--   0        0        0     2720 2023-07-10 23:20:55.560126 peelml-0.0.1/peelml/cli.py
--rw-r--r--   0        0        0      141 2023-07-10 23:20:55.560265 peelml-0.0.1/peelml/client/.gitignore
--rw-r--r--   0        0        0       43 2023-07-10 23:20:55.560334 peelml-0.0.1/peelml/client/.npmrc
--rw-r--r--   0        0        0      944 2023-07-10 23:20:55.560416 peelml-0.0.1/peelml/client/README.md
--rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.560841 peelml-0.0.1/peelml/client/build/_app/immutable/assets/0.fd99616d.css
--rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.560933 peelml-0.0.1/peelml/client/build/_app/immutable/assets/5.8f04d108.css
--rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561002 peelml-0.0.1/peelml/client/build/_app/immutable/assets/6.98c9af80.css
--rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561142 peelml-0.0.1/peelml/client/build/_app/immutable/assets/7.6f6c636b.css
--rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561359 peelml-0.0.1/peelml/client/build/_app/immutable/assets/8.a14237ec.css
--rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561420 peelml-0.0.1/peelml/client/build/_app/immutable/assets/9.6d9bf5de.css
--rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.561495 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css
--rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561552 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.6d9bf5de.css
--rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561616 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css
--rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.561787 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.8f04d108.css
--rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561861 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.98c9af80.css
--rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561967 peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.a14237ec.css
--rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.562041 peelml-0.0.1/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg
--rw-r--r--   0        0        0      806 2023-07-10 23:20:55.562102 peelml-0.0.1/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg
--rw-r--r--   0        0        0     3654 2023-07-10 23:20:55.562209 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/UploadFiles.c03ead87.js
--rw-r--r--   0        0        0       27 2023-07-10 23:20:55.562274 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/environment.9aa685ef.js
--rw-r--r--   0        0        0    14062 2023-07-10 23:20:55.562379 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/index.84b8b39e.js
--rw-r--r--   0        0        0      825 2023-07-10 23:20:55.562440 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/index.eb24f9d9.js
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.562534 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/logo.be2f9f40.js
--rw-r--r--   0        0        0     2458 2023-07-10 23:20:55.562644 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/singletons.96029e7d.js
--rw-r--r--   0        0        0     1985 2023-07-10 23:20:55.562880 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/store.322467ea.js
--rw-r--r--   0        0        0    20948 2023-07-10 23:20:55.563135 peelml-0.0.1/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js
--rw-r--r--   0        0        0     8932 2023-07-10 23:20:55.563333 peelml-0.0.1/peelml/client/build/_app/immutable/entry/app.ec7afc1f.js
--rw-r--r--   0        0        0    24059 2023-07-10 23:20:55.563532 peelml-0.0.1/peelml/client/build/_app/immutable/entry/start.dd2cf025.js
--rw-r--r--   0        0        0     6466 2023-07-10 23:20:55.563716 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/0.b9c3e59d.js
--rw-r--r--   0        0        0      981 2023-07-10 23:20:55.563831 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/1.77aa025a.js
--rw-r--r--   0        0        0     1707 2023-07-10 23:20:55.564012 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/10.7909aaae.js
--rw-r--r--   0        0        0     1707 2023-07-10 23:20:55.564077 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/11.7909aaae.js
--rw-r--r--   0        0        0     1322 2023-07-10 23:20:55.564142 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/12.512086c8.js
--rw-r--r--   0        0        0      996 2023-07-10 23:20:55.564206 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/13.c0f6c67f.js
--rw-r--r--   0        0        0     1319 2023-07-10 23:20:55.564269 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/14.59fcfc6f.js
--rw-r--r--   0        0        0     2707 2023-07-10 23:20:55.564342 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/15.916fb8a4.js
--rw-r--r--   0        0        0     3447 2023-07-10 23:20:55.564416 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/2.75c7eb74.js
--rw-r--r--   0        0        0     2771 2023-07-10 23:20:55.564514 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/3.f27f0658.js
--rw-r--r--   0        0        0     4787 2023-07-10 23:20:55.564589 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/4.e26998a1.js
--rw-r--r--   0        0        0     5901 2023-07-10 23:20:55.564719 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/5.627b2dc7.js
--rw-r--r--   0        0        0   102790 2023-07-10 23:20:55.565503 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/6.e941ef4d.js
--rw-r--r--   0        0        0   692826 2023-07-10 23:20:55.568087 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/7.6a37f45a.js
--rw-r--r--   0        0        0    39619 2023-07-10 23:20:55.568403 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/8.59c844c2.js
--rw-r--r--   0        0        0      996 2023-07-10 23:20:55.568505 peelml-0.0.1/peelml/client/build/_app/immutable/nodes/9.4133202d.js
--rw-r--r--   0        0        0       27 2023-07-10 23:20:55.568618 peelml-0.0.1/peelml/client/build/_app/version.json
--rw-r--r--   0        0        0     2358 2023-07-10 23:20:55.568686 peelml-0.0.1/peelml/client/build/about.html
--rw-r--r--   0        0        0     1706 2023-07-10 23:20:55.568764 peelml-0.0.1/peelml/client/build/addbook.html
--rw-r--r--   0        0        0     3338 2023-07-10 23:20:55.568846 peelml-0.0.1/peelml/client/build/chatbot.html
--rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.569035 peelml-0.0.1/peelml/client/build/favicon.png
--rw-r--r--   0        0        0     1033 2023-07-10 23:20:55.569183 peelml-0.0.1/peelml/client/build/index.html
--rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569264 peelml-0.0.1/peelml/client/build/process copy.html
--rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569330 peelml-0.0.1/peelml/client/build/process.html
--rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569403 peelml-0.0.1/peelml/client/build/randomnumber.html
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.569463 peelml-0.0.1/peelml/client/build/robots.txt
--rw-r--r--   0        0        0     1927 2023-07-10 23:20:55.569530 peelml-0.0.1/peelml/client/build/upload.html
--rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569585 peelml-0.0.1/peelml/client/build/uploadOld.html
--rw-r--r--   0        0        0     1876 2023-07-10 23:20:55.569651 peelml-0.0.1/peelml/client/build/uploadTest.html
--rw-r--r--   0        0        0    66757 2023-07-10 23:20:55.570129 peelml-0.0.1/peelml/client/package-lock.json
--rw-r--r--   0        0        0      793 2023-07-10 23:20:55.570207 peelml-0.0.1/peelml/client/package.json
--rw-r--r--   0        0        0       80 2023-07-10 23:20:55.570261 peelml-0.0.1/peelml/client/postcss.config.js
--rw-r--r--   0        0        0       58 2023-07-10 23:20:55.570341 peelml-0.0.1/peelml/client/src/app.css
--rw-r--r--   0        0        0      329 2023-07-10 23:20:55.570398 peelml-0.0.1/peelml/client/src/app.html
--rw-r--r--   0        0        0      251 2023-07-10 23:20:55.570539 peelml-0.0.1/peelml/client/src/lib/UI/Card.svelte
--rw-r--r--   0        0        0      493 2023-07-10 23:20:55.570636 peelml-0.0.1/peelml/client/src/lib/components/AddBookForm.svelte
--rw-r--r--   0        0        0     4214 2023-07-10 23:20:55.570732 peelml-0.0.1/peelml/client/src/lib/components/Charts/Bubble.svelte
--rw-r--r--   0        0        0      420 2023-07-10 23:20:55.570998 peelml-0.0.1/peelml/client/src/lib/components/Charts/Tooltip.svelte
--rw-r--r--   0        0        0     1219 2023-07-10 23:20:55.571096 peelml-0.0.1/peelml/client/src/lib/components/ChatMessage.svelte
--rw-r--r--   0        0        0     7938 2023-07-10 23:20:55.571379 peelml-0.0.1/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte
--rw-r--r--   0        0        0      381 2023-07-10 23:20:55.571560 peelml-0.0.1/peelml/client/src/lib/components/Embedding/data/projection.js
--rw-r--r--   0        0        0      542 2023-07-10 23:20:55.571457 peelml-0.0.1/peelml/client/src/lib/components/Embedding/data.js
--rw-r--r--   0        0        0      801 2023-07-10 23:20:55.571753 peelml-0.0.1/peelml/client/src/lib/components/Embedding/sequences.js
--rw-r--r--   0        0        0     2075 2023-07-10 23:20:55.571820 peelml-0.0.1/peelml/client/src/lib/components/IndexFiles.svelte
--rw-r--r--   0        0        0      235 2023-07-10 23:20:55.571882 peelml-0.0.1/peelml/client/src/lib/components/Modal.svelte
--rw-r--r--   0        0        0     2219 2023-07-10 23:20:55.571944 peelml-0.0.1/peelml/client/src/lib/components/UploadFiles.svelte
--rw-r--r--   0        0        0      935 2023-07-10 23:20:55.571999 peelml-0.0.1/peelml/client/src/lib/components/UploadTest.svelte
--rw-r--r--   0        0        0     1945 2023-07-10 23:20:55.572100 peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte
--rw-r--r--   0        0        0     1909 2023-07-10 23:20:55.572162 peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte
--rw-r--r--   0        0        0     7958 2023-07-10 23:20:55.572255 peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/Table.svelte
--rw-r--r--   0        0        0     3898 2023-07-10 23:20:55.572453 peelml-0.0.1/peelml/client/src/lib/feedback/ColumnChart.svelte
--rw-r--r--   0        0        0     3888 2023-07-10 23:20:55.572621 peelml-0.0.1/peelml/client/src/lib/feedback/HistogramAnswer.svelte
--rw-r--r--   0        0        0     3873 2023-07-10 23:20:55.572774 peelml-0.0.1/peelml/client/src/lib/feedback/HistogramQuestion.svelte
--rw-r--r--   0        0        0     4967 2023-07-10 23:20:55.572931 peelml-0.0.1/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte
--rw-r--r--   0        0        0     2685 2023-07-10 23:20:55.573089 peelml-0.0.1/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte
--rw-r--r--   0        0        0     2619 2023-07-10 23:20:55.573242 peelml-0.0.1/peelml/client/src/lib/feedback/MetricCardPercentage.svelte
--rw-r--r--   0        0        0     1381 2023-07-10 23:20:55.573380 peelml-0.0.1/peelml/client/src/lib/feedback/QACard.svelte
--rw-r--r--   0        0        0      991 2023-07-10 23:20:55.573495 peelml-0.0.1/peelml/client/src/lib/feedback/QATable.svelte
--rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.573622 peelml-0.0.1/peelml/client/src/lib/images/github.svg
--rw-r--r--   0        0        0      806 2023-07-10 23:20:55.573699 peelml-0.0.1/peelml/client/src/lib/images/logo.svg
--rw-r--r--   0        0        0     1892 2023-07-10 23:20:55.573768 peelml-0.0.1/peelml/client/src/lib/images/svelte-logo.svg
--rw-r--r--   0        0        0   360807 2023-07-10 23:20:55.576100 peelml-0.0.1/peelml/client/src/lib/images/svelte-welcome.png
--rw-r--r--   0        0        0   115470 2023-07-10 23:20:55.576232 peelml-0.0.1/peelml/client/src/lib/images/svelte-welcome.webp
--rw-r--r--   0        0        0      653 2023-07-10 23:20:55.576502 peelml-0.0.1/peelml/client/src/routes/+layout.svelte
--rw-r--r--   0        0        0      148 2023-07-10 23:20:55.576561 peelml-0.0.1/peelml/client/src/routes/+page.js
--rw-r--r--   0        0        0     1038 2023-07-10 23:20:55.576614 peelml-0.0.1/peelml/client/src/routes/+page.svelte
--rw-r--r--   0        0        0     1972 2023-07-10 23:20:55.576667 peelml-0.0.1/peelml/client/src/routes/Counter.svelte
--rw-r--r--   0        0        0     1152 2023-07-10 23:20:55.576719 peelml-0.0.1/peelml/client/src/routes/Header.svelte
--rw-r--r--   0        0        0     2163 2023-07-10 23:20:55.576775 peelml-0.0.1/peelml/client/src/routes/Sidemenu.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576854 peelml-0.0.1/peelml/client/src/routes/about/+page.js
--rw-r--r--   0        0        0      895 2023-07-10 23:20:55.576912 peelml-0.0.1/peelml/client/src/routes/about/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576992 peelml-0.0.1/peelml/client/src/routes/addbook/+page.js
--rw-r--r--   0        0        0      683 2023-07-10 23:20:55.577049 peelml-0.0.1/peelml/client/src/routes/addbook/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.577118 peelml-0.0.1/peelml/client/src/routes/chatbot/+page.js
--rw-r--r--   0        0        0     7547 2023-07-10 23:20:55.577257 peelml-0.0.1/peelml/client/src/routes/chatbot/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577313 peelml-0.0.1/peelml/client/src/routes/data/+page.js
--rw-r--r--   0        0        0     3645 2023-07-10 23:20:55.577504 peelml-0.0.1/peelml/client/src/routes/data/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577571 peelml-0.0.1/peelml/client/src/routes/embeddings/+page.js
--rw-r--r--   0        0        0      133 2023-07-10 23:20:55.577635 peelml-0.0.1/peelml/client/src/routes/embeddings/+page.svelte
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577709 peelml-0.0.1/peelml/client/src/routes/feedback/+page.js
--rw-r--r--   0        0        0     2923 2023-07-10 23:20:55.577847 peelml-0.0.1/peelml/client/src/routes/feedback/+page.svelte
--rw-r--r--   0        0        0      322 2023-07-10 23:20:55.577941 peelml-0.0.1/peelml/client/src/routes/index/+page.js
--rw-r--r--   0        0        0     1867 2023-07-10 23:20:55.578011 peelml-0.0.1/peelml/client/src/routes/index/+page.svelte
--rw-r--r--   0        0        0     6814 2023-07-10 23:20:55.578093 peelml-0.0.1/peelml/client/src/routes/normalize.css
--rw-r--r--   0        0        0     1061 2023-07-10 23:20:55.578154 peelml-0.0.1/peelml/client/src/routes/oldpage.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578436 peelml-0.0.1/peelml/client/src/routes/process/+page.js
--rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578510 peelml-0.0.1/peelml/client/src/routes/process/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578255 peelml-0.0.1/peelml/client/src/routes/process copy/+page.js
--rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578323 peelml-0.0.1/peelml/client/src/routes/process copy/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578620 peelml-0.0.1/peelml/client/src/routes/randomnumber/+page.js
--rw-r--r--   0        0        0      369 2023-07-10 23:20:55.578707 peelml-0.0.1/peelml/client/src/routes/randomnumber/+page.svelte
--rw-r--r--   0        0        0     9118 2023-07-10 23:20:55.578806 peelml-0.0.1/peelml/client/src/routes/styles.css
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578911 peelml-0.0.1/peelml/client/src/routes/upload/+page.js
--rw-r--r--   0        0        0     1621 2023-07-10 23:20:55.578988 peelml-0.0.1/peelml/client/src/routes/upload/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579092 peelml-0.0.1/peelml/client/src/routes/uploadOld/+page.js
--rw-r--r--   0        0        0      366 2023-07-10 23:20:55.579159 peelml-0.0.1/peelml/client/src/routes/uploadOld/+page.svelte
--rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579256 peelml-0.0.1/peelml/client/src/routes/uploadTest/+page.js
--rw-r--r--   0        0        0      241 2023-07-10 23:20:55.579319 peelml-0.0.1/peelml/client/src/routes/uploadTest/+page.svelte
--rw-r--r--   0        0        0     8569 2023-07-10 23:20:55.579487 peelml-0.0.1/peelml/client/src/store.js
--rw-r--r--   0        0        0     1641 2023-07-10 23:20:55.579561 peelml-0.0.1/peelml/client/src/utils.js
--rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.579678 peelml-0.0.1/peelml/client/static/favicon.png
--rw-r--r--   0        0        0       67 2023-07-10 23:20:55.579741 peelml-0.0.1/peelml/client/static/robots.txt
--rw-r--r--   0        0        0      144 2023-07-10 23:20:55.579808 peelml-0.0.1/peelml/client/svelte.config.js
--rw-r--r--   0        0        0      242 2023-07-10 23:20:55.579875 peelml-0.0.1/peelml/client/tailwind.config.cjs
--rw-r--r--   0        0        0      364 2023-07-10 23:20:55.579949 peelml-0.0.1/peelml/client/vite.config.js
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580015 peelml-0.0.1/peelml/duck/__init__.py
--rw-r--r--   0        0        0     1430 2023-07-10 23:20:55.580108 peelml-0.0.1/peelml/duck/answer_table.py
--rw-r--r--   0        0        0     3963 2023-07-10 23:20:55.580231 peelml-0.0.1/peelml/duck/preference_table.py
--rw-r--r--   0        0        0     1452 2023-07-10 23:20:55.580323 peelml-0.0.1/peelml/duck/question_table.py
--rw-r--r--   0        0        0     1895 2023-07-10 23:20:55.580436 peelml-0.0.1/peelml/duck/ranking_table.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580514 peelml-0.0.1/peelml/llm/__init__.py
--rw-r--r--   0        0        0      253 2023-07-10 23:20:55.580601 peelml-0.0.1/peelml/llm/abs_llm.py
--rw-r--r--   0        0        0      123 2023-07-10 23:20:55.580667 peelml-0.0.1/peelml/llm/constants.py
--rw-r--r--   0        0        0     1094 2023-07-10 23:20:55.580784 peelml-0.0.1/peelml/llm/embedding_factory.py
--rw-r--r--   0        0        0     1105 2023-07-10 23:20:55.580901 peelml-0.0.1/peelml/llm/llama_cpp.py
--rw-r--r--   0        0        0      895 2023-07-10 23:20:55.581016 peelml-0.0.1/peelml/llm/model_factory.py
--rw-r--r--   0        0        0      935 2023-07-10 23:20:55.581137 peelml-0.0.1/peelml/llm/openai.py
--rw-r--r--   0        0        0     1989 2023-07-10 23:20:55.581256 peelml-0.0.1/peelml/llm/sagemaker.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581335 peelml-0.0.1/peelml/model/__init__.py
--rw-r--r--   0        0        0     3298 2023-07-10 23:20:55.581431 peelml-0.0.1/peelml/model/sagemaker.py
--rw-r--r--   0        0        0    12745 2023-07-11 02:20:41.389261 peelml-0.0.1/peelml/server.py
--rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581661 peelml-0.0.1/peelml/vectordb/__init__.py
--rw-r--r--   0        0        0     3096 2023-07-10 23:20:55.581906 peelml-0.0.1/peelml/vectordb/abs_vectordb.py
--rw-r--r--   0        0        0     1520 2023-07-10 23:20:55.582037 peelml-0.0.1/peelml/vectordb/chroma.py
--rw-r--r--   0        0        0       72 2023-07-10 23:20:55.582106 peelml-0.0.1/peelml/vectordb/constants.py
--rw-r--r--   0        0        0      878 2023-07-10 23:20:55.582223 peelml-0.0.1/peelml/vectordb/vectordb_factory.py
--rw-r--r--   0        0        0      947 2023-07-11 02:28:10.794860 peelml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2823 1970-01-01 00:00:00.000000 peelml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-10 23:20:55.559708 peelml-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1471 2023-07-10 23:20:55.559872 peelml-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.559964 peelml-0.0.2/peelml/__init__.py
+-rw-r--r--   0        0        0     2720 2023-07-10 23:20:55.560126 peelml-0.0.2/peelml/cli.py
+-rw-r--r--   0        0        0      141 2023-07-10 23:20:55.560265 peelml-0.0.2/peelml/client/.gitignore
+-rw-r--r--   0        0        0       43 2023-07-10 23:20:55.560334 peelml-0.0.2/peelml/client/.npmrc
+-rw-r--r--   0        0        0      944 2023-07-10 23:20:55.560416 peelml-0.0.2/peelml/client/README.md
+-rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.560841 peelml-0.0.2/peelml/client/build/_app/immutable/assets/0.fd99616d.css
+-rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.560933 peelml-0.0.2/peelml/client/build/_app/immutable/assets/5.8f04d108.css
+-rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561002 peelml-0.0.2/peelml/client/build/_app/immutable/assets/6.98c9af80.css
+-rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561142 peelml-0.0.2/peelml/client/build/_app/immutable/assets/7.6f6c636b.css
+-rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561359 peelml-0.0.2/peelml/client/build/_app/immutable/assets/8.a14237ec.css
+-rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561420 peelml-0.0.2/peelml/client/build/_app/immutable/assets/9.6d9bf5de.css
+-rw-r--r--   0        0        0     9171 2023-07-10 23:20:55.561495 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css
+-rw-r--r--   0        0        0       76 2023-07-10 23:20:55.561552 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6d9bf5de.css
+-rw-r--r--   0        0        0      877 2023-07-10 23:20:55.561616 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css
+-rw-r--r--   0        0        0     2814 2023-07-10 23:20:55.561787 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.8f04d108.css
+-rw-r--r--   0        0        0     2276 2023-07-10 23:20:55.561861 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.98c9af80.css
+-rw-r--r--   0        0        0     4843 2023-07-10 23:20:55.561967 peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.a14237ec.css
+-rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.562041 peelml-0.0.2/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg
+-rw-r--r--   0        0        0      806 2023-07-10 23:20:55.562102 peelml-0.0.2/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg
+-rw-r--r--   0        0        0     3654 2023-07-11 04:05:51.112457 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js
+-rw-r--r--   0        0        0       27 2023-07-10 23:20:55.562274 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/environment.9aa685ef.js
+-rw-r--r--   0        0        0    14062 2023-07-11 04:05:51.112735 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.463cc238.js
+-rw-r--r--   0        0        0      825 2023-07-11 04:05:51.112841 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.562534 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/logo.be2f9f40.js
+-rw-r--r--   0        0        0     2458 2023-07-11 04:05:51.112970 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js
+-rw-r--r--   0        0        0     1985 2023-07-11 04:05:51.113089 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/store.4903bc61.js
+-rw-r--r--   0        0        0    20948 2023-07-10 23:20:55.563135 peelml-0.0.2/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js
+-rw-r--r--   0        0        0     8932 2023-07-11 04:05:51.113263 peelml-0.0.2/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js
+-rw-r--r--   0        0        0    24059 2023-07-11 04:05:51.113479 peelml-0.0.2/peelml/client/build/_app/immutable/entry/start.c3258ab5.js
+-rw-r--r--   0        0        0     6466 2023-07-11 04:05:51.113663 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js
+-rw-r--r--   0        0        0      981 2023-07-11 04:05:51.113784 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js
+-rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114000 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/10.758b2886.js
+-rw-r--r--   0        0        0     1707 2023-07-11 04:05:51.114067 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/11.758b2886.js
+-rw-r--r--   0        0        0     1322 2023-07-11 04:05:51.114128 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js
+-rw-r--r--   0        0        0      996 2023-07-11 04:05:51.114190 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js
+-rw-r--r--   0        0        0     1319 2023-07-11 04:05:51.114243 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/14.2e678f15.js
+-rw-r--r--   0        0        0     2707 2023-07-11 04:05:51.114504 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js
+-rw-r--r--   0        0        0     3447 2023-07-11 04:05:51.114577 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js
+-rw-r--r--   0        0        0     2771 2023-07-11 04:05:51.114638 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js
+-rw-r--r--   0        0        0     4787 2023-07-11 04:05:51.114706 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/4.177858de.js
+-rw-r--r--   0        0        0     6007 2023-07-11 04:05:51.114829 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js
+-rw-r--r--   0        0        0   102790 2023-07-11 04:05:51.115307 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js
+-rw-r--r--   0        0        0   692826 2023-07-11 04:05:51.117880 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/7.cba8d470.js
+-rw-r--r--   0        0        0    39619 2023-07-11 04:05:51.118162 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js
+-rw-r--r--   0        0        0      996 2023-07-11 04:05:51.118279 peelml-0.0.2/peelml/client/build/_app/immutable/nodes/9.21929747.js
+-rw-r--r--   0        0        0       27 2023-07-11 04:05:51.118441 peelml-0.0.2/peelml/client/build/_app/version.json
+-rw-r--r--   0        0        0     2358 2023-07-10 23:20:55.568686 peelml-0.0.2/peelml/client/build/about.html
+-rw-r--r--   0        0        0     1706 2023-07-10 23:20:55.568764 peelml-0.0.2/peelml/client/build/addbook.html
+-rw-r--r--   0        0        0     3338 2023-07-10 23:20:55.568846 peelml-0.0.2/peelml/client/build/chatbot.html
+-rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.569035 peelml-0.0.2/peelml/client/build/favicon.png
+-rw-r--r--   0        0        0     1033 2023-07-11 04:05:51.118659 peelml-0.0.2/peelml/client/build/index.html
+-rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569264 peelml-0.0.2/peelml/client/build/process copy.html
+-rw-r--r--   0        0        0     1800 2023-07-10 23:20:55.569330 peelml-0.0.2/peelml/client/build/process.html
+-rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569403 peelml-0.0.2/peelml/client/build/randomnumber.html
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.569463 peelml-0.0.2/peelml/client/build/robots.txt
+-rw-r--r--   0        0        0     1927 2023-07-10 23:20:55.569530 peelml-0.0.2/peelml/client/build/upload.html
+-rw-r--r--   0        0        0     1833 2023-07-10 23:20:55.569585 peelml-0.0.2/peelml/client/build/uploadOld.html
+-rw-r--r--   0        0        0     1876 2023-07-10 23:20:55.569651 peelml-0.0.2/peelml/client/build/uploadTest.html
+-rw-r--r--   0        0        0    66757 2023-07-10 23:20:55.570129 peelml-0.0.2/peelml/client/package-lock.json
+-rw-r--r--   0        0        0      793 2023-07-10 23:20:55.570207 peelml-0.0.2/peelml/client/package.json
+-rw-r--r--   0        0        0       80 2023-07-10 23:20:55.570261 peelml-0.0.2/peelml/client/postcss.config.js
+-rw-r--r--   0        0        0       58 2023-07-10 23:20:55.570341 peelml-0.0.2/peelml/client/src/app.css
+-rw-r--r--   0        0        0      329 2023-07-10 23:20:55.570398 peelml-0.0.2/peelml/client/src/app.html
+-rw-r--r--   0        0        0      251 2023-07-10 23:20:55.570539 peelml-0.0.2/peelml/client/src/lib/UI/Card.svelte
+-rw-r--r--   0        0        0      493 2023-07-10 23:20:55.570636 peelml-0.0.2/peelml/client/src/lib/components/AddBookForm.svelte
+-rw-r--r--   0        0        0     4214 2023-07-10 23:20:55.570732 peelml-0.0.2/peelml/client/src/lib/components/Charts/Bubble.svelte
+-rw-r--r--   0        0        0      420 2023-07-10 23:20:55.570998 peelml-0.0.2/peelml/client/src/lib/components/Charts/Tooltip.svelte
+-rw-r--r--   0        0        0     1219 2023-07-10 23:20:55.571096 peelml-0.0.2/peelml/client/src/lib/components/ChatMessage.svelte
+-rw-r--r--   0        0        0     7938 2023-07-10 23:20:55.571379 peelml-0.0.2/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte
+-rw-r--r--   0        0        0      381 2023-07-10 23:20:55.571560 peelml-0.0.2/peelml/client/src/lib/components/Embedding/data/projection.js
+-rw-r--r--   0        0        0      542 2023-07-10 23:20:55.571457 peelml-0.0.2/peelml/client/src/lib/components/Embedding/data.js
+-rw-r--r--   0        0        0      801 2023-07-10 23:20:55.571753 peelml-0.0.2/peelml/client/src/lib/components/Embedding/sequences.js
+-rw-r--r--   0        0        0     2075 2023-07-10 23:20:55.571820 peelml-0.0.2/peelml/client/src/lib/components/IndexFiles.svelte
+-rw-r--r--   0        0        0      235 2023-07-10 23:20:55.571882 peelml-0.0.2/peelml/client/src/lib/components/Modal.svelte
+-rw-r--r--   0        0        0     2219 2023-07-10 23:20:55.571944 peelml-0.0.2/peelml/client/src/lib/components/UploadFiles.svelte
+-rw-r--r--   0        0        0      935 2023-07-10 23:20:55.571999 peelml-0.0.2/peelml/client/src/lib/components/UploadTest.svelte
+-rw-r--r--   0        0        0     1945 2023-07-10 23:20:55.572100 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte
+-rw-r--r--   0        0        0     1909 2023-07-10 23:20:55.572162 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte
+-rw-r--r--   0        0        0     7958 2023-07-10 23:20:55.572255 peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/Table.svelte
+-rw-r--r--   0        0        0     3898 2023-07-10 23:20:55.572453 peelml-0.0.2/peelml/client/src/lib/feedback/ColumnChart.svelte
+-rw-r--r--   0        0        0     3888 2023-07-10 23:20:55.572621 peelml-0.0.2/peelml/client/src/lib/feedback/HistogramAnswer.svelte
+-rw-r--r--   0        0        0     3873 2023-07-10 23:20:55.572774 peelml-0.0.2/peelml/client/src/lib/feedback/HistogramQuestion.svelte
+-rw-r--r--   0        0        0     4967 2023-07-10 23:20:55.572931 peelml-0.0.2/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte
+-rw-r--r--   0        0        0     2685 2023-07-10 23:20:55.573089 peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte
+-rw-r--r--   0        0        0     2619 2023-07-10 23:20:55.573242 peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardPercentage.svelte
+-rw-r--r--   0        0        0     1381 2023-07-10 23:20:55.573380 peelml-0.0.2/peelml/client/src/lib/feedback/QACard.svelte
+-rw-r--r--   0        0        0      991 2023-07-10 23:20:55.573495 peelml-0.0.2/peelml/client/src/lib/feedback/QATable.svelte
+-rw-r--r--   0        0        0     1753 2023-07-10 23:20:55.573622 peelml-0.0.2/peelml/client/src/lib/images/github.svg
+-rw-r--r--   0        0        0      806 2023-07-10 23:20:55.573699 peelml-0.0.2/peelml/client/src/lib/images/logo.svg
+-rw-r--r--   0        0        0     1892 2023-07-10 23:20:55.573768 peelml-0.0.2/peelml/client/src/lib/images/svelte-logo.svg
+-rw-r--r--   0        0        0   360807 2023-07-10 23:20:55.576100 peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.png
+-rw-r--r--   0        0        0   115470 2023-07-10 23:20:55.576232 peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.webp
+-rw-r--r--   0        0        0      653 2023-07-10 23:20:55.576502 peelml-0.0.2/peelml/client/src/routes/+layout.svelte
+-rw-r--r--   0        0        0      148 2023-07-10 23:20:55.576561 peelml-0.0.2/peelml/client/src/routes/+page.js
+-rw-r--r--   0        0        0     1038 2023-07-10 23:20:55.576614 peelml-0.0.2/peelml/client/src/routes/+page.svelte
+-rw-r--r--   0        0        0     1972 2023-07-10 23:20:55.576667 peelml-0.0.2/peelml/client/src/routes/Counter.svelte
+-rw-r--r--   0        0        0     1152 2023-07-10 23:20:55.576719 peelml-0.0.2/peelml/client/src/routes/Header.svelte
+-rw-r--r--   0        0        0     2163 2023-07-10 23:20:55.576775 peelml-0.0.2/peelml/client/src/routes/Sidemenu.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576854 peelml-0.0.2/peelml/client/src/routes/about/+page.js
+-rw-r--r--   0        0        0      895 2023-07-10 23:20:55.576912 peelml-0.0.2/peelml/client/src/routes/about/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.576992 peelml-0.0.2/peelml/client/src/routes/addbook/+page.js
+-rw-r--r--   0        0        0      683 2023-07-10 23:20:55.577049 peelml-0.0.2/peelml/client/src/routes/addbook/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.577118 peelml-0.0.2/peelml/client/src/routes/chatbot/+page.js
+-rw-r--r--   0        0        0     8031 2023-07-11 04:05:51.118959 peelml-0.0.2/peelml/client/src/routes/chatbot/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577313 peelml-0.0.2/peelml/client/src/routes/data/+page.js
+-rw-r--r--   0        0        0     3645 2023-07-10 23:20:55.577504 peelml-0.0.2/peelml/client/src/routes/data/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577571 peelml-0.0.2/peelml/client/src/routes/embeddings/+page.js
+-rw-r--r--   0        0        0      133 2023-07-10 23:20:55.577635 peelml-0.0.2/peelml/client/src/routes/embeddings/+page.svelte
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.577709 peelml-0.0.2/peelml/client/src/routes/feedback/+page.js
+-rw-r--r--   0        0        0     2923 2023-07-10 23:20:55.577847 peelml-0.0.2/peelml/client/src/routes/feedback/+page.svelte
+-rw-r--r--   0        0        0      322 2023-07-10 23:20:55.577941 peelml-0.0.2/peelml/client/src/routes/index/+page.js
+-rw-r--r--   0        0        0     1867 2023-07-10 23:20:55.578011 peelml-0.0.2/peelml/client/src/routes/index/+page.svelte
+-rw-r--r--   0        0        0     6814 2023-07-10 23:20:55.578093 peelml-0.0.2/peelml/client/src/routes/normalize.css
+-rw-r--r--   0        0        0     1061 2023-07-10 23:20:55.578154 peelml-0.0.2/peelml/client/src/routes/oldpage.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578436 peelml-0.0.2/peelml/client/src/routes/process/+page.js
+-rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578510 peelml-0.0.2/peelml/client/src/routes/process/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578255 peelml-0.0.2/peelml/client/src/routes/process copy/+page.js
+-rw-r--r--   0        0        0     1729 2023-07-10 23:20:55.578323 peelml-0.0.2/peelml/client/src/routes/process copy/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578620 peelml-0.0.2/peelml/client/src/routes/randomnumber/+page.js
+-rw-r--r--   0        0        0      369 2023-07-10 23:20:55.578707 peelml-0.0.2/peelml/client/src/routes/randomnumber/+page.svelte
+-rw-r--r--   0        0        0     9118 2023-07-10 23:20:55.578806 peelml-0.0.2/peelml/client/src/routes/styles.css
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.578911 peelml-0.0.2/peelml/client/src/routes/upload/+page.js
+-rw-r--r--   0        0        0     1621 2023-07-10 23:20:55.578988 peelml-0.0.2/peelml/client/src/routes/upload/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579092 peelml-0.0.2/peelml/client/src/routes/uploadOld/+page.js
+-rw-r--r--   0        0        0      366 2023-07-10 23:20:55.579159 peelml-0.0.2/peelml/client/src/routes/uploadOld/+page.svelte
+-rw-r--r--   0        0        0      321 2023-07-10 23:20:55.579256 peelml-0.0.2/peelml/client/src/routes/uploadTest/+page.js
+-rw-r--r--   0        0        0      241 2023-07-10 23:20:55.579319 peelml-0.0.2/peelml/client/src/routes/uploadTest/+page.svelte
+-rw-r--r--   0        0        0     8569 2023-07-10 23:20:55.579487 peelml-0.0.2/peelml/client/src/store.js
+-rw-r--r--   0        0        0     1641 2023-07-10 23:20:55.579561 peelml-0.0.2/peelml/client/src/utils.js
+-rw-r--r--   0        0        0     1571 2023-07-10 23:20:55.579678 peelml-0.0.2/peelml/client/static/favicon.png
+-rw-r--r--   0        0        0       67 2023-07-10 23:20:55.579741 peelml-0.0.2/peelml/client/static/robots.txt
+-rw-r--r--   0        0        0      144 2023-07-10 23:20:55.579808 peelml-0.0.2/peelml/client/svelte.config.js
+-rw-r--r--   0        0        0      242 2023-07-10 23:20:55.579875 peelml-0.0.2/peelml/client/tailwind.config.cjs
+-rw-r--r--   0        0        0      364 2023-07-10 23:20:55.579949 peelml-0.0.2/peelml/client/vite.config.js
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580015 peelml-0.0.2/peelml/duck/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-10 23:20:55.580108 peelml-0.0.2/peelml/duck/answer_table.py
+-rw-r--r--   0        0        0     3963 2023-07-10 23:20:55.580231 peelml-0.0.2/peelml/duck/preference_table.py
+-rw-r--r--   0        0        0     1452 2023-07-10 23:20:55.580323 peelml-0.0.2/peelml/duck/question_table.py
+-rw-r--r--   0        0        0     1895 2023-07-10 23:20:55.580436 peelml-0.0.2/peelml/duck/ranking_table.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.580514 peelml-0.0.2/peelml/llm/__init__.py
+-rw-r--r--   0        0        0      253 2023-07-10 23:20:55.580601 peelml-0.0.2/peelml/llm/abs_llm.py
+-rw-r--r--   0        0        0      123 2023-07-10 23:20:55.580667 peelml-0.0.2/peelml/llm/constants.py
+-rw-r--r--   0        0        0     1094 2023-07-10 23:20:55.580784 peelml-0.0.2/peelml/llm/embedding_factory.py
+-rw-r--r--   0        0        0     1105 2023-07-10 23:20:55.580901 peelml-0.0.2/peelml/llm/llama_cpp.py
+-rw-r--r--   0        0        0      895 2023-07-10 23:20:55.581016 peelml-0.0.2/peelml/llm/model_factory.py
+-rw-r--r--   0        0        0      935 2023-07-10 23:20:55.581137 peelml-0.0.2/peelml/llm/openai.py
+-rw-r--r--   0        0        0     1989 2023-07-10 23:20:55.581256 peelml-0.0.2/peelml/llm/sagemaker.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581335 peelml-0.0.2/peelml/model/__init__.py
+-rw-r--r--   0        0        0     3298 2023-07-10 23:20:55.581431 peelml-0.0.2/peelml/model/sagemaker.py
+-rw-r--r--   0        0        0    12796 2023-07-11 04:11:21.634754 peelml-0.0.2/peelml/server.py
+-rw-r--r--   0        0        0        0 2023-07-10 23:20:55.581661 peelml-0.0.2/peelml/vectordb/__init__.py
+-rw-r--r--   0        0        0     3096 2023-07-10 23:20:55.581906 peelml-0.0.2/peelml/vectordb/abs_vectordb.py
+-rw-r--r--   0        0        0     1520 2023-07-10 23:20:55.582037 peelml-0.0.2/peelml/vectordb/chroma.py
+-rw-r--r--   0        0        0       72 2023-07-10 23:20:55.582106 peelml-0.0.2/peelml/vectordb/constants.py
+-rw-r--r--   0        0        0      878 2023-07-10 23:20:55.582223 peelml-0.0.2/peelml/vectordb/vectordb_factory.py
+-rw-r--r--   0        0        0      990 2023-07-11 04:25:56.182782 peelml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2896 1970-01-01 00:00:00.000000 peelml-0.0.2/PKG-INFO
```

### Comparing `peelml-0.0.1/LICENSE.txt` & `peelml-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/README.md` & `peelml-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/cli.py` & `peelml-0.0.2/peelml/cli.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/README.md` & `peelml-0.0.2/peelml/client/README.md`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/0.fd99616d.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/0.fd99616d.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/5.8f04d108.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/5.8f04d108.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/6.98c9af80.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/6.98c9af80.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/7.6f6c636b.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/7.6f6c636b.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/8.a14237ec.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/8.a14237ec.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_layout.fd99616d.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.6f6c636b.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.8f04d108.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.8f04d108.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.98c9af80.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.98c9af80.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/_page.a14237ec.css` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/_page.a14237ec.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/github.1ea8d62e.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg` & `peelml-0.0.2/peelml/client/build/_app/immutable/assets/logo.8b972bb6.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/UploadFiles.c03ead87.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/UploadFiles.20ed0f81.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -13,15 +13,15 @@
     E as L,
     n as B,
     F as M,
     R as O,
     G as D,
     q as k,
     r as P
-} from "./index.84b8b39e.js";
+} from "./index.463cc238.js";
 
 function N(m) {
     let e, n, a, r, s, t, l, o, v, p, F, b, h;
     return {
         c() {
             e = u("p"), n = k(`Files successfully indexed!
       `), a = u("br"), r = k(`
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/index.84b8b39e.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.463cc238.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -869,9 +869,9 @@
         }
     }
     $set(e) {
         this.$$set && !$t(e) && (this.$$.skip_bound = !0, this.$$set(e), this.$$.skip_bound = !1)
     }
 }
 export {
-    W as $, Yt as A, Jt as B, Ut as C, Ct as D, N as E, et as F, x as G, te as H, ne as I, ie as J, ee as K, Zt as L, ke as M, Ee as N, de as O, Ce as P, we as Q, fe as R, Fe as S, Me as T, qe as U, Re as V, se as W, oe as X, B as Y, Tt as Z, pe as _, le as a, ve as a0, ae as a1, Oe as a2, Vt as a3, Le as a4, Pe as a5, Ie as a6, ze as a7, ot as a8, he as a9, re as aa, $e as ab, xe as ac, bt as ad, xt as ae, vt as af, wt as ag, ce as b, ye as c, Ht as d, ue as e, De as f, gt as g, U as h, He as i, Ae as j, V as k, me as l, jt as m, _e as n, Se as o, be as p, Z as q, Ot as r, Qt as s, Te as t, ge as u, je as v, it as w, Ne as x, We as y, Be as z
+    W as $, Yt as A, Jt as B, Ut as C, Ct as D, N as E, et as F, x as G, te as H, ne as I, ie as J, ee as K, Zt as L, ke as M, Ee as N, de as O, Ce as P, we as Q, fe as R, Fe as S, Me as T, qe as U, Re as V, oe as W, B as X, se as Y, Tt as Z, pe as _, le as a, ve as a0, ae as a1, Oe as a2, Vt as a3, Le as a4, Pe as a5, Ie as a6, ze as a7, ot as a8, he as a9, re as aa, $e as ab, xe as ac, bt as ad, xt as ae, vt as af, wt as ag, ce as b, ye as c, Ht as d, ue as e, De as f, gt as g, U as h, He as i, Ae as j, V as k, me as l, jt as m, _e as n, Se as o, be as p, Z as q, Ot as r, Qt as s, Te as t, ge as u, je as v, it as w, Ne as x, We as y, Be as z
 };
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/index.eb24f9d9.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/index.6ec942b9.js`

 * *Files 24% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     E as f,
     a8 as y,
     G as m,
     s as q,
-    Y as w
-} from "./index.84b8b39e.js";
+    X as w
+} from "./index.463cc238.js";
 const o = [];
 
 function z(e, u) {
     return {
         subscribe: A(e, u).subscribe
     }
 }
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/singletons.96029e7d.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/singletons.752702b8.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 import {
     w as u
-} from "./index.eb24f9d9.js";
+} from "./index.6ec942b9.js";
 var _;
-const v = ((_ = globalThis.__sveltekit_1ul2cy) == null ? void 0 : _.base) ?? "";
+const v = ((_ = globalThis.__sveltekit_gtqpua) == null ? void 0 : _.base) ?? "";
 var g;
-const k = ((g = globalThis.__sveltekit_1ul2cy) == null ? void 0 : g.assets) ?? v,
-    m = "1689010576620",
-    A = "sveltekit:snapshot",
-    R = "sveltekit:scroll",
-    T = "sveltekit:index",
+const k = ((g = globalThis.__sveltekit_gtqpua) == null ? void 0 : g.assets) ?? v,
+    m = "1689048268230",
+    R = "sveltekit:snapshot",
+    T = "sveltekit:scroll",
+    y = "sveltekit:index",
     f = {
         tap: 1,
         hover: 2,
         viewport: 3,
         eager: 4,
         off: -1
     };
@@ -55,33 +55,33 @@
 
 function O(e, t) {
     let n;
     try {
         n = new URL(e instanceof SVGAElement ? e.href.baseVal : e.href, document.baseURI)
     } catch {}
     const o = e instanceof SVGAElement ? e.target.baseVal : e.target,
-        l = !n || !!o || y(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
-        r = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
+        r = !n || !!o || E(n, t) || (e.getAttribute("rel") || "").split(/\s+/).includes("external"),
+        l = (n == null ? void 0 : n.origin) === location.origin && e.hasAttribute("download");
     return {
         url: n,
-        external: l,
+        external: r,
         target: o,
-        download: r
+        download: l
     }
 }
 
 function U(e) {
     let t = null,
         n = null,
         o = null,
-        l = null,
         r = null,
+        l = null,
         a = null,
         s = e;
-    for (; s && s !== document.documentElement;) o === null && (o = c(s, "preload-code")), l === null && (l = c(s, "preload-data")), t === null && (t = c(s, "keepfocus")), n === null && (n = c(s, "noscroll")), r === null && (r = c(s, "reload")), a === null && (a = c(s, "replacestate")), s = h(s);
+    for (; s && s !== document.documentElement;) o === null && (o = c(s, "preload-code")), r === null && (r = c(s, "preload-data")), t === null && (t = c(s, "keepfocus")), n === null && (n = c(s, "noscroll")), l === null && (l = c(s, "reload")), a === null && (a = c(s, "replacestate")), s = h(s);
 
     function i(b) {
         switch (b) {
             case "":
             case "true":
                 return !0;
             case "off":
@@ -89,84 +89,84 @@
                 return !1;
             default:
                 return null
         }
     }
     return {
         preload_code: d[o ?? "off"],
-        preload_data: d[l ?? "off"],
+        preload_data: d[r ?? "off"],
         keep_focus: i(t),
         noscroll: i(n),
-        reload: i(r),
+        reload: i(l),
         replace_state: i(a)
     }
 }
 
 function p(e) {
     const t = u(e);
     let n = !0;
 
     function o() {
         n = !0, t.update(a => a)
     }
 
-    function l(a) {
+    function r(a) {
         n = !1, t.set(a)
     }
 
-    function r(a) {
+    function l(a) {
         let s;
         return t.subscribe(i => {
             (s === void 0 || n && i !== s) && a(s = i)
         })
     }
     return {
         notify: o,
-        set: l,
-        subscribe: r
+        set: r,
+        subscribe: l
     }
 }
 
 function w() {
     const {
         set: e,
         subscribe: t
     } = u(!1);
     let n;
     async function o() {
         clearTimeout(n);
         try {
-            const l = await fetch(`${k}/_app/version.json`, {
+            const r = await fetch(`${k}/_app/version.json`, {
                 headers: {
                     pragma: "no-cache",
                     "cache-control": "no-cache"
                 }
             });
-            if (!l.ok) return !1;
-            const a = (await l.json()).version !== m;
+            if (!r.ok) return !1;
+            const a = (await r.json()).version !== m;
             return a && (e(!0), clearTimeout(n)), a
         } catch {
             return !1
         }
     }
     return {
         subscribe: t,
         check: o
     }
 }
 
-function y(e, t) {
+function E(e, t) {
     return e.origin !== location.origin || !e.pathname.startsWith(t)
 }
 
 function L(e) {
     e.client
 }
 const N = {
     url: p({}),
     page: p({}),
     navigating: u(null),
     updated: w()
 };
 export {
-    T as I, f as P, R as S, A as a, O as b, U as c, N as d, v as e, x as f, I as g, L as h, y as i, S as s
+    y as I, f as P, T as S, R as a, O as b, U as c, N as d, v as e, x as f, I as g, L as h, E as i, S as s
 };
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/store.322467ea.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/store.4903bc61.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,17 @@
 import {
     w as f,
     d as E
-} from "./index.eb24f9d9.js";
+} from "./index.6ec942b9.js";
 import {
     ad as w,
     ae as T,
     af as D,
     ag as W
-} from "./index.84b8b39e.js";
+} from "./index.463cc238.js";
 
 function g(t) {
     return Object.prototype.toString.call(t) === "[object Date]"
 }
 
 function u(t, e) {
     if (t === e || t !== t) return () => t;
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/chunks/utils.12623cfb.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/entry/app.ec7afc1f.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/entry/app.6ffb33b8.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -23,15 +23,15 @@
     v as O,
     w as A,
     x as v,
     y as k,
     z as D,
     A as R,
     B as P
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const X = "modulepreload",
     Y = function(_) {
         return "/" + _
     },
     I = {},
     m = function(e, n, s) {
         if (!n || n.length === 0) return e();
@@ -357,15 +357,15 @@
             components: 0,
             form: 2,
             data_0: 3,
             data_1: 4
         })
     }
 }
-const re = [() => m(() => import("../nodes/0.b9c3e59d.js"), ["_app/immutable/nodes/0.b9c3e59d.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/logo.be2f9f40.js", "_app/immutable/assets/0.fd99616d.css"]), () => m(() => import("../nodes/1.77aa025a.js"), ["_app/immutable/nodes/1.77aa025a.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/singletons.96029e7d.js", "_app/immutable/chunks/index.eb24f9d9.js"]), () => m(() => import("../nodes/2.75c7eb74.js"), ["_app/immutable/nodes/2.75c7eb74.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/3.f27f0658.js"), ["_app/immutable/nodes/3.f27f0658.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/4.e26998a1.js"), ["_app/immutable/nodes/4.e26998a1.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/5.627b2dc7.js"), ["_app/immutable/nodes/5.627b2dc7.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/logo.be2f9f40.js", "_app/immutable/chunks/store.322467ea.js", "_app/immutable/chunks/index.eb24f9d9.js", "_app/immutable/assets/5.8f04d108.css"]), () => m(() => import("../nodes/6.e941ef4d.js"), ["_app/immutable/nodes/6.e941ef4d.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/utils.12623cfb.js", "_app/immutable/chunks/store.322467ea.js", "_app/immutable/chunks/index.eb24f9d9.js", "_app/immutable/assets/6.98c9af80.css"]), () => m(() => import("../nodes/7.6a37f45a.js"), ["_app/immutable/nodes/7.6a37f45a.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/store.322467ea.js", "_app/immutable/chunks/index.eb24f9d9.js", "_app/immutable/assets/7.6f6c636b.css"]), () => m(() => import("../nodes/8.59c844c2.js"), ["_app/immutable/nodes/8.59c844c2.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/store.322467ea.js", "_app/immutable/chunks/index.eb24f9d9.js", "_app/immutable/chunks/utils.12623cfb.js", "_app/immutable/assets/8.a14237ec.css"]), () => m(() => import("../nodes/9.4133202d.js"), ["_app/immutable/nodes/9.4133202d.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/UploadFiles.c03ead87.js", "_app/immutable/assets/9.6d9bf5de.css"]), () => m(() => import("../nodes/10.7909aaae.js"), ["_app/immutable/nodes/10.7909aaae.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/11.7909aaae.js"), ["_app/immutable/nodes/11.7909aaae.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/12.512086c8.js"), ["_app/immutable/nodes/12.512086c8.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/13.c0f6c67f.js"), ["_app/immutable/nodes/13.c0f6c67f.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/chunks/UploadFiles.c03ead87.js", "_app/immutable/assets/9.6d9bf5de.css"]), () => m(() => import("../nodes/14.59fcfc6f.js"), ["_app/immutable/nodes/14.59fcfc6f.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js"]), () => m(() => import("../nodes/15.916fb8a4.js"), ["_app/immutable/nodes/15.916fb8a4.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.84b8b39e.js", "_app/immutable/assets/9.6d9bf5de.css"])],
+const re = [() => m(() => import("../nodes/0.d404e6c9.js"), ["_app/immutable/nodes/0.d404e6c9.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/logo.be2f9f40.js", "_app/immutable/assets/0.fd99616d.css"]), () => m(() => import("../nodes/1.9c2d3365.js"), ["_app/immutable/nodes/1.9c2d3365.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/singletons.752702b8.js", "_app/immutable/chunks/index.6ec942b9.js"]), () => m(() => import("../nodes/2.e901a5fc.js"), ["_app/immutable/nodes/2.e901a5fc.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/3.ccd2af49.js"), ["_app/immutable/nodes/3.ccd2af49.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/4.177858de.js"), ["_app/immutable/nodes/4.177858de.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/5.ed0a9b7b.js"), ["_app/immutable/nodes/5.ed0a9b7b.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/logo.be2f9f40.js", "_app/immutable/chunks/store.4903bc61.js", "_app/immutable/chunks/index.6ec942b9.js", "_app/immutable/assets/5.8f04d108.css"]), () => m(() => import("../nodes/6.3aea1c37.js"), ["_app/immutable/nodes/6.3aea1c37.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/utils.12623cfb.js", "_app/immutable/chunks/store.4903bc61.js", "_app/immutable/chunks/index.6ec942b9.js", "_app/immutable/assets/6.98c9af80.css"]), () => m(() => import("../nodes/7.cba8d470.js"), ["_app/immutable/nodes/7.cba8d470.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/store.4903bc61.js", "_app/immutable/chunks/index.6ec942b9.js", "_app/immutable/assets/7.6f6c636b.css"]), () => m(() => import("../nodes/8.2e3ebaaf.js"), ["_app/immutable/nodes/8.2e3ebaaf.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/store.4903bc61.js", "_app/immutable/chunks/index.6ec942b9.js", "_app/immutable/chunks/utils.12623cfb.js", "_app/immutable/assets/8.a14237ec.css"]), () => m(() => import("../nodes/9.21929747.js"), ["_app/immutable/nodes/9.21929747.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/UploadFiles.20ed0f81.js", "_app/immutable/assets/9.6d9bf5de.css"]), () => m(() => import("../nodes/10.758b2886.js"), ["_app/immutable/nodes/10.758b2886.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/11.758b2886.js"), ["_app/immutable/nodes/11.758b2886.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/12.acf3ba70.js"), ["_app/immutable/nodes/12.acf3ba70.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/13.a5b47bbf.js"), ["_app/immutable/nodes/13.a5b47bbf.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/chunks/UploadFiles.20ed0f81.js", "_app/immutable/assets/9.6d9bf5de.css"]), () => m(() => import("../nodes/14.2e678f15.js"), ["_app/immutable/nodes/14.2e678f15.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js"]), () => m(() => import("../nodes/15.0c5d77af.js"), ["_app/immutable/nodes/15.0c5d77af.js", "_app/immutable/chunks/environment.9aa685ef.js", "_app/immutable/chunks/index.463cc238.js", "_app/immutable/assets/9.6d9bf5de.css"])],
     oe = [],
     _e = {
         "/": [2],
         "/about": [3],
         "/addbook": [4],
         "/chatbot": [5],
         "/data": [6],
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/entry/start.dd2cf025.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/entry/start.c3258ab5.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,26 +1,26 @@
 import {
     o as De,
     t as ye
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     S as He,
     a as Je,
     I as V,
     g as Ce,
     f as Ve,
     b as we,
     c as le,
     s as ee,
     i as _e,
     d as M,
     e as K,
     P as qe,
     h as We
-} from "../chunks/singletons.96029e7d.js";
+} from "../chunks/singletons.752702b8.js";
 
 function Xe(n, o) {
     return n === "/" || o === "ignore" ? n : o === "never" ? n.endsWith("/") ? n.slice(0, -1) : n : o === "always" && !n.endsWith("/") ? n + "/" : n
 }
 
 function Ze(n) {
     return n.split("%25").map(decodeURI).join("%25")
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/0.b9c3e59d.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/0.d404e6c9.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     A as _e,
     I as ve,
     J as pe,
     K as ke,
     g as P,
     d as Q,
     B as ue
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     l as be
 } from "../chunks/logo.be2f9f40.js";
 const $e = "/_app/immutable/assets/github.1ea8d62e.svg";
 
 function ye(o) {
     let e, a, d, r, l, b, k, p, _, u, c, $, y, V, g, L, E, C, q, R, M, t, f, S, N, B, I, z, Y;
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/1.77aa025a.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/1.9c2d3365.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -11,18 +11,18 @@
     h as u,
     c as y,
     b as m,
     D as v,
     u as E,
     E as $,
     L as C
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     d as D
-} from "../chunks/singletons.96029e7d.js";
+} from "../chunks/singletons.752702b8.js";
 const H = () => {
         const s = D;
         return {
             page: {
                 subscribe: s.page.subscribe
             },
             navigating: {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/10.7909aaae.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/10.758b2886.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     b as M,
     D as l,
     Q as D,
     F as E,
     R as N,
     E as P,
     G as q
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const A = Q,
     C = !0,
     B = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: A,
         prerender: C
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/11.7909aaae.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/11.758b2886.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     b as M,
     D as l,
     Q as D,
     F as E,
     R as N,
     E as P,
     G as q
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const A = Q,
     C = !0,
     B = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: A,
         prerender: C
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/12.512086c8.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/12.acf3ba70.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
     r as p,
     n as M,
     D as u,
     b as f,
     F as R,
     u as Y,
     E as O
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const g = j,
     w = !0,
     F = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: g,
         prerender: w
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/13.c0f6c67f.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/13.a5b47bbf.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -14,18 +14,18 @@
     E as v,
     g as l,
     d as i,
     y as $,
     z as y,
     A as b,
     B as S
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     U as x
-} from "../chunks/UploadFiles.c03ead87.js";
+} from "../chunks/UploadFiles.20ed0f81.js";
 const k = c,
     j = !0,
     q = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: k,
         prerender: j
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/14.59fcfc6f.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/14.2e678f15.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
     r as p,
     n as M,
     D as u,
     b as f,
     F as R,
     u as Y,
     E as O
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const g = j,
     w = !0,
     F = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: g,
         prerender: w
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/15.916fb8a4.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/15.0c5d77af.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -24,15 +24,15 @@
     G as A,
     y as G,
     z as H,
     A as Q,
     g as K,
     d as L,
     B as W
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 
 function J(a) {
     let e;
     return {
         c() {
             e = _("div"), this.h()
         },
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/2.75c7eb74.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/2.e901a5fc.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -17,15 +17,15 @@
     E as N,
     y as O,
     z as V,
     A as j,
     g as q,
     d as W,
     B as Y
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const Q = !0,
     at = Object.freeze(Object.defineProperty({
         __proto__: null,
         prerender: Q
     }, Symbol.toStringTag, {
         value: "Module"
     }));
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/3.f27f0658.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/3.ccd2af49.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -16,15 +16,15 @@
     r as s,
     n as L,
     D as e,
     b as U,
     F as te,
     u as ne,
     E as V
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const ae = Q,
     oe = !0,
     de = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: ae,
         prerender: oe
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/4.e26998a1.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/4.177858de.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -37,15 +37,15 @@
     y as L,
     z as W,
     A as X,
     u as U,
     U as ce,
     B as Y,
     V as de
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 const _e = Z,
     he = !0,
     Ie = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: _e,
         prerender: he
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/5.627b2dc7.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/5.ed0a9b7b.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,212 +1,212 @@
 import {
     d as oe
 } from "../chunks/environment.9aa685ef.js";
 import {
     S as ne,
     i as re,
     s as ce,
-    k as g,
+    k as m,
     a as C,
     q as U,
     l as b,
     m as w,
     h as y,
     c as L,
     r as q,
-    n as u,
+    n as i,
     b as se,
     D as s,
-    Q as $,
+    Q as Z,
     F as R,
     U as ie,
-    u as W,
-    E as x,
+    u as K,
+    E as $,
     G as ae,
-    L as ue,
-    o as de,
-    W as K,
+    L as de,
+    o as ue,
     C as he,
-    X as fe,
-    Y as pe,
-    V as _e
-} from "../chunks/index.84b8b39e.js";
+    W as fe,
+    X as pe,
+    V as _e,
+    Y as x
+} from "../chunks/index.463cc238.js";
 import {
     l as ve
 } from "../chunks/logo.be2f9f40.js";
 import {
     c as G
-} from "../chunks/store.322467ea.js";
-const me = oe,
-    ge = !0,
+} from "../chunks/store.4903bc61.js";
+const ge = oe,
+    me = !0,
     Oe = Object.freeze(Object.defineProperty({
         __proto__: null,
-        csr: me,
-        prerender: ge
+        csr: ge,
+        prerender: me
     }, Symbol.toStringTag, {
         value: "Module"
     }));
 
 function ee(r, e, t) {
     const a = r.slice();
     return a[12] = e[t], a[14] = t, a
 }
 
 function te(r, e) {
-    let t, a, c, v, h, f, n, T, p, j = e[12].question + "",
-        S, I, E, i, d = e[12].answer + "",
-        _, O, m, V, l, o, k, P, D, F, J;
+    let t, a, d, g, f, p, n, T, _, j = e[12].question + "",
+        S, I, E, c, h = e[12].answer + "",
+        v, O, u, V, l, o, k, P, D, F, J;
 
     function Q() {
         return e[7](e[14])
     }
 
     function le() {
         return e[8](e[14])
     }
     return {
         key: r,
         first: null,
         c() {
-            t = g("div"), a = g("div"), c = g("div"), v = g("img"), f = C(), n = g("div"), T = g("p"), p = U("Q: "), S = U(j), I = C(), E = g("p"), i = U("A: "), _ = U(d), O = C(), m = g("button"), V = U("👍"), l = C(), o = g("button"), k = U("👎"), P = C(), this.h()
+            t = m("div"), a = m("div"), d = m("div"), g = m("img"), p = C(), n = m("div"), T = m("p"), _ = U("Q: "), S = U(j), I = C(), E = m("p"), c = U("A: "), v = U(h), O = C(), u = m("button"), V = U("👍"), l = C(), o = m("button"), k = U("👎"), P = C(), this.h()
         },
         l(B) {
             t = b(B, "DIV", {
                 class: !0
             });
             var N = w(t);
             a = b(N, "DIV", {
                 class: !0
             });
             var A = w(a);
-            c = b(A, "DIV", {
+            d = b(A, "DIV", {
                 class: !0
             });
-            var X = w(c);
-            v = b(X, "IMG", {
+            var W = w(d);
+            g = b(W, "IMG", {
                 src: !0,
                 alt: !0,
                 class: !0
-            }), X.forEach(y), f = L(A), n = b(A, "DIV", {
+            }), W.forEach(y), p = L(A), n = b(A, "DIV", {
                 class: !0
             });
             var M = w(n);
             T = b(M, "P", {
                 class: !0
             });
             var z = w(T);
-            p = q(z, "Q: "), S = q(z, j), z.forEach(y), I = L(M), E = b(M, "P", {
+            _ = q(z, "Q: "), S = q(z, j), z.forEach(y), I = L(M), E = b(M, "P", {
                 class: !0
             });
             var H = w(E);
-            i = q(H, "A: "), _ = q(H, d), H.forEach(y), O = L(M), m = b(M, "BUTTON", {
+            c = q(H, "A: "), v = q(H, h), H.forEach(y), O = L(M), u = b(M, "BUTTON", {
                 class: !0
             });
-            var Y = w(m);
-            V = q(Y, "👍"), Y.forEach(y), l = L(M), o = b(M, "BUTTON", {
+            var X = w(u);
+            V = q(X, "👍"), X.forEach(y), l = L(M), o = b(M, "BUTTON", {
                 class: !0
             });
-            var Z = w(o);
-            k = q(Z, "👎"), Z.forEach(y), M.forEach(y), A.forEach(y), P = L(N), N.forEach(y), this.h()
+            var Y = w(o);
+            k = q(Y, "👎"), Y.forEach(y), M.forEach(y), A.forEach(y), P = L(N), N.forEach(y), this.h()
         },
         h() {
-            he(v.src, h = ve) || u(v, "src", h), u(v, "alt", "SvelteKit"), u(v, "class", "svelte-ji0dhf"), u(c, "class", "avatar svelte-ji0dhf"), u(T, "class", "svelte-ji0dhf"), u(E, "class", "svelte-ji0dhf"), u(m, "class", "small-button thumbs-up svelte-ji0dhf"), u(o, "class", "small-button thumbs-down svelte-ji0dhf"), u(n, "class", "message-content svelte-ji0dhf"), u(a, "class", "chat-message-center svelte-ji0dhf"), u(t, "class", "chat-message svelte-ji0dhf"), this.first = t
+            he(g.src, f = ve) || i(g, "src", f), i(g, "alt", "SvelteKit"), i(g, "class", "svelte-ji0dhf"), i(d, "class", "avatar svelte-ji0dhf"), i(T, "class", "svelte-ji0dhf"), i(E, "class", "svelte-ji0dhf"), i(u, "class", "small-button thumbs-up svelte-ji0dhf"), i(o, "class", "small-button thumbs-down svelte-ji0dhf"), i(n, "class", "message-content svelte-ji0dhf"), i(a, "class", "chat-message-center svelte-ji0dhf"), i(t, "class", "chat-message svelte-ji0dhf"), this.first = t
         },
         m(B, N) {
-            se(B, t, N), s(t, a), s(a, c), s(c, v), s(a, f), s(a, n), s(n, T), s(T, p), s(T, S), s(n, I), s(n, E), s(E, i), s(E, _), s(n, O), s(n, m), s(m, V), s(n, l), s(n, o), s(o, k), s(t, P), F || (J = [R(m, "click", Q), R(o, "click", le), fe(D = je.call(null, t, e[14] === e[0].length - 1))], F = !0)
+            se(B, t, N), s(t, a), s(a, d), s(d, g), s(a, p), s(a, n), s(n, T), s(T, _), s(T, S), s(n, I), s(n, E), s(E, c), s(E, v), s(n, O), s(n, u), s(u, V), s(n, l), s(n, o), s(o, k), s(t, P), F || (J = [R(u, "click", Q), R(o, "click", le), fe(D = je.call(null, t, e[14] === e[0].length - 1))], F = !0)
         },
         p(B, N) {
-            e = B, N & 1 && j !== (j = e[12].question + "") && W(S, j), N & 1 && d !== (d = e[12].answer + "") && W(_, d), D && pe(D.update) && N & 1 && D.update.call(null, e[14] === e[0].length - 1)
+            e = B, N & 1 && j !== (j = e[12].question + "") && K(S, j), N & 1 && h !== (h = e[12].answer + "") && K(v, h), D && pe(D.update) && N & 1 && D.update.call(null, e[14] === e[0].length - 1)
         },
         d(B) {
             B && y(t), F = !1, ae(J)
         }
     }
 }
 
 function be(r) {
     let e, t, a = [],
-        c = new Map,
-        v, h, f, n, T, p, j = (r[2] ? r[3] : "Send") + "",
-        S, I, E, i, d, _, O, m = r[0];
+        d = new Map,
+        g, f, p, n, T, _, j = (r[2] ? r[3] : "Send") + "",
+        S, I, E, c, h, v, O, u = r[0];
     const V = l => l[14];
-    for (let l = 0; l < m.length; l += 1) {
-        let o = ee(r, m, l),
+    for (let l = 0; l < u.length; l += 1) {
+        let o = ee(r, u, l),
             k = V(o);
-        c.set(k, a[l] = te(k, o))
+        d.set(k, a[l] = te(k, o))
     }
     return {
         c() {
-            e = g("section"), t = g("div");
+            e = m("section"), t = m("div");
             for (let l = 0; l < a.length; l += 1) a[l].c();
-            v = C(), h = g("div"), f = g("form"), n = g("input"), T = C(), p = g("button"), S = U(j), E = C(), i = g("p"), d = U("Note - may produce inaccurate information."), this.h()
+            g = C(), f = m("div"), p = m("form"), n = m("input"), T = C(), _ = m("button"), S = U(j), E = C(), c = m("p"), h = U("Note - may produce inaccurate information."), this.h()
         },
         l(l) {
             e = b(l, "SECTION", {
                 class: !0
             });
             var o = w(e);
             t = b(o, "DIV", {
                 class: !0
             });
             var k = w(t);
             for (let Q = 0; Q < a.length; Q += 1) a[Q].l(k);
-            k.forEach(y), v = L(o), h = b(o, "DIV", {
+            k.forEach(y), g = L(o), f = b(o, "DIV", {
                 class: !0
             });
-            var P = w(h);
-            f = b(P, "FORM", {
+            var P = w(f);
+            p = b(P, "FORM", {
                 class: !0
             });
-            var D = w(f);
+            var D = w(p);
             n = b(D, "INPUT", {
                 rows: !0,
                 class: !0,
                 placeholder: !0
-            }), T = L(D), p = b(D, "BUTTON", {
+            }), T = L(D), _ = b(D, "BUTTON", {
                 class: !0,
                 type: !0
             });
-            var F = w(p);
-            S = q(F, j), F.forEach(y), D.forEach(y), E = L(P), i = b(P, "P", {
+            var F = w(_);
+            S = q(F, j), F.forEach(y), D.forEach(y), E = L(P), c = b(P, "P", {
                 class: !0
             });
-            var J = w(i);
-            d = q(J, "Note - may produce inaccurate information."), J.forEach(y), P.forEach(y), o.forEach(y), this.h()
+            var J = w(c);
+            h = q(J, "Note - may produce inaccurate information."), J.forEach(y), P.forEach(y), o.forEach(y), this.h()
         },
         h() {
-            u(t, "class", "chat-log svelte-ji0dhf"), u(n, "rows", "1"), u(n, "class", "chat-input-textarea svelte-ji0dhf"), u(n, "placeholder", "Type Message Here"), u(p, "class", I = "btnyousend " + (r[1] === "" ? "" : "active") + " svelte-ji0dhf"), u(p, "type", "submit"), u(f, "class", "chat-input-form svelte-ji0dhf"), u(i, "class", "message svelte-ji0dhf"), u(h, "class", "chat-input-holder svelte-ji0dhf"), u(e, "class", "chatbox svelte-ji0dhf")
+            i(t, "class", "chat-log svelte-ji0dhf"), i(n, "rows", "1"), i(n, "class", "chat-input-textarea svelte-ji0dhf"), i(n, "placeholder", "Type Message Here"), i(_, "class", I = "btnyousend " + (r[1] === "" ? "" : "active") + " svelte-ji0dhf"), i(_, "type", "submit"), i(p, "class", "chat-input-form svelte-ji0dhf"), i(c, "class", "message svelte-ji0dhf"), i(f, "class", "chat-input-holder svelte-ji0dhf"), i(e, "class", "chatbox svelte-ji0dhf")
         },
         m(l, o) {
             se(l, e, o), s(e, t);
             for (let k = 0; k < a.length; k += 1) a[k] && a[k].m(t, null);
-            s(e, v), s(e, h), s(h, f), s(f, n), $(n, r[1]), s(f, T), s(f, p), s(p, S), s(h, E), s(h, i), s(i, d), _ || (O = [R(n, "input", r[9]), R(f, "submit", r[4])], _ = !0)
+            s(e, g), s(e, f), s(f, p), s(p, n), Z(n, r[1]), s(p, T), s(p, _), s(_, S), s(f, E), s(f, c), s(c, h), v || (O = [R(n, "input", r[9]), R(p, "submit", r[4])], v = !0)
         },
         p(l, [o]) {
-            o & 33 && (m = l[0], a = ie(a, o, V, 1, l, m, c, t, _e, te, null, ee)), o & 2 && n.value !== l[1] && $(n, l[1]), o & 12 && j !== (j = (l[2] ? l[3] : "Send") + "") && W(S, j), o & 2 && I !== (I = "btnyousend " + (l[1] === "" ? "" : "active") + " svelte-ji0dhf") && u(p, "class", I)
+            o & 33 && (u = l[0], a = ie(a, o, V, 1, l, u, d, t, _e, te, null, ee)), o & 2 && n.value !== l[1] && Z(n, l[1]), o & 12 && j !== (j = (l[2] ? l[3] : "Send") + "") && K(S, j), o & 2 && I !== (I = "btnyousend " + (l[1] === "" ? "" : "active") + " svelte-ji0dhf") && i(_, "class", I)
         },
-        i: x,
-        o: x,
+        i: $,
+        o: $,
         d(l) {
             l && y(e);
             for (let o = 0; o < a.length; o += 1) a[o].d();
-            _ = !1, ae(O)
+            v = !1, ae(O)
         }
     }
 }
 async function ye(r) {
     console.log("INSERT"), console.log("entry", r);
     const e = await fetch("http://127.0.0.1:5000/preference_table/insert", {
         method: "POST",
         headers: {
             "Content-Type": "application/json"
         },
         body: JSON.stringify(r)
     });
-    if (e.ok) console.log("ok! data inserted", e), print("entry", r);
+    if (e.ok) console.log("ok! data inserted", e), console.log("entry", r);
     else {
         const t = await e.text();
         alert(t)
     }
 }
 
 function je(r) {
@@ -214,85 +214,86 @@
         r.scrollIntoView({
             behavior: "smooth"
         })
     }, 0)
 }
 
 function ke(r, e, t) {
-    let a, c;
-    ue(r, G, i => t(0, c = i));
-    let v = "",
-        h = "",
-        f = !1;
-    de(() => {
-        console.log("hey"), n()
+    let a, d;
+    de(r, G, c => t(0, d = c));
+    let g = "",
+        f = "",
+        p = !1;
+    ue(() => {
+        console.log("here we go"), d.length < 1 && n()
     });
     async function n() {
-        const _ = (await (await fetch("http://127.0.0.1:5000/preference_table/get")).json()).preference_result;
-        K(G, c = [..._], c), console.log("db", _)
+        console.log("fetching data from db");
+        const v = (await (await fetch("http://127.0.0.1:5000/preference_table/get")).json()).preference_result;
+        x(G, d = [...v], d), console.log("db", v)
     }
-    const T = async i => {
-        i.preventDefault(), v = h, t(1, h = ""), t(2, f = !0);
-        let d = {
-            id: c.length + 1,
-            question: v,
+    const T = async c => {
+        c.preventDefault(), g = f, t(1, f = ""), t(2, p = !0);
+        let h = {
+            id: d.length + 1,
+            question: g,
             answer: "Loading...",
             vote: "na"
         };
-        K(G, c = [...c, d], c);
-        const _ = await fetch(`http://127.0.0.1:5000/objects/retrieve/${v}`, {
+        console.log("adding to log here"), x(G, d = [...d, h], d);
+        const v = await fetch(`http://127.0.0.1:5000/objects/retrieve/${g}`, {
             method: "POST",
             headers: {
                 "Content-Type": "application/json"
             },
             body: JSON.stringify({
-                prompt: v
+                prompt: g
             })
         });
-        if (_.ok) {
-            const O = await _.json();
-            d.answer = O.answer, K(G, c[c.length - 1] = d, c), ye(d)
+        if (v.ok) {
+            const O = await v.json();
+            h.answer = O.answer, G.update(u => (u[u.length - 1] = h, u)), ye(h)
         } else {
-            const O = await _.text();
+            const O = await v.text();
             alert(O)
         }
-        t(2, f = !1)
+        t(2, p = !1)
     };
-    let p = 0;
+    let _ = 0;
     setInterval(() => {
-        t(6, p = (p + 1) % 4)
+        t(6, _ = (_ + 1) % 4)
     }, 200);
-    async function j(i, d) {
-        const _ = c[d];
-        _.vote = i;
-        const m = await fetch("http://127.0.0.1:5000/preference_table/update", {
+    async function j(c, h) {
+        const v = d[h];
+        v.vote = c;
+        const u = await fetch("http://127.0.0.1:5000/preference_table/update", {
             method: "POST",
             headers: {
                 "Content-Type": "application/json"
             },
             body: JSON.stringify({
-                id: d,
-                vote: i
+                id: h,
+                vote: c
             })
         });
-        if (m.ok) console.log("update worked!", m);
+        if (u.ok) console.log("update worked!", u);
         else {
-            const V = await m.text();
+            const V = await u.text();
             alert(V)
         }
     }
-    const S = i => j("good", i),
-        I = i => j("bad", i);
+    const S = c => j("good", c),
+        I = c => j("bad", c);
 
     function E() {
-        h = this.value, t(1, h)
+        f = this.value, t(1, f)
     }
     return r.$$.update = () => {
-        r.$$.dirty & 64 && t(3, a = ".".repeat(p).padEnd(3)), r.$$.dirty & 1 && console.log("chat updated!", c)
-    }, [c, h, f, a, T, j, p, S, I, E]
+        r.$$.dirty & 64 && t(3, a = ".".repeat(_).padEnd(3)), r.$$.dirty & 1 && console.log("chat updated!", d)
+    }, [d, f, p, a, T, j, _, S, I, E]
 }
 class Ie extends ne {
     constructor(e) {
         super(), re(this, e, ke, be, ce, {})
     }
 }
 export {
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/6.e941ef4d.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/6.3aea1c37.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -12,18 +12,18 @@
     $ as ht,
     b as se,
     D as C,
     a0 as sr,
     g as O,
     v as he,
     f as _e,
-    d as W,
+    d as X,
     a1 as Ye,
     L as Qe,
-    q as X,
+    q as W,
     r as K,
     F as ue,
     u as Ne,
     a2 as Ue,
     G as bn,
     a3 as ur,
     y as Se,
@@ -38,34 +38,34 @@
     c as j,
     N as He,
     U as fr,
     a7 as gr,
     a8 as dr,
     x as Ze,
     o as pr,
-    W as zt
-} from "../chunks/index.84b8b39e.js";
+    Y as zt
+} from "../chunks/index.463cc238.js";
 import {
     a as Nt,
     n as hr,
     m as Ot,
     l as st,
     e as Lt,
     f as _t,
     s as qe
 } from "../chunks/utils.12623cfb.js";
 import {
     u as et,
     p as Gt
-} from "../chunks/store.322467ea.js";
+} from "../chunks/store.4903bc61.js";
 import {
     r as Tt,
     w as mt,
     d as _r
-} from "../chunks/index.eb24f9d9.js";
+} from "../chunks/index.6ec942b9.js";
 const Ql = Object.freeze(Object.defineProperty({
     __proto__: null
 }, Symbol.toStringTag, {
     value: "Module"
 }));
 
 function mr(e = Nt) {
@@ -565,15 +565,15 @@
 
 function Tr() {
     Dn(), ++Fe;
     for (var e = tt, t; e;)(t = Re - e._time) >= 0 && e._call.call(void 0, t), e = e._next;
     --Fe
 }
 
-function Wt() {
+function Xt() {
     Re = (nt = Oe.now()) + lt, Fe = ke = 0;
     try {
         Tr()
     } finally {
         Fe = 0, Ur(), Re = 0
     }
 }
@@ -589,38 +589,38 @@
     ze = e, wt(r)
 }
 
 function wt(e) {
     if (!Fe) {
         ke && (ke = clearTimeout(ke));
         var t = e - Re;
-        t > 24 ? (e < 1 / 0 && (ke = setTimeout(Wt, e - Oe.now() - lt)), Ve && (Ve = clearInterval(Ve))) : (Ve || (nt = Oe.now(), Ve = setInterval(Br, En)), Fe = 1, Pn(Wt))
+        t > 24 ? (e < 1 / 0 && (ke = setTimeout(Xt, e - Oe.now() - lt)), Ve && (Ve = clearInterval(Ve))) : (Ve || (nt = Oe.now(), Ve = setInterval(Br, En)), Fe = 1, Pn(Xt))
     }
 }
 const qr = 1664525,
     jr = 1013904223,
-    Xt = 4294967296;
+    Wt = 4294967296;
 
-function Wr() {
+function Xr() {
     let e = 1;
-    return () => (e = (qr * e + jr) % Xt) / Xt
+    return () => (e = (qr * e + jr) % Wt) / Wt
 }
-var Xr = 10,
+var Wr = 10,
     Kr = Math.PI * (3 - Math.sqrt(5));
 
 function Yr(e) {
     var t, n = 1,
         r = .001,
         o = 1 - Math.pow(r, 1 / 300),
         i = 0,
         l = .6,
         u = new Map,
         s = Hn(g),
         a = Vn("tick", "end"),
-        c = Wr();
+        c = Xr();
     e == null && (e = []);
 
     function g() {
         d(), a.call("tick", t), n < r && (s.stop(), a.call("end", t))
     }
 
     function d(p) {
@@ -633,15 +633,15 @@
                 }), m = 0; m < _; ++m) w = e[m], w.fx == null ? w.x += w.vx *= l : (w.x = w.fx, w.vx = 0), w.fy == null ? w.y += w.vy *= l : (w.y = w.fy, w.vy = 0);
         return t
     }
 
     function f() {
         for (var p = 0, m = e.length, _; p < m; ++p) {
             if (_ = e[p], _.index = p, _.fx != null && (_.x = _.fx), _.fy != null && (_.y = _.fy), isNaN(_.x) || isNaN(_.y)) {
-                var w = Xr * Math.sqrt(.5 + p),
+                var w = Wr * Math.sqrt(.5 + p),
                     S = p * Kr;
                 _.x = w * Math.cos(S), _.y = w * Math.sin(S)
             }(isNaN(_.vx) || isNaN(_.vy)) && (_.vx = _.vy = 0)
         }
     }
 
     function h(p) {
@@ -1090,19 +1090,19 @@
 function jo(e, t, n) {
     return function() {
         var r = t.apply(this, arguments);
         r == null ? this.style.removeProperty(e) : this.style.setProperty(e, r, n)
     }
 }
 
-function Wo(e, t, n) {
-    return arguments.length > 1 ? this.each((t == null ? Uo : typeof t == "function" ? jo : qo)(e, t, n ?? "")) : Xo(this.node(), e)
+function Xo(e, t, n) {
+    return arguments.length > 1 ? this.each((t == null ? Uo : typeof t == "function" ? jo : qo)(e, t, n ?? "")) : Wo(this.node(), e)
 }
 
-function Xo(e, t) {
+function Wo(e, t) {
     return e.style.getPropertyValue(t) || Tn(e).getComputedStyle(e, null).getPropertyValue(t)
 }
 
 function Ko(e) {
     return function() {
         delete this[e]
     }
@@ -1353,41 +1353,41 @@
         }
         return
     }
     for (u = t ? Fi : Ai, o = 0; o < i; ++o) this.each(u(r[o], t, n));
     return this
 }
 
-function Wn(e, t, n) {
+function Xn(e, t, n) {
     var r = Tn(e),
         o = r.CustomEvent;
     typeof o == "function" ? o = new o(t, n) : (o = r.document.createEvent("Event"), n ? (o.initEvent(t, n.bubbles, n.cancelable), o.detail = n.detail) : o.initEvent(t, !1, !1)), e.dispatchEvent(o)
 }
 
 function Mi(e, t) {
     return function() {
-        return Wn(this, e, t)
+        return Xn(this, e, t)
     }
 }
 
 function Ii(e, t) {
     return function() {
-        return Wn(this, e, t.apply(this, arguments))
+        return Xn(this, e, t.apply(this, arguments))
     }
 }
 
 function Vi(e, t) {
     return this.each((typeof t == "function" ? Ii : Mi)(e, t))
 }
 
 function* Ei() {
     for (var e = this._groups, t = 0, n = e.length; t < n; ++t)
         for (var r = e[t], o = 0, i = r.length, l; o < i; ++o)(l = r[o]) && (yield l)
 }
-var Xn = [null];
+var Wn = [null];
 
 function ne(e, t) {
     this._groups = e, this._parents = t
 }
 
 function Pi() {
     return this
@@ -1410,15 +1410,15 @@
     call: Vo,
     nodes: Eo,
     node: Po,
     size: Do,
     empty: Ho,
     each: ko,
     attr: Bo,
-    style: Wo,
+    style: Xo,
     property: Jo,
     classed: ni,
     text: li,
     html: ci,
     raise: gi,
     lower: pi,
     append: hi,
@@ -1432,33 +1432,33 @@
 };
 
 function Di(e) {
     return typeof e == "string" ? new ne([
         [document.querySelector(e)]
     ], [document.documentElement]) : new ne([
         [e]
-    ], Xn)
+    ], Wn)
 }
 
 function ut(e) {
-    return typeof e == "string" ? new ne([document.querySelectorAll(e)], [document.documentElement]) : new ne([On(e)], Xn)
+    return typeof e == "string" ? new ne([document.querySelectorAll(e)], [document.documentElement]) : new ne([On(e)], Wn)
 }
 
 function Yt(e, t, n) {
     const r = e.slice();
     return r[20] = t[n], r[22] = n, r
 }
 
 function Qt(e) {
     let t, n, r, o, i, l = e[20].file + "",
         u, s, a = _t(e[20].size) + "",
         c, g, d, f, h, p, m, _;
     return {
         c() {
-            t = Pe("g"), n = Pe("circle"), i = Pe("text"), u = X(l), s = Pe("tspan"), c = X(a), this.h()
+            t = Pe("g"), n = Pe("circle"), i = Pe("text"), u = W(l), s = Pe("tspan"), c = W(a), this.h()
         },
         l(w) {
             t = De(w, "g", {
                 class: !0,
                 style: !0,
                 role: !0
             });
@@ -1516,15 +1516,15 @@
     }
 }
 
 function Hi(e) {
     let t, n, r, o, i = e[2],
         l = [];
     for (let s = 0; s < i.length; s += 1) l[s] = Qt(Yt(e, i, s));
-    const u = s => W(l[s], 1, 1, () => {
+    const u = s => X(l[s], 1, 1, () => {
         l[s] = null
     });
     return {
         c() {
             t = E("div"), n = Pe("svg");
             for (let s = 0; s < l.length; s += 1) l[s].c();
             this.h()
@@ -1567,15 +1567,15 @@
             if (!o) {
                 for (let a = 0; a < i.length; a += 1) O(l[a]);
                 o = !0
             }
         },
         o(s) {
             l = l.filter(Boolean);
-            for (let a = 0; a < l.length; a += 1) W(l[a]);
+            for (let a = 0; a < l.length; a += 1) X(l[a]);
             o = !1
         },
         d(s) {
             s && $(t), Ye(l, s), r()
         }
     }
 }
@@ -1973,44 +1973,44 @@
         return m = m + w, h.colSpan = p, h.rowSpan = m, {
             colSpan: p,
             rowSpan: m
         }
     });
     return g((o = (i = s[0]) == null ? void 0 : i.headers) != null ? o : []), s
 }
-const We = {
+const Xe = {
         size: 150,
         minSize: 20,
         maxSize: Number.MAX_SAFE_INTEGER
     },
     at = () => ({
         startOffset: null,
         startSize: null,
         deltaOffset: null,
         deltaPercentage: null,
         isResizingColumn: !1,
         columnSizingStart: []
     }),
     Ti = {
-        getDefaultColumnDef: () => We,
+        getDefaultColumnDef: () => Xe,
         getInitialState: e => ({
             columnSizing: {},
             columnSizingInfo: at(),
             ...e
         }),
         getDefaultOptions: e => ({
             columnResizeMode: "onEnd",
             onColumnSizingChange: le("columnSizing", e),
             onColumnSizingInfoChange: le("columnSizingInfo", e)
         }),
         createColumn: (e, t) => ({
             getSize: () => {
                 var n, r, o;
                 const i = t.getState().columnSizing[e.id];
-                return Math.min(Math.max((n = e.columnDef.minSize) != null ? n : We.minSize, (r = i ?? e.columnDef.size) != null ? r : We.size), (o = e.columnDef.maxSize) != null ? o : We.maxSize)
+                return Math.min(Math.max((n = e.columnDef.minSize) != null ? n : Xe.minSize, (r = i ?? e.columnDef.size) != null ? r : Xe.size), (o = e.columnDef.maxSize) != null ? o : Xe.maxSize)
             },
             getStart: n => {
                 const r = n ? n === "left" ? t.getLeftVisibleLeafColumns() : t.getRightVisibleLeafColumns() : t.getVisibleLeafColumns(),
                     o = r.findIndex(i => i.id === e.id);
                 if (o > 0) {
                     const i = r[o - 1];
                     return i.getStart(n) + i.getSize()
@@ -2144,31 +2144,31 @@
             },
             getRightTotalSize: () => {
                 var t, n;
                 return (t = (n = e.getRightHeaderGroups()[0]) == null ? void 0 : n.headers.reduce((r, o) => r + o.getSize(), 0)) != null ? t : 0
             }
         })
     };
-let Xe = null;
+let We = null;
 
 function Bi() {
-    if (typeof Xe == "boolean") return Xe;
+    if (typeof We == "boolean") return We;
     let e = !1;
     try {
         const t = {
                 get passive() {
                     return e = !0, !1
                 }
             },
             n = () => {};
         window.addEventListener("test", n, t), window.removeEventListener("test", n)
     } catch {
         e = !1
     }
-    return Xe = e, Xe
+    return We = e, We
 }
 
 function ct(e) {
     return e.type === "touchstart"
 }
 const Ui = {
         getInitialState: e => ({
@@ -2462,22 +2462,22 @@
 function Zt(e, t, n) {
     return (e && e.autoRemove ? e.autoRemove(t, n) : !1) || typeof t > "u" || typeof t == "string" && !t
 }
 const ji = (e, t, n) => n.reduce((r, o) => {
         const i = o.getValue(e);
         return r + (typeof i == "number" ? i : 0)
     }, 0),
-    Wi = (e, t, n) => {
+    Xi = (e, t, n) => {
         let r;
         return n.forEach(o => {
             const i = o.getValue(e);
             i != null && (r > i || r === void 0 && i >= i) && (r = i)
         }), r
     },
-    Xi = (e, t, n) => {
+    Wi = (e, t, n) => {
         let r;
         return n.forEach(o => {
             const i = o.getValue(e);
             i != null && (r < i || r === void 0 && i >= i) && (r = i)
         }), r
     },
     Ki = (e, t, n) => {
@@ -2505,16 +2505,16 @@
         return n.length % 2 !== 0 ? o[r] : (o[r - 1] + o[r]) / 2
     },
     Ji = (e, t) => Array.from(new Set(t.map(n => n.getValue(e))).values()),
     Zi = (e, t) => new Set(t.map(n => n.getValue(e))).size,
     el = (e, t) => t.length,
     ft = {
         sum: ji,
-        min: Wi,
-        max: Xi,
+        min: Xi,
+        max: Wi,
         extent: Ki,
         mean: Yi,
         median: Qi,
         unique: Ji,
         uniqueCount: Zi,
         count: el
     },
@@ -3836,15 +3836,15 @@
  *
  * @license MIT
  */
 function Cl(e) {
     let t;
     return {
         c() {
-            t = X(e[0])
+            t = W(e[0])
         },
         l(n) {
             t = K(n, e[0])
         },
         m(n, r) {
             se(n, t, r)
         },
@@ -3893,15 +3893,15 @@
             Ce(r, i, l), o = !0
         },
         p: Je,
         i(i) {
             o || (O(r.$$.fragment, i), o = !0)
         },
         o(i) {
-            W(r.$$.fragment, i), o = !1
+            X(r.$$.fragment, i), o = !1
         },
         d(i) {
             ye(r, i)
         }
     }
 }
 
@@ -4551,15 +4551,15 @@
     var c = it(e[26].column.columnDef.header, e[26].getContext());
 
     function g(d) {
         return {}
     }
     return c && (n = Ze(c, g())), {
         c() {
-            t = E("button"), n && Se(n.$$.fragment), r = q(), o = E("span"), l = X(i), this.h()
+            t = E("button"), n && Se(n.$$.fragment), r = q(), o = E("span"), l = W(i), this.h()
         },
         l(d) {
             t = P(d, "BUTTON", {});
             var f = I(t);
             n && Te(n.$$.fragment, f), r = j(f), o = P(f, "SPAN", {});
             var h = I(o);
             l = K(h, i), h.forEach($), f.forEach($), this.h()
@@ -4571,26 +4571,26 @@
             se(d, t, f), n && Ce(n, t, null), C(t, r), C(t, o), C(o, l), u = !0, s || (a = ue(t, "click", e[26].column.getToggleSortingHandler()), s = !0)
         },
         p(d, f) {
             if (e = d, c !== (c = it(e[26].column.columnDef.header, e[26].getContext()))) {
                 if (n) {
                     he();
                     const h = n;
-                    W(h.$$.fragment, 1, 0, () => {
+                    X(h.$$.fragment, 1, 0, () => {
                         ye(h, 1)
                     }), _e()
                 }
                 c ? (n = Ze(c, g()), Se(n.$$.fragment), O(n.$$.fragment, 1), Ce(n, t, r)) : n = null
             }
         },
         i(d) {
             u || (n && O(n.$$.fragment, d), u = !0)
         },
         o(d) {
-            n && W(n.$$.fragment, d), u = !1
+            n && X(n.$$.fragment, d), u = !1
         },
         d(d) {
             d && $(t), n && ye(n), s = !1, a()
         }
     }
 }
 
@@ -4617,27 +4617,27 @@
         p(o, i) {
             o[26].isPlaceholder || r.p(o, i)
         },
         i(o) {
             n || (O(r), n = !0)
         },
         o(o) {
-            W(r), n = !1
+            X(r), n = !1
         },
         d(o) {
             o && $(t), r && r.d()
         }
     }
 }
 
 function wn(e) {
     let t, n, r, o = e[23].headers,
         i = [];
     for (let u = 0; u < o.length; u += 1) i[u] = vn(mn(e, o, u));
-    const l = u => W(i[u], 1, 1, () => {
+    const l = u => X(i[u], 1, 1, () => {
         i[u] = null
     });
     return {
         c() {
             t = E("tr");
             for (let u = 0; u < i.length; u += 1) i[u].c();
             n = q()
@@ -4669,15 +4669,15 @@
             if (!r) {
                 for (let s = 0; s < o.length; s += 1) O(i[s]);
                 r = !0
             }
         },
         o(u) {
             i = i.filter(Boolean);
-            for (let s = 0; s < i.length; s += 1) W(i[s]);
+            for (let s = 0; s < i.length; s += 1) X(i[s]);
             r = !1
         },
         d(u) {
             u && $(t), Ye(i, u)
         }
     }
 }
@@ -4709,26 +4709,26 @@
             se(u, n, s), r && Ce(r, n, null), o = !0
         },
         p(u, s) {
             if (t = u, s & 2 && i !== (i = it(t[20].column.columnDef.cell, t[20].getContext()))) {
                 if (r) {
                     he();
                     const a = r;
-                    W(a.$$.fragment, 1, 0, () => {
+                    X(a.$$.fragment, 1, 0, () => {
                         ye(a, 1)
                     }), _e()
                 }
                 i ? (r = Ze(i, l()), Se(r.$$.fragment), O(r.$$.fragment, 1), Ce(r, n, null)) : r = null
             }
         },
         i(u) {
             o || (r && O(r.$$.fragment, u), o = !0)
         },
         o(u) {
-            r && W(r.$$.fragment, u), o = !1
+            r && X(r.$$.fragment, u), o = !1
         },
         d(u) {
             u && $(n), r && ye(r)
         }
     }
 }
 
@@ -4770,15 +4770,15 @@
         i(s) {
             if (!i) {
                 for (let a = 0; a < l.length; a += 1) O(n[a]);
                 i = !0
             }
         },
         o(s) {
-            for (let a = 0; a < n.length; a += 1) W(n[a]);
+            for (let a = 0; a < n.length; a += 1) X(n[a]);
             i = !1
         },
         d(s) {
             s && $(t);
             for (let a = 0; a < n.length; a += 1) n[a].d()
         }
     }
@@ -4789,30 +4789,30 @@
         f, h, p, m, _, w, S, R, v, x, V, D = " ",
         U, T, Y = " ",
         Q, J, G = e[1].getPageCount() + "",
         B, L, k, re = ">",
         $e, ve, z, be, Me, ce = e[5],
         H = [];
     for (let b = 0; b < ce.length; b += 1) H[b] = wn(_n(e, ce, b));
-    const Be = b => W(H[b], 1, 1, () => {
+    const Be = b => X(H[b], 1, 1, () => {
         H[b] = null
     });
     let oe = e[1].getRowModel().rows,
         N = [];
     for (let b = 0; b < oe.length; b += 1) N[b] = Cn(pn(e, oe, b));
-    const lr = b => W(N[b], 1, 1, () => {
+    const lr = b => X(N[b], 1, 1, () => {
         N[b] = null
     });
     return {
         c() {
             t = E("div"), n = E("input"), r = q(), o = E("div"), i = E("table"), l = E("thead");
             for (let b = 0; b < H.length; b += 1) H[b].c();
             u = q(), s = E("tbody");
             for (let b = 0; b < N.length; b += 1) N[b].c();
-            a = q(), c = E("div"), g = E("button"), f = X(d), p = q(), m = E("span"), _ = X("Page"), w = q(), S = E("input"), x = q(), V = E("span"), U = X(D), T = X("of"), Q = X(Y), J = q(), B = X(G), L = q(), k = E("button"), $e = X(re), this.h()
+            a = q(), c = E("div"), g = E("button"), f = W(d), p = q(), m = E("span"), _ = W("Page"), w = q(), S = E("input"), x = q(), V = E("span"), U = W(D), T = W("of"), Q = W(Y), J = q(), B = W(G), L = q(), k = E("button"), $e = W(re), this.h()
         },
         l(b) {
             t = P(b, "DIV", {});
             var M = I(t);
             n = P(M, "INPUT", {
                 type: !0,
                 class: !0,
@@ -4895,17 +4895,17 @@
                 for (let M = 0; M < ce.length; M += 1) O(H[M]);
                 for (let M = 0; M < oe.length; M += 1) O(N[M]);
                 z = !0
             }
         },
         o(b) {
             H = H.filter(Boolean);
-            for (let M = 0; M < H.length; M += 1) W(H[M]);
+            for (let M = 0; M < H.length; M += 1) X(H[M]);
             N = N.filter(Boolean);
-            for (let M = 0; M < N.length; M += 1) W(N[M]);
+            for (let M = 0; M < N.length; M += 1) X(N[M]);
             z = !1
         },
         d(b) {
             b && $(t), Ye(H, b), Ye(N, b), be = !1, bn(Me)
         }
     }
 }
@@ -5030,15 +5030,15 @@
     }
 }
 
 function yn(e) {
     let t, n;
     return {
         c() {
-            t = E("p"), n = X(e[3])
+            t = E("p"), n = W(e[3])
         },
         l(r) {
             t = P(r, "P", {});
             var o = I(t);
             n = K(o, e[3]), o.forEach($)
         },
         m(r, o) {
@@ -5053,15 +5053,15 @@
     }
 }
 
 function Rn(e) {
     let t, n;
     return {
         c() {
-            t = E("p"), n = X("Data Successfully indexed!")
+            t = E("p"), n = W("Data Successfully indexed!")
         },
         l(r) {
             t = P(r, "P", {});
             var o = I(t);
             n = K(o, "Data Successfully indexed!"), o.forEach($)
         },
         m(r, o) {
@@ -5085,30 +5085,30 @@
         m(r, o) {
             Ce(t, r, o), n = !0
         },
         i(r) {
             n || (O(t.$$.fragment, r), n = !0)
         },
         o(r) {
-            W(t.$$.fragment, r), n = !1
+            X(t.$$.fragment, r), n = !1
         },
         d(r) {
             ye(t, r)
         }
     }
 }
 
 function ql(e) {
     let t, n, r, o, i, l, u, s, a, c, g, d, f, h, p, m, _, w, S, R, v, x, V, D, U, T, Y, Q, J, G = e[2] && !e[1] && yn(e),
         B = e[1] && Rn();
     U = new zi({});
     let L = e[0] && $n();
     return {
         c() {
-            t = E("div"), n = E("div"), r = E("div"), o = E("div"), i = E("h4"), l = X("Upload Data"), u = q(), s = E("br"), a = q(), c = E("form"), g = E("input"), d = q(), G && G.c(), f = q(), B && B.c(), h = q(), p = E("p"), m = X("These are the files your model will use as context."), _ = q(), w = E("p"), S = X("Currently "), R = E("strong"), v = X("pdf"), x = X(", txt, and md are supported."), V = q(), D = E("div"), Se(U.$$.fragment), T = q(), L && L.c(), this.h()
+            t = E("div"), n = E("div"), r = E("div"), o = E("div"), i = E("h4"), l = W("Upload Data"), u = q(), s = E("br"), a = q(), c = E("form"), g = E("input"), d = q(), G && G.c(), f = q(), B && B.c(), h = q(), p = E("p"), m = W("These are the files your model will use as context."), _ = q(), w = E("p"), S = W("Currently "), R = E("strong"), v = W("pdf"), x = W(", txt, and md are supported."), V = q(), D = E("div"), Se(U.$$.fragment), T = q(), L && L.c(), this.h()
         },
         l(k) {
             t = P(k, "DIV", {
                 class: !0
             });
             var re = I(t);
             n = P(re, "DIV", {
@@ -5144,23 +5144,23 @@
         h() {
             y(g, "type", "file"), g.multiple = !0, y(o, "class", "upload-box svelte-m0f0ym"), y(r, "class", "upload-container svelte-m0f0ym"), y(n, "class", "file-container svelte-m0f0ym"), y(D, "class", "charts-container svelte-m0f0ym"), y(t, "class", "data-grid svelte-m0f0ym")
         },
         m(k, re) {
             se(k, t, re), C(t, n), C(n, r), C(r, o), C(o, i), C(i, l), C(o, u), C(o, s), C(o, a), C(o, c), C(c, g), C(o, d), G && G.m(o, null), C(o, f), B && B.m(o, null), C(o, h), C(o, p), C(p, m), C(o, _), C(o, w), C(w, S), C(w, R), C(R, v), C(w, x), C(t, V), C(t, D), Ce(U, D, null), C(D, T), L && L.m(D, null), Y = !0, Q || (J = ue(g, "change", e[4]), Q = !0)
         },
         p(k, [re]) {
-            k[2] && !k[1] ? G ? G.p(k, re) : (G = yn(k), G.c(), G.m(o, f)) : G && (G.d(1), G = null), k[1] ? B || (B = Rn(), B.c(), B.m(o, h)) : B && (B.d(1), B = null), k[0] ? L ? re & 1 && O(L, 1) : (L = $n(), L.c(), O(L, 1), L.m(D, null)) : L && (he(), W(L, 1, 1, () => {
+            k[2] && !k[1] ? G ? G.p(k, re) : (G = yn(k), G.c(), G.m(o, f)) : G && (G.d(1), G = null), k[1] ? B || (B = Rn(), B.c(), B.m(o, h)) : B && (B.d(1), B = null), k[0] ? L ? re & 1 && O(L, 1) : (L = $n(), L.c(), O(L, 1), L.m(D, null)) : L && (he(), X(L, 1, 1, () => {
                 L = null
             }), _e())
         },
         i(k) {
             Y || (O(U.$$.fragment, k), O(L), Y = !0)
         },
         o(k) {
-            W(U.$$.fragment, k), W(L), Y = !1
+            X(U.$$.fragment, k), X(L), Y = !1
         },
         d(k) {
             k && $(t), G && G.d(), B && B.d(), ye(U), L && L.d(), Q = !1, J()
         }
     }
 }
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/7.6a37f45a.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/7.cba8d470.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -24,18 +24,18 @@
     o as ep,
     y as tp,
     z as np,
     A as ip,
     g as rp,
     d as sp,
     B as op
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     p as ap
-} from "../chunks/store.322467ea.js";
+} from "../chunks/store.4903bc61.js";
 const mb = Object.freeze(Object.defineProperty({
         __proto__: null
     }, Symbol.toStringTag, {
         value: "Module"
     })),
     eh = {
         labelNames: ["txt2.txt", "pdf2.txt"],
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/8.59c844c2.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/8.2e3ebaaf.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -10,45 +10,45 @@
     m as q,
     r as C,
     h as y,
     c as R,
     _ as F,
     n as r,
     $ as le,
-    b as W,
+    b as L,
     D as k,
     a0 as ye,
     E as $,
     a1 as ee,
     L as G,
     F as ze,
     G as mt,
-    W as ht,
-    u as K,
-    g as U,
+    Y as ht,
+    u as J,
+    g as K,
     v as pt,
     f as bt,
     d as x,
     y as ce,
     z as _e,
     A as de,
     a2 as Pe,
     B as ge,
     e as ve,
     p as me,
     ab as Ae,
     ac as ft
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     f as te,
     s as kt,
     q as Oe,
     c as we,
     t as ct
-} from "../chunks/store.322467ea.js";
+} from "../chunks/store.4903bc61.js";
 import {
     t as Se,
     e as De,
     b as yt,
     c as wt,
     i as _t,
     d as Ee,
@@ -341,20 +341,20 @@
     }, n.order = function(s) {
         return arguments.length ? (l = s == null ? Ne : typeof s == "function" ? s : Ve(Array.from(s)), n) : l
     }, n.offset = function(s) {
         return arguments.length ? (t = s ?? je, n) : t
     }, n
 }
 
-function We(e, l, t) {
+function Le(e, l, t) {
     const a = e.slice();
     return a[20] = l[t], a[22] = t, a
 }
 
-function Le(e, l, t) {
+function We(e, l, t) {
     const a = e.slice();
     a[23] = l[t];
     const n = a[3][0][a[20].key];
     return a[24] = n, a
 }
 
 function Be(e) {
@@ -398,29 +398,29 @@
             var T = q(w);
             V = C(T, f), T.forEach(y), H = R(A), A.forEach(y), this.h()
         },
         h() {
             r(l, "class", t = "horizontal-bar-rect " + (e[4] === e[22] ? "selected" : "unselected") + " svelte-175eim1"), r(l, "y", a = e[7](e[23].data.xVal)), r(l, "x", n = e[6](e[23][0])), r(l, "stroke", "var(--black)"), r(l, "width", s = e[6](e[23][1]) - e[6](e[23][0])), r(l, "fill", i = e[9](e[20].key)), r(l, "opacity", u = e[4] === "all" || e[4] === e[22] ? "1" : "0.25"), r(l, "height", o = e[7].bandwidth()), r(h, "class", "line svelte-175eim1"), r(h, "x1", d = e[6](e[23][0])), r(h, "x2", b = e[6](e[23][0])), r(h, "y1", p = e[7](e[23].data.xVal) - pe), r(h, "y2", c = e[7].bandwidth() + e[7](e[23].data.xVal) + pe), r(h, "stroke", "black"), r(w, "x", z = (e[6](e[23][0]) + e[6](e[23][1])) / 2), r(w, "dy", "16"), r(w, "text-anchor", "middle"), r(g, "class", "horizontal-bar-text svelte-175eim1"), r(g, "y", O = e[7](e[23].data.xVal) + e[7].bandwidth() / 2), r(g, "x", E = (e[6](e[23][0]) + e[6](e[23][1])) / 2), r(g, "opacity", M = e[4] === "all" || e[4] === e[22] ? "1" : "0.25"), r(g, "text-anchor", "middle")
         },
         m(m, A) {
-            W(m, l, A), W(m, h, A), W(m, g, A), k(g, _), k(g, w), k(w, V), k(g, H)
+            L(m, l, A), L(m, h, A), L(m, g, A), k(g, _), k(g, w), k(w, V), k(g, H)
         },
         p(m, A) {
-            A & 16 && t !== (t = "horizontal-bar-rect " + (m[4] === m[22] ? "selected" : "unselected") + " svelte-175eim1") && r(l, "class", t), A & 160 && a !== (a = m[7](m[23].data.xVal)) && r(l, "y", a), A & 96 && n !== (n = m[6](m[23][0])) && r(l, "x", n), A & 96 && s !== (s = m[6](m[23][1]) - m[6](m[23][0])) && r(l, "width", s), A & 32 && i !== (i = m[9](m[20].key)) && r(l, "fill", i), A & 16 && u !== (u = m[4] === "all" || m[4] === m[22] ? "1" : "0.25") && r(l, "opacity", u), A & 128 && o !== (o = m[7].bandwidth()) && r(l, "height", o), A & 96 && d !== (d = m[6](m[23][0])) && r(h, "x1", d), A & 96 && b !== (b = m[6](m[23][0])) && r(h, "x2", b), A & 160 && p !== (p = m[7](m[23].data.xVal) - pe) && r(h, "y1", p), A & 160 && c !== (c = m[7].bandwidth() + m[7](m[23].data.xVal) + pe) && r(h, "y2", c), A & 32 && v !== (v = m[20].key + "") && K(_, v), A & 40 && f !== (f = m[10](m[24] / m[11]) + "") && K(V, f), A & 96 && z !== (z = (m[6](m[23][0]) + m[6](m[23][1])) / 2) && r(w, "x", z), A & 160 && O !== (O = m[7](m[23].data.xVal) + m[7].bandwidth() / 2) && r(g, "y", O), A & 96 && E !== (E = (m[6](m[23][0]) + m[6](m[23][1])) / 2) && r(g, "x", E), A & 16 && M !== (M = m[4] === "all" || m[4] === m[22] ? "1" : "0.25") && r(g, "opacity", M)
+            A & 16 && t !== (t = "horizontal-bar-rect " + (m[4] === m[22] ? "selected" : "unselected") + " svelte-175eim1") && r(l, "class", t), A & 160 && a !== (a = m[7](m[23].data.xVal)) && r(l, "y", a), A & 96 && n !== (n = m[6](m[23][0])) && r(l, "x", n), A & 96 && s !== (s = m[6](m[23][1]) - m[6](m[23][0])) && r(l, "width", s), A & 32 && i !== (i = m[9](m[20].key)) && r(l, "fill", i), A & 16 && u !== (u = m[4] === "all" || m[4] === m[22] ? "1" : "0.25") && r(l, "opacity", u), A & 128 && o !== (o = m[7].bandwidth()) && r(l, "height", o), A & 96 && d !== (d = m[6](m[23][0])) && r(h, "x1", d), A & 96 && b !== (b = m[6](m[23][0])) && r(h, "x2", b), A & 160 && p !== (p = m[7](m[23].data.xVal) - pe) && r(h, "y1", p), A & 160 && c !== (c = m[7].bandwidth() + m[7](m[23].data.xVal) + pe) && r(h, "y2", c), A & 32 && v !== (v = m[20].key + "") && J(_, v), A & 40 && f !== (f = m[10](m[24] / m[11]) + "") && J(V, f), A & 96 && z !== (z = (m[6](m[23][0]) + m[6](m[23][1])) / 2) && r(w, "x", z), A & 160 && O !== (O = m[7](m[23].data.xVal) + m[7].bandwidth() / 2) && r(g, "y", O), A & 96 && E !== (E = (m[6](m[23][0]) + m[6](m[23][1])) / 2) && r(g, "x", E), A & 16 && M !== (M = m[4] === "all" || m[4] === m[22] ? "1" : "0.25") && r(g, "opacity", M)
         },
         d(m) {
             m && y(l), m && y(h), m && y(g)
         }
     }
 }
 
 function Re(e) {
     let l, t, a, n, s, i, u, o, h = e[20],
         d = [];
-    for (let c = 0; c < h.length; c += 1) d[c] = Be(Le(e, h, c));
+    for (let c = 0; c < h.length; c += 1) d[c] = Be(We(e, h, c));
 
     function b() {
         return e[15](e[22], e[20])
     }
 
     function p() {
         return e[16](e[22], e[20])
@@ -448,24 +448,24 @@
                 stroke: !0
             }), q(t).forEach(y), g.forEach(y), this.h()
         },
         h() {
             r(t, "class", "line svelte-175eim1"), r(t, "x1", a = e[2] - e[8].right), r(t, "x2", n = e[2] - e[8].right), r(t, "y1", s = e[7]("A") - pe), r(t, "y2", i = e[7].bandwidth() + e[7]("A") + pe), r(t, "stroke", "black"), r(l, "class", "series svelte-175eim1"), r(l, "role", "button"), r(l, "tabindex", "0")
         },
         m(c, g) {
-            W(c, l, g);
+            L(c, l, g);
             for (let v = 0; v < d.length; v += 1) d[v] && d[v].m(l, null);
             k(l, t), u || (o = [ze(l, "click", b), ze(l, "keypress", p)], u = !0)
         },
         p(c, g) {
             if (e = c, g & 3832) {
                 h = e[20];
                 let v;
                 for (v = 0; v < h.length; v += 1) {
-                    const _ = Le(e, h, v);
+                    const _ = We(e, h, v);
                     d[v] ? d[v].p(_, g) : (d[v] = Be(_), d[v].c(), d[v].m(l, t))
                 }
                 for (; v < d.length; v += 1) d[v].d(1);
                 d.length = h.length
             }
             g & 4 && a !== (a = e[2] - e[8].right) && r(t, "x1", a), g & 4 && n !== (n = e[2] - e[8].right) && r(t, "x2", n), g & 128 && s !== (s = e[7]("A") - pe) && r(t, "y1", s), g & 128 && i !== (i = e[7].bandwidth() + e[7]("A") + pe) && r(t, "y2", i)
         },
@@ -474,15 +474,15 @@
         }
     }
 }
 
 function Tt(e) {
     let l, t, a, n, s, i, u, o = e[5],
         h = [];
-    for (let d = 0; d < o.length; d += 1) h[d] = Re(We(e, o, d));
+    for (let d = 0; d < o.length; d += 1) h[d] = Re(Le(e, o, d));
     return {
         c() {
             l = I("div"), t = I("p"), a = Q("Feedback Distribution"), n = B(), s = I("div"), i = N("svg");
             for (let d = 0; d < h.length; d += 1) h[d].c();
             this.h()
         },
         l(d) {
@@ -503,24 +503,24 @@
             for (let v = 0; v < h.length; v += 1) h[v].l(g);
             g.forEach(y), c.forEach(y), this.h()
         },
         h() {
             r(i, "width", e[1]), r(i, "height", e[0]), r(s, "id", "stackedrect-holder"), r(s, "class", "svelte-175eim1"), le(() => e[17].call(s))
         },
         m(d, b) {
-            W(d, l, b), k(l, t), k(t, a), W(d, n, b), W(d, s, b), k(s, i);
+            L(d, l, b), k(l, t), k(t, a), L(d, n, b), L(d, s, b), k(s, i);
             for (let p = 0; p < h.length; p += 1) h[p] && h[p].m(i, null);
             u = ye(s, e[17].bind(s))
         },
         p(d, [b]) {
             if (b & 8188) {
                 o = d[5];
                 let p;
                 for (p = 0; p < o.length; p += 1) {
-                    const c = We(d, o, p);
+                    const c = Le(d, o, p);
                     h[p] ? h[p].p(c, b) : (h[p] = Re(c), h[p].c(), h[p].m(i, null))
                 }
                 for (; p < h.length; p += 1) h[p].d(1);
                 h.length = o.length
             }
             b & 2 && r(i, "width", d[1]), b & 1 && r(i, "height", d[0])
         },
@@ -529,15 +529,15 @@
         d(d) {
             d && y(l), d && y(n), d && y(s), ee(h, d), u()
         }
     }
 }
 const pe = 5;
 
-function Wt(e, l, t) {
+function Lt(e, l, t) {
     let a, n, s, i, u, o, h, d;
     G(e, te, E => t(14, h = E)), G(e, kt, E => t(3, d = E));
     let b = 300,
         p = 300;
     const c = {
             good: 2,
             bad: 1,
@@ -564,17 +564,17 @@
     function O() {
         p = this.offsetWidth, b = this.offsetHeight, t(1, p), t(0, b)
     }
     return e.$$.update = () => {
         e.$$.dirty & 16384 && t(4, a = c[h]), e.$$.dirty & 2 && t(2, n = p - g.left - g.right), e.$$.dirty & 1 && t(13, s = b - g.top - g.bottom), e.$$.dirty & 8200 && t(7, i = Fe().rangeRound([g.top, s - g.bottom]).padding(.3).domain(d.map(E => E.xVal))), e.$$.dirty & 4 && t(6, u = be().rangeRound([g.left, n - g.right]).domain([0, w])), e.$$.dirty & 8 && t(5, o = f(d))
     }, [b, p, n, d, a, o, u, i, g, v, _, w, V, s, h, z, H, O]
 }
-class Lt extends ne {
+class Wt extends ne {
     constructor(l) {
-        super(), re(this, l, Wt, Tt, ae, {})
+        super(), re(this, l, Lt, Tt, ae, {})
     }
 }
 
 function Bt(e) {
     let l, t, a, n, s, i, u, o, h, d, b, p = e[3][e[2]] + "",
         c, g;
     return {
@@ -600,18 +600,18 @@
             var V = q(d);
             b = C(V, "Rating: "), c = C(V, p), V.forEach(y), _.forEach(y), this.h()
         },
         h() {
             r(t, "class", "question svelte-tstxel"), r(i, "class", "answer svelte-tstxel"), r(d, "class", g = "feedback " + e[2] + " svelte-tstxel"), r(l, "class", "qa-card svelte-tstxel")
         },
         m(v, _) {
-            W(v, l, _), k(l, t), k(t, a), k(t, n), k(l, s), k(l, i), k(i, u), k(i, o), k(l, h), k(l, d), k(d, b), k(d, c)
+            L(v, l, _), k(l, t), k(t, a), k(t, n), k(l, s), k(l, i), k(i, u), k(i, o), k(l, h), k(l, d), k(d, b), k(d, c)
         },
         p(v, [_]) {
-            _ & 1 && K(n, v[0]), _ & 2 && K(o, v[1]), _ & 4 && p !== (p = v[3][v[2]] + "") && K(c, p), _ & 4 && g !== (g = "feedback " + v[2] + " svelte-tstxel") && r(d, "class", g)
+            _ & 1 && J(n, v[0]), _ & 2 && J(o, v[1]), _ & 4 && p !== (p = v[3][v[2]] + "") && J(c, p), _ & 4 && g !== (g = "feedback " + v[2] + " svelte-tstxel") && r(d, "class", g)
         },
         i: $,
         o: $,
         d(v) {
             v && y(l)
         }
     }
@@ -664,22 +664,22 @@
         },
         l(i) {
             l = D(i, "DIV", {});
             var u = q(l);
             _e(t.$$.fragment, u), a = R(u), u.forEach(y)
         },
         m(i, u) {
-            W(i, l, u), de(t, l, null), k(l, a), s = !0
+            L(i, l, u), de(t, l, null), k(l, a), s = !0
         },
         p(i, u) {
             const o = {};
             u & 1 && (o.question = i[5]), u & 1 && (o.answer = i[6]), u & 1 && (o.feedback = i[7]), t.$set(o)
         },
         i(i) {
-            s || (U(t.$$.fragment, i), i && le(() => {
+            s || (K(t.$$.fragment, i), i && le(() => {
                 s && (n || (n = Pe(l, e[1], {
                     duration: 300
                 }, !0)), n.run(1))
             }), s = !0)
         },
         o(i) {
             x(t.$$.fragment, i), i && (n || (n = Pe(l, e[1], {
@@ -713,48 +713,48 @@
             for (let o = 0; o < n.length; o += 1) n[o].l(u);
             u.forEach(y), this.h()
         },
         h() {
             r(l, "class", "qa-container svelte-1xv9cfi")
         },
         m(i, u) {
-            W(i, l, u);
+            L(i, l, u);
             for (let o = 0; o < n.length; o += 1) n[o] && n[o].m(l, null);
             t = !0
         },
         p(i, [u]) {
             if (u & 1) {
                 a = i[0];
                 let o;
                 for (o = 0; o < a.length; o += 1) {
                     const h = Ge(i, a, o);
-                    n[o] ? (n[o].p(h, u), U(n[o], 1)) : (n[o] = $e(h), n[o].c(), U(n[o], 1), n[o].m(l, null))
+                    n[o] ? (n[o].p(h, u), K(n[o], 1)) : (n[o] = $e(h), n[o].c(), K(n[o], 1), n[o].m(l, null))
                 }
                 for (pt(), o = a.length; o < n.length; o += 1) s(o);
                 bt()
             }
         },
         i(i) {
             if (!t) {
-                for (let u = 0; u < a.length; u += 1) U(n[u]);
+                for (let u = 0; u < a.length; u += 1) K(n[u]);
                 t = !0
             }
         },
         o(i) {
             n = n.filter(Boolean);
             for (let u = 0; u < n.length; u += 1) x(n[u]);
             t = !1
         },
         d(i) {
             i && y(l), ee(n, i)
         }
     }
 }
 
-function Zt(e, l, t) {
+function Yt(e, l, t) {
     let a, n, s, i;
     G(e, Oe, o => t(4, n = o)), G(e, te, o => t(2, s = o)), G(e, we, o => t(3, i = o));
     const u = (o, {
         delay: h = 0,
         duration: d = 1e3,
         easing: b = Vt
     }) => qt(o, {
@@ -762,36 +762,36 @@
         duration: d,
         easing: b
     });
     return e.$$.update = () => {
         e.$$.dirty & 12 && t(0, a = s === "all" ? i : i.filter(o => o.vote === s)), e.$$.dirty & 1 && ht(Oe, n = Et(a), n)
     }, [a, u, s, i]
 }
-class Jt extends ne {
+class Zt extends ne {
     constructor(l) {
-        super(), re(this, l, Zt, $t, ae, {})
+        super(), re(this, l, Yt, $t, ae, {})
     }
 }
 
-function Ze(e, l, t) {
+function Ye(e, l, t) {
     const a = e.slice();
     return a[15] = l[t], a
 }
 
-function Je(e, l, t) {
+function Ze(e, l, t) {
     const a = e.slice();
     return a[18] = l[t], a
 }
 
-function Ke(e, l, t) {
+function Je(e, l, t) {
     const a = e.slice();
     return a[18] = l[t], a
 }
 
-function Ue(e) {
+function Ke(e) {
     let l, t, a, n, s = e[18] + "",
         i, u;
     return {
         c() {
             l = N("g"), t = N("line"), n = N("text"), i = Q(s), this.h()
         },
         l(o) {
@@ -815,26 +815,26 @@
             var d = q(n);
             i = C(d, s), d.forEach(y), h.forEach(y), this.h()
         },
         h() {
             r(t, "class", "axis-tick svelte-1oikip4"), r(t, "x1", "0"), r(t, "x2", "0"), r(t, "y1", 0), r(t, "y2", a = -e[2] + e[10].bottom + e[10].top), r(t, "stroke", "var(--squidink)"), r(t, "stroke-dasharray", "4"), r(n, "class", "axis-text svelte-1oikip4"), r(n, "y", "15"), r(n, "text-anchor", "middle"), r(l, "transform", u = `translate(${e[8](e[18])+e[8].bandwidth()/2} ${e[2]-e[10].bottom})`)
         },
         m(o, h) {
-            W(o, l, h), k(l, t), k(l, n), k(n, i)
+            L(o, l, h), k(l, t), k(l, n), k(n, i)
         },
         p(o, h) {
-            h & 4 && a !== (a = -o[2] + o[10].bottom + o[10].top) && r(t, "y2", a), h & 32 && s !== (s = o[18] + "") && K(i, s), h & 292 && u !== (u = `translate(${o[8](o[18])+o[8].bandwidth()/2} ${o[2]-o[10].bottom})`) && r(l, "transform", u)
+            h & 4 && a !== (a = -o[2] + o[10].bottom + o[10].top) && r(t, "y2", a), h & 32 && s !== (s = o[18] + "") && J(i, s), h & 292 && u !== (u = `translate(${o[8](o[18])+o[8].bandwidth()/2} ${o[2]-o[10].bottom})`) && r(l, "transform", u)
         },
         d(o) {
             o && y(l)
         }
     }
 }
 
-function Xe(e) {
+function Ue(e) {
     let l, t, a, n;
     return {
         c() {
             l = N("g"), t = N("line"), this.h()
         },
         l(s) {
             l = F(s, "g", {
@@ -850,26 +850,26 @@
                 stroke: !0
             }), q(t).forEach(y), i.forEach(y), this.h()
         },
         h() {
             r(t, "class", "axis-tick svelte-1oikip4"), r(t, "x1", 0), r(t, "x2", a = e[3] - e[10].right - e[10].left), r(t, "y1", "0"), r(t, "y2", "0"), r(t, "stroke", "black"), r(l, "transform", n = `translate(${e[10].left} ${e[7](e[18])+0})`)
         },
         m(s, i) {
-            W(s, l, i), k(l, t)
+            L(s, l, i), k(l, t)
         },
         p(s, i) {
             i & 8 && a !== (a = s[3] - s[10].right - s[10].left) && r(t, "x2", a), i & 128 && n !== (n = `translate(${s[10].left} ${s[7](s[18])+0})`) && r(l, "transform", n)
         },
         d(s) {
             s && y(l)
         }
     }
 }
 
-function Ye(e) {
+function Xe(e) {
     let l, t, a, n, s, i, u, o, h = Math.round(e[11](e[15].count)) + "",
         d, b, p;
     return {
         c() {
             l = N("g"), t = N("rect"), o = N("text"), d = Q(h), this.h()
         },
         l(c) {
@@ -894,36 +894,36 @@
             var v = q(o);
             d = C(v, h), v.forEach(y), g.forEach(y), this.h()
         },
         h() {
             r(t, "x", a = e[8](e[15].question)), r(t, "y", n = e[7](e[15].count)), r(t, "height", s = e[2] - e[7](e[15].count) - e[10].bottom), r(t, "fill", i = e[6](e[15].count)), r(t, "fill-opacity", "0.95"), r(t, "width", u = e[8].bandwidth()), r(t, "class", "svelte-1oikip4"), r(o, "class", "axis-text svelte-1oikip4"), r(o, "x", b = e[8](e[15].question) + e[8].bandwidth() / 2), r(o, "y", p = e[7](e[15].count) - 5), r(o, "text-anchor", "middle"), r(l, "class", "series")
         },
         m(c, g) {
-            W(c, l, g), k(l, t), k(l, o), k(o, d)
+            L(c, l, g), k(l, t), k(l, o), k(o, d)
         },
         p(c, g) {
-            g & 288 && a !== (a = c[8](c[15].question)) && r(t, "x", a), g & 160 && n !== (n = c[7](c[15].count)) && r(t, "y", n), g & 164 && s !== (s = c[2] - c[7](c[15].count) - c[10].bottom) && r(t, "height", s), g & 96 && i !== (i = c[6](c[15].count)) && r(t, "fill", i), g & 256 && u !== (u = c[8].bandwidth()) && r(t, "width", u), g & 32 && h !== (h = Math.round(c[11](c[15].count)) + "") && K(d, h), g & 288 && b !== (b = c[8](c[15].question) + c[8].bandwidth() / 2) && r(o, "x", b), g & 160 && p !== (p = c[7](c[15].count) - 5) && r(o, "y", p)
+            g & 288 && a !== (a = c[8](c[15].question)) && r(t, "x", a), g & 160 && n !== (n = c[7](c[15].count)) && r(t, "y", n), g & 164 && s !== (s = c[2] - c[7](c[15].count) - c[10].bottom) && r(t, "height", s), g & 96 && i !== (i = c[6](c[15].count)) && r(t, "fill", i), g & 256 && u !== (u = c[8].bandwidth()) && r(t, "width", u), g & 32 && h !== (h = Math.round(c[11](c[15].count)) + "") && J(d, h), g & 288 && b !== (b = c[8](c[15].question) + c[8].bandwidth() / 2) && r(o, "x", b), g & 160 && p !== (p = c[7](c[15].count) - 5) && r(o, "y", p)
         },
         d(c) {
             c && y(l)
         }
     }
 }
 
-function Kt(e) {
+function Jt(e) {
     let l, t, a, n, s, i, u = e[9][e[4]] + "",
         o, h, d, b, p, c, g, v, _, w = e[5].map(xe),
         f = [];
-    for (let E = 0; E < w.length; E += 1) f[E] = Ue(Ke(e, w, E));
+    for (let E = 0; E < w.length; E += 1) f[E] = Ke(Je(e, w, E));
     let V = e[7].ticks(),
         z = [];
-    for (let E = 0; E < V.length; E += 1) z[E] = Xe(Je(e, V, E));
+    for (let E = 0; E < V.length; E += 1) z[E] = Ue(Ze(e, V, E));
     let H = e[5],
         O = [];
-    for (let E = 0; E < H.length; E += 1) O[E] = Ye(Ze(e, H, E));
+    for (let E = 0; E < H.length; E += 1) O[E] = Xe(Ye(e, H, E));
     return {
         c() {
             l = I("div"), t = N("svg");
             for (let E = 0; E < f.length; E += 1) f[E].c();
             a = ve();
             for (let E = 0; E < z.length; E += 1) z[E].c();
             n = ve();
@@ -968,65 +968,65 @@
                 opacity: !0
             }), q(g).forEach(y), m.forEach(y), M.forEach(y), this.h()
         },
         h() {
             r(s, "class", "chart-title svelte-1oikip4"), r(s, "y", e[10].top / 2 + 1), r(s, "x", h = (e[3] + e[10].left) / 2), r(s, "text-anchor", "middle"), r(d, "class", "axis-line svelte-1oikip4"), r(d, "x1", e[10].left), r(d, "x2", b = e[3] - e[10].right), r(d, "y1", p = e[2] - e[10].bottom), r(d, "y2", c = e[2] - e[10].bottom), r(g, "class", "axis-line svelte-1oikip4"), r(g, "x1", e[10].left), r(g, "x2", e[10].left), r(g, "y1", e[10].top), r(g, "y2", v = e[2] - e[10].bottom), r(g, "opacity", "0"), r(t, "width", e[1]), r(t, "height", e[0]), r(l, "id", "stackedrect-holder"), r(l, "class", "svelte-1oikip4"), le(() => e[13].call(l))
         },
         m(E, M) {
-            W(E, l, M), k(l, t);
+            L(E, l, M), k(l, t);
             for (let m = 0; m < f.length; m += 1) f[m] && f[m].m(t, null);
             k(t, a);
             for (let m = 0; m < z.length; m += 1) z[m] && z[m].m(t, null);
             k(t, n);
             for (let m = 0; m < O.length; m += 1) O[m] && O[m].m(t, null);
             k(t, s), k(s, i), k(s, o), k(t, d), k(t, g), _ = ye(l, e[13].bind(l))
         },
         p(E, [M]) {
             if (M & 1316) {
                 w = E[5].map(xe);
                 let m;
                 for (m = 0; m < w.length; m += 1) {
-                    const A = Ke(E, w, m);
-                    f[m] ? f[m].p(A, M) : (f[m] = Ue(A), f[m].c(), f[m].m(t, a))
+                    const A = Je(E, w, m);
+                    f[m] ? f[m].p(A, M) : (f[m] = Ke(A), f[m].c(), f[m].m(t, a))
                 }
                 for (; m < f.length; m += 1) f[m].d(1);
                 f.length = w.length
             }
             if (M & 1160) {
                 V = E[7].ticks();
                 let m;
                 for (m = 0; m < V.length; m += 1) {
-                    const A = Je(E, V, m);
-                    z[m] ? z[m].p(A, M) : (z[m] = Xe(A), z[m].c(), z[m].m(t, n))
+                    const A = Ze(E, V, m);
+                    z[m] ? z[m].p(A, M) : (z[m] = Ue(A), z[m].c(), z[m].m(t, n))
                 }
                 for (; m < z.length; m += 1) z[m].d(1);
                 z.length = V.length
             }
             if (M & 3556) {
                 H = E[5];
                 let m;
                 for (m = 0; m < H.length; m += 1) {
-                    const A = Ze(E, H, m);
-                    O[m] ? O[m].p(A, M) : (O[m] = Ye(A), O[m].c(), O[m].m(t, s))
+                    const A = Ye(E, H, m);
+                    O[m] ? O[m].p(A, M) : (O[m] = Xe(A), O[m].c(), O[m].m(t, s))
                 }
                 for (; m < O.length; m += 1) O[m].d(1);
                 O.length = H.length
             }
-            M & 16 && u !== (u = E[9][E[4]] + "") && K(o, u), M & 8 && h !== (h = (E[3] + E[10].left) / 2) && r(s, "x", h), M & 8 && b !== (b = E[3] - E[10].right) && r(d, "x2", b), M & 4 && p !== (p = E[2] - E[10].bottom) && r(d, "y1", p), M & 4 && c !== (c = E[2] - E[10].bottom) && r(d, "y2", c), M & 4 && v !== (v = E[2] - E[10].bottom) && r(g, "y2", v), M & 2 && r(t, "width", E[1]), M & 1 && r(t, "height", E[0])
+            M & 16 && u !== (u = E[9][E[4]] + "") && J(o, u), M & 8 && h !== (h = (E[3] + E[10].left) / 2) && r(s, "x", h), M & 8 && b !== (b = E[3] - E[10].right) && r(d, "x2", b), M & 4 && p !== (p = E[2] - E[10].bottom) && r(d, "y1", p), M & 4 && c !== (c = E[2] - E[10].bottom) && r(d, "y2", c), M & 4 && v !== (v = E[2] - E[10].bottom) && r(g, "y2", v), M & 2 && r(t, "width", E[1]), M & 1 && r(t, "height", E[0])
         },
         i: $,
         o: $,
         d(E) {
             E && y(l), ee(f, E), ee(z, E), ee(O, E), _()
         }
     }
 }
 const xe = e => e.question;
 
-function Ut(e, l, t) {
+function Kt(e, l, t) {
     let a, n, s, i, u, o, h, d;
     G(e, te, f => t(4, h = f)), G(e, Oe, f => t(5, d = f));
     const b = {
             good: "Good 👍",
             bad: "Bad 👎",
             na: "No Rating",
             all: "All"
@@ -1050,17 +1050,17 @@
     function w() {
         g = this.offsetWidth, c = this.offsetHeight, t(1, g), t(0, c)
     }
     return e.$$.update = () => {
         e.$$.dirty & 2 && t(3, a = g - v.left - v.right), e.$$.dirty & 1 && t(2, n = c - v.top - v.bottom), e.$$.dirty & 40 && t(8, s = Fe().rangeRound([v.left, a - v.right]).padding(.05).domain(d.map(f => f.question))), e.$$.dirty & 36 && t(7, i = be().rangeRound([n - v.bottom, v.top]).domain([0, ke(d, f => f.count)])), e.$$.dirty & 32 && t(12, u = ke(d, f => f.count)), e.$$.dirty & 4112 && t(6, o = be().domain([0, u]).range(["white", p[h]]).interpolate(dt))
     }, [c, g, n, a, h, d, o, i, s, b, v, _, u, w]
 }
-class Xt extends ne {
+class Ut extends ne {
     constructor(l) {
-        super(), re(this, l, Ut, Kt, ae, {})
+        super(), re(this, l, Kt, Jt, ae, {})
     }
 }
 
 function et(e, l, t) {
     const a = e.slice();
     a[19] = l[t];
     const n = a[7](a[19].x1) - a[7](a[19].x0);
@@ -1101,18 +1101,18 @@
             var d = q(n);
             i = C(d, s), d.forEach(y), h.forEach(y), this.h()
         },
         h() {
             r(t, "class", "axis-tick svelte-kz2qh6"), r(t, "x1", "0"), r(t, "x2", "0"), r(t, "y1", 0), r(t, "y2", a = -e[2] + e[9].bottom + e[9].top), r(t, "stroke", "var(--squidink)"), r(t, "stroke-dasharray", "4"), r(n, "class", "axis-text svelte-kz2qh6"), r(n, "y", "15"), r(n, "text-anchor", "middle"), r(l, "transform", u = `translate(${e[7](e[23])+(e[7](1)-e[7](0))/2} ${e[2]-e[9].bottom})`), r(l, "class", "svelte-kz2qh6")
         },
         m(o, h) {
-            W(o, l, h), k(l, t), k(l, n), k(n, i)
+            L(o, l, h), k(l, t), k(l, n), k(n, i)
         },
         p(o, h) {
-            h & 4 && a !== (a = -o[2] + o[9].bottom + o[9].top) && r(t, "y2", a), h & 128 && s !== (s = o[23] + "") && K(i, s), h & 132 && u !== (u = `translate(${o[7](o[23])+(o[7](1)-o[7](0))/2} ${o[2]-o[9].bottom})`) && r(l, "transform", u)
+            h & 4 && a !== (a = -o[2] + o[9].bottom + o[9].top) && r(t, "y2", a), h & 128 && s !== (s = o[23] + "") && J(i, s), h & 132 && u !== (u = `translate(${o[7](o[23])+(o[7](1)-o[7](0))/2} ${o[2]-o[9].bottom})`) && r(l, "transform", u)
         },
         d(o) {
             o && y(l)
         }
     }
 }
 
@@ -1136,26 +1136,26 @@
                 class: !0
             }), q(t).forEach(y), h.forEach(y), this.h()
         },
         h() {
             r(t, "x", a = e[7](e[19].x0) + 1), r(t, "width", n = e[20]), r(t, "y", s = e[6](e[19].length)), r(t, "height", i = e[6](0) - e[6](e[19].length)), r(t, "fill", u = e[8][e[5]]), r(t, "class", "svelte-kz2qh6"), r(l, "class", "histogram-bin svelte-kz2qh6")
         },
         m(o, h) {
-            W(o, l, h), k(l, t)
+            L(o, l, h), k(l, t)
         },
         p(o, h) {
             h & 136 && a !== (a = o[7](o[19].x0) + 1) && r(t, "x", a), h & 136 && n !== (n = o[20]) && r(t, "width", n), h & 72 && s !== (s = o[6](o[19].length)) && r(t, "y", s), h & 72 && i !== (i = o[6](0) - o[6](o[19].length)) && r(t, "height", i), h & 32 && u !== (u = o[8][o[5]]) && r(t, "fill", u)
         },
         d(o) {
             o && y(l)
         }
     }
 }
 
-function Yt(e) {
+function Xt(e) {
     let l, t, a, n, s, i, u, o, h, d, b, p = e[7].ticks(),
         c = [];
     for (let _ = 0; _ < p.length; _ += 1) c[_] = lt(tt(e, p, _));
     let g = e[3],
         v = [];
     for (let _ = 0; _ < g.length; _ += 1) v[_] = nt(et(e, g, _));
     return {
@@ -1195,15 +1195,15 @@
                 y2: !0
             }), q(u).forEach(y), f.forEach(y), w.forEach(y), this.h()
         },
         h() {
             r(n, "class", "chart-title svelte-kz2qh6"), r(n, "y", e[9].top / 2 + 5), r(n, "x", i = (e[4] + e[9].left) / 2), r(n, "text-anchor", "middle"), r(u, "class", "axis-line svelte-kz2qh6"), r(u, "x1", e[9].left), r(u, "x2", o = e[4] - e[9].right), r(u, "y1", h = e[2] - e[9].bottom), r(u, "y2", d = e[2] - e[9].bottom), r(t, "width", e[1]), r(t, "height", e[0]), r(t, "class", "svelte-kz2qh6"), r(l, "class", "histogram-container svelte-kz2qh6"), le(() => e[14].call(l))
         },
         m(_, w) {
-            W(_, l, w), k(l, t);
+            L(_, l, w), k(l, t);
             for (let f = 0; f < c.length; f += 1) c[f] && c[f].m(t, null);
             k(t, a);
             for (let f = 0; f < v.length; f += 1) v[f] && v[f].m(t, null);
             k(t, n), k(n, s), k(t, u), b = ye(l, e[14].bind(l))
         },
         p(_, [w]) {
             if (w & 644) {
@@ -1264,15 +1264,15 @@
     }
     return e.$$.update = () => {
         e.$$.dirty & 8224 && t(12, a = b === "all" ? p : p.filter(V => V.vote === b)), e.$$.dirty & 4096 && t(11, n = gt(a)), e.$$.dirty & 2 && t(4, s = v - _.left - _.right), e.$$.dirty & 1 && t(2, i = g - _.top - _.bottom), e.$$.dirty & 2048 && t(3, u = vt().thresholds(w).value(V => V.answer)(n)), e.$$.dirty & 16 && t(7, o = be().domain([3, rt]).range([_.left, s - _.right])), e.$$.dirty & 12 && t(6, h = be().domain([0, ke(u, V => V.length)]).range([i - _.bottom, _.top])), e.$$.dirty & 2048 && t(10, d = ke(n, V => V.length)), e.$$.dirty & 1056 && be().domain([0, d]).range(["white", c[b]]).interpolate(dt)
     }, [g, v, i, u, s, b, h, o, c, _, d, n, a, p, f]
 }
 class el extends ne {
     constructor(l) {
-        super(), re(this, l, xt, Yt, ae, {})
+        super(), re(this, l, xt, Xt, ae, {})
     }
 }
 
 function at(e, l, t) {
     const a = e.slice();
     a[18] = l[t];
     const n = a[7](a[18].x1) - a[7](a[18].x0);
@@ -1313,18 +1313,18 @@
             var d = q(n);
             i = C(d, s), d.forEach(y), h.forEach(y), this.h()
         },
         h() {
             r(t, "class", "axis-tick svelte-kz2qh6"), r(t, "x1", "0"), r(t, "x2", "0"), r(t, "y1", 0), r(t, "y2", a = -e[2] + e[9].bottom + e[9].top), r(t, "stroke", "var(--squidink)"), r(t, "stroke-dasharray", "4"), r(n, "class", "axis-text svelte-kz2qh6"), r(n, "y", "15"), r(n, "text-anchor", "middle"), r(l, "transform", u = `translate(${e[7](e[22])+(e[7](1)-e[7](0))/2} ${e[2]-e[9].bottom})`), r(l, "class", "svelte-kz2qh6")
         },
         m(o, h) {
-            W(o, l, h), k(l, t), k(l, n), k(n, i)
+            L(o, l, h), k(l, t), k(l, n), k(n, i)
         },
         p(o, h) {
-            h & 4 && a !== (a = -o[2] + o[9].bottom + o[9].top) && r(t, "y2", a), h & 128 && s !== (s = o[22] + "") && K(i, s), h & 132 && u !== (u = `translate(${o[7](o[22])+(o[7](1)-o[7](0))/2} ${o[2]-o[9].bottom})`) && r(l, "transform", u)
+            h & 4 && a !== (a = -o[2] + o[9].bottom + o[9].top) && r(t, "y2", a), h & 128 && s !== (s = o[22] + "") && J(i, s), h & 132 && u !== (u = `translate(${o[7](o[22])+(o[7](1)-o[7](0))/2} ${o[2]-o[9].bottom})`) && r(l, "transform", u)
         },
         d(o) {
             o && y(l)
         }
     }
 }
 
@@ -1348,15 +1348,15 @@
                 class: !0
             }), q(t).forEach(y), h.forEach(y), this.h()
         },
         h() {
             r(t, "x", a = e[7](e[18].x0) + 1), r(t, "width", n = e[19]), r(t, "y", s = e[6](e[18].length)), r(t, "height", i = e[6](0) - e[6](e[18].length)), r(t, "fill", u = e[8][e[5]]), r(t, "class", "svelte-kz2qh6"), r(l, "class", "histogram-bin svelte-kz2qh6")
         },
         m(o, h) {
-            W(o, l, h), k(l, t)
+            L(o, l, h), k(l, t)
         },
         p(o, h) {
             h & 136 && a !== (a = o[7](o[18].x0) + 1) && r(t, "x", a), h & 136 && n !== (n = o[19]) && r(t, "width", n), h & 72 && s !== (s = o[6](o[18].length)) && r(t, "y", s), h & 72 && i !== (i = o[6](0) - o[6](o[18].length)) && r(t, "height", i), h & 32 && u !== (u = o[8][o[5]]) && r(t, "fill", u)
         },
         d(o) {
             o && y(l)
         }
@@ -1407,15 +1407,15 @@
                 y2: !0
             }), q(u).forEach(y), f.forEach(y), w.forEach(y), this.h()
         },
         h() {
             r(n, "class", "chart-title svelte-kz2qh6"), r(n, "y", e[9].top / 2 + 5), r(n, "x", i = (e[4] + e[9].left) / 2), r(n, "text-anchor", "middle"), r(u, "class", "axis-line svelte-kz2qh6"), r(u, "x1", e[9].left), r(u, "x2", o = e[4] - e[9].right), r(u, "y1", h = e[2] - e[9].bottom), r(u, "y2", d = e[2] - e[9].bottom), r(t, "width", e[1]), r(t, "height", e[0]), r(t, "class", "svelte-kz2qh6"), r(l, "class", "histogram-container svelte-kz2qh6"), le(() => e[13].call(l))
         },
         m(_, w) {
-            W(_, l, w), k(l, t);
+            L(_, l, w), k(l, t);
             for (let f = 0; f < c.length; f += 1) c[f] && c[f].m(t, null);
             k(t, a);
             for (let f = 0; f < v.length; f += 1) v[f] && v[f].m(t, null);
             k(t, n), k(n, s), k(t, u), b = ye(l, e[13].bind(l))
         },
         p(_, [w]) {
             if (w & 644) {
@@ -1482,15 +1482,15 @@
     constructor(l) {
         super(), re(this, l, ll, tl, ae, {})
     }
 }
 
 function rl(e) {
     let l, t, a, n, s, i, u, o, h, d, b, p, c, g, v, _, w, f, V = Math.round(e[5](e[3])) + "",
-        z, H, O, E, M, m, A, T, Z;
+        z, H, O, E, M, m, A, T, Y;
     return {
         c() {
             l = I("div"), t = I("div"), a = I("p"), n = Q("Questions"), s = B(), i = I("select"), u = I("option"), o = Q("All"), h = I("option"), d = Q("Good"), b = I("option"), p = Q("Bad"), c = I("option"), g = Q("N/A"), v = B(), _ = I("div"), w = N("svg"), f = N("text"), z = Q(V), M = B(), m = I("p"), A = Q("number of responses"), this.h()
         },
         l(S) {
             l = D(S, "DIV", {
                 class: !0,
@@ -1500,39 +1500,39 @@
             t = D(j, "DIV", {
                 class: !0
             });
             var P = q(t);
             a = D(P, "P", {
                 class: !0
             });
-            var J = q(a);
-            n = C(J, "Questions"), J.forEach(y), s = R(P), i = D(P, "SELECT", {
+            var Z = q(a);
+            n = C(Z, "Questions"), Z.forEach(y), s = R(P), i = D(P, "SELECT", {
                 id: !0,
                 name: !0,
                 style: !0,
                 class: !0
             });
-            var L = q(i);
-            u = D(L, "OPTION", {
+            var W = q(i);
+            u = D(W, "OPTION", {
                 class: !0
             });
-            var X = q(u);
-            o = C(X, "All"), X.forEach(y), h = D(L, "OPTION", {
+            var U = q(u);
+            o = C(U, "All"), U.forEach(y), h = D(W, "OPTION", {
                 class: !0
             });
             var oe = q(h);
-            d = C(oe, "Good"), oe.forEach(y), b = D(L, "OPTION", {
+            d = C(oe, "Good"), oe.forEach(y), b = D(W, "OPTION", {
                 class: !0
             });
             var se = q(b);
-            p = C(se, "Bad"), se.forEach(y), c = D(L, "OPTION", {
+            p = C(se, "Bad"), se.forEach(y), c = D(W, "OPTION", {
                 class: !0
             });
             var ie = q(c);
-            g = C(ie, "N/A"), ie.forEach(y), L.forEach(y), P.forEach(y), v = R(j), _ = D(j, "DIV", {
+            g = C(ie, "N/A"), ie.forEach(y), W.forEach(y), P.forEach(y), v = R(j), _ = D(j, "DIV", {
                 class: !0
             });
             var ue = q(_);
             w = F(ue, "svg", {
                 width: !0,
                 height: !0,
                 class: !0
@@ -1545,30 +1545,30 @@
                 "text-anchor": !0,
                 class: !0
             });
             var fe = q(f);
             z = C(fe, V), fe.forEach(y), he.forEach(y), ue.forEach(y), M = R(j), m = D(j, "P", {
                 class: !0
             });
-            var Y = q(m);
-            A = C(Y, "number of responses"), Y.forEach(y), j.forEach(y), this.h()
+            var X = q(m);
+            A = C(X, "number of responses"), X.forEach(y), j.forEach(y), this.h()
         },
         h() {
             r(a, "class", "card-text svelte-1pknxov"), u.__value = "all", u.value = u.__value, r(u, "class", "svelte-1pknxov"), h.__value = "good", h.value = h.__value, r(h, "class", "svelte-1pknxov"), b.__value = "bad", b.value = b.__value, r(b, "class", "svelte-1pknxov"), c.__value = "na", c.value = c.__value, r(c, "class", "svelte-1pknxov"), r(i, "id", "feedback-dropdown"), r(i, "name", "feedback-dropdown"), me(i, "background", e[6][e[0]]), r(i, "class", "svelte-1pknxov"), e[0] === void 0 && le(() => e[9].call(i)), r(t, "class", "svelte-1pknxov"), r(f, "dominant-baseline", "middle"), r(f, "x", H = e[2] / 2), r(f, "y", O = e[1] / 2), r(f, "text-anchor", "middle"), r(f, "class", "svelte-1pknxov"), r(w, "width", e[2]), r(w, "height", e[1]), r(w, "class", "svelte-1pknxov"), r(_, "class", "svelte-1pknxov"), le(() => e[10].call(_)), r(m, "class", "small svelte-1pknxov"), r(l, "class", "card-container svelte-1pknxov"), me(l, "background", e[6][e[0]])
         },
         m(S, j) {
-            W(S, l, j), k(l, t), k(t, a), k(a, n), k(t, s), k(t, i), k(i, u), k(u, o), k(i, h), k(h, d), k(i, b), k(b, p), k(i, c), k(c, g), Ae(i, e[0], !0), k(l, v), k(l, _), k(_, w), k(w, f), k(f, z), E = ye(_, e[10].bind(_)), k(l, M), k(l, m), k(m, A), T || (Z = ze(i, "change", e[9]), T = !0)
+            L(S, l, j), k(l, t), k(t, a), k(a, n), k(t, s), k(t, i), k(i, u), k(u, o), k(i, h), k(h, d), k(i, b), k(b, p), k(i, c), k(c, g), Ae(i, e[0], !0), k(l, v), k(l, _), k(_, w), k(w, f), k(f, z), E = ye(_, e[10].bind(_)), k(l, M), k(l, m), k(m, A), T || (Y = ze(i, "change", e[9]), T = !0)
         },
         p(S, [j]) {
-            j & 1 && me(i, "background", S[6][S[0]]), j & 1 && Ae(i, S[0]), j & 8 && V !== (V = Math.round(S[5](S[3])) + "") && K(z, V), j & 4 && H !== (H = S[2] / 2) && r(f, "x", H), j & 2 && O !== (O = S[1] / 2) && r(f, "y", O), j & 4 && r(w, "width", S[2]), j & 2 && r(w, "height", S[1]), j & 1 && me(l, "background", S[6][S[0]])
+            j & 1 && me(i, "background", S[6][S[0]]), j & 1 && Ae(i, S[0]), j & 8 && V !== (V = Math.round(S[5](S[3])) + "") && J(z, V), j & 4 && H !== (H = S[2] / 2) && r(f, "x", H), j & 2 && O !== (O = S[1] / 2) && r(f, "y", O), j & 4 && r(w, "width", S[2]), j & 2 && r(w, "height", S[1]), j & 1 && me(l, "background", S[6][S[0]])
         },
         i: $,
         o: $,
         d(S) {
-            S && y(l), E(), T = !1, Z()
+            S && y(l), E(), T = !1, Y()
         }
     }
 }
 
 function al(e, l) {
     return l === "all" ? e.length : e.filter(a => a.vote === l).length
 }
@@ -1601,15 +1601,15 @@
     constructor(l) {
         super(), re(this, l, ol, rl, ae, {})
     }
 }
 
 function il(e) {
     let l, t, a, n, s, i, u, o, h, d, b, p, c, g, v, _, w, f, V = e[5](e[3]) + "",
-        z, H, O, E, M, m, A, T, Z;
+        z, H, O, E, M, m, A, T, Y;
     return {
         c() {
             l = I("div"), t = I("div"), a = I("p"), n = Q("Questions"), s = B(), i = I("select"), u = I("option"), o = Q("All"), h = I("option"), d = Q("Good"), b = I("option"), p = Q("Bad"), c = I("option"), g = Q("N/A"), v = B(), _ = I("div"), w = N("svg"), f = N("text"), z = Q(V), M = B(), m = I("p"), A = Q("percentage of responses"), this.h()
         },
         l(S) {
             l = D(S, "DIV", {
                 class: !0,
@@ -1617,31 +1617,31 @@
             });
             var j = q(l);
             t = D(j, "DIV", {});
             var P = q(t);
             a = D(P, "P", {
                 class: !0
             });
-            var J = q(a);
-            n = C(J, "Questions"), J.forEach(y), s = R(P), i = D(P, "SELECT", {
+            var Z = q(a);
+            n = C(Z, "Questions"), Z.forEach(y), s = R(P), i = D(P, "SELECT", {
                 id: !0,
                 name: !0,
                 style: !0,
                 class: !0
             });
-            var L = q(i);
-            u = D(L, "OPTION", {});
-            var X = q(u);
-            o = C(X, "All"), X.forEach(y), h = D(L, "OPTION", {});
+            var W = q(i);
+            u = D(W, "OPTION", {});
+            var U = q(u);
+            o = C(U, "All"), U.forEach(y), h = D(W, "OPTION", {});
             var oe = q(h);
-            d = C(oe, "Good"), oe.forEach(y), b = D(L, "OPTION", {});
+            d = C(oe, "Good"), oe.forEach(y), b = D(W, "OPTION", {});
             var se = q(b);
-            p = C(se, "Bad"), se.forEach(y), c = D(L, "OPTION", {});
+            p = C(se, "Bad"), se.forEach(y), c = D(W, "OPTION", {});
             var ie = q(c);
-            g = C(ie, "N/A"), ie.forEach(y), L.forEach(y), P.forEach(y), v = R(j), _ = D(j, "DIV", {});
+            g = C(ie, "N/A"), ie.forEach(y), W.forEach(y), P.forEach(y), v = R(j), _ = D(j, "DIV", {});
             var ue = q(_);
             w = F(ue, "svg", {
                 width: !0,
                 height: !0,
                 class: !0
             });
             var he = q(w);
@@ -1652,30 +1652,30 @@
                 "text-anchor": !0,
                 class: !0
             });
             var fe = q(f);
             z = C(fe, V), fe.forEach(y), he.forEach(y), ue.forEach(y), M = R(j), m = D(j, "P", {
                 class: !0
             });
-            var Y = q(m);
-            A = C(Y, "percentage of responses"), Y.forEach(y), j.forEach(y), this.h()
+            var X = q(m);
+            A = C(X, "percentage of responses"), X.forEach(y), j.forEach(y), this.h()
         },
         h() {
             r(a, "class", "card-text svelte-mchgj2"), u.__value = "all", u.value = u.__value, h.__value = "good", h.value = h.__value, b.__value = "bad", b.value = b.__value, c.__value = "na", c.value = c.__value, r(i, "id", "feedback-dropdown"), r(i, "name", "feedback-dropdown"), me(i, "background", e[6][e[0]]), r(i, "class", "svelte-mchgj2"), e[0] === void 0 && le(() => e[9].call(i)), r(f, "dominant-baseline", "middle"), r(f, "x", H = e[2] / 2), r(f, "y", O = e[1] / 2), r(f, "text-anchor", "middle"), r(f, "class", "svelte-mchgj2"), r(w, "width", e[2]), r(w, "height", e[1]), r(w, "class", "svelte-mchgj2"), le(() => e[10].call(_)), r(m, "class", "small svelte-mchgj2"), r(l, "class", "card-container svelte-mchgj2"), me(l, "background", e[6][e[0]])
         },
         m(S, j) {
-            W(S, l, j), k(l, t), k(t, a), k(a, n), k(t, s), k(t, i), k(i, u), k(u, o), k(i, h), k(h, d), k(i, b), k(b, p), k(i, c), k(c, g), Ae(i, e[0], !0), k(l, v), k(l, _), k(_, w), k(w, f), k(f, z), E = ye(_, e[10].bind(_)), k(l, M), k(l, m), k(m, A), T || (Z = ze(i, "change", e[9]), T = !0)
+            L(S, l, j), k(l, t), k(t, a), k(a, n), k(t, s), k(t, i), k(i, u), k(u, o), k(i, h), k(h, d), k(i, b), k(b, p), k(i, c), k(c, g), Ae(i, e[0], !0), k(l, v), k(l, _), k(_, w), k(w, f), k(f, z), E = ye(_, e[10].bind(_)), k(l, M), k(l, m), k(m, A), T || (Y = ze(i, "change", e[9]), T = !0)
         },
         p(S, [j]) {
-            j & 1 && me(i, "background", S[6][S[0]]), j & 1 && Ae(i, S[0]), j & 8 && V !== (V = S[5](S[3]) + "") && K(z, V), j & 4 && H !== (H = S[2] / 2) && r(f, "x", H), j & 2 && O !== (O = S[1] / 2) && r(f, "y", O), j & 4 && r(w, "width", S[2]), j & 2 && r(w, "height", S[1]), j & 1 && me(l, "background", S[6][S[0]])
+            j & 1 && me(i, "background", S[6][S[0]]), j & 1 && Ae(i, S[0]), j & 8 && V !== (V = S[5](S[3]) + "") && J(z, V), j & 4 && H !== (H = S[2] / 2) && r(f, "x", H), j & 2 && O !== (O = S[1] / 2) && r(f, "y", O), j & 4 && r(w, "width", S[2]), j & 2 && r(w, "height", S[1]), j & 1 && me(l, "background", S[6][S[0]])
         },
         i: $,
         o: $,
         d(S) {
-            S && y(l), E(), T = !1, Z()
+            S && y(l), E(), T = !1, Y()
         }
     }
 }
 
 function ul(e, l) {
     const t = e.length;
     return l === "all" ? 1 : e.filter(n => n.vote === l).length / t
@@ -1708,87 +1708,87 @@
 class fl extends ne {
     constructor(l) {
         super(), re(this, l, hl, il, ae, {})
     }
 }
 
 function cl(e) {
-    let l, t, a, n, s, i, u, o, h, d, b, p, c, g, v, _, w, f, V, z, H, O, E, M, m, A, T, Z, S, j;
-    return s = new sl({}), o = new fl({}), b = new Lt({}), g = new Xt({
+    let l, t, a, n, s, i, u, o, h, d, b, p, c, g, v, _, w, f, V, z, H, O, E, M, m, A, T, Y, S, j;
+    return s = new sl({}), o = new fl({}), b = new Wt({}), g = new Ut({
         props: {
             feedback: "Bad"
         }
-    }), w = new nl({}), z = new el({}), S = new Jt({}), {
+    }), w = new nl({}), z = new el({}), S = new Zt({}), {
         c() {
-            l = I("div"), t = I("div"), a = I("div"), n = I("div"), ce(s.$$.fragment), i = B(), u = I("div"), ce(o.$$.fragment), h = B(), d = I("div"), ce(b.$$.fragment), p = B(), c = I("div"), ce(g.$$.fragment), v = B(), _ = I("div"), ce(w.$$.fragment), f = B(), V = I("div"), ce(z.$$.fragment), H = B(), O = I("div"), E = I("div"), M = I("div"), m = B(), A = I("div"), T = B(), Z = I("div"), ce(S.$$.fragment), this.h()
+            l = I("div"), t = I("div"), a = I("div"), n = I("div"), ce(s.$$.fragment), i = B(), u = I("div"), ce(o.$$.fragment), h = B(), d = I("div"), ce(b.$$.fragment), p = B(), c = I("div"), ce(g.$$.fragment), v = B(), _ = I("div"), ce(w.$$.fragment), f = B(), V = I("div"), ce(z.$$.fragment), H = B(), O = I("div"), E = I("div"), M = I("div"), m = B(), A = I("div"), T = B(), Y = I("div"), ce(S.$$.fragment), this.h()
         },
         l(P) {
             l = D(P, "DIV", {
                 class: !0
             });
-            var J = q(l);
-            t = D(J, "DIV", {
+            var Z = q(l);
+            t = D(Z, "DIV", {
                 class: !0
             });
-            var L = q(t);
-            a = D(L, "DIV", {
+            var W = q(t);
+            a = D(W, "DIV", {
                 class: !0
             });
-            var X = q(a);
-            n = D(X, "DIV", {
+            var U = q(a);
+            n = D(U, "DIV", {
                 class: !0
             });
             var oe = q(n);
-            _e(s.$$.fragment, oe), oe.forEach(y), i = R(X), u = D(X, "DIV", {
+            _e(s.$$.fragment, oe), oe.forEach(y), i = R(U), u = D(U, "DIV", {
                 class: !0
             });
             var se = q(u);
-            _e(o.$$.fragment, se), se.forEach(y), X.forEach(y), h = R(L), d = D(L, "DIV", {
+            _e(o.$$.fragment, se), se.forEach(y), U.forEach(y), h = R(W), d = D(W, "DIV", {
                 class: !0
             });
             var ie = q(d);
-            _e(b.$$.fragment, ie), ie.forEach(y), p = R(L), c = D(L, "DIV", {
+            _e(b.$$.fragment, ie), ie.forEach(y), p = R(W), c = D(W, "DIV", {
                 class: !0
             });
             var ue = q(c);
-            _e(g.$$.fragment, ue), ue.forEach(y), v = R(L), _ = D(L, "DIV", {
+            _e(g.$$.fragment, ue), ue.forEach(y), v = R(W), _ = D(W, "DIV", {
                 class: !0
             });
             var he = q(_);
-            _e(w.$$.fragment, he), he.forEach(y), f = R(L), V = D(L, "DIV", {
+            _e(w.$$.fragment, he), he.forEach(y), f = R(W), V = D(W, "DIV", {
                 class: !0
             });
             var fe = q(V);
-            _e(z.$$.fragment, fe), fe.forEach(y), L.forEach(y), H = R(J), O = D(J, "DIV", {
+            _e(z.$$.fragment, fe), fe.forEach(y), W.forEach(y), H = R(Z), O = D(Z, "DIV", {
                 class: !0
             });
-            var Y = q(O);
-            E = D(Y, "DIV", {
+            var X = q(O);
+            E = D(X, "DIV", {
                 class: !0
             });
             var qe = q(E);
             M = D(qe, "DIV", {
                 class: !0
             }), q(M).forEach(y), m = R(qe), A = D(qe, "DIV", {
                 class: !0
-            }), q(A).forEach(y), qe.forEach(y), T = R(Y), Z = D(Y, "DIV", {
+            }), q(A).forEach(y), qe.forEach(y), T = R(X), Y = D(X, "DIV", {
                 class: !0
             });
-            var He = q(Z);
-            _e(S.$$.fragment, He), He.forEach(y), Y.forEach(y), J.forEach(y), this.h()
+            var He = q(Y);
+            _e(S.$$.fragment, He), He.forEach(y), X.forEach(y), Z.forEach(y), this.h()
         },
         h() {
-            r(n, "class", "card-1 svelte-1hev6jh"), r(u, "class", "card-2"), r(a, "class", "left-text svelte-1hev6jh"), r(d, "class", "left-confidence svelte-1hev6jh"), r(c, "class", "left-question svelte-1hev6jh"), r(_, "class", "left-filter svelte-1hev6jh"), r(V, "class", "left-filter2"), r(t, "class", "feedback-left svelte-1hev6jh"), r(M, "class", "right-chart-1 svelte-1hev6jh"), r(A, "class", "right-chart-2 svelte-1hev6jh"), r(E, "class", "right-chart svelte-1hev6jh"), r(Z, "class", "right-table svelte-1hev6jh"), r(O, "class", "feedback-right svelte-1hev6jh"), r(l, "class", "feedback-container svelte-1hev6jh")
+            r(n, "class", "card-1 svelte-1hev6jh"), r(u, "class", "card-2"), r(a, "class", "left-text svelte-1hev6jh"), r(d, "class", "left-confidence svelte-1hev6jh"), r(c, "class", "left-question svelte-1hev6jh"), r(_, "class", "left-filter svelte-1hev6jh"), r(V, "class", "left-filter2"), r(t, "class", "feedback-left svelte-1hev6jh"), r(M, "class", "right-chart-1 svelte-1hev6jh"), r(A, "class", "right-chart-2 svelte-1hev6jh"), r(E, "class", "right-chart svelte-1hev6jh"), r(Y, "class", "right-table svelte-1hev6jh"), r(O, "class", "feedback-right svelte-1hev6jh"), r(l, "class", "feedback-container svelte-1hev6jh")
         },
-        m(P, J) {
-            W(P, l, J), k(l, t), k(t, a), k(a, n), de(s, n, null), k(a, i), k(a, u), de(o, u, null), k(t, h), k(t, d), de(b, d, null), k(t, p), k(t, c), de(g, c, null), k(t, v), k(t, _), de(w, _, null), k(t, f), k(t, V), de(z, V, null), k(l, H), k(l, O), k(O, E), k(E, M), k(E, m), k(E, A), k(O, T), k(O, Z), de(S, Z, null), j = !0
+        m(P, Z) {
+            L(P, l, Z), k(l, t), k(t, a), k(a, n), de(s, n, null), k(a, i), k(a, u), de(o, u, null), k(t, h), k(t, d), de(b, d, null), k(t, p), k(t, c), de(g, c, null), k(t, v), k(t, _), de(w, _, null), k(t, f), k(t, V), de(z, V, null), k(l, H), k(l, O), k(O, E), k(E, M), k(E, m), k(E, A), k(O, T), k(O, Y), de(S, Y, null), j = !0
         },
         p: $,
         i(P) {
-            j || (U(s.$$.fragment, P), U(o.$$.fragment, P), U(b.$$.fragment, P), U(g.$$.fragment, P), U(w.$$.fragment, P), U(z.$$.fragment, P), U(S.$$.fragment, P), j = !0)
+            j || (K(s.$$.fragment, P), K(o.$$.fragment, P), K(b.$$.fragment, P), K(g.$$.fragment, P), K(w.$$.fragment, P), K(z.$$.fragment, P), K(S.$$.fragment, P), j = !0)
         },
         o(P) {
             x(s.$$.fragment, P), x(o.$$.fragment, P), x(b.$$.fragment, P), x(g.$$.fragment, P), x(w.$$.fragment, P), x(z.$$.fragment, P), x(S.$$.fragment, P), j = !1
         },
         d(P) {
             P && y(l), ge(s), ge(o), ge(b), ge(g), ge(w), ge(z), ge(S)
         }
```

### Comparing `peelml-0.0.1/peelml/client/build/_app/immutable/nodes/9.4133202d.js` & `peelml-0.0.2/peelml/client/build/_app/immutable/nodes/9.21929747.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -14,18 +14,18 @@
     E as v,
     g as l,
     d as i,
     y as $,
     z as y,
     A as b,
     B as S
-} from "../chunks/index.84b8b39e.js";
+} from "../chunks/index.463cc238.js";
 import {
     U as x
-} from "../chunks/UploadFiles.c03ead87.js";
+} from "../chunks/UploadFiles.20ed0f81.js";
 const k = c,
     j = !1,
     q = Object.freeze(Object.defineProperty({
         __proto__: null,
         csr: k,
         prerender: j
     }, Symbol.toStringTag, {
```

### Comparing `peelml-0.0.1/peelml/client/build/about.html` & `peelml-0.0.2/peelml/client/build/about.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/addbook.html` & `peelml-0.0.2/peelml/client/build/addbook.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/chatbot.html` & `peelml-0.0.2/peelml/client/build/chatbot.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/favicon.png` & `peelml-0.0.2/peelml/client/build/favicon.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/index.html` & `peelml-0.0.2/peelml/client/build/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
 		<meta charset="utf-8" />
 		<link rel="icon" href="/favicon.png" />
 		<meta name="viewport" content="width=device-width" />
 		
-		<link rel="modulepreload" href="/_app/immutable/entry/start.dd2cf025.js">
-		<link rel="modulepreload" href="/_app/immutable/chunks/index.84b8b39e.js">
-		<link rel="modulepreload" href="/_app/immutable/chunks/singletons.96029e7d.js">
-		<link rel="modulepreload" href="/_app/immutable/chunks/index.eb24f9d9.js">
-		<link rel="modulepreload" href="/_app/immutable/entry/app.ec7afc1f.js">
+		<link rel="modulepreload" href="/_app/immutable/entry/start.c3258ab5.js">
+		<link rel="modulepreload" href="/_app/immutable/chunks/index.463cc238.js">
+		<link rel="modulepreload" href="/_app/immutable/chunks/singletons.752702b8.js">
+		<link rel="modulepreload" href="/_app/immutable/chunks/index.6ec942b9.js">
+		<link rel="modulepreload" href="/_app/immutable/entry/app.6ffb33b8.js">
 	</head>
 	<body data-sveltekit-preload-data="hover">
 		<div style="display: contents">
 			<script>
 				{
-					__sveltekit_1ul2cy = {
+					__sveltekit_gtqpua = {
 						base: "",
 						env: {}
 					};
 
 					const element = document.currentScript.parentElement;
 
 					Promise.all([
-						import("/_app/immutable/entry/start.dd2cf025.js"),
-						import("/_app/immutable/entry/app.ec7afc1f.js")
+						import("/_app/immutable/entry/start.c3258ab5.js"),
+						import("/_app/immutable/entry/app.6ffb33b8.js")
 					]).then(([kit, app]) => {
 						kit.start(app, element);
 					});
 				}
 			</script>
 		</div>
 	</body>
```

### Comparing `peelml-0.0.1/peelml/client/build/process copy.html` & `peelml-0.0.2/peelml/client/build/process copy.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/process.html` & `peelml-0.0.2/peelml/client/build/process.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/randomnumber.html` & `peelml-0.0.2/peelml/client/build/randomnumber.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/upload.html` & `peelml-0.0.2/peelml/client/build/upload.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/uploadOld.html` & `peelml-0.0.2/peelml/client/build/uploadOld.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/build/uploadTest.html` & `peelml-0.0.2/peelml/client/build/uploadTest.html`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/package-lock.json` & `peelml-0.0.2/peelml/client/package-lock.json`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/package.json` & `peelml-0.0.2/peelml/client/package.json`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/Charts/Bubble.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/Charts/Bubble.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/ChatMessage.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/ChatMessage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/Embedding/ScatterplotGL.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/Embedding/data.js` & `peelml-0.0.2/peelml/client/src/lib/components/Embedding/data.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/Embedding/sequences.js` & `peelml-0.0.2/peelml/client/src/lib/components/Embedding/sequences.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/IndexFiles.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/IndexFiles.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/UploadFiles.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/UploadFiles.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/UploadTest.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/UploadTest.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetCheckBoxes.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/FacetMinMax.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/components/tanstackTable/Table.svelte` & `peelml-0.0.2/peelml/client/src/lib/components/tanstackTable/Table.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/ColumnChart.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/ColumnChart.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/HistogramAnswer.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/HistogramAnswer.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/HistogramQuestion.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/HistogramQuestion.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/HorizontalStackedBar.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardAbsolute.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/MetricCardPercentage.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/MetricCardPercentage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/QACard.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/QACard.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/feedback/QATable.svelte` & `peelml-0.0.2/peelml/client/src/lib/feedback/QATable.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/images/github.svg` & `peelml-0.0.2/peelml/client/src/lib/images/github.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/images/logo.svg` & `peelml-0.0.2/peelml/client/src/lib/images/logo.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/images/svelte-logo.svg` & `peelml-0.0.2/peelml/client/src/lib/images/svelte-logo.svg`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/images/svelte-welcome.png` & `peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/lib/images/svelte-welcome.webp` & `peelml-0.0.2/peelml/client/src/lib/images/svelte-welcome.webp`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/+layout.svelte` & `peelml-0.0.2/peelml/client/src/routes/+layout.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/Counter.svelte` & `peelml-0.0.2/peelml/client/src/routes/Counter.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/Header.svelte` & `peelml-0.0.2/peelml/client/src/routes/Header.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/Sidemenu.svelte` & `peelml-0.0.2/peelml/client/src/routes/Sidemenu.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/about/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/about/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/addbook/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/addbook/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/chatbot/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/chatbot/+page.svelte`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,28 @@
   import { onMount } from "svelte";
 
   let mymessage = "";
   let messageplaceholder = "";
   let chatLoading = false;
 
   onMount(() => {
-    console.log("hey");
-    getDataFromDB();
+    console.log("here we go");
+    if ($chatLog.length < 1) {
+      getDataFromDB();
+    }
   });
 
   async function getDataFromDB() {
+    console.log("fetching data from db");
     const response = await fetch("http://127.0.0.1:5000/preference_table/get");
     const data = await response.json();
     const db = data["preference_result"];
+    // db doesn't appear to be updating correctly...
     $chatLog = [...db];
+    console.log("db", db);
   }
 
   // insert entry into database
   async function insertToDatabase(entry) {
     console.log("INSERT");
     console.log("entry", entry);
     const response = await fetch(
@@ -31,15 +36,18 @@
           "Content-Type": "application/json",
         },
         body: JSON.stringify(entry),
       }
     );
 
     if (response.ok) {
-      console.log("ok!", response);
+      console.log("ok! data inserted", response);
+      console.log("entry", entry);
+      // update chatlog
+      // $chatLog = [...$chatLog, entry];
     } else {
       const err = await response.text();
       alert(err);
     }
   }
 
   const askModel = async (event) => {
@@ -49,15 +57,15 @@
     chatLoading = true;
     let currentEntry = {
       id: $chatLog.length + 1,
       question: mymessage,
       answer: "Loading...",
       vote: "na",
     };
-
+    console.log("adding to log here");
     $chatLog = [...$chatLog, currentEntry];
 
     const response = await fetch(
       `http://127.0.0.1:5000/objects/retrieve/${mymessage}`,
       {
         method: "POST",
         headers: {
@@ -68,15 +76,19 @@
         }),
       }
     );
 
     if (response.ok) {
       const data = await response.json();
       currentEntry["answer"] = data["answer"];
-      $chatLog[$chatLog.length - 1] = currentEntry;
+      // $chatLog[$chatLog.length - 1] = currentEntry;
+      chatLog.update((state) => {
+        state[state.length - 1] = currentEntry;
+        return state;
+      });
       insertToDatabase(currentEntry);
     } else {
       const err = await response.text();
       alert(err);
     }
     chatLoading = false;
   };
@@ -116,14 +128,16 @@
     if (response.ok) {
       console.log("update worked!", response);
     } else {
       const err = await response.text();
       alert(err);
     }
   }
+
+  $: console.log("chat updated!", $chatLog);
 </script>
 
 <section class="chatbox">
   <div class="chat-log">
     {#each $chatLog as message, index (index)}
       <div
         class="chat-message"
```

### Comparing `peelml-0.0.1/peelml/client/src/routes/data/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/data/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/feedback/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/feedback/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/index/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/index/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/normalize.css` & `peelml-0.0.2/peelml/client/src/routes/normalize.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/oldpage.svelte` & `peelml-0.0.2/peelml/client/src/routes/oldpage.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/process/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/process/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/process copy/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/process copy/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/styles.css` & `peelml-0.0.2/peelml/client/src/routes/styles.css`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/routes/upload/+page.svelte` & `peelml-0.0.2/peelml/client/src/routes/upload/+page.svelte`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/store.js` & `peelml-0.0.2/peelml/client/src/store.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/src/utils.js` & `peelml-0.0.2/peelml/client/src/utils.js`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/client/static/favicon.png` & `peelml-0.0.2/peelml/client/static/favicon.png`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/duck/answer_table.py` & `peelml-0.0.2/peelml/duck/answer_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/duck/preference_table.py` & `peelml-0.0.2/peelml/duck/preference_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/duck/question_table.py` & `peelml-0.0.2/peelml/duck/question_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/duck/ranking_table.py` & `peelml-0.0.2/peelml/duck/ranking_table.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/llm/embedding_factory.py` & `peelml-0.0.2/peelml/llm/embedding_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/llm/llama_cpp.py` & `peelml-0.0.2/peelml/llm/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/llm/model_factory.py` & `peelml-0.0.2/peelml/llm/model_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/llm/openai.py` & `peelml-0.0.2/peelml/llm/openai.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/llm/sagemaker.py` & `peelml-0.0.2/peelml/llm/sagemaker.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/model/sagemaker.py` & `peelml-0.0.2/peelml/model/sagemaker.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/server.py` & `peelml-0.0.2/peelml/server.py`

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
-    os.environ["OPENAI_API_KEY"] = ""
+    os.environ["OPENAI_API_KEY"] = "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"
     app.config["vectordb"] = "chroma"
     app.config["model"] = "openai"
     if os.environ["OPENAI_API_KEY"] == "":
         raise ValueError("OPENAI_API_KEY is not set")
     app.run(port=5000, debug=True)
```

### Comparing `peelml-0.0.1/peelml/vectordb/abs_vectordb.py` & `peelml-0.0.2/peelml/vectordb/abs_vectordb.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/vectordb/chroma.py` & `peelml-0.0.2/peelml/vectordb/chroma.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/peelml/vectordb/vectordb_factory.py` & `peelml-0.0.2/peelml/vectordb/vectordb_factory.py`

 * *Files identical despite different names*

### Comparing `peelml-0.0.1/pyproject.toml` & `peelml-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peelml"
-version = "0.0.1"
+version = "0.0.2"
 description = "Peel away the pain of ml deployment"
 authors = ["Rachel Hu <goldpiggy@berkeley.edu>"]
 maintainers = [
     "Jared Wilber <jdwlbr@gmail.com>",
     "Rachel Hu <goldpiggy@berkeley.edu>"
     ]
 readme = "README.md"
@@ -31,15 +31,17 @@
 sagemaker = "2.169.0"
 numba = "0.57.1"
 llvmlite = "0.40.1"
 umap = "0.1.1"
 umap-learn = "0.5.3"
 scikit-learn = "1.3.0"
 duckdb = "0.8.1"
-fastapi = "0.98.0"
+fastapi = "0.100.0"
+pydantic = "1.10.11"
+starlette = "0.27.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 peelml = "peelml.cli:cli"
```

### Comparing `peelml-0.0.1/PKG-INFO` & `peelml-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peelml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Peel away the pain of ml deployment
 Author: Rachel Hu
 Author-email: goldpiggy@berkeley.edu
 Maintainer: Jared Wilber
 Maintainer-email: jdwlbr@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -12,28 +12,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (==1.26.165)
 Requires-Dist: chromadb (==0.3.26)
 Requires-Dist: click (==8.0.4)
 Requires-Dist: docx2txt (==0.8)
 Requires-Dist: duckdb (==0.8.1)
-Requires-Dist: fastapi (==0.98.0)
+Requires-Dist: fastapi (==0.100.0)
 Requires-Dist: flask (==2.2.3)
 Requires-Dist: flask-cors (==4.0.0)
 Requires-Dist: inquirer (==3.1.3)
 Requires-Dist: langchain (==0.0.220)
 Requires-Dist: llama-cpp-python (==0.1.66)
 Requires-Dist: llvmlite (==0.40.1)
 Requires-Dist: numba (==0.57.1)
 Requires-Dist: openai (==0.27.8)
 Requires-Dist: pdfminer-six (==20221105)
 Requires-Dist: poetry (==1.4.2)
+Requires-Dist: pydantic (==1.10.11)
 Requires-Dist: python-dotenv (==1.0.0)
 Requires-Dist: sagemaker (==2.169.0)
 Requires-Dist: scikit-learn (==1.3.0)
+Requires-Dist: starlette (==0.27.0)
 Requires-Dist: tiktoken (==0.4.0)
 Requires-Dist: tokenizers (==0.13.3)
 Requires-Dist: typer (==0.9.0)
 Requires-Dist: umap (==0.1.1)
 Requires-Dist: umap-learn (==0.5.3)
 Requires-Dist: virtualenv (==20.16.5)
 Description-Content-Type: text/markdown
```

