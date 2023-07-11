# Comparing `tmp/bbot-1.0.5.1817rc0.tar.gz` & `tmp/bbot-1.0.5.1821rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1817rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1821rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1817rc0.tar` & `bbot-1.0.5.1821rc0.tar`

### file list

```diff
@@ -1,283 +1,283 @@
--rw-r--r--   0        0        0    32473 2023-07-11 18:39:32.678112 bbot-1.0.5.1817rc0/LICENSE
--rw-r--r--   0        0        0    51778 2023-07-11 18:39:32.678112 bbot-1.0.5.1817rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-11 18:40:00.154777 bbot-1.0.5.1817rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14606 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5150 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9311 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    27442 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    34828 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14831 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2251 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13229 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3786 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25482 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4760 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-11 18:39:32.682112 bbot-1.0.5.1817rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      680 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5520 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13670 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11304 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7437 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5749 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9552 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5124 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1820 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1315 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1395 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     7296 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2273 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1744 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-11 18:39:32.686112 bbot-1.0.5.1817rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11359 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1711 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10812 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     2668 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0    15109 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    24751 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7959 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     7688 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     6867 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-11 18:39:32.690112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1726 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0     9708 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     5562 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-11 18:39:32.694112 bbot-1.0.5.1817rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-11 18:39:32.702112 bbot-1.0.5.1817rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-11 18:40:00.154777 bbot-1.0.5.1817rc0/pyproject.toml
--rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1817rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/LICENSE
+-rw-r--r--   0        0        0    51778 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-11 18:56:26.764174 bbot-1.0.5.1821rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14606 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5150 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9311 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    27442 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    34834 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14831 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2251 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13229 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3786 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25482 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4760 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      680 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5520 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13670 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15858 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11304 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7437 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5749 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9552 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5124 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     4269 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     4993 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1820 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     8363 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2273 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1744 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11359 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1711 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10812 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     2681 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0    15109 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    24751 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7959 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     7688 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     6867 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1726 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      419 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2107 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10661 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2124 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     5562 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-07-11 18:56:26.764174 bbot-1.0.5.1821rc0/pyproject.toml
+-rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1821rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1817rc0/LICENSE` & `bbot-1.0.5.1821rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/README.md` & `bbot-1.0.5.1821rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/agent/agent.py` & `bbot-1.0.5.1821rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/cli.py` & `bbot-1.0.5.1821rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1821rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1821rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1821rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1821rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/errors.py` & `bbot-1.0.5.1821rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/event/base.py` & `bbot-1.0.5.1821rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1821rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/files.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -377,24 +377,24 @@
 
 
 def extract_params_json(json_data):
     try:
         data = json.loads(json_data)
     except json.JSONDecodeError:
         log.debug("Invalid JSON supplied. Returning empty list.")
-        return []
+        return set()
 
-    keys = []
+    keys = set()
     stack = [data]
 
     while stack:
         current_data = stack.pop()
         if isinstance(current_data, dict):
             for key, value in current_data.items():
-                keys.append(key)
+                keys.add(key)
                 if isinstance(value, (dict, list)):
                     stack.append(value)
         elif isinstance(current_data, list):
             for item in current_data:
                 if isinstance(item, (dict, list)):
                     stack.append(item)
 
@@ -402,22 +402,22 @@
 
 
 def extract_params_xml(xml_data):
     try:
         root = ET.fromstring(xml_data)
     except ET.ParseError:
         log.debug("Invalid XML supplied. Returning empty list.")
-        return []
+        return set()
 
-    tags = []
+    tags = set()
     stack = [root]
 
     while stack:
         current_element = stack.pop()
-        tags.append(current_element.tag)
+        tags.add(current_element.tag)
         for child in current_element:
             stack.append(child)
     return tags
 
 
 def extract_params_html(html_data):
     input_tag = regexes.input_tag_regex.findall(html_data)
```

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1821rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1821rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1821rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/defaults.yml` & `bbot-1.0.5.1821rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1821rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1821rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1821rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/base.py` & `bbot-1.0.5.1821rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1821rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1821rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1821rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1821rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1821rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1821rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1821rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1821rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1821rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/c99.py` & `bbot-1.0.5.1821rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/censys.py` & `bbot-1.0.5.1821rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1821rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/columbus.py` & `bbot-1.0.5.1821rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1821rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/crt.py` & `bbot-1.0.5.1821rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1821rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1821rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1821rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1821rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1821rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1821rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1821rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1821rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1821rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1821rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1821rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/git.py` & `bbot-1.0.5.1821rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/github.py` & `bbot-1.0.5.1821rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1821rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1821rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1821rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1821rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1821rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1821rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1821rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1821rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1821rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1821rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1821rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1821rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1821rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1821rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1821rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/myssl.py` & `bbot-1.0.5.1821rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1821rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/nmap.py` & `bbot-1.0.5.1821rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/nsec.py` & `bbot-1.0.5.1821rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1821rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/otx.py` & `bbot-1.0.5.1821rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1821rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1821rc0/bbot/modules/paramminer_cookies.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,18 +8,27 @@
 
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-paramminer"]
     meta = {
         "description": "Smart brute-force to check for common HTTP cookie parameters",
     }
