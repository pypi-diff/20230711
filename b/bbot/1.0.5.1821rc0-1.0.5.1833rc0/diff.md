# Comparing `tmp/bbot-1.0.5.1821rc0.tar.gz` & `tmp/bbot-1.0.5.1833rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1821rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1833rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1821rc0.tar` & `bbot-1.0.5.1833rc0.tar`

### file list

```diff
@@ -1,283 +1,283 @@
--rw-r--r--   0        0        0    32473 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/LICENSE
--rw-r--r--   0        0        0    51778 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/README.md
--rw-r--r--   0        0        0      211 2023-07-11 18:56:26.764174 bbot-1.0.5.1821rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7527 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    14606 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-07-11 18:55:56.059685 bbot-1.0.5.1821rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8720 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5150 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      574 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    31059 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1496 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     1993 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     3475 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1394 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     4006 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     5022 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14159 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9311 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    27442 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     3104 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     4373 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5687 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    34834 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14831 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9603 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     1548 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     2251 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     4153 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3192 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    13229 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    11137 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8300 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3786 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1395 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3491 2023-07-11 18:55:56.063685 bbot-1.0.5.1821rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2600 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25482 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2257 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1263 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5461 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1004 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      758 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1102 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2119 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4760 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5125 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1140 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3260 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      764 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0      680 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     5520 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1184 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13670 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15858 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5227 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2539 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2929 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2976 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      743 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11304 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2176 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1159 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7776 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1307 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2939 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10065 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      807 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7437 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5749 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5997 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2032 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9552 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16933 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     5124 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1292 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2128 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1496 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11285 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    15167 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      811 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     4269 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     5248 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     1545 2023-07-11 18:55:56.067685 bbot-1.0.5.1821rc0/bbot/modules/nsec.py
--rw-r--r--   0        0        0     4993 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    11391 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1623 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2579 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1944 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1820 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1031 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1420 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3627 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2079 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1688 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     8363 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1571 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1380 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      786 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8302 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      782 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2273 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2768 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1153 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1290 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1466 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1744 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1539 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7882 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6110 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11359 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      644 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3843 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2866 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2554 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1555 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1711 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1245 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2291 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2295 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    24694 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    27042 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3225 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4044 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    10812 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     2681 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/conftest.py
--rwxr-xr-x   0        0        0      607 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1086 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5153 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6435 2023-07-11 18:55:56.071685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0      965 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     4943 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     6082 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0    15109 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    24751 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0     7959 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_manager.py
--rw-r--r--   0        0        0     7688 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     1694 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     2664 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0     6867 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     4850 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      346 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      313 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0      546 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     1886 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1949 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     4779 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3882 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
--rw-r--r--   0        0        0      546 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      901 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0      502 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1088 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
--rw-r--r--   0        0        0     5051 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     2069 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      555 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0      762 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0      972 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     1794 2023-07-11 18:55:56.075685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
--rw-r--r--   0        0        0      461 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0     7339 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     1964 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0      445 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1726 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0     8204 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_github.py
--rw-r--r--   0        0        0     1752 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0      706 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     1572 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2600 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     1297 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2900 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0      474 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0      987 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1945 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      698 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      419 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
--rw-r--r--   0        0        0      659 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0      337 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1262 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
--rw-r--r--   0        0        0     1116 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     4708 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     1160 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2107 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10661 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2124 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0      184 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      888 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      717 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     2321 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0     2426 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0      588 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     1004 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0      318 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0     1925 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
--rw-r--r--   0        0        0      611 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     5562 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0     1144 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0      563 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2370 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1948 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     3268 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2023-07-11 18:55:56.079685 bbot-1.0.5.1821rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-07-11 18:55:56.087685 bbot-1.0.5.1821rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1537 2023-07-11 18:56:26.764174 bbot-1.0.5.1821rc0/pyproject.toml
--rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1821rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/LICENSE
+-rw-r--r--   0        0        0    51778 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/README.md
+-rw-r--r--   0        0        0      211 2023-07-11 21:18:45.504590 bbot-1.0.5.1833rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7527 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    14606 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8720 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5247 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      574 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    31059 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1496 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     1993 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     3475 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1394 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     4006 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     5022 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14159 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9311 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    28361 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     3104 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     4373 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5687 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    34834 2023-07-11 21:18:22.860422 bbot-1.0.5.1833rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14831 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9603 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     1548 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     2251 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     4153 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3192 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    13681 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    11137 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8300 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     4078 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1395 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3491 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2600 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    25482 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2257 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1263 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5461 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1004 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      758 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1102 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2119 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4851 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5125 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1140 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3260 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      764 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0      680 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     5718 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1184 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13670 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15858 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5227 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2539 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2929 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2976 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      743 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11304 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2176 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1159 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7776 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1307 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2939 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10065 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      807 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7437 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5795 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5997 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2032 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9552 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16933 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     5124 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1292 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2128 2023-07-11 21:18:22.864422 bbot-1.0.5.1833rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1496 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11285 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    15167 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      811 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     4269 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     5248 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     1545 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/nsec.py
+-rw-r--r--   0        0        0     4993 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11391 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1623 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2579 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1944 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1820 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1031 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1420 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3627 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2079 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1688 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     8363 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1571 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1380 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      786 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8302 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      782 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2273 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2768 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1153 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1290 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1466 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1744 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1539 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7882 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6110 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11359 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      644 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3843 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2866 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2554 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1555 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1711 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1245 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2291 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2295 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    24694 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    27042 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4044 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    10812 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     3987 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/conftest.py
+-rwxr-xr-x   0        0        0      607 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1086 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5153 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6435 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0      965 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     4943 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     6082 2023-07-11 21:18:22.868422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0    15109 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    24751 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0     7959 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_manager.py
+-rw-r--r--   0        0        0     7688 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     1694 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     2664 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2148 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0     8916 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     4850 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      346 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      313 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0      546 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     1886 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1949 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     4779 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3882 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py
+-rw-r--r--   0        0        0      546 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      901 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0      502 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1088 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py
+-rw-r--r--   0        0        0     5051 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     2069 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      555 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0      762 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0      972 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0     1794 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py
+-rw-r--r--   0        0        0      461 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0     7339 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     1964 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0      445 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0     8204 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_github.py
+-rw-r--r--   0        0        0     1752 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0      706 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     1572 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2600 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     1297 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2900 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0      474 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0      987 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1945 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      698 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0      419 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_naabu.py
+-rw-r--r--   0        0        0      659 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0      337 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1262 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py
+-rw-r--r--   0        0        0     1116 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     4708 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     1160 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2107 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10661 2023-07-11 21:18:22.872422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2124 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0      184 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      888 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      717 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     2321 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0     2426 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0      588 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     1004 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0      318 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0     1925 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py
+-rw-r--r--   0        0        0      611 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     5562 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0     1144 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0      563 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2370 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1984 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1948 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     3268 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2023-07-11 21:18:22.876422 bbot-1.0.5.1833rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-07-11 21:18:22.880422 bbot-1.0.5.1833rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-07-11 21:18:22.880422 bbot-1.0.5.1833rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2023-07-11 21:18:22.884422 bbot-1.0.5.1833rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2023-07-11 21:18:22.884422 bbot-1.0.5.1833rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2023-07-11 21:18:22.884422 bbot-1.0.5.1833rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-07-11 21:18:22.884422 bbot-1.0.5.1833rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1537 2023-07-11 21:18:45.504590 bbot-1.0.5.1833rc0/pyproject.toml
+-rw-r--r--   0        0        0    53180 1970-01-01 00:00:00.000000 bbot-1.0.5.1833rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1821rc0/LICENSE` & `bbot-1.0.5.1833rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/README.md` & `bbot-1.0.5.1833rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/agent/agent.py` & `bbot-1.0.5.1833rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/cli.py` & `bbot-1.0.5.1833rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1833rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1833rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1833rc0/bbot/core/configurator/environ.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,17 @@
     os.environ.update(bbot_environ)
 
     # handle HTTP proxy
     http_proxy = bbot_config.get("http_proxy", "")
     if http_proxy:
         os.environ["HTTP_PROXY"] = http_proxy
         os.environ["HTTPS_PROXY"] = http_proxy
+    else:
+        os.environ.pop("HTTP_PROXY", None)
+        os.environ.pop("HTTPS_PROXY", None)
 
     # replace environment variables in preloaded modules
     module_loader.find_and_replace(**os.environ)
 
     # ssl verification
     import urllib3
```

