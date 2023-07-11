# Comparing `tmp/bbot-1.0.5.1839rc0.tar.gz` & `tmp/bbot-1.1.0.1903rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1839rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.0.1903rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1839rc0.tar` & `bbot-1.1.0.1903rc0.tar`

### file list

```diff
@@ -1,283 +1,286 @@
--rw-r--r--   0        0        0    32473 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/LICENSE
--rw-r--r--   0        0        0    51778 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-11 21:31:20.657490 bbot-1.0.5.1839rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14606 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5247 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-11 21:30:56.593060 bbot-1.0.5.1839rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9311 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    28361 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    34332 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14831 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2240 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13681 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4078 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25482 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4851 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      680 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5718 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13670 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-11 21:30:56.597060 bbot-1.0.5.1839rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11304 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7437 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5795 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9552 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5124 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1820 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     8575 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2273 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1744 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11359 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1711 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-11 21:30:56.601060 bbot-1.0.5.1839rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10812 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     3987 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0    15109 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    24751 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7959 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     7688 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     8916 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-11 21:30:56.605060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10661 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     5562 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-11 21:30:56.609060 bbot-1.0.5.1839rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-11 21:30:56.617060 bbot-1.0.5.1839rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-11 21:31:20.657490 bbot-1.0.5.1839rc0/pyproject.toml
--rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1839rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/LICENSE
+-rw-r--r--   0        0        0     6762 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-11 21:34:30.835101 bbot-1.1.0.1903rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14945 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-11 21:34:05.782396 bbot-1.1.0.1903rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9721 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5290 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1314 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1115 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       61 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9311 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    28361 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    34635 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    17481 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2240 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13681 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8020 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4094 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25482 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-11 21:34:05.786396 bbot-1.1.0.1903rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      908 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5718 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13670 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15858 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11304 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7437 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5795 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9552 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5124 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     4269 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     4993 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1845 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     8575 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2273 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1744 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-11 21:34:05.790397 bbot-1.1.0.1903rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11359 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1711 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     4763 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10812 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    15109 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    24751 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7957 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     8129 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     8916 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-07-11 21:34:05.794397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      419 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2107 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10661 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2124 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     5562 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-11 21:34:05.798397 bbot-1.1.0.1903rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-11 21:34:05.806397 bbot-1.1.0.1903rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-07-11 21:34:30.835101 bbot-1.1.0.1903rc0/pyproject.toml
+-rw-r--r--   0        0        0     8164 1970-01-01 00:00:00.000000 bbot-1.1.0.1903rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1839rc0/LICENSE` & `bbot-1.1.0.1903rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/agent/agent.py` & `bbot-1.1.0.1903rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/cli.py` & `bbot-1.1.0.1903rc0/bbot/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,28 +224,36 @@
                 help_modules = list(modules)
                 if module_filtering:
                     help_modules = None
 
                 if options.help_all:
                     log_fn(parser.format_help())
 
+                if options.list_flags:
+                    log.stdout("")
+                    log.stdout("### FLAGS ###")
+                    log.stdout("")
+                    for row in module_loader.flags_table(flags=options.flags).splitlines():
+                        log.stdout(row)
+                    return
+
                 log_fn("")
                 log_fn("### MODULES ###")
                 log_fn("")
                 for row in module_loader.modules_table(modules=help_modules).splitlines():
                     log_fn(row)
 
                 if options.help_all:
                     log_fn("")
                     log_fn("### MODULE OPTIONS ###")
                     log_fn("")
                     for row in module_loader.modules_options_table(modules=help_modules).splitlines():
                         log_fn(row)
 
-                if options.list_modules or options.help_all:
+                if options.list_modules or options.list_flags or options.help_all:
                     return
 
                 module_list = module_loader.filter_modules(modules=modules)
                 deadly_modules = []
                 active_modules = []
                 active_aggressive_modules = []
                 slow_modules = []
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.0.1903rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/configurator/args.py` & `bbot-1.1.0.1903rc0/bbot/core/configurator/args.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
     def parse_args(self, *args, **kwargs):
         """
         Allow space or comma-separated entries for modules and targets
         For targets, also allow input files containing additional targets
         """
         ret = super().parse_args(*args, **kwargs)
+        # silent implies -y
+        if ret.silent:
+            ret.yes = True
         ret.modules = chain_lists(ret.modules)
         ret.output_modules = chain_lists(ret.output_modules)
         ret.targets = chain_lists(ret.targets, try_files=True, msg="Reading targets from file: {filename}")
         ret.whitelist = chain_lists(ret.whitelist, try_files=True, msg="Reading whitelist from file: {filename}")
         ret.blacklist = chain_lists(ret.blacklist, try_files=True, msg="Reading blacklist from file: {filename}")
         ret.flags = chain_lists(ret.flags)
         ret.require_flags = chain_lists(ret.require_flags)
@@ -51,38 +54,65 @@
 class DummyArgumentParser(BBOTArgumentParser):
     _dummy = True
 
     def error(self, message):
         pass
 
 
-epilog = """EXAMPLES
-
-    Subdomains:
-        bbot -t evilcorp.com -f subdomain-enum
-
-    Subdomains (passive only):
-        bbot -t evilcorp.com -f subdomain-enum -rf passive
-
-    Subdomains + port scan + web screenshots:
-        bbot -t evilcorp.com -f subdomain-enum -m naabu gowitness -n my_scan -o .
-
-    Subdomains + basic web scan (wappalyzer, robots.txt, iis shortnames, etc.):
-        bbot -t evilcorp.com -f subdomain-enum web-basic
-
-    Subdomains + web spider (search for emails, etc.):
-        bbot -t evilcorp.com -f subdomain-enum -c web_spider_distance=2 web_spider_depth=2
-
-    Subdomains + emails + cloud + port scan + non-intrusive web + web screenshots + nuclei:
-        bbot -t evilcorp.com -f subdomain-enum email-enum cloud-enum web-basic -m naabu gowitness nuclei --allow-deadly
-
-    List modules:
-        bbot -l
-
-"""
+scan_examples = [
+    (
+        "Subdomains",
+        "Perform a full subdomain enumeration on evilcorp.com",
+        "bbot -t evilcorp.com -f subdomain-enum",
+    ),
+    (
+        "Subdomains (passive only)",
+        "Perform a passive-only subdomain enumeration on evilcorp.com",
+        "bbot -t evilcorp.com -f subdomain-enum -rf passive",
+    ),
+    (
+        "Subdomains + port scan + web screenshots",
+        "Port-scan every subdomain, screenshot every webpage, output to current directory",
+        "bbot -t evilcorp.com -f subdomain-enum -m nmap gowitness -n my_scan -o .",
+    ),
+    (
+        "Subdomains + basic web scan",
+        "A basic web scan includes wappalyzer, robots.txt, and other non-intrusive web modules",
+        "bbot -t evilcorp.com -f subdomain-enum web-basic",
+    ),
+    (
+        "Web spider",
+        "Crawl www.evilcorp.com up to a max depth of 2, automatically extracting emails, secrets, etc.",
+        "bbot -t www.evilcorp.com -m httpx robots badsecrets secretsdb -c web_spider_distance=2 web_spider_depth=2",
+    ),
+    (
+        "Everything everywhere all at once",
+        "Subdomains, emails, cloud buckets, port scan, basic web, web screenshots, nuclei",
+        "bbot -t evilcorp.com -f subdomain-enum email-enum cloud-enum web-basic -m nmap gowitness nuclei --allow-deadly",
+    ),
+]
+
+usage_examples = [
+    (
+        "List modules",
+        "",
+        "bbot -l",
+    ),
+    (
+        "List flags",
+        "",
+        "bbot -lf",
+    ),
+]
+
+
+epilog = "EXAMPLES\n"
+for example in (scan_examples, usage_examples):
+    for title, description, command in example:
+        epilog += f"\n    {title}:\n        {command}\n"
 
 
 parser = BBOTArgumentParser(
     description="Bighuge BLS OSINT Tool", formatter_class=argparse.RawTextHelpFormatter, epilog=epilog
 )
 dummy_parser = DummyArgumentParser(
     description="Bighuge BLS OSINT Tool", formatter_class=argparse.RawTextHelpFormatter, epilog=epilog
@@ -121,14 +151,15 @@
         "-f",
         "--flags",
         nargs="+",
         default=[],
         help=f'Enable modules by flag. Choices: {",".join(sorted(flag_choices))}',
         metavar="FLAG",
     )
+    modules.add_argument("-lf", "--list-flags", action="store_true", help=f"List available flags.")
     modules.add_argument(
         "-rf",
         "--require-flags",
         nargs="+",
         default=[],
         help=f"Only enable modules with these flags (e.g. -rf passive)",
         metavar="FLAG",
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/configurator/environ.py` & `bbot-1.1.0.1903rc0/bbot/core/configurator/environ.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,20 +110,21 @@
         if args.cli_options.output_dir:
             bbot_config["output_dir"] = args.cli_options.output_dir
 
     import logging
 
     log = logging.getLogger()
     if bbot_config.get("debug", False):
-        global _log_level_override
         bbot_config["silent"] = False
-        _log_level_override = logging.DEBUG
         log = logging.getLogger("bbot")
         log.setLevel(logging.DEBUG)
         logging.getLogger("asyncio").setLevel(logging.DEBUG)
+    elif bbot_config.get("silent", False):
+        log = logging.getLogger("bbot")
+        log.setLevel(logging.CRITICAL)
 
     # copy config to environment
     bbot_environ = flatten_config(bbot_config)
     os.environ.update(bbot_environ)
 
     # handle HTTP proxy
     http_proxy = bbot_config.get("http_proxy", "")
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/configurator/files.py` & `bbot-1.1.0.1903rc0/bbot/core/configurator/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 from pathlib import Path
 from omegaconf import OmegaConf
 
 from ..helpers.misc import mkdir
 from ..errors import ConfigLoadError
 from ..helpers.logger import log_to_stderr
 
@@ -9,15 +10,18 @@
 defaults_filename = (Path(__file__).parent.parent.parent / "defaults.yml").resolve()
 mkdir(config_dir)
 config_filename = (config_dir / "bbot.yml").resolve()
 secrets_filename = (config_dir / "secrets.yml").resolve()
 default_config = None
 
 
-def _get_config(filename, name="config", notify=True):
+def _get_config(filename, name="config"):
+    notify = False
+    if sys.argv and sys.argv[0].endswith("bbot") and not any(x in sys.argv for x in ("-s", "--silent")):
+        notify = True
     filename = Path(filename).resolve()
     try:
         conf = OmegaConf.load(str(filename))
         if notify:
             log_to_stderr(f"Loaded {name} from {filename}")
         return conf
     except Exception as e:
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/errors.py` & `bbot-1.1.0.1903rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/event/base.py` & `bbot-1.1.0.1903rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/event/helpers.py` & `bbot-1.1.0.1903rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/cache.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/command.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/diff.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/dns.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/files.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/helper.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/logger.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/misc.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -906,18 +906,26 @@
     +-----------+-----------+
     | row2      | row2      |
     +-----------+-----------+
     """
     # fix IndexError: list index out of range
     if args and not args[0]:
         args = ([[]],) + args[1:]
-    defaults = {"tablefmt": "grid", "disable_numparse": True, "maxcolwidths": 40}
+    tablefmt = os.environ.get("BBOT_TABLE_FORMAT", None)
+    defaults = {"tablefmt": "grid", "disable_numparse": True, "maxcolwidths": None}
+    if tablefmt is None:
+        defaults.update({"maxcolwidths": 40})
+    else:
+        defaults.update({"tablefmt": tablefmt})
     for k, v in defaults.items():
         if k not in kwargs:
             kwargs[k] = v
+    # don't wrap columns in markdown
+    if tablefmt in ("github", "markdown"):
+        kwargs.pop("maxcolwidths")
     return tabulate(*args, **kwargs)
 
 
 def human_timedelta(d):
     """
     Format a TimeDelta object in human-readable form
     """
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/modules.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/modules.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 import importlib
 import traceback
 from pathlib import Path
 from omegaconf import OmegaConf
 from contextlib import suppress
 
+from ..flags import flag_descriptions
 from .misc import list_files, sha1, search_dict_by_key, search_format_dict, make_table, os_platform
 
 
 class ModuleLoader:
     def __init__(self):
         self._preloaded = {}
         self._preloaded_orig = None
@@ -265,27 +266,35 @@
         try:
             d[k].update(set(items))
         except KeyError:
             d[k] = set(items)
 
     def modules_table(self, modules=None, mod_type=None):
         table = []
-        header = ["Module", "Type", "Needs\nAPI\nKey", "Description", "Flags", "Produced Events"]
-        maxcolwidths = [20, 20, 5, 40, 40, 40]
+        header = ["Module", "Type", "Needs API Key", "Description", "Flags", "Consumed Events", "Produced Events"]
+        maxcolwidths = [20, 10, 5, 30, 30, 20, 20]
         for module_name, preloaded in self.filter_modules(modules, mod_type):
             module_type = preloaded["type"]
+            consumed_events = sorted(preloaded.get("watched_events", []))
             produced_events = sorted(preloaded.get("produced_events", []))
             flags = sorted(preloaded.get("flags", []))
             api_key_required = ""
             meta = preloaded.get("meta", {})
-            if meta.get("auth_required", False):
-                api_key_required = "X"
+            api_key_required = "Yes" if meta.get("auth_required", False) else "No"
             description = meta.get("description", "")
             table.append(
-                [module_name, module_type, api_key_required, description, ",".join(flags), ",".join(produced_events)]
+                [
+                    module_name,
+                    module_type,
+                    api_key_required,
+                    description,
+                    ", ".join(flags),
+                    ", ".join(consumed_events),
+                    ", ".join(produced_events),
+                ]
             )
         return make_table(table, header, maxcolwidths=maxcolwidths)
 
     def modules_options(self, modules=None, mod_type=None):
         """
         Return a list of module options
         """
@@ -298,24 +307,77 @@
             for k, v in sorted(module_options.items(), key=lambda x: x[0]):
                 module_key = "modules"
                 if module_type in ("internal", "output"):
                     module_key = f"{module_type}_modules"
                 option_name = f"{module_key}.{module_name}.{k}"
                 option_type = type(v).__name__
                 option_description = module_options_desc[k]
-                modules_options[module_name].append((option_name, option_type, str(v), option_description))
+                modules_options[module_name].append((option_name, option_type, option_description, str(v)))
         return modules_options
 
     def modules_options_table(self, modules=None, mod_type=None):
         table = []
-        header = ["Option", "Type", "Default", "Description"]
+        header = ["Config Option", "Type", "Description", "Default"]
         for module_name, module_options in self.modules_options(modules, mod_type).items():
             table += module_options
         return make_table(table, header)
 
+    def flags(self, flags=None):
+        _flags = {}
+        for module_name, preloaded in self.preloaded().items():
+            for flag in preloaded.get("flags", []):
+                if not flags or flag in flags:
+                    try:
+                        _flags[flag].add(module_name)
+                    except KeyError:
+                        _flags[flag] = {module_name}
+
+        _flags = sorted(_flags.items(), key=lambda x: x[0])
+        _flags = sorted(_flags, key=lambda x: len(x[-1]), reverse=True)
+        return _flags
+
+    def flags_table(self, flags=None):
+        table = []
+        header = ["Flag", "# Modules", "Description", "Modules"]
+        maxcolwidths = [20, 5, 40, 80]
+        _flags = self.flags(flags=flags)
+        for flag, modules in _flags:
+            description = flag_descriptions.get(flag, "")
+            table.append([flag, f"{len(modules)}", description, ", ".join(sorted(modules))])
+        return make_table(table, header, maxcolwidths=maxcolwidths)
+
+    def events(self):
+        consuming_events = {}
+        producing_events = {}
+        for module_name, preloaded in self.preloaded().items():
+            consumed = preloaded.get("watched_events", [])
+            produced = preloaded.get("produced_events", [])
+            for c in consumed:
+                try:
+                    consuming_events[c].add(module_name)
+                except KeyError:
+                    consuming_events[c] = {module_name}
+            for c in produced:
+                try:
+                    producing_events[c].add(module_name)
+                except KeyError:
+                    producing_events[c] = {module_name}
+        return consuming_events, producing_events
+
+    def events_table(self):
+        table = []
+        header = ["Event Type", "# Consuming Modules", "# Producing Modules", "Consuming Modules", "Producing Modules"]
+        consuming_events, producing_events = self.events()
+        all_event_types = sorted(set(consuming_events).union(set(producing_events)))
+        for e in all_event_types:
+            consuming = sorted(consuming_events.get(e, []))
+            producing = sorted(producing_events.get(e, []))
+            table.append([e, len(consuming), len(producing), ", ".join(consuming), ", ".join(producing)])
+        return make_table(table, header)
+
     def filter_modules(self, modules=None, mod_type=None):
         if modules is None:
             module_list = list(self.preloaded(type=mod_type).items())
         else:
             module_list = [(m, self._preloaded[m]) for m in modules]
         module_list.sort(key=lambda x: x[0])
         module_list.sort(key=lambda x: "passive" in x[-1]["flags"])
```

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/punycode.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/url.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/validators.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/web.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.0.1903rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/core/logger/logger.py` & `bbot-1.1.0.1903rc0/bbot/core/logger/logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -143,27 +143,19 @@
 
     # Separate log file for debugging
     debug_handler = logging.handlers.TimedRotatingFileHandler(
         f"{log_dir}/bbot.debug.log", when="d", interval=1, backupCount=14
     )
 
     def stderr_filter(record):
