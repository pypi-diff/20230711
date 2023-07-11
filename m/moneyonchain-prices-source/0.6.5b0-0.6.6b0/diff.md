# Comparing `tmp/moneyonchain_prices_source-0.6.5b0.tar.gz` & `tmp/moneyonchain_prices_source-0.6.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneyonchain_prices_source-0.6.5b0.tar", last modified: Fri May 12 18:36:48 2023, max compression
+gzip compressed data, was "moneyonchain_prices_source-0.6.6b0.tar", last modified: Tue Jul 11 17:05:59 2023, max compression
```

## Comparing `moneyonchain_prices_source-0.6.5b0.tar` & `moneyonchain_prices_source-0.6.6b0.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 18:36:48.135496 moneyonchain_prices_source-0.6.5b0/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-05-12 18:36:48.135496 moneyonchain_prices_source-0.6.5b0/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/README.md
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 18:36:48.083495 moneyonchain_prices_source-0.6.5b0/moc_prices_source/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/cli.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4392 2022-12-28 13:52:38.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/cli_check.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1785 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/computed_pairs.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/conf.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 18:36:48.087495 moneyonchain_prices_source-0.6.5b0/moc_prices_source/data/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/data/database_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/data/redis_default.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2196 2023-05-12 17:58:25.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/data/weighing.json
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/database.py
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 18:36:48.131496 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/__init__.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      552 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/bnb_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_argenbtc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_belo_app.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_buenbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_cryptomkt.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_decrypto.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_ripio.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_ripio_exch.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_satoshitango.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      550 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitgo.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bittrex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_blockchain.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_cex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_itbit.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_okcoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      552 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_coinbase.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4400 2023-05-12 17:56:54.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/coins.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13390 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/engine_base.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      549 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_bitstamp.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_gemini.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_kraken.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1485 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/moc_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_bitfinex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_bithumbpro.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_coinbene.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_coingecko.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_kucoin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_mexc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_mxc.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1485 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_sovryn.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-05-12 17:57:28.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_usdt_binance.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccb_emdx.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccb_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_ambito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_rofex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_clarin.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_criptoya.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_cronista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarhoy.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarito.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarsi.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_infobae.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_lanacion.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_bitso.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_citibanamex.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_coinmonitor.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_currencymeuk.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_eldolar_info.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_eleconomista.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_infodolar.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_intercam.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_wise.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-05-12 17:55:12.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_xrates.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/my_logging.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/to_db.py
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        6 2023-05-12 18:31:43.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/version.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source/weighing.py
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source_check
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/moc_prices_source_to_db
-drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-05-12 18:36:48.131496 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-05-12 18:36:47.000000 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/PKG-INFO
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4531 2023-05-12 18:36:47.000000 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/SOURCES.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-05-12 18:36:47.000000 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/dependency_links.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-05-12 18:36:47.000000 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/requires.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-05-12 18:36:47.000000 moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/top_level.txt
--rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-05-12 18:36:48.135496 moneyonchain_prices_source-0.6.5b0/setup.cfg
--rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.5b0/setup.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    10484 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/README.md
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.172159 moneyonchain_prices_source-0.6.6b0/moc_prices_source/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6610 2023-05-11 20:02:22.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      486 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4577 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli_check.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      625 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2213 2023-07-11 14:14:12.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/computed_pairs.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     3892 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/conf.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.176159 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      174 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/database_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       17 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/redis_default.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2219 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/weighing.json
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     5715 2023-07-10 20:39:21.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/database.py
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.196160 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     2521 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/__init__.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      766 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/bnb_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      720 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_argenbtc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      791 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_belo_app.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      770 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      762 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_buenbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      756 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_cryptomkt.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      836 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_decrypto.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      805 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      677 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio_exch.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      643 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_satoshitango.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      693 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitgo.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bittrex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      503 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_blockchain.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      518 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_cex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      526 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      513 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_itbit.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      582 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      559 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      524 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_okcoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-10 19:48:43.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      525 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      538 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_coinbase.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      581 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4635 2023-07-11 14:12:57.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/coins.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    13823 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/engine_base.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-07-10 19:46:36.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      523 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      535 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitstamp.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      505 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_gemini.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      580 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_kraken.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1033 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/gas_btc_rsk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/moc_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      856 2023-05-12 17:54:43.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      584 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bitfinex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bithumbpro.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      666 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coinbene.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      636 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coingecko.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      639 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_kucoin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mexc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      627 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mxc.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1484 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_sovryn.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      859 2023-07-11 14:34:01.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_usdt_binance.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      822 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      950 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_emdx.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      651 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      829 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_ambito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      640 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      615 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1321 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1299 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      866 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1177 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1358 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      858 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      653 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_rofex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      982 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_clarin.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      632 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      612 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_criptoya.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1305 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_cronista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1281 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarhoy.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      867 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarito.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1108 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarsi.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1164 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infobae.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1331 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      855 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_lanacion.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      921 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_bitso.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1069 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_citibanamex.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1224 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_coinmonitor.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1181 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_currencymeuk.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1193 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eldolar_info.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1155 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eleconomista.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1344 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_infodolar.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1078 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_intercam.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1125 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      806 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_wise.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     1223 2023-07-11 14:46:03.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_xrates.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      718 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/my_logging.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     6008 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/to_db.py
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        6 2023-07-11 14:48:15.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/version.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4710 2022-12-28 13:47:46.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source/weighing.py
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      118 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source_check
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)      128 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/moc_prices_source_to_db
+drwxrwxr-x   0 jbokser   (1000) jbokser   (1000)        0 2023-07-11 17:05:59.196160 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)    14035 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/PKG-INFO
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)     4527 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/SOURCES.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)        1 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/dependency_links.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)      100 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/requires.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       18 2023-07-11 17:05:59.000000 moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/top_level.txt
+-rw-rw-r--   0 jbokser   (1000) jbokser   (1000)       38 2023-07-11 17:05:59.200160 moneyonchain_prices_source-0.6.6b0/setup.cfg
+-rwxrwxr-x   0 jbokser   (1000) jbokser   (1000)     1565 2022-12-01 15:35:40.000000 moneyonchain_prices_source-0.6.6b0/setup.py
```

### Comparing `moneyonchain_prices_source-0.6.5b0/PKG-INFO` & `moneyonchain_prices_source-0.6.6b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain_prices_source
-Version: 0.6.5b0
+Version: 0.6.6b0
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.5b0/README.md` & `moneyonchain_prices_source-0.6.6b0/README.md`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/__init__.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/cli_check.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/cli_check.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,19 +81,24 @@
     for p in prices:
         row = []
         row.append(p["coinpair"].from_.name)
         row.append(p["coinpair"].to_.name)
         row.append(p["coinpair"].variant)
         row.append(p["description"])
         if p["ok"]:
-            row.append(f"{p['price']:.8f}")
-            row.append(p["coinpair"].to_.small_symbol)
+            unit = 'p'
+            v = p['price'] * (1000**4)
+            if v > 1000:
+                for unit in ['p', 'µ', 'm', ' ', 'K', 'M', 'G']:
+                    v = v/1000
+                    if v<1000:
+                        break
+            row.append(f"{p['coinpair'].to_.small_symbol} {v:9.5f}{unit}")
         else:
-            row.append(trim(p["error"], 25))
-            row.append(None)
+            row.append(trim(p["error"], 20))
         row.append(round(p["weighing"], 2))
         if p["percentual_weighing"]:
             row.append(round(p[
                 "percentual_weighing"]*100, 1))
         else:
             row.append('N/A')
         if p["time"]:
@@ -101,22 +106,22 @@
         else:
             row.append('N/A')
         table.append(row)
     if table:
         table.sort(key=str)
         print()
         print(tabulate(table, headers=[
-            'From', 'To', 'V.', 'Exchnage', 'Response', 'U.', 'Weigh', '%', 'Time'
+            'From', 'To', 'V.', 'Exchnage', 'Response', 'Weigh', '%', 'Time'
         ]))
 
     table=[]
     for coinpair, d in values.items():
         row = []
         if 'prices' in d:
-            row.append('🠻')
+            row.append('↓')
         else:
             row.append('ƒ')
         row.append(coinpair)
         row.append(d['median_price'])
         row.append(d['mean_price'])
         row.append(d['weighted_median_price'])
         if 'prices' in d:
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/coins.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/coins.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/computed_pairs.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/computed_pairs.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,40 +4,48 @@
 from types   import LambdaType
 
 base_dir = dirname(abspath(__file__))
 
 bkpath   = sys.path[:]
 sys.path.append(dirname(base_dir))
 
-from moc_prices_source.engines.coins import BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, ETH_USD, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS
+from moc_prices_source.engines.coins import RIF_USDT, BTC_USD, MOC_BTC, RIF_BTC, ETH_BTC, MOC_USD, RIF_USD, RIF_USD_B, RIF_USD_T, ETH_USD, USDT_USD, BTC_USDT, BNB_USD, BNB_USDT, USD_ARS_CCB_MOC, BTC_ARS
 
 sys.path = bkpath
 
 
 
 computed_pairs = {
     MOC_USD: {
         'requirements': [MOC_BTC, BTC_USD],
         'formula': lambda moc_btc, btc_usd: moc_btc * btc_usd
     },
-    RIF_USD: {
+    RIF_USD_B: { # Passing through Bitcoin
+        'requirements': [RIF_BTC, BTC_USD],
+        'formula': lambda rif_btc, btc_usd: rif_btc * btc_usd
+    },
+    RIF_USD_T: { # Passing through Tether
+        'requirements': [RIF_USDT, BTC_USD, BTC_USDT],
+        'formula': lambda rif_usdt, btc_usd, btc_usdt: rif_usdt * btc_usd / btc_usdt
+    },
+    RIF_USD: { # Leave this as legacy
         'requirements': [RIF_BTC, BTC_USD],
         'formula': lambda rif_btc, btc_usd: rif_btc * btc_usd
     },
     ETH_USD: {
         'requirements': [ETH_BTC, BTC_USD],
         'formula': lambda eth_btc, btc_usd: eth_btc * btc_usd
     },
     USDT_USD: {
         'requirements': [BTC_USD, BTC_USDT],
         'formula': lambda btc_usd, btc_usdt: btc_usd / btc_usdt
     },
     BNB_USD: {
-        'requirements': [BNB_USDT, USDT_USD],
-        'formula': lambda bnb_usdt, usdt_usd: bnb_usdt * usdt_usd
+        'requirements': [BNB_USDT, BTC_USD, BTC_USDT],
+        'formula': lambda bnb_usdt, btc_usd, btc_usdt: bnb_usdt * btc_usd / btc_usdt
     },
     USD_ARS_CCB_MOC: {
         'requirements': [BTC_ARS, BTC_USD],
         'formula': lambda btc_ars, btc_usd: btc_ars / btc_usd
     },
 }
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/conf.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/conf.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/data/weighing.json` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/data/weighing.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9850746268656716%*

 * *Differences: {"'gas_btc_rsk'": '1'}*