### Comparing `bbot-1.0.5.1821rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1833rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/errors.py` & `bbot-1.0.5.1833rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/event/base.py` & `bbot-1.0.5.1833rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1833rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,30 @@
         self.retries = self.parent_helper.config.get("dns_retries", 1)
         self.abort_threshold = self.parent_helper.config.get("dns_abort_threshold", 5)
         self.max_dns_resolve_distance = self.parent_helper.config.get("max_dns_resolve_distance", 4)
         self.resolver.timeout = self.timeout
         self.resolver.lifetime = self.timeout
         self._resolver_list = None
 
+        # skip certain queries
+        dns_omit_queries = self.parent_helper.config.get("dns_omit_queries", None)
+        if not dns_omit_queries:
+            dns_omit_queries = []
+        self.dns_omit_queries = dict()
+        for d in dns_omit_queries:
+            d = d.split(":")
+            if len(d) == 2:
+                rdtype, query = d
+                rdtype = rdtype.upper()
+                query = query.lower()
+                try:
+                    self.dns_omit_queries[rdtype].add(query)
+                except KeyError:
+                    self.dns_omit_queries[rdtype] = {query}
+
         self.wildcard_ignore = self.parent_helper.config.get("dns_wildcard_ignore", None)
         if not self.wildcard_ignore:
             self.wildcard_ignore = []
         self.wildcard_ignore = tuple([str(d).strip().lower() for d in self.wildcard_ignore])
         self.wildcard_tests = self.parent_helper.config.get("dns_wildcard_tests", 5)
         self._wildcard_cache = dict()
         # since wildcard detection takes some time, This is to prevent multiple