-        config_silent = config.get("silent", False)
         log_level = get_log_level()
-        excluded_levels = [logging.STDOUT]
-        if log_level > logging.DEBUG:
-            excluded_levels.append(logging.TRACE)
-        if record.levelno in excluded_levels:
+        if record.levelno == logging.STDOUT or (record.levelno == logging.TRACE and log_level > logging.DEBUG):
             return False
-        if record.levelno >= logging.ERROR:
-            return True
         if record.levelno < log_level:
             return False
-        if config_silent and not record.levelname.startswith("HUGE"):
-            return False
         return True
 
     stderr_handler.addFilter(stderr_filter)
     stdout_handler.addFilter(lambda x: x.levelno == logging.STDOUT)
     debug_handler.addFilter(lambda x: x.levelno != logging.STDOUT and x.levelno >= logging.DEBUG)
     main_handler.addFilter(lambda x: x.levelno not in (logging.STDOUT, logging.TRACE) and x.levelno >= logging.VERBOSE)
```

### Comparing `bbot-1.0.5.1839rc0/bbot/db/neo4j.py` & `bbot-1.1.0.1903rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/defaults.yml` & `bbot-1.1.0.1903rc0/bbot/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,31 @@
 # Interval for displaying status messages
 status_frequency: 15
 # HTTP proxy
 http_proxy: 
 # Web user-agent
 user_agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
 