```diff
@@ -20,14 +20,15 @@
     "btc_usdt_coinbase": 0.25,
     "btc_usdt_kraken": 0.25,
     "eth_btc_binance": 0.25,
     "eth_btc_bitfinex": 0.25,
     "eth_btc_bitstamp": 0.25,
     "eth_btc_gemini": 0,
     "eth_btc_kraken": 0.25,
+    "gas_btc_rsk": 1,
     "moc_btc_sovryn": 1,
     "rif_btc_binance": 1,
     "rif_btc_bithumbpro": 0,
     "rif_btc_coingecko": 0,
     "rif_btc_mexc": 0,
     "rif_btc_sovryn": 0,
     "rif_usdt_binance": 1,
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/database.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/database.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/__init__.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/bnb_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kucoin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from engine_base import Base, BNB_USDT
+from engine_base import Base, BTC_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Binance"
-    _uri         = "https://api.binance.com/api/v3/ticker/24hr?symbol=BNBUSDT"
-    _coinpair    = BNB_USDT
+    _description = "Kucoin"
+    _uri         = "https://api.kucoin.com/api/v1/market/stats?symbol=BTC-USDT"
+    _coinpair    = BTC_USD
 
     def _map(self, data):
         return {
-            'price':  data['lastPrice'],
-            'volume': data['volume']}
+            'price':  data['data']['last'],
+            'volume': data['data']['vol'] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_argenbtc.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_argenbtc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_belo_app.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_belo_app.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_bitso.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_buenbit.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_buenbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_cryptomkt.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_cryptomkt.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_decrypto.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_decrypto.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_ripio.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_ripio_exch.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_ripio_exch.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_rofex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_ars_satoshitango.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_ars_satoshitango.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bittrex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from engine_base import Base, BTC_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Binance"
-    _uri         = "https://api.binance.com/api/v3/ticker/24hr?symbol=BTCUSDT"
+    _description = "Bittrex"
+    _uri         = "https://api.bittrex.com/api/v1.1/public/getticker?market=USD-BTC"
     _coinpair    = BTC_USD
 
     def _map(self, data):
         return {
-            'price':  data['lastPrice'],
-            'volume': data['volume']}
+            'price':  data['result']['Last'],
+            }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitfinex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitgo.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitgo.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bitstamp.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_bitstamp.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_bittrex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_coinbase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from engine_base import Base, BTC_USD
+from engine_base import Base, BTC_USDT
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Bittrex"
-    _uri         = "https://api.bittrex.com/api/v1.1/public/getticker?market=USD-BTC"
-    _coinpair    = BTC_USD
+    _description = "Coinbase"
+    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=BTC"
+    _coinpair    = BTC_USDT
 
     def _map(self, data):
         return {
-            'price':  data['result']['Last'],
+            'price':  data['data']['rates']['USDT']
             }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_cex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_cex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_coinbase.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_coinbase.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_itbit.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_itbit.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_kraken.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_kraken.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_kucoin.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usd_okcoin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from engine_base import Base, BTC_USD
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Kucoin"
-    _uri         = "https://api.kucoin.com/api/v1/market/stats?symbol=BTC-USDT"
+    _description = "OkCoin"
+    _uri         = "https://www.okcoin.com/api/spot/v3/instruments/BTC-USD/ticker"
     _coinpair    = BTC_USD
 
     def _map(self, data):
         return {
-            'price':  data['data']['last'],
-            'volume': data['data']['vol'] }
+            'price':  data['last'],
+            }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usd_okcoin.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitstamp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from engine_base import Base, BTC_USD
+from engine_base import Base, ETH_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "OkCoin"
-    _uri         = "https://www.okcoin.com/api/spot/v3/instruments/BTC-USD/ticker"
-    _coinpair    = BTC_USD
+    _description = "Bitstamp"
+    _uri         = "https://www.bitstamp.net/api/v2/ticker/ethbtc/"
+    _coinpair    = ETH_BTC
 
     def _map(self, data):
         return {
             'price':  data['last'],
-            }
+            'volume': data['volume']}
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_bitfinex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from engine_base import Base, BTC_USDT
+from engine_base import Base, ETH_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Binance"
-    _uri         = "https://api.binance.com/api/v3/ticker/24hr?symbol=BTCUSDT"
-    _coinpair    = BTC_USDT
+    _description = "Bitfinex"
+    _uri         = "https://api-pub.bitfinex.com/v2/ticker/tETHBTC"
+    _coinpair    = ETH_BTC
 
     def _map(self, data):
         return {
-            'price':  data['lastPrice'],
-            'volume': data['volume']}
+            'price':  data[6],
+            'volume': data[7]}
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_bitfinex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/btc_usdt_coinbase.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/btc_usdt_kraken.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from engine_base import Base, BTC_USDT
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Coinbase"
-    _uri         = "https://api.coinbase.com/v2/exchange-rates?currency=BTC"
+    _description = "Kraken"
+    _uri         = "https://api.kraken.com/0/public/Ticker?pair=XBTUSDT"
     _coinpair    = BTC_USDT
 
     def _map(self, data):
         return {
-            'price':  data['data']['rates']['USDT']
-            }
+            'price':  data['result']['XBTUSDT']['c'][0],
+            'volume': data['result']['XBTUSDT']['v'][1] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/coins.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/coins.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 RIF  = Coin('RIF Token',      'rif')
 MOC  = Coin('MOC Token',      'moc')
 ETH  = Coin('Ether',          'eth',  '⟠')
 USDT = Coin('Tether',         'usdt', '₮')
 BNB  = Coin('Binance Coin',   'bnb',  'Ƀ')
 ARS  = Coin('Peso Argentino', 'ars',  '$')
 MXN  = Coin('Peso Mexicano',  'mxn',  '$')
+GAS  = Coin('Gas',            'gas')
 
 
 Coins = [ c for c in locals().values() if isinstance(c, Coin) ]
 
 
 
 def get_coin(value):
@@ -116,29 +117,32 @@
     def __hash__(self):
         return hash(str(self))
 
 
 BTC_USD         = CoinPair(BTC,  USD)
 BTC_ARS         = CoinPair(BTC,  ARS)
 RIF_BTC         = CoinPair(RIF,  BTC)
-RIF_USD         = CoinPair(RIF,  USD)
+RIF_USD         = CoinPair(RIF,  USD) # Leave this as legacy
+RIF_USD_B       = CoinPair(RIF,  USD, "B") # Passing through Tether
+RIF_USD_T       = CoinPair(RIF,  USD, "T") # Passing through Bitcoin
 RIF_USDT        = CoinPair(RIF,  USDT)
 MOC_BTC         = CoinPair(MOC,  BTC)
 MOC_USD         = CoinPair(MOC,  USD)
 ETH_BTC         = CoinPair(ETH,  BTC)
 ETH_USD         = CoinPair(ETH,  USD)
 BTC_USDT        = CoinPair(BTC,  USDT)
 USDT_USD        = CoinPair(USDT, USD)
 BNB_USDT        = CoinPair(BNB,  USDT)
 BNB_USD         = CoinPair(BNB,  USD)
 USD_ARS         = CoinPair(USD,  ARS)
 USD_ARS_CCL     = CoinPair(USD,  ARS, "CCL")
 USD_ARS_CCB     = CoinPair(USD,  ARS, "CCB")
 USD_ARS_CCB_MOC = CoinPair(USD,  ARS, "CCB by MOC")
 USD_MXN         = CoinPair(USD,  MXN)
+GAS_BTC         = CoinPair(GAS,  BTC)
 
 
 CoinPairs = [ c for c in locals().values() if isinstance(c, CoinPair) ]
 
 
 
 def get_coin_pair(value):
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/engine_base.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/engine_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path      import basename, dirname, abspath, expanduser
 from decimal      import Decimal
 from json.decoder import JSONDecodeError
 from redis        import Redis, ConnectionError
 from coins        import *
 from bs4          import BeautifulSoup
 from web3         import Web3, HTTPProvider
-
+from os           import environ
 
 
 class Base(object):
 
     _name                          = "base"
     _description                   = "Base Engine"
     _method                        = 'get'
@@ -441,14 +441,23 @@
         "type": "function"
     }
 ]
 """
     Web3 = Web3
     HTTPProvider = HTTPProvider
 
+    def to_checksum_address(self, value):
+        try:
+            return self.Web3.to_checksum_address(value)
+        except:
+            return self.Web3.toChecksumAddress(value)
+    
+    def make_web3_obj_with_uri(self):
+        return self.Web3(self.HTTPProvider(self._uri))
+
     def _get_price(self):
 
         try:
 
             return 0
 
         except Exception as e:
@@ -478,11 +487,17 @@
         self._last_change_timestamp = self._timestamp
 
         self._volume = 0.0
         self._time = datetime.datetime.now() - start_time
 
         return True
 
+def get_env(name, default):
+    try:
+        return str(environ[name])
+    except KeyError :
+        return default
+    
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_binance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from engine_base import Base, ETH_BTC
+from engine_base import BaseWithFailover, ETH_BTC
 
+base_uri = "https://{}/api/v3/ticker/24hr?symbol=ETHBTC"
 
-class Engine(Base):
+class Engine(BaseWithFailover):
 
-    _name        = Base._name_from_file(__file__)
-    _description = "Binance"
-    _uri         = "https://api.binance.com/api/v3/ticker/24hr?symbol=ETHBTC"
-    _coinpair    = ETH_BTC
+    _name         = BaseWithFailover._name_from_file(__file__)
+    _description  = "Binance"
+    _uri          = base_uri.format("api.binance.com")
+    _uri_failover = base_uri.format("moc-proxy-api-binance.moneyonchain.com")
+    _coinpair     = ETH_BTC
+    _max_time_without_price_change = 0 # zero means infinity
 
     def _map(self, data):
         return {
             'price':  data['lastPrice'],
             'volume': data['volume']}
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
+    print(f"URI = {repr(engine.uri)}")
+    print()
     print(engine)
+    print()
     if engine.error:
+        print()
         print(engine.error)
+        print()
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/eth_btc_kraken.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from engine_base import Base, ETH_BTC
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Bitfinex"
-    _uri         = "https://api-pub.bitfinex.com/v2/ticker/tETHBTC"
+    _description = "Kraken"
+    _uri         = "https://api.kraken.com/0/public/Ticker?pair=ETHBTC"
     _coinpair    = ETH_BTC
 
     def _map(self, data):
         return {
-            'price':  data[6],
-            'volume': data[7]}
+            'price':  data['result']['XETHXXBT']['c'][0],
+            'volume': data['result']['XETHXXBT']['v'][1] }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/eth_btc_bitstamp.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_clarin.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,32 @@
-from engine_base import Base, ETH_BTC
+from engine_base import Base, USD_ARS
+from decimal     import Decimal
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Bitstamp"
-    _uri         = "https://www.bitstamp.net/api/v2/ticker/ethbtc/"
-    _coinpair    = ETH_BTC
+    _description = "Clarin.com"
+    _uri         = "https://www.clarin.com/economia/divisas-acciones-bonos/monedas.json"
+    _coinpair    = USD_ARS
+
+    _max_age                       = 3600 # 1hs.
+    _max_time_without_price_change = 0    # zero means infinity
 
     def _map(self, data):
+        value = None
+        for i in data:
+            if 'nombre' in i and i['papel']=="DLRBLE":
+                values = [i['ultimoval'], i['compraval']]
+                values = list(map(lambda x: Decimal(str(x).replace(',', '')), values))
+                value = sum(values)/len(values)
+                break
         return {
-            'price':  data['last'],
-            'volume': data['volume']}
+            'price':  value
+        }
 
 
 if __name__ == '__main__':
     print("File: {}, Ok!".format(repr(__file__)))
     engine = Engine()
     engine()
     print(engine)
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/moc_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/moc_btc_sovryn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from engine_base import BaseOnChain, MOC_BTC
+from engine_base import BaseOnChain, MOC_BTC, get_env
 
 
 
 class Engine(BaseOnChain):
 
     _name          = BaseOnChain._name_from_file(__file__)
     _description   = "Sovryn onchain"
     _coinpair      = MOC_BTC
-    _uri           = 'https://public-node.rsk.co'
+    _uri           = get_env('RSK_NODE', 'https://public-node.rsk.co')
     _pool_sc_addr  = '0xe321442dc4793c17f41fe3fb192a856a4864ceaf'
     _wrbtc_tk_addr = '0x542fda317318ebf1d3deaf76e0b632741a7e677d'
     _moc_tk_addr   = '0x9ac7fe28967b30e3a4e6e03286d715b42b453d10'
 
     def _get_price(self):
 
+        pool_sc_addr = self.to_checksum_address(self._pool_sc_addr)
+        wrbtc_tk_addr = self.to_checksum_address(self._wrbtc_tk_addr)
+        moc_tk_addr = self.to_checksum_address(self._moc_tk_addr)
+
         try:
             
-            pool_sc_addr = self.Web3.toChecksumAddress(self._pool_sc_addr)
-            wrbtc_tk_addr = self.Web3.toChecksumAddress(self._wrbtc_tk_addr)
-            moc_tk_addr = self.Web3.toChecksumAddress(self._moc_tk_addr)
-
-            w3 = self.Web3(self.HTTPProvider(self._uri))
+            w3 = self.make_web3_obj_with_uri()
 
             moc_token = w3.eth.contract(address=moc_tk_addr, abi=self.erc20_simplified_abi)
             wrbtc_token = w3.eth.contract(address=wrbtc_tk_addr, abi=self.erc20_simplified_abi)
 
             moc_reserve = moc_token.functions.balanceOf(pool_sc_addr).call()
             btc_reserve = wrbtc_token.functions.balanceOf(pool_sc_addr).call()
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_bitfinex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bitfinex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_bithumbpro.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_bithumbpro.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_coinbene.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coinbene.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_coingecko.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_coingecko.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_kucoin.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_kucoin.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_mexc.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mexc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_mxc.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_mxc.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_btc_sovryn.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_btc_sovryn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from engine_base import BaseOnChain, RIF_BTC
+from engine_base import BaseOnChain, RIF_BTC, get_env
 
 
 
 class Engine(BaseOnChain):
 
     _name          = BaseOnChain._name_from_file(__file__)
     _description   = "Sovryn onchain"
     _coinpair      = RIF_BTC
-    _uri           = 'https://public-node.rsk.co'
+    _uri           = get_env('RSK_NODE', 'https://public-node.rsk.co')
     _pool_sc_addr  = '0x65528e06371635a338ca804cd65958a11cb11009'
     _wrbtc_tk_addr = '0x542fda317318ebf1d3deaf76e0b632741a7e677d'
     _rif_tk_addr   = '0x2acc95758f8b5f583470ba265eb685a8f45fc9d5'
 
     def _get_price(self):
 
-        try:
-            
-            pool_sc_addr = self.Web3.toChecksumAddress(self._pool_sc_addr)
-            wrbtc_tk_addr = self.Web3.toChecksumAddress(self._wrbtc_tk_addr)
-            rif_tk_addr = self.Web3.toChecksumAddress(self._rif_tk_addr)
+        pool_sc_addr = self.to_checksum_address(self._pool_sc_addr)
+        wrbtc_tk_addr = self.to_checksum_address(self._wrbtc_tk_addr)
+        rif_tk_addr = self.to_checksum_address(self._rif_tk_addr)
 
-            w3 = self.Web3(self.HTTPProvider(self._uri))
+        try:            
+
+            w3 = self.make_web3_obj_with_uri()
 
             rif_token = w3.eth.contract(address=rif_tk_addr, abi=self.erc20_simplified_abi)
             wrbtc_token = w3.eth.contract(address=wrbtc_tk_addr, abi=self.erc20_simplified_abi)
 
             rif_reserve = rif_token.functions.balanceOf(pool_sc_addr).call()
             btc_reserve = wrbtc_token.functions.balanceOf(pool_sc_addr).call()
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/rif_usdt_binance.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/rif_usdt_binance.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ambito.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccb_emdx.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_emdx.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccb_rofex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccb_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_ambito.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_ambito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_cronista.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_infobae.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_ccl_rofex.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_ccl_rofex.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_clarin.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_citibanamex.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from engine_base import Base, USD_ARS
+from engine_base import Base, USD_MXN
 from decimal     import Decimal
 
 
 class Engine(Base):
 
     _name        = Base._name_from_file(__file__)
-    _description = "Clarin.com"
-    _uri         = "https://www.clarin.com/economia/divisas-acciones-bonos/monedas.json"
-    _coinpair    = USD_ARS
+    _description = "CitiBanamex"
+    _uri         = "https://finanzasenlinea.infosel.com/banamex/WSFeedJSON/service.asmx/DivisasLast?callback="
+    _coinpair    = USD_MXN
 
     _max_age                       = 3600 # 1hs.
     _max_time_without_price_change = 0    # zero means infinity
 
     def _map(self, data):
         value = None
         for i in data:
-            if 'nombre' in i and i['papel']=="DLRBLE":
-                values = [i['ultimoval'], i['compraval']]
-                values = list(map(lambda x: Decimal(str(x).replace(',', '')), values))
+            if i['cveInstrumento']=="MXNUS":
+                values = [
+                    i['ValorActualCompra'],
+                    i['ValorActualVenta']
+                ]
+                values = list(map(lambda x: Decimal(str(x).replace(',', '.')), values))
                 value = sum(values)/len(values)
                 break
         return {
             'price':  value
         }
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_criptoya.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_criptoya.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_cronista.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_cronista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarhoy.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarhoy.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarito.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarito.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_dolarsi.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_dolarsi.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_infobae.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infobae.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_infodolar.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_ars_lanacion.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_ars_lanacion.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_bitso.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_bitso.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_coinmonitor.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_coinmonitor.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_currencymeuk.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_currencymeuk.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_eldolar_info.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eldolar_info.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_eleconomista.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_eleconomista.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_infodolar.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_infodolar.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_intercam.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_intercam.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_themoneyconverter.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_wise.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_wise.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/engines/usd_mxn_xrates.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/engines/usd_mxn_xrates.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/my_logging.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/my_logging.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/to_db.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/to_db.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moc_prices_source/weighing.py` & `moneyonchain_prices_source-0.6.6b0/moc_prices_source/weighing.py`

 * *Files identical despite different names*