@@ -120,16 +136,23 @@
 
         return (results, errors)
 
     async def _resolve_hostname(self, query, **kwargs):
         self.debug(f"Resolving {query} with kwargs={kwargs}")
         results = []
         errors = []
-        parent = self.parent_helper.parent_domain(query)
         rdtype = kwargs.get("rdtype", "A")
+
+        # skip certain queries if requested
+        if rdtype in self.dns_omit_queries:
+            if any(h == query or query.endswith(f".{h}") for h in self.dns_omit_queries[rdtype]):
+                self.debug(f"Skipping {rdtype}:{query} because it's omitted in the config")
+                return results, errors
+
+        parent = self.parent_helper.parent_domain(query)
         retries = kwargs.pop("retries", self.retries)
         cache_result = kwargs.pop("cache_result", False)
         tries_left = int(retries) + 1
         parent_hash = hash(f"{parent}:{rdtype}")
         dns_cache_hash = hash(f"{query}:{rdtype}")
         while tries_left > 0:
             try:
```

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/files.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/web.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,26 @@
         if not "timeout" in kwargs:
             kwargs["timeout"] = http_timeout
 
         # headers
         headers = kwargs.get("headers", None)
         if headers is None:
             headers = {}
+        # user agent
         user_agent = self._bbot_scan.config.get("user_agent", "BBOT")
         if "User-Agent" not in headers:
             headers["User-Agent"] = user_agent
         kwargs["headers"] = headers
+        # proxy
+        proxies = self._bbot_scan.config.get("http_proxy", None)
+        kwargs["proxies"] = proxies
+
+        http_debug = self._bbot_scan.config.get("http_debug", None)
+        if http_debug:
+            log.debug(f"Creating AsyncClient: {args}, {kwargs}")
 
         super().__init__(*args, **kwargs)
 
     def build_request(self, *args, **kwargs):
         request = super().build_request(*args, **kwargs)
         # add custom headers if the URL is in-scope
         if self._bbot_scan.in_scope(str(request.url)):
@@ -58,22 +66,24 @@
         "timeout",
         "follow_redirects",
         "max_redirects",
     )
 
     def __init__(self, parent_helper):
         self.parent_helper = parent_helper
+        self.http_debug = self.parent_helper.config.get("http_debug", False)
         self.ssl_verify = self.parent_helper.config.get("ssl_verify", False)
         self.web_requests_per_second = self.parent_helper.config.get("web_requests_per_second", 50)
         self.web_rate_limiter = RateLimiter(self.web_requests_per_second, "Web")
 
     def AsyncClient(self, *args, **kwargs):
         kwargs["_bbot_scan"] = self.parent_helper.scan
         retries = kwargs.pop("retries", self.parent_helper.config.get("http_retries", 1))
         kwargs["transport"] = httpx.AsyncHTTPTransport(retries=retries, verify=self.ssl_verify)
+        kwargs["verify"] = self.ssl_verify
         return BBOTAsyncClient(*args, **kwargs)
 
     async def request(self, *args, **kwargs):
         raise_error = kwargs.pop("raise_error", False)
         # TODO: use this
         cache_for = kwargs.pop("cache_for", None)  # noqa
 
@@ -86,39 +96,39 @@
         if len(args) == 1:
             kwargs["url"] = args[0]
             args = []
 
         if not args and "method" not in kwargs:
             kwargs["method"] = "GET"
 
-        http_debug = self.parent_helper.config.get("http_debug", False)
-
         client_kwargs = {}
         for k in list(kwargs):
             if k in self.client_options:
                 v = kwargs.pop(k)
                 client_kwargs[k] = v
         async with self.AsyncClient(**client_kwargs) as client:
             try:
-                if http_debug:
+                if self.http_debug:
                     logstr = f"Web request: {str(args)}, {str(kwargs)}"
                     log.debug(logstr)
                 async with self.web_rate_limiter:
                     response = await client.request(*args, **kwargs)
-                if http_debug:
+                if self.http_debug:
                     log.debug(
                         f"Web response: {response} (Length: {len(response.content)}) headers: {response.headers}"
                     )
                 return response
             except httpx.RequestError as e:
                 log.debug(f"Error with request: {e}")
+                log.trace(traceback.format_exc())
                 if raise_error:
                     raise
             except ssl.SSLError as e:
                 log.debug(f"SSL error with request: {e}")
+                log.trace(traceback.format_exc())
 
     async def download(self, url, **kwargs):
         """
         Downloads file, returns full path of filename
         If download failed, returns None
 
         Caching supported via "cache_hrs"
```