+### WEB SPIDER ###
+
+# Set the maximum number of HTTP links that can be followed in a row (0 == no spidering allowed)
+web_spider_distance: 0
+# Set the maximum directory depth for the web spider
+web_spider_depth: 1
+# Set the maximum number of links that can be followed per page
+web_spider_links_per_page: 25
+
 
 ### ADVANCED OPTIONS ###
 
 # How far out from the main scope to search
 scope_search_distance: 0
 # How far out from the main scope to resolve DNS names / IPs
 scope_dns_search_distance: 2
-# Limit how many DNS records can be followed in a row (for malicious/misconfigured DNS records)
+# Limit how many DNS records can be followed in a row (stop malicious/runaway DNS records)
 dns_resolve_distance: 5
 
 # Infer certain events from others, e.g. IPs from IP ranges, DNS_NAMEs from URLs, etc.
 speculate: True
 # Passively search event data for URLs, hostnames, emails, etc.
 excavate: True
 # Summarize activity at the end of a scan
@@ -51,20 +60,14 @@
 http_retries: 1
 # HTTP retries (for httpx)
 httpx_retries: 1
 # Enable/disable debug messages for web requests/responses
 http_debug: false
 # Maximum number of HTTP redirects to follow
 http_max_redirects: 5
-# Set the maximum number of HTTP links that can be followed in a row (0 == no spidering allowed)
-web_spider_distance: 0
-# Set the maximum directory depth for the web spider
-web_spider_depth: 1
-# Set the maximum number of links that can be followed per page
-web_spider_links_per_page: 25
 # DNS query timeout
 dns_timeout: 5
 # How many times to retry DNS queries
 dns_retries: 1
 # Disable BBOT's smart DNS wildcard handling for select domains
 dns_wildcard_ignore: []
 # How many sanity checks to make when verifying wildcard DNS