### Comparing `moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/PKG-INFO` & `moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moneyonchain-prices-source
-Version: 0.6.5b0
+Version: 0.6.6b0
 Summary: Prices source for MoC projects
 Home-page: UNKNOWN
 Author: Juan S. Bokser
 Author-email: juan.bokser@moneyonchain.com
 License: UNKNOWN
 Description: # MoC prices source
```

### Comparing `moneyonchain_prices_source-0.6.5b0/moneyonchain_prices_source.egg-info/SOURCES.txt` & `moneyonchain_prices_source-0.6.6b0/moneyonchain_prices_source.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 moc_prices_source/engines/btc_ars_buenbit.py
 moc_prices_source/engines/btc_ars_cryptomkt.py
 moc_prices_source/engines/btc_ars_decrypto.py
 moc_prices_source/engines/btc_ars_ripio.py
 moc_prices_source/engines/btc_ars_ripio_exch.py
 moc_prices_source/engines/btc_ars_rofex.py
 moc_prices_source/engines/btc_ars_satoshitango.py
-moc_prices_source/engines/btc_usd_binance.py
 moc_prices_source/engines/btc_usd_bitfinex.py
 moc_prices_source/engines/btc_usd_bitgo.py
 moc_prices_source/engines/btc_usd_bitstamp.py
 moc_prices_source/engines/btc_usd_bittrex.py
 moc_prices_source/engines/btc_usd_blockchain.py
 moc_prices_source/engines/btc_usd_cex.py
 moc_prices_source/engines/btc_usd_coinbase.py
@@ -48,14 +47,15 @@
 moc_prices_source/engines/coins.py
 moc_prices_source/engines/engine_base.py
 moc_prices_source/engines/eth_btc_binance.py
 moc_prices_source/engines/eth_btc_bitfinex.py
 moc_prices_source/engines/eth_btc_bitstamp.py
 moc_prices_source/engines/eth_btc_gemini.py
 moc_prices_source/engines/eth_btc_kraken.py
+moc_prices_source/engines/gas_btc_rsk.py
 moc_prices_source/engines/moc_btc_sovryn.py
 moc_prices_source/engines/rif_btc_binance.py
 moc_prices_source/engines/rif_btc_bitfinex.py
 moc_prices_source/engines/rif_btc_bithumbpro.py
 moc_prices_source/engines/rif_btc_coinbene.py
 moc_prices_source/engines/rif_btc_coingecko.py
 moc_prices_source/engines/rif_btc_kucoin.py
```

### Comparing `moneyonchain_prices_source-0.6.5b0/setup.py` & `moneyonchain_prices_source-0.6.6b0/setup.py`

 * *Files identical despite different names*