### Comparing `bbot-1.0.5.1821rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1833rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1833rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1833rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/defaults.yml` & `bbot-1.0.5.1833rc0/bbot/defaults.yml`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # Rate-limit HTTP
 web_requests_per_second: 100
 # Interval for displaying status messages
 status_frequency: 15
 # HTTP proxy
 http_proxy: 
 # Web user-agent
-user_agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.79 Safari/537.36
+user_agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/114.0.0.0 Safari/537.36
 
 
 ### ADVANCED OPTIONS ###
 
 # How far out from the main scope to search
 scope_search_distance: 0
 # How far out from the main scope to resolve DNS names / IPs
@@ -112,18 +112,25 @@
 # Distribute URLs with these extensions only to httpx (these are omitted from output)
 url_extension_httpx_only:
     - js
 # Don't output these types of events (they are still distributed to modules)
 omit_event_types:
     - HTTP_RESPONSE
     - URL_UNVERIFIED
-    # - DNS_NAME_UNRESOLVED
+    - DNS_NAME_UNRESOLVED
     # - IP_ADDRESS
 # URL of BBOT server
 agent_url: ''
 # Agent Bearer authentication token
 agent_token: ''
 
 # Custom interactsh server settings
 interactsh_server: null
 interactsh_token: null
 interactsh_disable: false
