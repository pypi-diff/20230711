# Comparing `tmp/moneyonchain_prices_source-0.6.6b0.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.6b0.tar", last modified: Tue Jul 11 17:05:59 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b1.tar", last modified: Tue Jul 11 17:57:21 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.6b0.tar` & `moneyonchain_prices_source-0.6.6b1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.172159 moneyonchain_prices_source-0.6.6b0/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2213 2023-07-11 14:14:12.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.176159 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2219 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.196160 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-10 19:48:43.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4635 2023-07-11 14:12:57.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1033 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/gas_btc_rsk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        6 2023-07-11 14:48:15.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.196160 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4527 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.858010 moneyonchain_prices_source-0.6.6b1/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.830008 moneyonchain_prices_source-0.6.6b1/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2213 2023-07-11 14:14:12.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.834009 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2219 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-10 19:48:43.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4635 2023-07-11 14:12:57.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1616 2023-07-11 17:52:42.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        7 2023-07-11 17:54:55.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:57:21.854010 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4527 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-11 17:57:21.000000 moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-11 17:57:21.858010 moneyonchain_prices_source-0.6.6b1/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b1/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.6b0/PKG-INFO` & `moneyonchain_prices_source-0.6.6b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.6.6b0
+Version: 0.6.6b1
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.6b0/README.md` & `moneyonchain_prices_source-0.6.6b1/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/cli_check.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/computed_pairs.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/data/weighing.json`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/bnb_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_kraken.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/engine_base.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_kraken.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/gas_btc_rsk.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-from engine_base import BaseOnChain, GAS_BTC, get_env, Decimal
+from engine_base import EngineWebScraping, USD_MXN
+from decimal     import Decimal
 
 
+class Engine(EngineWebScraping):
 
-class Engine(BaseOnChain):
-
-    _name          = BaseOnChain._name_from_file(__file__)
-    _description   = "RSK onchain"
-    _coinpair      = GAS_BTC
-    _uri           = get_env('RSK_NODE', 'https://public-node.rsk.co')
-    _max           = 2*(10**10) #20Gwei
-
-
-    def _get_price(self):
-
-        try:
-            value = self.make_web3_obj_with_uri().eth.gas_price
-        except Exception as e:
-            self._error = str(e)
-            return None
+    _name        = EngineWebScraping._name_from_file(__file__)
+    _description = "X-rates.com"
+    _uri         = "https://www.x-rates.com/calculator/?from=USD&to=MXN&amount=1"
+    _coinpair    = USD_MXN
+
+    _max_age                       = 3600 # 1hs.
+    _max_time_without_price_change = 0    # zero means infinity
+
+    def _scraping(self, html):
+        value = None
+        for s in html.find_all ('span', attrs={'class':'ccOutputTxt'}):
+            d = list(filter(bool, map(lambda x: x.strip(), s.parent.strings)))
+            if len(d)==4 and d[0]=="1.00 USD =" and d[3]=="MXN":
+                try:
+                    value = Decimal(''.join(d[1:3]))
+                except:
+                    value = None
+                if value:
+                    break
         if not value:
-            self._error = f"No gas price value given from {self._uri}"
-            return None
-        elif value >= self._max:
-            self._error = f"Gas price value >= {self._max}"
+            self._error = "Response format error"
             return None
-        else:
-            return Decimal(value) / (10**18)
-
+        return {
+            'price':  value
+        }
 
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
+    print(engine)
     if engine.error:
-        print(f"{engine} Error: {engine.error}")
-    else:
-        print(engine)
+        print(engine.error)
```

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_citibanamex.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b1/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.6.6b0
+Version: 0.6.6b1
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b1/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.6b0/setup.py` & `moneyonchain_prices_source-0.6.6b1/setup.py`

 * *Files identical despite different names*