```

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/anubisdb.py` & `bbot-1.1.0.1903rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.0.1903rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/badsecrets.py` & `bbot-1.1.0.1903rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/base.py` & `bbot-1.1.0.1903rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bevigil.py` & `bbot-1.1.0.1903rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/binaryedge.py` & `bbot-1.1.0.1903rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bucket_aws.py` & `bbot-1.1.0.1903rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.0.1903rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.0.1903rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.0.1903rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bucket_gcp.py` & `bbot-1.1.0.1903rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/builtwith.py` & `bbot-1.1.0.1903rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/bypass403.py` & `bbot-1.1.0.1903rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/c99.py` & `bbot-1.1.0.1903rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/censys.py` & `bbot-1.1.0.1903rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/certspotter.py` & `bbot-1.1.0.1903rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/columbus.py` & `bbot-1.1.0.1903rc0/bbot/modules/threatminer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .crobat import crobat
+from bbot.modules.crobat import crobat
 
 
-class columbus(crobat):
-    flags = ["subdomain-enum", "passive", "safe"]
+class threatminer(crobat):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query the Columbus Project API for subdomains"}
+    flags = ["subdomain-enum", "passive", "safe"]
+    meta = {
+        "description": "Query threatminer's API for subdomains",
+    }
 
-    base_url = "https://columbus.elmasy.com/api/lookup"
+    base_url = "https://api.threatminer.org/v2"
 
     async def request_url(self, query):
-        url = f"{self.base_url}/{self.helpers.quote(query)}"
-        return await self.request_with_fail_count(url)
+        url = f"{self.base_url}/domain.php?q={self.helpers.quote(query)}&rt=5"
+        r = await self.request_with_fail_count(url, timeout=self.http_timeout + 30)
+        return r
 
     def parse_results(self, r, query):
-        results = set()
-        json = r.json()
-        if json and isinstance(json, list):
-            return set([f"{s.lower()}.{query}" for s in json])
-        return results
+        j = r.json()
+        return list(j.get("results", []))
```

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/crobat.py` & `bbot-1.1.0.1903rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/crt.py` & `bbot-1.1.0.1903rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.0.1903rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.0.1903rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.0.1903rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.0.1903rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.0.1903rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.1.0.1903rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/emailformat.py` & `bbot-1.1.0.1903rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.0.1903rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.0.1903rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/fullhunt.py` & `bbot-1.1.0.1903rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.0.1903rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/git.py` & `bbot-1.1.0.1903rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/github.py` & `bbot-1.1.0.1903rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/gowitness.py` & `bbot-1.1.0.1903rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/hackertarget.py` & `bbot-1.1.0.1903rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/host_header.py` & `bbot-1.1.0.1903rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/httpx.py` & `bbot-1.1.0.1903rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/hunt.py` & `bbot-1.1.0.1903rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/hunterio.py` & `bbot-1.1.0.1903rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.0.1903rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/internal/base.py` & `bbot-1.1.0.1903rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.0.1903rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.0.1903rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.0.1903rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/ipstack.py` & `bbot-1.1.0.1903rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/leakix.py` & `bbot-1.1.0.1903rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/masscan.py` & `bbot-1.1.0.1903rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/massdns.py` & `bbot-1.1.0.1903rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/myssl.py` & `bbot-1.1.0.1903rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/naabu.py` & `bbot-1.1.0.1903rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/nmap.py` & `bbot-1.1.0.1903rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/nsec.py` & `bbot-1.1.0.1903rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/ntlm.py` & `bbot-1.1.0.1903rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/otx.py` & `bbot-1.1.0.1903rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/base.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/csv.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/http.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/human.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/human.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 class Human(BaseOutputModule):
     watched_events = ["*"]
     meta = {"description": "Output to text"}
     options = {"output_file": "", "console": True}
     options_desc = {"output_file": "Output to file", "console": "Output to console"}
     vuln_severity_map = {"LOW": "HUGEWARNING", "MEDIUM": "HUGEWARNING", "HIGH": "CRITICAL", "CRITICAL": "CRITICAL"}