+
+# For performance reasons, always skip these DNS queries
+# Microsoft's DNS infrastructure is misconfigured so that some queries to mail.protection.outlook.com always time out
+dns_omit_queries:
+  - SRV:mail.protection.outlook.com
+  - CNAME:mail.protection.outlook.com
+  - TXT:mail.protection.outlook.com
```

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1833rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1833rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1833rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/base.py` & `bbot-1.0.5.1833rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1833rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1833rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1833rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1833rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1833rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1833rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1833rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1833rc0/bbot/modules/builtwith.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,28 +58,29 @@
         Parameters
         ----------
         r (requests Response): The raw requests response from the API
         query (string): The query used against the API
         """
         results_set = set()
         json = r.json()
-        if json:
+        if json and isinstance(json, dict):
             results = json.get("Results", [])
             if results:
                 for result in results:
                     for chunk in result.get("Result", {}).get("Paths", []):
                         domain = chunk.get("Domain", "")
                         subdomain = chunk.get("SubDomain", "")
                         if domain:
                             if subdomain:
                                 domain = f"{subdomain}.{domain}"
                             results_set.add(domain)
             else:
-                error = json.get("Errors", [{}])[0].get("Message", "Unknown Error")
-                if error:
+                errors = json.get("Errors", [{}])
+                if errors:
+                    error = errors[0].get("Message", "Unknown Error")
                     self.verbose(f"No results for {query}: {error}")
         return results_set
 
     def parse_redirects(self, r, query):
         """
         This method creates a set.
         Each entry in the set is either an Inbound or Outbound Redirect reported in the "Redirect Profile" page on builtwith.com
@@ -91,15 +92,15 @@
 
         Returns
         -------
         results (set)
         """
         results = set()
         json = r.json()
-        if json:
+        if json and isinstance(json, dict):
             inbound = json.get("Inbound", [])
             outbound = json.get("Outbound", [])
             if inbound:
                 for i in inbound:
                     domain = i.get("Domain", "")
                     if domain:
                         results.add(domain)
```

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1833rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/c99.py` & `bbot-1.0.5.1833rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/censys.py` & `bbot-1.0.5.1833rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1833rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/columbus.py` & `bbot-1.0.5.1833rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1833rc0/bbot/modules/crobat.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,20 +120,25 @@
     async def query(self, query, parse_fn=None, request_fn=None):
         if parse_fn is None:
             parse_fn = self.parse_results
         if request_fn is None:
             request_fn = self.request_url
         try:
             response = await request_fn(query)
+            if response is None:
+                self.info(f'Query "{query}" failed')
+                return []
             try:
                 results = list(parse_fn(response, query))
             except Exception as e:
                 if response:
-                    self.info(f'Status code {response.status_code} for query "{query}"')
-                    self.debug(response.text)
+                    self.info(
+                        f'Error parsing results for query "{query}" (status code {response.status_code})', trace=True
+                    )
+                    self.log.trace(response.text)
                 else:
                     self.info(f'Error parsing results for "{query}": {e}', trace=True)
                 return
             if results:
                 return results
             self.debug(f'No results for "{query}"')
         except Exception as e:
```

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/crt.py` & `bbot-1.0.5.1833rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1833rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1833rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1833rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1833rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1833rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1833rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1833rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1833rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1833rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1833rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1833rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/git.py` & `bbot-1.0.5.1833rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/github.py` & `bbot-1.0.5.1833rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1833rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1833rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1833rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1833rc0/bbot/modules/httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,16 +128,18 @@
 
             # discard 404s from unverified URLs
             if source_event.type == "URL_UNVERIFIED" and status_code in (404,):
                 self.debug(f'Discarding 404 from "{url}"')
                 continue
 
             # main URL
-            httpx_ip = j.get("host", "unknown")
-            tags = [f"status-{status_code}", f"ip-{httpx_ip}"]
+            tags = [f"status-{status_code}"]
+            httpx_ip = j.get("host", "")
+            if httpx_ip:
+                tags.append(f"ip-{httpx_ip}")
             # detect login pages
             if is_login_page(j.get("body", "")):
                 tags.append("login-page")
             # grab title
             title = self.helpers.tagify(j.get("title", ""), maxlen=30)
             if title:
                 tags.append(f"http-title-{title}")
```

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1833rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1833rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1833rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1833rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1833rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1833rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1833rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1833rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1833rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1833rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1833rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/myssl.py` & `bbot-1.0.5.1833rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1833rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/nmap.py` & `bbot-1.0.5.1833rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/nsec.py` & `bbot-1.0.5.1833rc0/bbot/modules/nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1833rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/otx.py` & `bbot-1.0.5.1833rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1833rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1833rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1833rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1833rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1833rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1833rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1833rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1833rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1833rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1833rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/robots.py` & `bbot-1.0.5.1833rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1833rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1833rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1833rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1833rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1833rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/social.py` & `bbot-1.0.5.1833rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1833rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1833rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1833rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1833rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1833rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1833rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1833rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1833rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1833rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1833rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1833rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1833rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/scanner/dispatcher.py` & `bbot-1.0.5.1833rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1833rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1833rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1833rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/scanner/target.py` & `bbot-1.0.5.1833rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1833rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/conftest.py` & `bbot-1.0.5.1833rc0/bbot/test/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -95,7 +95,57 @@
         pass
 
     async def poll(self):
         poll_results = []
         for subdomain_tag in self.interactions:
             poll_results.append({"full-id": f"{subdomain_tag}.fakedomain.fakeinteractsh.com", "protocol": "HTTP"})
         return poll_results
+
+
+import threading
+import http.server
+import socketserver
+import urllib.request
+
+
+class Proxy(http.server.SimpleHTTPRequestHandler):
+    protocol_version = "HTTP/1.0"
+    server_version = "Proxy"
+    urls = []
+
+    def do_GET(self):
+        self.urls.append(self.path)
+
+        # Extract host and port from path
+        netloc = urllib.parse.urlparse(self.path).netloc
+        host, _, port = netloc.partition(":")
+
+        # Fetch the content
+        conn = http.client.HTTPConnection(host, port if port else 80)
+        conn.request("GET", self.path, headers=self.headers)
+        response = conn.getresponse()
+
+        # Send the response back to the client
+        self.send_response(response.status)
+        for header, value in response.getheaders():
+            self.send_header(header, value)
+        self.end_headers()
+        self.copyfile(response, self.wfile)
+
+        response.close()
+        conn.close()
+
+
+@pytest.fixture
+def proxy_server():
+    # Set up an HTTP server that acts as a simple proxy.
+    server = socketserver.ThreadingTCPServer(("localhost", 0), Proxy)
+
+    # Start the server in a new thread.
+    server_thread = threading.Thread(target=server.serve_forever)
+    server_thread.start()
+
+    yield server
+
+    # Stop the server.
+    server.shutdown()
+    server_thread.join()
```

### Comparing `bbot-1.0.5.1821rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1833rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test.conf` & `bbot-1.0.5.1833rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_manager.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_1/test_web.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from omegaconf import OmegaConf
 
 from ..bbot_fixtures import *
 
 
 @pytest.mark.asyncio
 async def test_web_helpers(bbot_scanner, bbot_config, bbot_httpserver):
     scan1 = bbot_scanner("8.8.8.8", config=bbot_config)