-    options = {"wordlist": ""}  # default is defined separately
+    options = {
+        "wordlist": "",  # default is defined within setup function
+        "http_extract": True,
+        "skip_boring_words": True,
+    }
+    options_desc = {
+        "wordlist": "Define the wordlist to be used to derive headers",
+        "http_extract": "Attempt to find additional wordlist words from the HTTP Response",
+        "skip_boring_words": "Remove commonly uninteresting words from the wordlist",
+    }
     options_desc = {"wordlist": "Define the wordlist to be used to derive cookies"}
     scanned_hosts = []
-    boringlist = []
+    boring_words = set()
     max_event_handlers = 12
     in_scope_only = True
     compare_mode = "cookie"
     default_wordlist = "paramminer_parameters.txt"
 
     async def check_batch(self, compare_helper, url, cookie_list):
         cookies = {p: self.rand_string(14) for p in cookie_list}
```

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1821rc0/bbot/modules/paramminer_headers.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     }
     options_desc = {
         "wordlist": "Define the wordlist to be used to derive headers",
         "http_extract": "Attempt to find additional wordlist words from the HTTP Response",
         "skip_boring_words": "Remove commonly uninteresting words from the wordlist",
     }
     scanned_hosts = []
-    boringlist = [
+    boring_words = {
         "accept",
         "accept-encoding",
         "accept-language",
         "action",
         "authorization",
         "cf-connecting-ip",
         "connection",
@@ -64,85 +64,103 @@
         "zaccess-control-request-method",
         "zmax-forwards",
         "zorigin",
         "zreferrer",
         "zvia",
         "zx-request-id",
         "zx-timer",
-    ]
+    }
     max_event_handlers = 12
     in_scope_only = True
     compare_mode = "header"
     default_wordlist = "paramminer_headers.txt"
 
     async def setup(self):
+        self.event_dict = {}
         wordlist = self.config.get("wordlist", "")
         if not wordlist:
             wordlist = f"{self.helpers.wordlist_dir}/{self.default_wordlist}"
         self.debug(f"Using wordlist: [{wordlist}]")
-        self.wordlist = await self.helpers.wordlist(wordlist)
+        self.wl = set(
+            h.strip().lower()
+            for h in self.helpers.read_file(await self.helpers.wordlist(wordlist))
+            if len(h) > 0 and "%" not in h
+        )
+
+        # check against the boring list (if the option is set)
+
+        if self.config.get("skip_boring_words", True):
+            self.wl -= self.boring_words
+        self.matched_words = {}
         return True
 
     def rand_string(self, *args, **kwargs):
         return self.helpers.rand_string(*args, **kwargs)
 
-    async def handle_event(self, event):
-        url = event.data.get("url")
-        try:
-            compare_helper = self.helpers.http_compare(url)
-        except HttpCompareError as e:
-            self.debug(e)
-            return
-        batch_size = await self.count_test(url)
-        if batch_size == None or batch_size <= 0:
-            self.debug(f"Failed to get baseline max {self.compare_mode} count, aborting")
-            return
-        self.debug(f"Resolved batch_size at {str(batch_size)}")
-
-        if await compare_helper.canary_check(url, mode=self.compare_mode) == False:
-            self.verbose(f'Aborting "{url}" due to failed canary check')
-            return
-
-        wl_raw = [h.strip().lower() for h in self.helpers.read_file(self.wordlist)]
-
-        # clean list against the boring list, if the option is set
-        if self.config.get("skip_boring_words", True):
-            wl = list(filter(self.clean_list, wl_raw))
-        else:
-            wl = wl_raw
-
-        if self.config.get("http_extract"):
-            wl = self.load_extracted_words(wl, event.data.get("body"), event.data.get("content_type"))
+    async def do_mining(self, wl, url, batch_size, compare_helper):
         results = set()
         abort_threshold = 25
         try:
             for group in self.helpers.grouper(wl, batch_size):
                 async for result, reasons, reflection in self.binary_search(compare_helper, url, group):
                     results.add((result, ",".join(reasons), reflection))
                     if len(results) >= abort_threshold:
                         self.warning(
                             f"Abort threshold ({abort_threshold}) reached, too many {self.compare_mode}s found"
                         )
                         results.clear()
                         assert False
         except AssertionError:
             pass
+        return results
 
+    def process_results(self, event, results):
+        url = event.data.get("url")
         for result, reasons, reflection in results:
             tags = []
             if reflection:
                 tags = ["http_reflection"]
             description = f"[Paramminer] {self.compare_mode.capitalize()}: [{result}] Reasons: [{reasons}] Reflection: [{str(reflection)}]"
             self.emit_event(
                 {"host": str(event.host), "url": url, "description": description},
                 "FINDING",
                 event,
                 tags=tags,
             )
 
+    async def handle_event(self, event):
+        url = event.data.get("url")
+
+        try:
+            compare_helper = self.helpers.http_compare(url)
+        except HttpCompareError as e:
+            self.debug(e)
+            return
+        batch_size = await self.count_test(url)
+        if batch_size == None or batch_size <= 0:
+            self.debug(f"Failed to get baseline max {self.compare_mode} count, aborting")
+            return
+        self.debug(f"Resolved batch_size at {str(batch_size)}")
+
+        self.event_dict[url] = (event, batch_size)
+
+        if await compare_helper.canary_check(url, mode=self.compare_mode) == False:
+            self.verbose(f'Aborting "{url}" due to failed canary check')
+            return
+
+        wl = set(self.wl)
+        if self.config.get("http_extract"):
+            extracted_words = self.load_extracted_words(event.data.get("body"), event.data.get("content_type"))
+            self.matched_words[url] = extracted_words
+            wl |= extracted_words
+            if self.config.get("skip_boring_words", True):
+                wl -= self.boring_words
+        results = await self.do_mining(wl, url, batch_size, compare_helper)
+        self.process_results(event, results)
+
     async def count_test(self, url):
         baseline = await self.helpers.request(url)
         if baseline is None:
             return
         if str(baseline.status_code)[0] in ("4", "5"):
             return
         for count, args, kwargs in self.gen_count_args(url):
@@ -157,44 +175,53 @@
                 break
             fake_headers = {}
             for i in range(0, header_count):
                 fake_headers[self.rand_string(14)] = self.rand_string(14)
             yield header_count, (url,), {"headers": fake_headers}
             header_count -= 5
 
-    def clean_list(self, header):
-        if (len(header) > 0) and ("%" not in header) and (header not in self.boringlist):
-            return True
-        return False
-
-    def load_extracted_words(self, wl, body, content_type):
+    def load_extracted_words(self, body, content_type):
         if "json" in content_type.lower():
-            return wl + extract_params_json(body)
+            return extract_params_json(body)
         elif "xml" in content_type.lower():
-            return wl + extract_params_xml(body)
+            return extract_params_xml(body)
         else:
-            return wl + list(extract_params_html(body))
-
-        return wl
+            return set(extract_params_html(body))
 
     async def binary_search(self, compare_helper, url, group, reasons=None, reflection=False):
         if reasons is None:
             reasons = []
         self.debug(f"Entering recursive binary_search with {len(group):,} sized group")
-        if len(group) == 1:
-            if reasons:
-                yield group[0], reasons, reflection
-        elif len(group) > 1:
+        if len(group) == 1 and len(reasons) > 0:
+            yield group[0], reasons, reflection
+        elif len(group) > 1 or (len(group) == 1 and len(reasons) == 0):
             for group_slice in self.helpers.split_list(group):
                 match, reasons, reflection, subject_response = await self.check_batch(compare_helper, url, group_slice)
                 if match == False:
                     async for r in self.binary_search(compare_helper, url, group_slice, reasons, reflection):
                         yield r
         else:
             self.warning(f"Submitted group of size 0 to binary_search()")
 
     async def check_batch(self, compare_helper, url, header_list):
         rand = self.rand_string()
         test_headers = {}
         for header in header_list:
             test_headers[header] = rand
         return await compare_helper.compare(url, headers=test_headers, check_reflection=(len(header_list) == 1))
+
+    async def finish(self):
+        for url, (event, batch_size) in self.event_dict.items():
+            compare_helper = self.helpers.http_compare(url)
+
+            untested_matches = set()
+            for k, s in self.matched_words.items():
+                if k != url:
+                    untested_matches.update(s)
+
+            untested_matches -= self.wl
+
+            if self.config.get("skip_boring_words", True):
+                untested_matches -= self.boring_words
+
+            results = await self.do_mining(untested_matches, url, batch_size, compare_helper)
+            self.process_results(event, results)
```

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1821rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1821rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1821rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1821rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1821rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1821rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/robots.py` & `bbot-1.0.5.1821rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1821rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1821rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1821rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1821rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1821rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/social.py` & `bbot-1.0.5.1821rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1821rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1821rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1821rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1821rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1821rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1821rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1821rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1821rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1821rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1821rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1821rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1821rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/scanner/dispatcher.py` & `bbot-1.0.5.1821rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1821rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1821rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1821rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/scanner/target.py` & `bbot-1.0.5.1821rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1821rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/conftest.py` & `bbot-1.0.5.1821rc0/bbot/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     shutil.rmtree("/tmp/.bbot_test", ignore_errors=True)
 
     yield
 
 
 @pytest.fixture
 def non_mocked_hosts() -> list:
-    return ["127.0.0.1"] + interactsh_servers
+    return ["127.0.0.1", "localhost"] + interactsh_servers
 
 
 @pytest.fixture
 def assert_all_responses_were_requested() -> bool:
     return False
```

### Comparing `bbot-1.0.5.1817rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1821rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test.conf` & `bbot-1.0.5.1821rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,24 +61,28 @@
         assert any(
             e.type == "FINDING"
             and "[Paramminer] Getparam: [id] Reasons: [body] Reflection: [False]" in e.data["description"]
             for e in events
         )
 
 
+class TestParamminer_Getparams_singlewordlist(TestParamminer_Getparams):
+    config_overrides = {"modules": {"paramminer_getparams": {"wordlist": tempwordlist(["id"])}}}
+
+
 class TestParamminer_Getparams_boring_off(TestParamminer_Getparams):
     config_overrides = {
         "modules": {
             "paramminer_getparams": {"skip_boring_words": False, "wordlist": tempwordlist(["canary", "boring"])}
         }
     }
 
     async def setup_after_prep(self, module_test):
         module_test.scan.modules["paramminer_getparams"].rand_string = lambda *args, **kwargs: "AAAAAAAAAAAAAA"
-        module_test.scan.modules["paramminer_getparams"].boringlist = ["boring"]
+        module_test.scan.modules["paramminer_getparams"].boring_words = {"boring"}
         module_test.monkeypatch.setattr(
             helper.HttpCompare, "gen_cache_buster", lambda *args, **kwargs: {"AAAAAA": "1"}
         )
         expect_args = {"query_string": b"boring=AAAAAAAAAAAAAA&AAAAAA=1"}
         respond_args = {"response_data": self.getparam_body_match}
         module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