+    accept_dupes = False
 
     async def setup(self):
         self._prep_output_dir("output.txt")
         return True
 
     async def handle_event(self, event):
         event_type = f"[{event.type}]"
```

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/json.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/web_report.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/output/websocket.py` & `bbot-1.1.0.1903rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.0.1903rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.0.1903rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.0.1903rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/passivetotal.py` & `bbot-1.1.0.1903rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/pgp.py` & `bbot-1.1.0.1903rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/rapiddns.py` & `bbot-1.1.0.1903rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.0.1903rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/report/asn.py` & `bbot-1.1.0.1903rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/riddler.py` & `bbot-1.1.0.1903rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/robots.py` & `bbot-1.1.0.1903rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/secretsdb.py` & `bbot-1.1.0.1903rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/securitytrails.py` & `bbot-1.1.0.1903rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.0.1903rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/skymem.py` & `bbot-1.1.0.1903rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/smuggler.py` & `bbot-1.1.0.1903rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/social.py` & `bbot-1.1.0.1903rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/sslcert.py` & `bbot-1.1.0.1903rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.1.0.1903rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/telerik.py` & `bbot-1.1.0.1903rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.0.1903rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/urlscan.py` & `bbot-1.1.0.1903rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/viewdns.py` & `bbot-1.1.0.1903rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/virustotal.py` & `bbot-1.1.0.1903rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/wafw00f.py` & `bbot-1.1.0.1903rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.0.1903rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/wayback.py` & `bbot-1.1.0.1903rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/modules/zoomeye.py` & `bbot-1.1.0.1903rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.0.1903rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/scanner/manager.py` & `bbot-1.1.0.1903rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/scanner/scanner.py` & `bbot-1.1.0.1903rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/scanner/stats.py` & `bbot-1.1.0.1903rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/scanner/target.py` & `bbot-1.1.0.1903rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.0.1903rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/conftest.py` & `bbot-1.1.0.1903rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/run_tests.sh` & `bbot-1.1.0.1903rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test.conf` & `bbot-1.1.0.1903rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,20 +18,20 @@
     async def output_append(e):
         output.append(e)
 
     def event_children_append(e):
         event_children.append(e)
 
     success_callback = lambda e: results.append("success")
-    scan1 = bbot_scanner("127.0.0.1", modules=["ipneighbor"], output_modules=["human"], config=dns_config)
+    scan1 = bbot_scanner("127.0.0.1", modules=["ipneighbor"], output_modules=["json"], config=dns_config)
     await scan1.load_modules()
     module = scan1.modules["ipneighbor"]
     module.scope_distance_modifier = 0
     module.queue_event = results_append
-    output_module = scan1.modules["human"]
+    output_module = scan1.modules["json"]
     output_module.queue_event = output_append
     scan1.status = "RUNNING"
     manager = scan1.manager
     # manager.distribute_event = lambda e: results.append(e)
     localhost = scan1.make_event("127.0.0.1", source=scan1.root_event, tags=["localhost"])
 
     class DummyModule1:
```

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         config=bbot_config,
     )
     scan2.helpers.dns.fallback_nameservers_file = fallback_nameservers
     await scan2.load_modules()
     scan2.status = "RUNNING"
 
     # attributes, descriptions, etc.