@@ -161,7 +162,52 @@
     compare_helper = helpers.http_compare("http://www.example.com")
     await compare_helper.compare("http://www.example.com", headers={"asdf": "asdf"})
     await compare_helper.compare("http://www.example.com", cookies={"asdf": "asdf"})
     await compare_helper.compare("http://www.example.com", check_reflection=True)
     compare_helper.compare_body({"asdf": "fdsa"}, {"fdsa": "asdf"})
     for mode in ("getparam", "header", "cookie"):
         assert await compare_helper.canary_check("http://www.example.com", mode=mode) == True
+
+
+@pytest.mark.asyncio
+async def test_http_proxy(bbot_scanner, bbot_config, bbot_httpserver, proxy_server):
+    endpoint = "/test_http_proxy"
+    url = bbot_httpserver.url_for(endpoint)
+    # test user agent + custom headers
+    bbot_httpserver.expect_request(uri=endpoint).respond_with_data("test_http_proxy_yep")
+
+    proxy_address = f"http://127.0.0.1:{proxy_server.server_address[1]}"
+
+    test_config = OmegaConf.merge(bbot_config, OmegaConf.create({"http_proxy": proxy_address}))
+
+    scan = bbot_scanner("127.0.0.1", config=test_config)
+
+    assert len(proxy_server.RequestHandlerClass.urls) == 0
+
+    r = await scan.helpers.request(url)
+
+    assert (
+        len(proxy_server.RequestHandlerClass.urls) == 1
+    ), f"Request to {url} did not go through proxy {proxy_address}"
+    visited_url = proxy_server.RequestHandlerClass.urls[0]
+    assert visited_url.endswith(endpoint), f"There was a problem with request to {url}: {visited_url}"
+    assert r.status_code == 200 and r.text == "test_http_proxy_yep"
+
+
+@pytest.mark.asyncio
+async def test_http_ssl(bbot_scanner, bbot_config, bbot_httpserver_ssl):
+    endpoint = "/test_http_ssl"
+    url = bbot_httpserver_ssl.url_for(endpoint)
+    # test user agent + custom headers
+    bbot_httpserver_ssl.expect_request(uri=endpoint).respond_with_data("test_http_ssl_yep")
+
+    verify_config = OmegaConf.merge(bbot_config, OmegaConf.create({"ssl_verify": True, "http_debug": True}))
+    scan1 = bbot_scanner("127.0.0.1", config=verify_config)
+
+    not_verify_config = OmegaConf.merge(bbot_config, OmegaConf.create({"ssl_verify": False, "http_debug": True}))
+    scan2 = bbot_scanner("127.0.0.1", config=not_verify_config)
+
+    r1 = await scan1.helpers.request(url)
+    assert r1 is None, "Request to self-signed SSL server went through even with ssl_verify=True"
+    r2 = await scan2.helpers.request(url)
+    assert r2 is not None, "Request to self-signed SSL server failed even with ssl_verify=False"
+    assert r2.status_code == 200 and r2.text == "test_http_ssl_yep"
```

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         )
         module_test.set_expect_requests(
             expect_args={"uri": "/test/asdf/.git/config"}, respond_args={"response_data": self.git_config}
         )
         module_test.set_expect_requests(expect_args={"uri": "/test2/.git/config"}, respond_args={"response_data": ""})
 
     def check(self, module_test, events):
-        for e in events:
-            module_test.log.critical(e.data)
         assert any(
             e.type == "FINDING" and "http://127.0.0.1:8888/.git/config" in e.data["description"] for e in events
         )
         assert any(
             e.type == "FINDING" and "http://127.0.0.1:8888/test/.git/config" in e.data["description"] for e in events
         )
         assert any(
```

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_github.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_nsec.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.0.5.1833rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/testsslcert.pem` & `bbot-1.0.5.1833rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/test/testsslkey.pem` & `bbot-1.0.5.1833rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1833rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1833rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.0.5.1833rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.0.5.1833rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1833rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1833rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1821rc0/pyproject.toml` & `bbot-1.0.5.1833rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1821rc"
+version = "v1.0.5.1833rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1821rc0/PKG-INFO` & `bbot-1.0.5.1833rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1821rc0
+Version: 1.0.5.1833rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