@@ -104,17 +108,15 @@
             e.type == "FINDING" and "[Paramminer] Getparam: [boring] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
 class TestParamminer_Getparams_Extract_Json(TestParamminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
-    config_overrides = {
-        "modules": {"paramminer_getparams": {"wordlist": tempwordlist(["canary", "id"]), "http_extract": True}}
-    }
+    config_overrides = {"modules": {"paramminer_getparams": {"wordlist": tempwordlist([]), "http_extract": True}}}
 
     getparam_extract_json = """
     {
   "obscureParameter": 1,
   "common": 1
 }
     """
@@ -128,21 +130,14 @@
 
     async def setup_after_prep(self, module_test):
         module_test.scan.modules["paramminer_getparams"].rand_string = lambda *args, **kwargs: "AAAAAAAAAAAAAA"
         module_test.monkeypatch.setattr(
             helper.HttpCompare, "gen_cache_buster", lambda *args, **kwargs: {"AAAAAA": "1"}
         )
 
-        expect_args = {"query_string": b"obscureParameter=AAAAAAAAAAAAAA&common=AAAAAAAAAAAAAA&AAAAAA=1"}
-        respond_args = {
-            "response_data": self.getparam_extract_json_match,
-            "headers": {"Content-Type": "application/json"},
-        }
-        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
-
         expect_args = {"query_string": b"obscureParameter=AAAAAAAAAAAAAA&AAAAAA=1"}
         respond_args = {
             "response_data": self.getparam_extract_json_match,
             "headers": {"Content-Type": "application/json"},
         }
         module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
@@ -155,15 +150,19 @@
             and "[Paramminer] Getparam: [obscureParameter] Reasons: [body]" in e.data["description"]
             for e in events
         )
 
 
 class TestParamminer_Getparams_Extract_Xml(TestParamminer_Headers):
     modules_overrides = ["httpx", "paramminer_getparams"]