+    # TODO: Ensure every flag has a description
     for module_name, module in sorted(scan2.modules.items()):
         # flags
         assert module._type in ("internal", "output", "scan")
         # async stuff
         not_async = []
         for func_name in ("setup", "ping", "filter_event", "handle_event", "finish", "report", "cleanup"):
             f = getattr(module, func_name)
@@ -109,17 +110,21 @@
     assert "subdomain-enum" in all_preloaded["massdns"]["flags"]
     assert "wordlist" in all_preloaded["massdns"]["config"]
     assert type(all_preloaded["massdns"]["config"]["max_resolvers"]) == int
     assert all_preloaded["sslcert"]["deps"]["pip"]
     assert all_preloaded["sslcert"]["deps"]["apt"]
     assert all_preloaded["massdns"]["deps"]["ansible"]
 
+    all_flags = set()
+
     for module_name, preloaded in all_preloaded.items():
         # either active or passive and never both
         flags = preloaded.get("flags", [])
+        for flag in flags:
+            all_flags.add(flag)
         if preloaded["type"] == "scan":
             assert ("active" in flags and not "passive" in flags) or (
                 not "active" in flags and "passive" in flags
             ), f'module "{module_name}" must have either "active" or "passive" flag'
             assert preloaded.get("meta", {}).get("description", ""), f"{module_name} must have a description"
 
         # attribute checks
@@ -151,7 +156,14 @@
         assert set(preloaded.get("config", {})) == set(
             preloaded.get("options_desc", {})
         ), f"{module_name}.options do not match options_desc"
         # descriptions most not be blank
         assert all(
             o for o in preloaded.get("options_desc", {}).values()
         ), f"{module_name}.options_desc descriptions must not be blank"
+
+    from bbot.core.flags import flag_descriptions
+
+    for flag in all_flags:
+        assert flag in flag_descriptions, f'Flag "{flag}" not listed in bbot/core/flags.py'
+        description = flag_descriptions.get(flag, "")
+        assert description, f'Flag "{flag}" has no description in bbot/core/flags.py'
```

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.0.1903rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/testsslcert.pem` & `bbot-1.1.0.1903rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/test/testsslkey.pem` & `bbot-1.1.0.1903rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.0.1903rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.0.1903rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.0.1903rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.0.1903rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.0.1903rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.0.1903rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1839rc0/pyproject.toml` & `bbot-1.1.0.1903rc0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1839rc"
+version = "v1.1.0.1903rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
 
@@ -57,11 +57,11 @@
 
 [tool.black]
 line-length = 119
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = false
-format-jinja = 'v1.0.5.{{ distance }}{% if branch == "dev" %}rc{% endif %}'
+format-jinja = 'v1.1.0.{{ distance }}{% if branch == "dev" %}rc{% endif %}'
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py"]
```