-    config_overrides = {"modules": {"paramminer_getparams": {"wordlist": tempwordlist([]), "http_extract": True}}}
+    config_overrides = {
+        "modules": {
+            "paramminer_getparams": {"wordlist": tempwordlist([]), "http_extract": True, "skip_boring_words": True}
+        }
+    }
 
     getparam_extract_xml = """
 <data>
     <obscureParameter>1</obscureParameter>
     <common>1</common>
 </data>
     """
@@ -176,30 +175,15 @@
     """
 
     async def setup_after_prep(self, module_test):
         module_test.scan.modules["paramminer_getparams"].rand_string = lambda *args, **kwargs: "AAAAAAAAAAAAAA"
         module_test.monkeypatch.setattr(
             helper.HttpCompare, "gen_cache_buster", lambda *args, **kwargs: {"AAAAAA": "1"}
         )
-
-        expect_args = {
-            "query_string": b"data=AAAAAAAAAAAAAA&obscureParameter=AAAAAAAAAAAAAA&common=AAAAAAAAAAAAAA&AAAAAA=1"
-        }
-        respond_args = {
-            "response_data": self.getparam_extract_xml_match,
-            "headers": {"Content-Type": "application/xml"},
-        }
-        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
-
-        expect_args = {"query_string": b"common=AAAAAAAAAAAAAA&obscureParameter=AAAAAAAAAAAAAA&AAAAAA=1"}
-        respond_args = {
-            "response_data": self.getparam_extract_xml_match,
-            "headers": {"Content-Type": "application/xml"},
-        }
-        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+        module_test.scan.modules["paramminer_getparams"].boring_words = {"data", "common"}
 
         expect_args = {"query_string": b"obscureParameter=AAAAAAAAAAAAAA&AAAAAA=1"}
         respond_args = {
             "response_data": self.getparam_extract_xml_match,
             "headers": {"Content-Type": "application/xml"},
         }
         module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
@@ -247,7 +231,52 @@
         module_test.set_expect_requests(respond_args=respond_args)
 
     def check(self, module_test, events):
         assert any(
             e.type == "FINDING" and "[Paramminer] Getparam: [hack] Reasons: [body]" in e.data["description"]
             for e in events
         )
+
+
+class TestParamminer_Getparams_finish(TestParamminer_Headers):
+    modules_overrides = ["httpx", "excavate", "paramminer_getparams"]
+    config_overrides = {
+        "modules": {"paramminer_getparams": {"wordlist": tempwordlist(["canary", "canary2"]), "http_extract": True}}
+    }
+
+    targets = ["http://127.0.0.1:8888/test1.php", "http://127.0.0.1:8888/test2.php"]
+
+    test_1_html = """
+<html><a href="/test2.php?abcd1234=foo">paramstest2</a></html>
+    """
+
+    test_2_html = """
+<html></a><p>Hello</p></html>
+    """
+
+    test_2_html_match = """
+<html></a><p>HackThePlanet!</p></html>
+    """
+
+    async def setup_after_prep(self, module_test):
+        module_test.scan.modules["paramminer_getparams"].rand_string = lambda *args, **kwargs: "AAAAAAAAAAAAAA"
+        module_test.monkeypatch.setattr(
+            helper.HttpCompare, "gen_cache_buster", lambda *args, **kwargs: {"AAAAAA": "1"}
+        )
+
+        expect_args = {"uri": "/test2.php", "query_string": b"abcd1234=AAAAAAAAAAAAAA&AAAAAA=1"}
+        respond_args = {"response_data": self.test_2_html_match}
+        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+        expect_args = {"uri": "/test2.php"}
+        respond_args = {"response_data": self.test_2_html}
+        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+        expect_args = {"uri": "/test1.php"}
+        respond_args = {"response_data": self.test_1_html}
+        module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
+
+    def check(self, module_test, events):
+        assert any(
+            e.type == "FINDING" and "[abcd1234] Reasons: [body] Reflection: [False]" in e.data["description"]
+            for e in events
+        )
```

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/testsslcert.pem` & `bbot-1.0.5.1821rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/test/testsslkey.pem` & `bbot-1.0.5.1821rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1821rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1821rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1821rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1821rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1817rc0/pyproject.toml` & `bbot-1.0.5.1821rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1817rc"
+version = "v1.0.5.1821rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1817rc0/PKG-INFO` & `bbot-1.0.5.1821rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1817rc0
+Version: 1.0.5.1821rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

