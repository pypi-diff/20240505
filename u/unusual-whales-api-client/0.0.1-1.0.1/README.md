# Comparing `tmp/unusual_whales_api_client-0.0.1.tar.gz` & `tmp/unusual_whales_api_client-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unusual_whales_api_client-0.0.1.tar", max compression
+gzip compressed data, was "unusual_whales_api_client-1.0.1.tar", max compression
```

## Comparing `unusual_whales_api_client-0.0.1.tar` & `unusual_whales_api_client-1.0.1.tar`

### file list

```diff
@@ -1,168 +1,173 @@
--rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusual_whales_api_client-0.0.1/LICENSE
--rw-r--r--   0        0        0     5152 2024-05-04 17:34:12.918794 unusual_whales_api_client-0.0.1/README.md
--rw-r--r--   0        0        0      604 2024-05-04 17:34:12.919059 unusual_whales_api_client-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      161 2024-05-04 17:34:12.919627 unusual_whales_api_client-0.0.1/unusual_whales_api_client/__init__.py
--rw-r--r--   0        0        0       45 2024-05-04 17:34:12.919815 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.919898 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/__init__.py
--rw-r--r--   0        0        0     6549 2024-05-04 17:34:12.920132 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_late_reports.py
--rw-r--r--   0        0        0     6567 2024-05-04 17:34:12.920302 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_recent_reports.py
--rw-r--r--   0        0        0     6538 2024-05-04 17:34:12.920485 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_recent_trades.py
--rw-r--r--   0        0        0     7572 2024-05-04 17:34:12.920676 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_trader.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.920778 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/darkpool/__init__.py
--rw-r--r--   0        0        0     6057 2024-05-04 17:34:12.921033 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/darkpool/public_api_darkpool_controller_darkpool_recent.py
--rw-r--r--   0        0        0     7133 2024-05-04 17:34:12.921383 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/darkpool/public_api_darkpool_controller_darkpool_ticker.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.921496 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/__init__.py
--rw-r--r--   0        0        0     5739 2024-05-04 17:34:12.921740 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_afterhours.py
--rw-r--r--   0        0        0     5730 2024-05-04 17:34:12.921928 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_premarket.py
--rw-r--r--   0        0        0     4463 2024-05-04 17:34:12.922113 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_ticker.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.922222 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/__init__.py
--rw-r--r--   0        0        0     3858 2024-05-04 17:34:12.922472 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_exposure.py
--rw-r--r--   0        0        0     3762 2024-05-04 17:34:12.922659 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_holdings.py
--rw-r--r--   0        0        0     4445 2024-05-04 17:34:12.922852 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_info.py
--rw-r--r--   0        0        0     4727 2024-05-04 17:34:12.923041 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_weights.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.923148 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/__init__.py
--rw-r--r--   0        0        0     6752 2024-05-04 17:34:12.923482 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_etf_tide.py
--rw-r--r--   0        0        0     3714 2024-05-04 17:34:12.923784 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_events.py
--rw-r--r--   0        0        0     3688 2024-05-04 17:34:12.924343 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_fda_calendar.py
--rw-r--r--   0        0        0     3663 2024-05-04 17:34:12.924489 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_holidays.py
--rw-r--r--   0        0        0     3683 2024-05-04 17:34:12.924645 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_imbalances.py
--rw-r--r--   0        0        0     5585 2024-05-04 17:34:12.924910 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_insider_buy_sells.py
--rw-r--r--   0        0        0    12411 2024-05-04 17:34:12.925080 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_market_tide.py
--rw-r--r--   0        0        0     7183 2024-05-04 17:34:12.925231 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py
--rw-r--r--   0        0        0     4225 2024-05-04 17:34:12.925369 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_sector_etfs.py
--rw-r--r--   0        0        0     5668 2024-05-04 17:34:12.925512 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_spike.py
--rw-r--r--   0        0        0     5948 2024-05-04 17:34:12.925654 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_total_options_volume.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.925726 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/__init__.py
--rw-r--r--   0        0        0     5802 2024-05-04 17:34:12.925914 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_expiry_breakdown.py
--rw-r--r--   0        0        0     9406 2024-05-04 17:34:12.926102 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_flow.py
--rw-r--r--   0        0        0     5766 2024-05-04 17:34:12.926246 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_history.py
--rw-r--r--   0        0        0    10684 2024-05-04 17:34:12.926583 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_option_contracts.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.926770 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_trade/__init__.py
--rw-r--r--   0        0        0    28812 2024-05-04 17:34:12.927163 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_trade/public_api_option_trade_controller_flow_alerts.py
--rw-r--r--   0        0        0     3002 2024-05-04 17:34:12.927497 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_trade/public_api_option_trade_controller_full_tape.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.927620 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/__init__.py
--rw-r--r--   0        0        0     8848 2024-05-04 17:34:12.927979 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_analyst_ratings.py
--rw-r--r--   0        0        0    45415 2024-05-04 17:34:12.928436 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_contract_screener.py
--rw-r--r--   0        0        0    64182 2024-05-04 17:34:12.928930 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_stock_screener.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.929058 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/__init__.py
--rw-r--r--   0        0        0     4093 2024-05-04 17:34:12.929324 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_market_seasonality.py
--rw-r--r--   0        0        0    13524 2024-05-04 17:34:12.929542 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_month_performers.py
--rw-r--r--   0        0        0     4674 2024-05-04 17:34:12.929731 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_monthly.py
--rw-r--r--   0        0        0     4800 2024-05-04 17:34:12.930033 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_year_month.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.930145 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/__init__.py
--rw-r--r--   0        0        0     5539 2024-05-04 17:34:12.930371 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_atm_chains.py
--rw-r--r--   0        0        0     4505 2024-05-04 17:34:12.930561 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_companies_in_sector.py
--rw-r--r--   0        0        0     5426 2024-05-04 17:34:12.930731 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_alerts.py
--rw-r--r--   0        0        0     3977 2024-05-04 17:34:12.930983 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_per_expiry.py
--rw-r--r--   0        0        0     4584 2024-05-04 17:34:12.931254 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_per_strike.py
--rw-r--r--   0        0        0     7120 2024-05-04 17:34:12.931660 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_recent.py
--rw-r--r--   0        0        0    14029 2024-05-04 17:34:12.931947 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure.py
--rw-r--r--   0        0        0     6063 2024-05-04 17:34:12.932530 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_expiry.py
--rw-r--r--   0        0        0     6063 2024-05-04 17:34:12.932670 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6713 2024-05-04 17:34:12.932814 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_strike_expiry.py
--rw-r--r--   0        0        0     6170 2024-05-04 17:34:12.933049 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greeks.py
--rw-r--r--   0        0        0     8800 2024-05-04 17:34:12.933222 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_historical_risk_reversal_skew.py
--rw-r--r--   0        0        0     6260 2024-05-04 17:34:12.933359 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_implied_volatility_term_structure.py
--rw-r--r--   0        0        0     6073 2024-05-04 17:34:12.933493 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py
--rw-r--r--   0        0        0     4905 2024-05-04 17:34:12.933629 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_insider_buy_sell.py
--rw-r--r--   0        0        0     4566 2024-05-04 17:34:12.933766 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_max_pain.py
--rw-r--r--   0        0        0    10450 2024-05-04 17:34:12.933924 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_net_prem_ticks.py
--rw-r--r--   0        0        0     8976 2024-05-04 17:34:12.934086 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_ohlc.py
--rw-r--r--   0        0        0     7629 2024-05-04 17:34:12.934235 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_oi_change.py
--rw-r--r--   0        0        0     7213 2024-05-04 17:34:12.934369 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_option_chains.py
--rw-r--r--   0        0        0     5861 2024-05-04 17:34:12.934517 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_option_price_level.py
--rw-r--r--   0        0        0     6568 2024-05-04 17:34:12.934797 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_options_volume.py
--rw-r--r--   0        0        0    14437 2024-05-04 17:34:12.934956 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_spot_exposures_by_strike.py
--rw-r--r--   0        0        0    14016 2024-05-04 17:34:12.935106 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_spot_exposures_one_minute.py
--rw-r--r--   0        0        0     6722 2024-05-04 17:34:12.935235 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_stock_volume_price_level.py
--rw-r--r--   0        0        0     5909 2024-05-04 17:34:12.935370 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_vol_oi_per_expiry.py
--rw-r--r--   0        0        0        0 2024-05-04 17:34:12.935456 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/websocket/__init__.py
--rw-r--r--   0        0        0    10037 2024-05-04 17:34:12.935696 unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/websocket/public_api_socket_controller_channels.py
--rw-r--r--   0        0        0     6788 2024-05-04 17:34:12.935867 unusual_whales_api_client-0.0.1/unusual_whales_api_client/client.py
--rw-r--r--   0        0        0      546 2024-05-04 17:34:12.936039 unusual_whales_api_client-0.0.1/unusual_whales_api_client/errors.py
--rw-r--r--   0        0        0     6501 2024-05-04 17:34:12.936224 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-04 17:34:12.936364 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_action.py
--rw-r--r--   0        0        0      267 2024-05-04 17:34:12.936521 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_field_action.py
--rw-r--r--   0        0        0      183 2024-05-04 17:34:12.936660 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_field_recommendation.py
--rw-r--r--   0        0        0     6691 2024-05-04 17:34:12.936909 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_rating.py
--rw-r--r--   0        0        0      178 2024-05-04 17:34:12.937183 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_recommendation.py
--rw-r--r--   0        0        0      428 2024-05-04 17:34:12.937596 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_sector.py
--rw-r--r--   0        0        0     5399 2024-05-04 17:34:12.937766 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/candle_data.py
--rw-r--r--   0        0        0      251 2024-05-04 17:34:12.937940 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/candle_size.py
--rw-r--r--   0        0        0     5200 2024-05-04 17:34:12.938084 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/country_sector_exposure.py
--rw-r--r--   0        0        0     3869 2024-05-04 17:34:12.938230 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/daily_market_tide.py
--rw-r--r--   0        0        0    10341 2024-05-04 17:34:12.938404 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/darkpool_trade.py
--rw-r--r--   0        0        0     8919 2024-05-04 17:34:12.938578 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/earning.py
--rw-r--r--   0        0        0     4185 2024-05-04 17:34:12.938847 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/economic_calendar.py
--rw-r--r--   0        0        0      189 2024-05-04 17:34:12.939016 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/economic_type.py
--rw-r--r--   0        0        0     2673 2024-05-04 17:34:12.939192 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/error_message.py
--rw-r--r--   0        0        0     1779 2024-05-04 17:34:12.939370 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
--rw-r--r--   0        0        0     2063 2024-05-04 17:34:12.939552 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_countries_item.py
--rw-r--r--   0        0        0     7575 2024-05-04 17:34:12.939830 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_info.py
--rw-r--r--   0        0        0     2044 2024-05-04 17:34:12.940009 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_sectors_item.py
--rw-r--r--   0        0        0     2953 2024-05-04 17:34:12.940155 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/expiry_breakdown.py
--rw-r--r--   0        0        0     5086 2024-05-04 17:34:12.940411 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/fda_calendar.py
--rw-r--r--   0        0        0    10635 2024-05-04 17:34:12.940588 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_alert.py
--rw-r--r--   0        0        0      590 2024-05-04 17:34:12.940754 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_alert_rule.py
--rw-r--r--   0        0        0    12800 2024-05-04 17:34:12.940916 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_per_expiry.py
--rw-r--r--   0        0        0    12688 2024-05-04 17:34:12.941079 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_per_strike.py
--rw-r--r--   0        0        0     6320 2024-05-04 17:34:12.941430 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure.py
--rw-r--r--   0        0        0     6349 2024-05-04 17:34:12.941745 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6808 2024-05-04 17:34:12.941885 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py
--rw-r--r--   0        0        0     9046 2024-05-04 17:34:12.942035 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greeks.py
--rw-r--r--   0        0        0     2535 2024-05-04 17:34:12.942168 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py
--rw-r--r--   0        0        0    10020 2024-05-04 17:34:12.942324 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/holdings.py
--rw-r--r--   0        0        0     4229 2024-05-04 17:34:12.942571 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/imbalances_volume.py
--rw-r--r--   0        0        0     4426 2024-05-04 17:34:12.942707 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py
--rw-r--r--   0        0        0     3678 2024-05-04 17:34:12.942900 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/insider_statistics.py
--rw-r--r--   0        0        0      190 2024-05-04 17:34:12.943147 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/insider_trades_member_type.py
--rw-r--r--   0        0        0      345 2024-05-04 17:34:12.943755 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/insider_trades_transaction_type.py
--rw-r--r--   0        0        0      164 2024-05-04 17:34:12.943900 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_imbalance_event.py
--rw-r--r--   0        0        0      165 2024-05-04 17:34:12.944039 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_imbalance_side.py
--rw-r--r--   0        0        0      213 2024-05-04 17:34:12.944166 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_imbalance_type.py
--rw-r--r--   0        0        0      168 2024-05-04 17:34:12.944286 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_market_time.py
--rw-r--r--   0        0        0      528 2024-05-04 17:34:12.944425 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_sector.py
--rw-r--r--   0        0        0     4512 2024-05-04 17:34:12.944573 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_holidays.py
--rw-r--r--   0        0        0     3378 2024-05-04 17:34:12.944707 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_options_volume.py
--rw-r--r--   0        0        0     2680 2024-05-04 17:34:12.944835 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/max_pain.py
--rw-r--r--   0        0        0     5964 2024-05-04 17:34:12.945014 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/net_prem_tick_response.py
--rw-r--r--   0        0        0     2494 2024-05-04 17:34:12.945148 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/off_lit_price_level.py
--rw-r--r--   0        0        0    11261 2024-05-04 17:34:12.945327 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/oi_change.py
--rw-r--r--   0        0        0     1742 2024-05-04 17:34:12.945472 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_chains_response.py
--rw-r--r--   0        0        0    10819 2024-05-04 17:34:12.945637 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contract.py
--rw-r--r--   0        0        0    14886 2024-05-04 17:34:12.945796 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contract_screener_response.py
--rw-r--r--   0        0        0      157 2024-05-04 17:34:12.945941 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contract_type.py
--rw-r--r--   0        0        0    11268 2024-05-04 17:34:12.946112 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contracts.py
--rw-r--r--   0        0        0     2522 2024-05-04 17:34:12.946262 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_price_level.py
--rw-r--r--   0        0        0      149 2024-05-04 17:34:12.946381 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_type.py
--rw-r--r--   0        0        0      153 2024-05-04 17:34:12.946510 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/order_direction.py
--rw-r--r--   0        0        0      949 2024-05-04 17:34:12.946646 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py
--rw-r--r--   0        0        0     1401 2024-05-04 17:34:12.946770 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/screener_order_by_field.py
--rw-r--r--   0        0        0     5330 2024-05-04 17:34:12.946907 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_market.py
--rw-r--r--   0        0        0     5009 2024-05-04 17:34:12.947077 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_monthly.py
--rw-r--r--   0        0        0      412 2024-05-04 17:34:12.947212 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_performance_order_by.py
--rw-r--r--   0        0        0     6634 2024-05-04 17:34:12.947383 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_performers.py
--rw-r--r--   0        0        0     3121 2024-05-04 17:34:12.947519 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_year_month.py
--rw-r--r--   0        0        0      515 2024-05-04 17:34:12.947646 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/sector.py
--rw-r--r--   0        0        0    10842 2024-05-04 17:34:12.947809 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/sector_etf.py
--rw-r--r--   0        0        0     5674 2024-05-04 17:34:12.948077 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/senate_stock.py
--rw-r--r--   0        0        0      173 2024-05-04 17:34:12.948298 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/side.py
--rw-r--r--   0        0        0      206 2024-05-04 17:34:12.948547 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_issue_type.py
--rw-r--r--   0        0        0      343 2024-05-04 17:34:12.948968 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_month_number.py
--rw-r--r--   0        0        0      521 2024-05-04 17:34:12.949092 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_sector.py
--rw-r--r--   0        0        0      334 2024-05-04 17:34:12.949216 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_trade_external_hour_sold_code.py
--rw-r--r--   0        0        0      312 2024-05-04 17:34:12.949349 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_trade_sale_cond_code.py
--rw-r--r--   0        0        0      304 2024-05-04 17:34:12.949480 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_trade_settlement.py
--rw-r--r--   0        0        0      275 2024-05-04 17:34:12.949601 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_trade_trade_code.py
--rw-r--r--   0        0        0     2304 2024-05-04 17:34:12.949724 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spike_value.py
--rw-r--r--   0        0        0     7769 2024-05-04 17:34:12.949990 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py
--rw-r--r--   0        0        0     8339 2024-05-04 17:34:12.950147 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py
--rw-r--r--   0        0        0      202 2024-05-04 17:34:12.950271 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/stock_earnings_time.py
--rw-r--r--   0        0        0      205 2024-05-04 17:34:12.950390 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/stock_issue_type.py
--rw-r--r--   0        0        0    24207 2024-05-04 17:34:12.950637 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/stock_screener_response.py
--rw-r--r--   0        0        0     8648 2024-05-04 17:34:12.950817 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/ticker_info.py
--rw-r--r--   0        0        0    11609 2024-05-04 17:34:12.950976 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/ticker_options_volume.py
--rw-r--r--   0        0        0     2436 2024-05-04 17:34:12.951121 unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py
--rw-r--r--   0        0        0       25 2024-05-04 17:34:12.951248 unusual_whales_api_client-0.0.1/unusual_whales_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-05-04 17:34:12.951493 unusual_whales_api_client-0.0.1/unusual_whales_api_client/types.py
--rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 unusual_whales_api_client-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusual_whales_api_client-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5152 2024-05-04 17:34:12.918794 unusual_whales_api_client-1.0.1/README.md
+-rw-r--r--   0        0        0      604 2024-05-05 00:05:59.438598 unusual_whales_api_client-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-05 00:05:50.800080 unusual_whales_api_client-1.0.1/unusual_whales_api_client/.DS_Store
+-rw-r--r--   0        0        0      161 2024-05-04 23:06:03.901106 unusual_whales_api_client-1.0.1/unusual_whales_api_client/__init__.py
+-rw-r--r--   0        0        0    10244 2024-05-05 00:05:42.270268 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/.DS_Store
+-rw-r--r--   0        0        0       45 2024-05-04 23:06:03.900019 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.254843 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-04 23:06:03.899211 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trade_report.py
+-rw-r--r--   0        0        0     7572 2024-05-04 23:06:03.899581 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trades.py
+-rw-r--r--   0        0        0     6538 2024-05-04 23:06:03.899164 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congressional_trades.py
+-rw-r--r--   0        0        0     6549 2024-05-04 23:06:03.898428 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_recent_late_reports.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.292207 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/__init__.py
+-rw-r--r--   0        0        0     5711 2024-05-04 23:06:03.901311 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_atm_contracts_for_expiries.py
+-rw-r--r--   0        0        0     5666 2024-05-04 23:06:03.902527 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_contract_price_history.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.271540 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/__init__.py
+-rw-r--r--   0        0        0     6057 2024-05-04 23:06:03.901371 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades.py
+-rw-r--r--   0        0        0     7133 2024-05-04 23:06:03.900367 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades_by_ticker.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.272908 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-04 23:06:03.898240 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_after_hours_earnings.py
+-rw-r--r--   0        0        0     4463 2024-05-04 23:06:03.899179 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_earnings_history.py
+-rw-r--r--   0        0        0     5730 2024-05-04 23:06:03.899777 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_premarket_earnings.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.275749 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/__init__.py
+-rw-r--r--   0        0        0     3778 2024-05-04 23:06:03.902152 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_holdings.py
+-rw-r--r--   0        0        0     4445 2024-05-04 23:06:03.903125 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_info.py
+-rw-r--r--   0        0        0     4727 2024-05-04 23:06:03.897476 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_sector_country_weights.py
+-rw-r--r--   0        0        0     3914 2024-05-04 23:06:03.897841 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_ticker_exposure_by_etf.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.285035 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/__init__.py
+-rw-r--r--   0        0        0     8758 2024-05-04 23:06:03.897691 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_contract_flow.py
+-rw-r--r--   0        0        0     6018 2024-05-04 23:06:03.897497 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_daily_expiry_breakdown.py
+-rw-r--r--   0        0        0     4221 2024-05-04 23:06:03.897850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_expiry.py
+-rw-r--r--   0        0        0     4716 2024-05-04 23:06:03.897790 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_strike.py
+-rw-r--r--   0        0        0     3110 2024-05-04 23:06:03.897218 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_full_tape.py
+-rw-r--r--   0        0        0     5518 2024-05-04 23:06:03.899198 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_order_flow_alerts.py
+-rw-r--r--   0        0        0    28988 2024-05-04 23:06:03.897976 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_ticker_order_flow.py
+-rw-r--r--   0        0        0     7172 2024-05-04 23:06:03.898647 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/public_api_ticker_controller_flow_recent.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.331076 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/__init__.py
+-rw-r--r--   0        0        0    14016 2024-05-04 23:06:03.898820 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures.py
+-rw-r--r--   0        0        0    14437 2024-05-04 23:06:03.898171 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures_by_strike.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.277994 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/__init__.py
+-rw-r--r--   0        0        0     3714 2024-05-04 23:06:03.901870 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_economic_calendar.py
+-rw-r--r--   0        0        0     3688 2024-05-04 23:06:03.903282 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_fda_calendar.py
+-rw-r--r--   0        0        0     3663 2024-05-04 23:06:03.900776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_holidays.py
+-rw-r--r--   0        0        0     3735 2024-05-04 23:06:03.903362 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_imbalances.py
+-rw-r--r--   0        0        0     5585 2024-05-04 23:06:03.903037 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_insider_trades.py
+-rw-r--r--   0        0        0     6092 2024-05-04 23:06:03.901315 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_options_volume.py
+-rw-r--r--   0        0        0    12539 2024-05-04 23:06:03.902895 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide.py
+-rw-r--r--   0        0        0     6888 2024-05-04 23:06:03.900097 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide_by_etf.py
+-rw-r--r--   0        0        0     4441 2024-05-04 23:06:03.900893 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_sector_stats.py
+-rw-r--r--   0        0        0     5668 2024-05-04 23:06:03.901797 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_spike.py
+-rw-r--r--   0        0        0     7443 2024-05-04 23:06:03.899547 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.319520 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/__init__.py
+-rw-r--r--   0        0        0    14029 2024-05-04 23:06:03.904164 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure.py
+-rw-r--r--   0        0        0     6143 2024-05-04 23:06:03.899839 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_expiry.py
+-rw-r--r--   0        0        0     6211 2024-05-04 23:06:03.903029 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6713 2024-05-04 23:06:03.903077 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike_expiry.py
+-rw-r--r--   0        0        0     6286 2024-05-04 23:06:03.903697 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greeks_by_strike_expiry.py
+-rw-r--r--   0        0        0     4566 2024-05-04 23:06:03.903668 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_max_pain.py
+-rw-r--r--   0        0        0    10450 2024-05-04 23:06:03.899392 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_net_premium_ticks.py
+-rw-r--r--   0        0        0     7629 2024-05-04 23:06:03.904034 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_open_interest_change.py
+-rw-r--r--   0        0        0     7213 2024-05-04 23:06:03.904169 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_chains.py
+-rw-r--r--   0        0        0    10684 2024-05-04 23:06:03.903715 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_contracts.py
+-rw-r--r--   0        0        0     5861 2024-05-04 23:06:03.903627 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_volume_by_price_level.py
+-rw-r--r--   0        0        0     5856 2024-05-04 23:06:03.903933 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_options_volume.py
+-rw-r--r--   0        0        0     5909 2024-05-04 23:06:03.904024 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_volume_open_interest_by_expiry.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.293446 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/__init__.py
+-rw-r--r--   0        0        0     8900 2024-05-04 23:06:03.901873 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_analyst_ratings.py
+-rw-r--r--   0        0        0    45475 2024-05-04 23:06:03.902568 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_option_contracts.py
+-rw-r--r--   0        0        0    64194 2024-05-04 23:06:03.901278 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_stocks.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.304536 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/__init__.py
+-rw-r--r--   0        0        0     4129 2024-05-04 23:06:03.902965 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_market_average_returns_by_month.py
+-rw-r--r--   0        0        0     4674 2024-05-04 23:06:03.903285 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_average_returns.py
+-rw-r--r--   0        0        0    13580 2024-05-04 23:06:03.900876 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_top_performers.py
+-rw-r--r--   0        0        0     4800 2024-05-04 23:06:03.901739 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_price_changes_by_month_and_year.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.308574 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/__init__.py
+-rw-r--r--   0        0        0     8976 2024-05-04 23:06:03.898970 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_candles.py
+-rw-r--r--   0        0        0     4905 2024-05-04 23:06:03.899798 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_insider_trades.py
+-rw-r--r--   0        0        0     4561 2024-05-04 23:06:03.898188 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_sector_tickers.py
+-rw-r--r--   0        0        0     6260 2024-05-04 23:06:03.899956 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volatility_term_structure.py
+-rw-r--r--   0        0        0     7026 2024-05-04 23:06:03.899490 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volume_by_price_level.py
+-rw-r--r--   0        0        0     6101 2024-05-04 23:06:03.897503 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.330040 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/__init__.py
+-rw-r--r--   0        0        0     8884 2024-05-04 23:06:03.900700 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/get_risk_reversal_skew.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.307484 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/__init__.py
+-rw-r--r--   0        0        0    10067 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/channels.py
+-rw-r--r--   0        0        0    12417 2024-05-04 23:06:03.901552 unusual_whales_api_client-1.0.1/unusual_whales_api_client/client.py
+-rw-r--r--   0        0        0      546 2024-05-04 23:06:03.897133 unusual_whales_api_client-1.0.1/unusual_whales_api_client/errors.py
+-rw-r--r--   0        0        0     6501 2024-05-04 23:06:03.901695 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-04 23:06:03.880396 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_action.py
+-rw-r--r--   0        0        0      267 2024-05-04 23:06:03.873332 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_field_action.py
+-rw-r--r--   0        0        0      183 2024-05-04 23:06:03.872281 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_field_recommendation.py
+-rw-r--r--   0        0        0     6697 2024-05-04 23:06:03.899197 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_rating.py
+-rw-r--r--   0        0        0      178 2024-05-04 23:06:03.867691 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_recommendation.py
+-rw-r--r--   0        0        0      428 2024-05-04 23:06:03.871869 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_sector.py
+-rw-r--r--   0        0        0     5399 2024-05-04 23:06:03.897314 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_data.py
+-rw-r--r--   0        0        0      251 2024-05-04 23:06:03.868214 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_size.py
+-rw-r--r--   0        0        0     5200 2024-05-04 23:06:03.899759 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/country_sector_exposure.py
+-rw-r--r--   0        0        0     3869 2024-05-04 23:06:03.899833 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/daily_market_tide.py
+-rw-r--r--   0        0        0    10341 2024-05-04 23:06:03.903785 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/darkpool_trade.py
+-rw-r--r--   0        0        0     8919 2024-05-04 23:06:03.901180 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/earning.py
+-rw-r--r--   0        0        0     4185 2024-05-04 23:06:03.901806 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_calendar.py
+-rw-r--r--   0        0        0      189 2024-05-04 23:06:03.868741 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_type.py
+-rw-r--r--   0        0        0     2673 2024-05-04 23:06:03.897366 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message.py
+-rw-r--r--   0        0        0     1779 2024-05-04 23:06:03.902052 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
+-rw-r--r--   0        0        0     2063 2024-05-04 23:06:03.897630 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_countries_item.py
+-rw-r--r--   0        0        0     7575 2024-05-04 23:06:03.901157 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_info.py
+-rw-r--r--   0        0        0     2044 2024-05-04 23:06:03.901145 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_sectors_item.py
+-rw-r--r--   0        0        0     2953 2024-05-04 23:06:03.903989 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/expiry_breakdown.py
+-rw-r--r--   0        0        0     5086 2024-05-04 23:06:03.898753 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/fda_calendar.py
+-rw-r--r--   0        0        0    10635 2024-05-04 23:06:03.899489 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert.py
+-rw-r--r--   0        0        0      590 2024-05-04 23:06:03.871726 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert_rule.py
+-rw-r--r--   0        0        0    12800 2024-05-04 23:06:03.904343 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_expiry.py
+-rw-r--r--   0        0        0    12688 2024-05-04 23:06:03.898718 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_strike.py
+-rw-r--r--   0        0        0     6320 2024-05-04 23:06:03.899850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure.py
+-rw-r--r--   0        0        0     6349 2024-05-04 23:06:03.898856 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6808 2024-05-04 23:06:03.903104 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py
+-rw-r--r--   0        0        0     9046 2024-05-04 23:06:03.899966 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greeks.py
+-rw-r--r--   0        0        0     2535 2024-05-04 23:06:03.900308 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py
+-rw-r--r--   0        0        0    10020 2024-05-04 23:06:03.900599 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/holdings.py
+-rw-r--r--   0        0        0     4229 2024-05-04 23:06:03.899326 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/imbalances_volume.py
+-rw-r--r--   0        0        0     4426 2024-05-04 23:06:03.900807 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py
+-rw-r--r--   0        0        0     3678 2024-05-04 23:06:03.898099 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_statistics.py
+-rw-r--r--   0        0        0      190 2024-05-04 23:06:03.870716 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_trades_member_type.py
+-rw-r--r--   0        0        0      345 2024-05-04 23:06:03.872052 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_trades_transaction_type.py
+-rw-r--r--   0        0        0      164 2024-05-04 23:06:03.875455 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_event.py
+-rw-r--r--   0        0        0      165 2024-05-04 23:06:03.877003 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_side.py
+-rw-r--r--   0        0        0      213 2024-05-04 23:06:03.876685 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_type.py
+-rw-r--r--   0        0        0      168 2024-05-04 23:06:03.868907 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_market_time.py
+-rw-r--r--   0        0        0      528 2024-05-04 23:06:03.878990 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_sector.py
+-rw-r--r--   0        0        0     4512 2024-05-04 23:06:03.898435 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_holidays.py
+-rw-r--r--   0        0        0     3378 2024-05-04 23:06:03.902850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_options_volume.py
+-rw-r--r--   0        0        0     2680 2024-05-04 23:06:03.901776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/max_pain.py
+-rw-r--r--   0        0        0     5964 2024-05-04 23:06:03.898508 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/net_prem_tick_response.py
+-rw-r--r--   0        0        0     2494 2024-05-04 23:06:03.901791 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/off_lit_price_level.py
+-rw-r--r--   0        0        0    11261 2024-05-04 23:06:03.900810 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/oi_change.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:06:03.898550 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_chains_response.py
+-rw-r--r--   0        0        0    10940 2024-05-04 23:06:03.898496 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract.py
+-rw-r--r--   0        0        0    14886 2024-05-04 23:06:03.898299 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_screener_response.py
+-rw-r--r--   0        0        0      157 2024-05-04 23:06:03.875604 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_type.py
+-rw-r--r--   0        0        0    11268 2024-05-04 23:06:03.900558 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contracts.py
+-rw-r--r--   0        0        0     2522 2024-05-04 23:06:03.899171 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_price_level.py
+-rw-r--r--   0        0        0      149 2024-05-04 23:06:03.877920 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_type.py
+-rw-r--r--   0        0        0      153 2024-05-04 23:06:03.870845 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/order_direction.py
+-rw-r--r--   0        0        0      949 2024-05-04 23:06:03.878579 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py
+-rw-r--r--   0        0        0     1401 2024-05-04 23:06:03.877776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_order_by_field.py
+-rw-r--r--   0        0        0     5330 2024-05-04 23:06:03.902577 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_market.py
+-rw-r--r--   0        0        0     5009 2024-05-04 23:06:03.897915 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_monthly.py
+-rw-r--r--   0        0        0      412 2024-05-04 23:06:03.871752 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performance_order_by.py
+-rw-r--r--   0        0        0     6634 2024-05-04 23:06:03.898503 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performers.py
+-rw-r--r--   0        0        0     3121 2024-05-04 23:06:03.903851 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_year_month.py
+-rw-r--r--   0        0        0      515 2024-05-04 23:06:03.867719 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector.py
+-rw-r--r--   0        0        0    10842 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector_etf.py
+-rw-r--r--   0        0        0     5674 2024-05-04 23:06:03.897567 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/senate_stock.py
+-rw-r--r--   0        0        0      173 2024-05-04 23:06:03.867695 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/side.py
+-rw-r--r--   0        0        0      206 2024-05-04 23:06:03.867692 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_issue_type.py
+-rw-r--r--   0        0        0      343 2024-05-04 23:06:03.879664 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_month_number.py
+-rw-r--r--   0        0        0      521 2024-05-04 23:06:03.869738 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_sector.py
+-rw-r--r--   0        0        0      334 2024-05-04 23:06:03.870776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_external_hour_sold_code.py
+-rw-r--r--   0        0        0      312 2024-05-04 23:06:03.879928 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_sale_cond_code.py
+-rw-r--r--   0        0        0      304 2024-05-04 23:06:03.871735 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_settlement.py
+-rw-r--r--   0        0        0      275 2024-05-04 23:06:03.871914 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_trade_code.py
+-rw-r--r--   0        0        0     2304 2024-05-04 23:06:03.903870 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spike_value.py
+-rw-r--r--   0        0        0     7769 2024-05-04 23:06:03.901158 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py
+-rw-r--r--   0        0        0     8339 2024-05-04 23:06:03.900787 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py
+-rw-r--r--   0        0        0      202 2024-05-04 23:06:03.869883 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_earnings_time.py
+-rw-r--r--   0        0        0      205 2024-05-04 23:06:03.874468 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_issue_type.py
+-rw-r--r--   0        0        0    24207 2024-05-04 23:06:03.900228 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_screener_response.py
+-rw-r--r--   0        0        0     8648 2024-05-04 23:06:03.899314 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_info.py
+-rw-r--r--   0        0        0    11609 2024-05-04 23:06:03.901548 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_options_volume.py
+-rw-r--r--   0        0        0     2436 2024-05-04 23:06:03.900259 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py
+-rw-r--r--   0        0        0       25 2024-05-04 23:06:03.164456 unusual_whales_api_client-1.0.1/unusual_whales_api_client/py.typed
+-rw-r--r--   0        0        0      985 2024-05-04 23:06:03.897220 unusual_whales_api_client-1.0.1/unusual_whales_api_client/types.py
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 unusual_whales_api_client-1.0.1/PKG-INFO
```

### Comparing `unusual_whales_api_client-0.0.1/LICENSE` & `unusual_whales_api_client-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/README.md` & `unusual_whales_api_client-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/pyproject.toml` & `unusual_whales_api_client-1.0.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unusual-whales-api-client"
-version = "0.0.1"
+version = "1.0.1"
 description = "A client library for accessing Unusual Whales API"
 authors = []
 readme = "README.md"
 packages = [
     {include = "unusual_whales_api_client"},
 ]
 include = ["CHANGELOG.md", "unusual_whales_api_client/py.typed"]
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_late_reports.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_recent_late_reports.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_recent_reports.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trade_report.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_recent_trades.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congressional_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/congress/public_api_congress_controller_congress_trader.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/darkpool/public_api_darkpool_controller_darkpool_recent.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/darkpool/public_api_darkpool_controller_darkpool_ticker.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades_by_ticker.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_afterhours.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_after_hours_earnings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_premarket.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_premarket_earnings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/earnings/public_api_earnings_controller_ticker.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_earnings_history.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_exposure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_ticker_exposure_by_etf.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Holdings]:
-    """Exposure
+    """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -72,15 +72,15 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Holdings]:
-    """Exposure
+    """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -98,15 +98,15 @@
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Holdings]:
-    """Exposure
+    """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -127,15 +127,15 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Holdings]:
-    """Exposure
+    """Ticker Exposure by ETF
 
      Returns all ETFs in which the given ticker is a holding
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_holdings.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_holdings.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Holdings]:
-    """Holdings
+    """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -72,15 +72,15 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Holdings]:
-    """Holdings
+    """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -98,15 +98,15 @@
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Holdings]:
-    """Holdings
+    """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -127,15 +127,15 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Holdings]:
-    """Holdings
+    """ETF Holdings
 
      Returns the holdings of the ETF
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_info.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/etfs/public_api_etf_controller_weights.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_sector_country_weights.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_etf_tide.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide_by_etf.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
-    """ETF Tide
+    """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
 
     Args:
         ticker (str): A comma separated list of tickers. To exclude certain tickers prefix the
@@ -102,15 +102,15 @@
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
-    """ETF Tide
+    """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
 
     Args:
         ticker (str): A comma separated list of tickers. To exclude certain tickers prefix the
@@ -136,15 +136,15 @@
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
-    """ETF Tide
+    """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
 
     Args:
         ticker (str): A comma separated list of tickers. To exclude certain tickers prefix the
@@ -173,15 +173,15 @@
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
-    """ETF Tide
+    """Get Options Activity for the Specified ETF
 
      The ETF tide is similar to the Market Tide. While the market tide is based on options activity of
     the whole market
     the ETF tide is only based on the options activity of the holdings of the specified ETF.
 
     Args:
         ticker (str): A comma separated list of tickers. To exclude certain tickers prefix the
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_events.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_fda_calendar.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_holidays.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_holidays.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_imbalances.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_imbalances.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[ImbalancesVolume, str]]:
-    """Imbalances
+    """MOC/MOO Imbalances Data
 
      Returns the MOC/MOO imbalances.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -70,15 +70,15 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[ImbalancesVolume, str]]:
-    """Imbalances
+    """MOC/MOO Imbalances Data
 
      Returns the MOC/MOO imbalances.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -91,15 +91,15 @@
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[ImbalancesVolume, str]]:
-    """Imbalances
+    """MOC/MOO Imbalances Data
 
      Returns the MOC/MOO imbalances.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -114,15 +114,15 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[ImbalancesVolume, str]]:
-    """Imbalances
+    """MOC/MOO Imbalances Data
 
      Returns the MOC/MOO imbalances.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_insider_buy_sells.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_market_tide.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
-    """Market Tide
+    """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
     chart provides real time data based on a proprietary formula that examines market wide options
     activity and filters out 'noise'.
 
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -142,15 +142,15 @@
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
-    """Market Tide
+    """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
     chart provides real time data based on a proprietary formula that examines market wide options
     activity and filters out 'noise'.
 
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -210,15 +210,15 @@
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Response[Union[DailyMarketTide, ErrorMessage, str]]:
-    """Market Tide
+    """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
     chart provides real time data based on a proprietary formula that examines market wide options
     activity and filters out 'noise'.
 
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
@@ -281,15 +281,15 @@
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     otm_only: Union[Unset, bool] = UNSET,
     interval_5m: Union[Unset, bool] = UNSET,
 ) -> Optional[Union[DailyMarketTide, ErrorMessage, str]]:
-    """Market Tide
+    """Returns The Unusual Whales Market Tide Data
 
      Market Tide is a proprietary tool that can be viewed from the Market Overview page. The Market Tide
     chart provides real time data based on a proprietary formula that examines market wide options
     activity and filters out 'noise'.
 
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_open_interest_change.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ...client import AuthenticatedClient, Client
 from ...models.oi_change import OIChange
 from ...models.order_direction import OrderDirection
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
+    ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
@@ -28,15 +29,15 @@
 
     params["order"] = json_order
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/market/oi-change",
+        "url": f"/api/stock/{ticker}/oi-change",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[OIChange]:
@@ -56,170 +57,178 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChange]:
     """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChange]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChange]:
     """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChange
     """
 
     return sync_detailed(
+        ticker=ticker,
         client=client,
         date=date,
         limit=limit,
         order=order,
     ).parsed
 
 
 async def asyncio_detailed(
+    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChange]:
     """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChange]
     """
 
     kwargs = _get_kwargs(
+        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChange]:
     """OI Change
 
-     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
-    descending).
+     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
+        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
-            Example: 10.
+        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
+            matching data. Min: 1. Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChange
     """
 
     return (
         await asyncio_detailed(
+            ticker=ticker,
             client=client,
             date=date,
             limit=limit,
             order=order,
         )
     ).parsed
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_sector_etfs.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_sector_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,17 +45,17 @@
     )
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[SectorETF, str]]:
-    """Sector Etfs
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the current trading days statistics for the SPDR sector etfs
+     Returns the current Trading Days statistics for the SPDR sector etfs
 
     ----
     This can be used to build a market overview such as:
 
     ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
@@ -75,17 +75,17 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[SectorETF, str]]:
-    """Sector Etfs
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the current trading days statistics for the SPDR sector etfs
+     Returns the current Trading Days statistics for the SPDR sector etfs
 
     ----
     This can be used to build a market overview such as:
 
     ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
@@ -101,17 +101,17 @@
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[SectorETF, str]]:
-    """Sector Etfs
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the current trading days statistics for the SPDR sector etfs
+     Returns the current Trading Days statistics for the SPDR sector etfs
 
     ----
     This can be used to build a market overview such as:
 
     ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
@@ -129,17 +129,17 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[SectorETF, str]]:
-    """Sector Etfs
+    """Returns the stats for sector etfs for the most recent trading day
 
-     Returns the current trading days statistics for the SPDR sector etfs
+     Returns the current Trading Days statistics for the SPDR sector etfs
 
     ----
     This can be used to build a market overview such as:
 
     ![sectors etf](https://i.imgur.com/yQ5o6rR.png)
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_spike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_spike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/market/public_api_market_controller_total_options_volume.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_options_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Total Options Volume
+    """Get Options Activity for the Entire Market (Market Tide)
 
      Returns the total options volume and premium for all trade executions
     that happened on a given trading date.
 
     ----
     This can be used to build a market options overview such as:
 
@@ -99,15 +99,15 @@
 
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Total Options Volume
+    """Get Options Activity for the Entire Market (Market Tide)
 
      Returns the total options volume and premium for all trade executions
     that happened on a given trading date.
 
     ----
     This can be used to build a market options overview such as:
 
@@ -132,15 +132,15 @@
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Total Options Volume
+    """Get Options Activity for the Entire Market (Market Tide)
 
      Returns the total options volume and premium for all trade executions
     that happened on a given trading date.
 
     ----
     This can be used to build a market options overview such as:
 
@@ -168,15 +168,15 @@
 
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, MarketOptionsVolume, str]]:
-    """Total Options Volume
+    """Get Options Activity for the Entire Market (Market Tide)
 
      Returns the total options volume and premium for all trade executions
     that happened on a given trading date.
 
     ----
     This can be used to build a market options overview such as:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_expiry_breakdown.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_volume_by_price_level.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.error_message import ErrorMessage
-from ...models.expiry_breakdown import ExpiryBreakdown
+from ...models.option_price_level import OptionPriceLevel
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
@@ -19,26 +19,26 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/expiry-breakdown",
+        "url": f"/api/stock/{ticker}/option/stock-price-levels",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
+) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ExpiryBreakdown.from_dict(response.json())
+        response_200 = OptionPriceLevel.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -48,45 +48,45 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
+) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
-    """Expiry Breakdown
+) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
+    """Option Price Levels
 
-     Returns all expirations for the given trading day for a ticker.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, ExpiryBreakdown, str]]
+        Response[Union[ErrorMessage, OptionPriceLevel, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -98,62 +98,62 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
-    """Expiry Breakdown
+) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
+    """Option Price Levels
 
-     Returns all expirations for the given trading day for a ticker.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, ExpiryBreakdown, str]
+        Union[ErrorMessage, OptionPriceLevel, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
-    """Expiry Breakdown
+) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
+    """Option Price Levels
 
-     Returns all expirations for the given trading day for a ticker.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, ExpiryBreakdown, str]]
+        Response[Union[ErrorMessage, OptionPriceLevel, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -163,31 +163,31 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
-    """Expiry Breakdown
+) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
+    """Option Price Levels
 
-     Returns all expirations for the given trading day for a ticker.
+     Returns the call and put volume per price level for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, ExpiryBreakdown, str]
+        Union[ErrorMessage, OptionPriceLevel, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_flow.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_contract_flow.py`

 * *Files 15% similar despite different names*

```diff
@@ -80,19 +80,17 @@
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Flow Data
+    """Get Option Order Flow for a Given Contract
 
-     Returns the latest flows for the given option chain. Optionally a min premium and a side can be
-    supplied in the query for further filtering.
-    If no date is specified data for the last trading day is being returned.
+     Option Contract Order Flow
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
             set, will return all side's trades. Example: ASK.
         min_premium (Union[Unset, int]): The minimum premium requested trades should have. Must be
             a positive integer. Example: 50000.
@@ -130,19 +128,17 @@
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Flow Data
+    """Get Option Order Flow for a Given Contract
 
-     Returns the latest flows for the given option chain. Optionally a min premium and a side can be
-    supplied in the query for further filtering.
-    If no date is specified data for the last trading day is being returned.
+     Option Contract Order Flow
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
             set, will return all side's trades. Example: ASK.
         min_premium (Union[Unset, int]): The minimum premium requested trades should have. Must be
             a positive integer. Example: 50000.
@@ -175,19 +171,17 @@
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Flow Data
+    """Get Option Order Flow for a Given Contract
 
-     Returns the latest flows for the given option chain. Optionally a min premium and a side can be
-    supplied in the query for further filtering.
-    If no date is specified data for the last trading day is being returned.
+     Option Contract Order Flow
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
             set, will return all side's trades. Example: ASK.
         min_premium (Union[Unset, int]): The minimum premium requested trades should have. Must be
             a positive integer. Example: 50000.
@@ -223,19 +217,17 @@
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Flow Data
+    """Get Option Order Flow for a Given Contract
 
-     Returns the latest flows for the given option chain. Optionally a min premium and a side can be
-    supplied in the query for further filtering.
-    If no date is specified data for the last trading day is being returned.
+     Option Contract Order Flow
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
             set, will return all side's trades. Example: ASK.
         min_premium (Union[Unset, int]): The minimum premium requested trades should have. Must be
             a positive integer. Example: 50000.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_history.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_contract_price_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     id: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionContract, str]]:
     """Historic Data
 
-     Returns for every trading day historic data for the given option contract
+     Historic EOD Stats for the given option contract
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
             matching data. Min: 1. Example: 10.
 
     Raises:
@@ -100,15 +100,15 @@
     id: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionContract, str]]:
     """Historic Data
 
-     Returns for every trading day historic data for the given option contract
+     Historic EOD Stats for the given option contract
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
             matching data. Min: 1. Example: 10.
 
     Raises:
@@ -130,15 +130,15 @@
     id: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionContract, str]]:
     """Historic Data
 
-     Returns for every trading day historic data for the given option contract
+     Historic EOD Stats for the given option contract
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
             matching data. Min: 1. Example: 10.
 
     Raises:
@@ -163,15 +163,15 @@
     id: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionContract, str]]:
     """Historic Data
 
-     Returns for every trading day historic data for the given option contract
+     Historic EOD Stats for the given option contract
 
     Args:
         id (str): An option contract in the ISO format. Example: TSLA230526P00167500.
         limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
             matching data. Min: 1. Example: 10.
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_contract/public_api_option_contract_controller_option_contracts.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_trade/public_api_option_trade_controller_flow_alerts.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_ticker_order_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,17 @@
     max_volume_oi_ratio: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Search Option Trades With Filters
 
-     Returns the latest flow alerts.
+     Search option trades based on a variety of parameters
 
     Args:
         ticker_symbol (Union[Unset, str]): A comma separated list of tickers. To exclude certain
             tickers prefix the first ticker with a `-`. Example: AAPL,INTC.
         min_premium (Union[Unset, int]): The minimum premium on that alert. Min: 0. Example:
             12500.5.
         max_premium (Union[Unset, int]): The maximum premium on that alert. Min: 0. Example:
@@ -300,17 +300,17 @@
     max_volume_oi_ratio: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Search Option Trades With Filters
 
-     Returns the latest flow alerts.
+     Search option trades based on a variety of parameters
 
     Args:
         ticker_symbol (Union[Unset, str]): A comma separated list of tickers. To exclude certain
             tickers prefix the first ticker with a `-`. Example: AAPL,INTC.
         min_premium (Union[Unset, int]): The minimum premium on that alert. Min: 0. Example:
             12500.5.
         max_premium (Union[Unset, int]): The maximum premium on that alert. Min: 0. Example:
@@ -426,17 +426,17 @@
     max_volume_oi_ratio: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Search Option Trades With Filters
 
-     Returns the latest flow alerts.
+     Search option trades based on a variety of parameters
 
     Args:
         ticker_symbol (Union[Unset, str]): A comma separated list of tickers. To exclude certain
             tickers prefix the first ticker with a `-`. Example: AAPL,INTC.
         min_premium (Union[Unset, int]): The minimum premium on that alert. Min: 0. Example:
             12500.5.
         max_premium (Union[Unset, int]): The maximum premium on that alert. Min: 0. Example:
@@ -555,17 +555,17 @@
     max_volume_oi_ratio: Union[Unset, int] = UNSET,
     is_otm: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     min_dte: Union[Unset, int] = UNSET,
     max_dte: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Search Option Trades With Filters
 
-     Returns the latest flow alerts.
+     Search option trades based on a variety of parameters
 
     Args:
         ticker_symbol (Union[Unset, str]): A comma separated list of tickers. To exclude certain
             tickers prefix the first ticker with a `-`. Example: AAPL,INTC.
         min_premium (Union[Unset, int]): The minimum premium on that alert. Min: 0. Example:
             12500.5.
         max_premium (Union[Unset, int]): The maximum premium on that alert. Min: 0. Example:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/option_trade/public_api_option_trade_controller_full_tape.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_full_tape.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 def sync_detailed(
     date: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Any]:
-    """Full Tape
+    """Full Tape all trades and statuses for all option orders by date
 
      Download the full tape of data for a given trading date.
 
     NOTICE:
     This endpoint is not included by default in your access.
     For information on how to access this data email support@unusualwhales.com
 
@@ -75,15 +75,15 @@
 
 
 async def asyncio_detailed(
     date: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Any]:
-    """Full Tape
+    """Full Tape all trades and statuses for all option orders by date
 
      Download the full tape of data for a given trading date.
 
     NOTICE:
     This endpoint is not included by default in your access.
     For information on how to access this data email support@unusualwhales.com
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_analyst_ratings.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_analyst_ratings.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,27 +92,27 @@
     client: Union[AuthenticatedClient, Client],
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Response[Union[AnalystRating, ErrorMessage, str]]:
-    """Analyst Rating
+    """Analyst Ratings for a Ticker
 
      Returns the latest analyst rating for the given ticker.
 
     Args:
         ticker (Union[Unset, str]): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 500. Max: 500. Min: 1.
             Example: 10.
         action (Union[Unset, AnalystAction]): The action of the recommendation. Example:
             maintained.
         recommendation (Union[Unset, AnalystRecommendation]): The recommendation the analyst gave
             out. Example: Hold.
-        sector (Union[Unset, AnalystSector]): A financial sector. Example: Financial.
+        sector (Union[Unset, AnalystSector]): A financial sector Example: Financial.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[AnalystRating, ErrorMessage, str]]
@@ -138,27 +138,27 @@
     client: Union[AuthenticatedClient, Client],
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Optional[Union[AnalystRating, ErrorMessage, str]]:
-    """Analyst Rating
+    """Analyst Ratings for a Ticker
 
      Returns the latest analyst rating for the given ticker.
 
     Args:
         ticker (Union[Unset, str]): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 500. Max: 500. Min: 1.
             Example: 10.
         action (Union[Unset, AnalystAction]): The action of the recommendation. Example:
             maintained.
         recommendation (Union[Unset, AnalystRecommendation]): The recommendation the analyst gave
             out. Example: Hold.
-        sector (Union[Unset, AnalystSector]): A financial sector. Example: Financial.
+        sector (Union[Unset, AnalystSector]): A financial sector Example: Financial.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[AnalystRating, ErrorMessage, str]
@@ -179,27 +179,27 @@
     client: Union[AuthenticatedClient, Client],
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Response[Union[AnalystRating, ErrorMessage, str]]:
-    """Analyst Rating
+    """Analyst Ratings for a Ticker
 
      Returns the latest analyst rating for the given ticker.
 
     Args:
         ticker (Union[Unset, str]): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 500. Max: 500. Min: 1.
             Example: 10.
         action (Union[Unset, AnalystAction]): The action of the recommendation. Example:
             maintained.
         recommendation (Union[Unset, AnalystRecommendation]): The recommendation the analyst gave
             out. Example: Hold.
-        sector (Union[Unset, AnalystSector]): A financial sector. Example: Financial.
+        sector (Union[Unset, AnalystSector]): A financial sector Example: Financial.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Union[AnalystRating, ErrorMessage, str]]
@@ -223,27 +223,27 @@
     client: Union[AuthenticatedClient, Client],
     ticker: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     action: Union[Unset, AnalystAction] = UNSET,
     recommendation: Union[Unset, AnalystRecommendation] = UNSET,
     sector: Union[Unset, AnalystSector] = UNSET,
 ) -> Optional[Union[AnalystRating, ErrorMessage, str]]:
-    """Analyst Rating
+    """Analyst Ratings for a Ticker
 
      Returns the latest analyst rating for the given ticker.
 
     Args:
         ticker (Union[Unset, str]): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 500. Max: 500. Min: 1.
             Example: 10.
         action (Union[Unset, AnalystAction]): The action of the recommendation. Example:
             maintained.
         recommendation (Union[Unset, AnalystRecommendation]): The recommendation the analyst gave
             out. Example: Hold.
-        sector (Union[Unset, AnalystSector]): A financial sector. Example: Financial.
+        sector (Union[Unset, AnalystSector]): A financial sector Example: Financial.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Union[AnalystRating, ErrorMessage, str]
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_contract_screener.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_option_contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
     min_floor_volume: Union[Unset, int] = UNSET,
     max_floor_volume: Union[Unset, int] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     order: Union[Unset, ScreenerContractOrderByField] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """Hottest Chains
+    """Screener for Option Contracts
 
      A contract screener endpoint to screen the market for contracts by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Hottest
     Contracts](https://unusualwhales.com/hottest-contracts?limit=100&hide_index_etf=true)
     on unusualwhales.
 
@@ -429,15 +429,15 @@
     min_floor_volume: Union[Unset, int] = UNSET,
     max_floor_volume: Union[Unset, int] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     order: Union[Unset, ScreenerContractOrderByField] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """Hottest Chains
+    """Screener for Option Contracts
 
      A contract screener endpoint to screen the market for contracts by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Hottest
     Contracts](https://unusualwhales.com/hottest-contracts?limit=100&hide_index_etf=true)
     on unusualwhales.
 
@@ -617,15 +617,15 @@
     min_floor_volume: Union[Unset, int] = UNSET,
     max_floor_volume: Union[Unset, int] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     order: Union[Unset, ScreenerContractOrderByField] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """Hottest Chains
+    """Screener for Option Contracts
 
      A contract screener endpoint to screen the market for contracts by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Hottest
     Contracts](https://unusualwhales.com/hottest-contracts?limit=100&hide_index_etf=true)
     on unusualwhales.
 
@@ -808,15 +808,15 @@
     min_floor_volume: Union[Unset, int] = UNSET,
     max_floor_volume: Union[Unset, int] = UNSET,
     vol_greater_oi: Union[Unset, bool] = UNSET,
     issue_types: Union[Unset, List[SingleIssueType]] = UNSET,
     order: Union[Unset, ScreenerContractOrderByField] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """Hottest Chains
+    """Screener for Option Contracts
 
      A contract screener endpoint to screen the market for contracts by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Hottest
     Contracts](https://unusualwhales.com/hottest-contracts?limit=100&hide_index_etf=true)
     on unusualwhales.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/screener/public_api_screener_controller_stock_screener.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_stocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,24 +325,24 @@
 ) -> Response[Union[ErrorMessage, StockScreenerResponse, str]]:
     """Stock Screener
 
      A stock screener endpoint to screen the market for stocks by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Stock
     Screener](https://unusualwhales.com/flow/ticker_flows)
-    on unusualwhales.
+    on unusualwhales.com
 
     Args:
         ticker (Union[Unset, str]): A comma separated list of tickers. To exclude certain tickers
             prefix the first ticker with a `-`. Example: AAPL,INTC.
         issue_types (Union[Unset, List[SingleIssueType]]): An array of 1 or more issue types.
             Example: ['Common Stock', 'Index'].
-        min_change (Union[Unset, int]): The minimum % change to the previous trading day. Min: -1.
+        min_change (Union[Unset, int]): The minimum % change to the previous Trading Day. Min: -1.
             Example: -0.45.
-        max_change (Union[Unset, int]): The maximum % change to the previous trading day. Min: -1.
+        max_change (Union[Unset, int]): The maximum % change to the previous Trading Day. Min: -1.
             Example: 0.2.
         min_underlying_price (Union[Unset, int]): The minimum stock price. Min: 0. Example: 5.23.
         max_underlying_price (Union[Unset, int]): The maximum stock price. Min: 0. Example: 10.53.
         is_s_p_500 (Union[Unset, bool]): Boolean whether to only include stocks which are part of
             the S&P 500. Setting this to false has no effect. Example: True.
         has_dividends (Union[Unset, bool]): Boolean wheter to only include stocks which pay
             dividends. Setting this to false has no effect. Example: True.
@@ -576,24 +576,24 @@
 ) -> Optional[Union[ErrorMessage, StockScreenerResponse, str]]:
     """Stock Screener
 
      A stock screener endpoint to screen the market for stocks by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Stock
     Screener](https://unusualwhales.com/flow/ticker_flows)
-    on unusualwhales.
+    on unusualwhales.com
 
     Args:
         ticker (Union[Unset, str]): A comma separated list of tickers. To exclude certain tickers
             prefix the first ticker with a `-`. Example: AAPL,INTC.
         issue_types (Union[Unset, List[SingleIssueType]]): An array of 1 or more issue types.
             Example: ['Common Stock', 'Index'].
-        min_change (Union[Unset, int]): The minimum % change to the previous trading day. Min: -1.
+        min_change (Union[Unset, int]): The minimum % change to the previous Trading Day. Min: -1.
             Example: -0.45.
-        max_change (Union[Unset, int]): The maximum % change to the previous trading day. Min: -1.
+        max_change (Union[Unset, int]): The maximum % change to the previous Trading Day. Min: -1.
             Example: 0.2.
         min_underlying_price (Union[Unset, int]): The minimum stock price. Min: 0. Example: 5.23.
         max_underlying_price (Union[Unset, int]): The maximum stock price. Min: 0. Example: 10.53.
         is_s_p_500 (Union[Unset, bool]): Boolean whether to only include stocks which are part of
             the S&P 500. Setting this to false has no effect. Example: True.
         has_dividends (Union[Unset, bool]): Boolean wheter to only include stocks which pay
             dividends. Setting this to false has no effect. Example: True.
@@ -822,24 +822,24 @@
 ) -> Response[Union[ErrorMessage, StockScreenerResponse, str]]:
     """Stock Screener
 
      A stock screener endpoint to screen the market for stocks by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Stock
     Screener](https://unusualwhales.com/flow/ticker_flows)
-    on unusualwhales.
+    on unusualwhales.com
 
     Args:
         ticker (Union[Unset, str]): A comma separated list of tickers. To exclude certain tickers
             prefix the first ticker with a `-`. Example: AAPL,INTC.
         issue_types (Union[Unset, List[SingleIssueType]]): An array of 1 or more issue types.
             Example: ['Common Stock', 'Index'].
-        min_change (Union[Unset, int]): The minimum % change to the previous trading day. Min: -1.
+        min_change (Union[Unset, int]): The minimum % change to the previous Trading Day. Min: -1.
             Example: -0.45.
-        max_change (Union[Unset, int]): The maximum % change to the previous trading day. Min: -1.
+        max_change (Union[Unset, int]): The maximum % change to the previous Trading Day. Min: -1.
             Example: 0.2.
         min_underlying_price (Union[Unset, int]): The minimum stock price. Min: 0. Example: 5.23.
         max_underlying_price (Union[Unset, int]): The maximum stock price. Min: 0. Example: 10.53.
         is_s_p_500 (Union[Unset, bool]): Boolean whether to only include stocks which are part of
             the S&P 500. Setting this to false has no effect. Example: True.
         has_dividends (Union[Unset, bool]): Boolean wheter to only include stocks which pay
             dividends. Setting this to false has no effect. Example: True.
@@ -1071,24 +1071,24 @@
 ) -> Optional[Union[ErrorMessage, StockScreenerResponse, str]]:
     """Stock Screener
 
      A stock screener endpoint to screen the market for stocks by a variety of filter options.
 
     For an example of what can be build with this endpoint check out the [Stock
     Screener](https://unusualwhales.com/flow/ticker_flows)
-    on unusualwhales.
+    on unusualwhales.com
 
     Args:
         ticker (Union[Unset, str]): A comma separated list of tickers. To exclude certain tickers
             prefix the first ticker with a `-`. Example: AAPL,INTC.
         issue_types (Union[Unset, List[SingleIssueType]]): An array of 1 or more issue types.
             Example: ['Common Stock', 'Index'].
-        min_change (Union[Unset, int]): The minimum % change to the previous trading day. Min: -1.
+        min_change (Union[Unset, int]): The minimum % change to the previous Trading Day. Min: -1.
             Example: -0.45.
-        max_change (Union[Unset, int]): The maximum % change to the previous trading day. Min: -1.
+        max_change (Union[Unset, int]): The maximum % change to the previous Trading Day. Min: -1.
             Example: 0.2.
         min_underlying_price (Union[Unset, int]): The minimum stock price. Min: 0. Example: 5.23.
         max_underlying_price (Union[Unset, int]): The maximum stock price. Min: 0. Example: 10.53.
         is_s_p_500 (Union[Unset, bool]): Boolean whether to only include stocks which are part of
             the S&P 500. Setting this to false has no effect. Example: True.
         has_dividends (Union[Unset, bool]): Boolean wheter to only include stocks which pay
             dividends. Setting this to false has no effect. Example: True.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_market_seasonality.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_market_average_returns_by_month.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[SeasonalityMarket, str]]:
-    """Market Seasonality
+    """Market Seasonality for ETFs
 
      Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
     XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -71,15 +71,15 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[SeasonalityMarket, str]]:
-    """Market Seasonality
+    """Market Seasonality for ETFs
 
      Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
     XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -93,15 +93,15 @@
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[SeasonalityMarket, str]]:
-    """Market Seasonality
+    """Market Seasonality for ETFs
 
      Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
     XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -117,15 +117,15 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[SeasonalityMarket, str]]:
-    """Market Seasonality
+    """Market Seasonality for ETFs
 
      Returns the average return by month for the tickers SPY, QQQ, IWM, XLE, XLC, XLK, XLV, XLP, XLY,
     XLRE, XLF, XLI, XLB .
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_month_performers.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_top_performers.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[Union[ErrorMessage, SeasonalityPerformers, str]]:
-    """Month Performers
+    """Get Top Performers for a Month
 
      Returns the tickers with the highest performance in terms of price change in the month over the
     years.
     Per default the result is ordered by 'positive_months_perc' descending, then 'median_change'
     descending, then 'marketcap' descending.
 
     Args:
@@ -160,15 +160,15 @@
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[Union[ErrorMessage, SeasonalityPerformers, str]]:
-    """Month Performers
+    """Get Top Performers for a Month
 
      Returns the tickers with the highest performance in terms of price change in the month over the
     years.
     Per default the result is ordered by 'positive_months_perc' descending, then 'median_change'
     descending, then 'marketcap' descending.
 
     Args:
@@ -217,15 +217,15 @@
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[Union[ErrorMessage, SeasonalityPerformers, str]]:
-    """Month Performers
+    """Get Top Performers for a Month
 
      Returns the tickers with the highest performance in terms of price change in the month over the
     years.
     Per default the result is ordered by 'positive_months_perc' descending, then 'median_change'
     descending, then 'marketcap' descending.
 
     Args:
@@ -277,15 +277,15 @@
     ticker_for_sector: Union[Unset, str] = UNSET,
     s_p_500_nasdaq_only: Union[Unset, bool] = UNSET,
     min_oi: Union[Unset, int] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, SeasonalityPerformanceOrderBy] = UNSET,
     order_direction: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[Union[ErrorMessage, SeasonalityPerformers, str]]:
-    """Month Performers
+    """Get Top Performers for a Month
 
      Returns the tickers with the highest performance in terms of price change in the month over the
     years.
     Per default the result is ordered by 'positive_months_perc' descending, then 'median_change'
     descending, then 'marketcap' descending.
 
     Args:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_monthly.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_average_returns.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/seasonality/public_api_seasonality_controller_year_month.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_price_changes_by_month_and_year.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_atm_chains.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_atm_contracts_for_expiries.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,17 +63,17 @@
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     expirations: str,
 ) -> Response[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """ATM Chains
+    """ATM option contracts for the given expiries
 
-     Returns the ATM chains for the given expirations
+     Returns the ATM option contracts for the given expirations
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         expirations (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -97,17 +97,17 @@
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     expirations: str,
 ) -> Optional[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """ATM Chains
+    """ATM option contracts for the given expiries
 
-     Returns the ATM chains for the given expirations
+     Returns the ATM option contracts for the given expirations
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         expirations (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -126,17 +126,17 @@
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     expirations: str,
 ) -> Response[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """ATM Chains
+    """ATM option contracts for the given expiries
 
-     Returns the ATM chains for the given expirations
+     Returns the ATM option contracts for the given expirations
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         expirations (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -158,17 +158,17 @@
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     expirations: str,
 ) -> Optional[Union[ErrorMessage, OptionContractScreenerResponse, str]]:
-    """ATM Chains
+    """ATM option contracts for the given expiries
 
-     Returns the ATM chains for the given expirations
+     Returns the ATM option contracts for the given expirations
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         expirations (str): A single expiry date in ISO date format. Example: 2024-02-02.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_companies_in_sector.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_sector_tickers.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 def sync_detailed(
     sector: Sector,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[Any, ErrorMessage, str]]:
-    """Companies in Sector
+    """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
 
     Raises:
@@ -83,15 +83,15 @@
 
 
 def sync(
     sector: Sector,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[Any, ErrorMessage, str]]:
-    """Companies in Sector
+    """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
 
     Raises:
@@ -109,15 +109,15 @@
 
 
 async def asyncio_detailed(
     sector: Sector,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[Any, ErrorMessage, str]]:
-    """Companies in Sector
+    """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
 
     Raises:
@@ -138,15 +138,15 @@
 
 
 async def asyncio(
     sector: Sector,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[Any, ErrorMessage, str]]:
-    """Companies in Sector
+    """Return Tickers for a Given Sector
 
      Returns a list of tickers which are in the given sector.
 
     Args:
         sector (Sector): A financial sector. Example: Technology.
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_alerts.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_order_flow_alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Unusual Whales Alerts for a Ticker
 
      Returns the latest flow alerts for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
@@ -98,15 +98,15 @@
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Unusual Whales Alerts for a Ticker
 
      Returns the latest flow alerts for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
@@ -128,15 +128,15 @@
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Unusual Whales Alerts for a Ticker
 
      Returns the latest flow alerts for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
@@ -161,15 +161,15 @@
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     limit: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowAlert, str]]:
-    """Flow Alerts
+    """Unusual Whales Alerts for a Ticker
 
      Returns the latest flow alerts for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
             Example: 10.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_per_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_expiry.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[FlowPerExpiry]:
-    """Flow per expiry
+    """Option Order Flow for a Ticker Grouped by Expiry
 
-     Returns the option flow per expiry for the last trading day
+     Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -72,17 +72,17 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[FlowPerExpiry]:
-    """Flow per expiry
+    """Option Order Flow for a Ticker Grouped by Expiry
 
-     Returns the option flow per expiry for the last trading day
+     Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -98,17 +98,17 @@
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[FlowPerExpiry]:
-    """Flow per expiry
+    """Option Order Flow for a Ticker Grouped by Expiry
 
-     Returns the option flow per expiry for the last trading day
+     Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -127,17 +127,17 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[FlowPerExpiry]:
-    """Flow per expiry
+    """Option Order Flow for a Ticker Grouped by Expiry
 
-     Returns the option flow per expiry for the last trading day
+     Returns all option orders grouped by expiry for a given ticker for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_per_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_strike.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[ErrorMessage, FlowPerStrike, str]]:
-    """Flow per strike
+    """Option Order Flow for a Ticker Grouped By Strike
 
-     Returns the option flow per strike for the last trading day
+     Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -84,17 +84,17 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[ErrorMessage, FlowPerStrike, str]]:
-    """Flow per strike
+    """Option Order Flow for a Ticker Grouped By Strike
 
-     Returns the option flow per strike for the last trading day
+     Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -110,17 +110,17 @@
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Union[ErrorMessage, FlowPerStrike, str]]:
-    """Flow per strike
+    """Option Order Flow for a Ticker Grouped By Strike
 
-     Returns the option flow per strike for the last trading day
+     Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -139,17 +139,17 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Optional[Union[ErrorMessage, FlowPerStrike, str]]:
-    """Flow per strike
+    """Option Order Flow for a Ticker Grouped By Strike
 
-     Returns the option flow per strike for the last trading day
+     Returns the option flow per strike for the last Trading Day
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_flow_recent.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/public_api_ticker_controller_flow_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Recent flows
+    """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
@@ -112,15 +112,15 @@
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Recent flows
+    """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
@@ -147,15 +147,15 @@
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Response[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Recent flows
+    """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
@@ -185,15 +185,15 @@
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     side: Union[Unset, Side] = UNSET,
     min_premium: Union[Unset, int] = UNSET,
 ) -> Optional[Union[ErrorMessage, FlowPerExpiry, str]]:
-    """Recent flows
+    """Option Order Flow By Date
 
      Returns the latest flows for the given ticker. Optionally a min premium and a side can be supplied
     in the query for further filtering.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         side (Union[Unset, Side]): The side of a stock trade. Must be one of ASK, BID, MID. If not
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_expiry.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Expiry
+    """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -99,15 +99,15 @@
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Expiry
+    """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -130,15 +130,15 @@
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Expiry
+    """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -164,15 +164,15 @@
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Expiry
+    """Greek Exposure Grouped By Expiry All Strikes
 
      The greek exposure of a ticker grouped by expiry dates across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Strike
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
      The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -99,15 +99,15 @@
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Strike
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
      The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -130,15 +130,15 @@
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Response[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Strike
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
      The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -164,15 +164,15 @@
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
 ) -> Optional[Union[ErrorMessage, GreekExposureByStrike, str]]:
-    """Greek Exposure By Strike
+    """Greek Exposure Grouped By Strike All Expiries On A Given Date
 
      The greek exposure of a ticker grouped by strike price across all contracts on a given market date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greek_exposure_by_strike_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_greeks.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greeks_by_strike_expiry.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
 ) -> Response[Union[ErrorMessage, Greeks, str]]:
-    """Greeks
+    """Option Greeks by Expiry All Strikes
 
      Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -106,15 +106,15 @@
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
 ) -> Optional[Union[ErrorMessage, Greeks, str]]:
-    """Greeks
+    """Option Greeks by Expiry All Strikes
 
      Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -140,15 +140,15 @@
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
 ) -> Response[Union[ErrorMessage, Greeks, str]]:
-    """Greeks
+    """Option Greeks by Expiry All Strikes
 
      Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
@@ -177,15 +177,15 @@
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
 ) -> Optional[Union[ErrorMessage, Greeks, str]]:
-    """Greeks
+    """Option Greeks by Expiry All Strikes
 
      Returns the greeks for each strike for a single expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_historical_risk_reversal_skew.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/get_risk_reversal_skew.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Response[Union[ErrorMessage, HistoricalRiskReversalSkew, str]]:
-    """Historical Risk Reversal Skew
+    """Historical Risk Reversal Skew by Expiry and Ticker
 
      Returns the historical risk reversal skew (the difference between put and call volatility) at a
     delta of 0.25 or 0.1 for a given expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
@@ -128,15 +128,15 @@
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Optional[Union[ErrorMessage, HistoricalRiskReversalSkew, str]]:
-    """Historical Risk Reversal Skew
+    """Historical Risk Reversal Skew by Expiry and Ticker
 
      Returns the historical risk reversal skew (the difference between put and call volatility) at a
     delta of 0.25 or 0.1 for a given expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
@@ -176,15 +176,15 @@
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Response[Union[ErrorMessage, HistoricalRiskReversalSkew, str]]:
-    """Historical Risk Reversal Skew
+    """Historical Risk Reversal Skew by Expiry and Ticker
 
      Returns the historical risk reversal skew (the difference between put and call volatility) at a
     delta of 0.25 or 0.1 for a given expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
@@ -227,15 +227,15 @@
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     expiry: str,
     timeframe: Union[Unset, str] = UNSET,
     delta: Any,
 ) -> Optional[Union[ErrorMessage, HistoricalRiskReversalSkew, str]]:
-    """Historical Risk Reversal Skew
+    """Historical Risk Reversal Skew by Expiry and Ticker
 
      Returns the historical risk reversal skew (the difference between put and call volatility) at a
     delta of 0.25 or 0.1 for a given expiry date.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_implied_volatility_term_structure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     Union[
         ErrorMessage,
         ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
         TickerInfo,
         str,
     ]
 ]:
-    """Information
+    """Ticker Information
 
      Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -121,15 +121,15 @@
     Union[
         ErrorMessage,
         ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
         TickerInfo,
         str,
     ]
 ]:
-    """Information
+    """Ticker Information
 
      Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -154,15 +154,15 @@
     Union[
         ErrorMessage,
         ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
         TickerInfo,
         str,
     ]
 ]:
-    """Information
+    """Ticker Information
 
      Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
@@ -190,15 +190,15 @@
     Union[
         ErrorMessage,
         ErrorMessageStatingThatTheRequestedElementWasNotFoundCausingAnEmptyResultToBeGenerated,
         TickerInfo,
         str,
     ]
 ]:
-    """Information
+    """Ticker Information
 
      Returns a information about the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
 
     Raises:
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_insider_buy_sell.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_max_pain.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_max_pain.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_net_prem_ticks.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_net_premium_ticks.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_ohlc.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_candles.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_oi_change.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from ...client import AuthenticatedClient, Client
 from ...models.oi_change import OIChange
 from ...models.order_direction import OrderDirection
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
@@ -29,15 +28,15 @@
 
     params["order"] = json_order
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/oi-change",
+        "url": "/api/market/oi-change",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[OIChange]:
@@ -57,178 +56,170 @@
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChange]:
-    """OI Change
+    """Returns the Option Contracts With The Highest Open Interest Change by Date
 
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
+     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
+    descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
-        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
+        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
+            Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChange]
     """
 
     kwargs = _get_kwargs(
-        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChange]:
-    """OI Change
+    """Returns the Option Contracts With The Highest Open Interest Change by Date
 
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
+     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
+    descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
-        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
+        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
+            Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChange
     """
 
     return sync_detailed(
-        ticker=ticker,
         client=client,
         date=date,
         limit=limit,
         order=order,
     ).parsed
 
 
 async def asyncio_detailed(
-    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Response[OIChange]:
-    """OI Change
+    """Returns the Option Contracts With The Highest Open Interest Change by Date
 
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
+     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
+    descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
-        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
+        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
+            Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[OIChange]
     """
 
     kwargs = _get_kwargs(
-        ticker=ticker,
         date=date,
         limit=limit,
         order=order,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
     limit: Union[Unset, int] = UNSET,
     order: Union[Unset, OrderDirection] = UNSET,
 ) -> Optional[OIChange]:
-    """OI Change
+    """Returns the Option Contracts With The Highest Open Interest Change by Date
 
-     Returns the tickers contracts' OI change data ordered by absolute OI change (default: descending).
+     Returns the non-Index/non-ETF contracts and OI change data with the highest OI change (default:
+    descending).
     Date must be the current or a past date. If no date is given, returns data for the current/last
     market day.
 
     Args:
-        ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
-        limit (Union[Unset, int]): How many items to return. If no limit is given, returns all
-            matching data. Min: 1. Example: 10.
+        limit (Union[Unset, int]): How many items to return. Default: 100. Max: 200. Min: 1.
+            Example: 10.
         order (Union[Unset, OrderDirection]): Whether to sort descending or ascending. Descending
             by default. Example: asc.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         OIChange
     """
 
     return (
         await asyncio_detailed(
-            ticker=ticker,
             client=client,
             date=date,
             limit=limit,
             order=order,
         )
     ).parsed
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_option_chains.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_chains.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_option_price_level.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_options_volume.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.error_message import ErrorMessage
-from ...models.option_price_level import OptionPriceLevel
+from ...models.ticker_options_volume import TickerOptionsVolume
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
-    date: Union[Unset, str] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
-    params["date"] = date
+    params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/option/stock-price-levels",
+        "url": f"/api/stock/{ticker}/options-volume",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = OptionPriceLevel.from_dict(response.json())
+        response_200 = TickerOptionsVolume.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -48,148 +48,148 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
-    """Option Price Levels
+    limit: Union[Unset, int] = UNSET,
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionPriceLevel, str]]
+        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
+        limit=limit,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
-    """Option Price Levels
+    limit: Union[Unset, int] = UNSET,
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionPriceLevel, str]
+        Union[ErrorMessage, TickerOptionsVolume, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
-        date=date,
+        limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OptionPriceLevel, str]]:
-    """Option Price Levels
+    limit: Union[Unset, int] = UNSET,
+) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OptionPriceLevel, str]]
+        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        date=date,
+        limit=limit,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OptionPriceLevel, str]]:
-    """Option Price Levels
+    limit: Union[Unset, int] = UNSET,
+) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+    """Options Volume
 
-     Returns the call and put volume per price level for the given ticker.
+     Returns the options volume & premium for all trade executions
+    that happened on a given trading date for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
-            This is optional and by default the last trading date.
-             Example: 2024-01-18.
+        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
+            Example: 10.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OptionPriceLevel, str]
+        Union[ErrorMessage, TickerOptionsVolume, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
-            date=date,
+            limit=limit,
         )
     ).parsed
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_options_volume.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volume_by_price_level.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.error_message import ErrorMessage
-from ...models.ticker_options_volume import TickerOptionsVolume
+from ...models.off_lit_price_level import OffLitPriceLevel
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
-    limit: Union[Unset, int] = UNSET,
+    date: Union[Unset, str] = UNSET,
 ) -> Dict[str, Any]:
     params: Dict[str, Any] = {}
 
-    params["limit"] = limit
+    params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/options-volume",
+        "url": f"/api/stock/{ticker}/stock-volume-price-levels",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
+) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TickerOptionsVolume.from_dict(response.json())
+        response_200 = OffLitPriceLevel.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -48,184 +48,172 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
+) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
+    """Off/Lit Price Levels
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
+    The price level is calculated by dividing the stock volume by the total
     ----
-    This can be used to build a ticker options overview such as:
-
-    ![Table](https://i.imgur.com/7FHyuqc.png)
-
-    ----
-
-    ![Line](https://i.imgur.com/UnVryDK.png)
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
+        Response[Union[ErrorMessage, OffLitPriceLevel, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        limit=limit,
+        date=date,
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
+    """Off/Lit Price Levels
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
+    The price level is calculated by dividing the stock volume by the total
     ----
-    This can be used to build a ticker options overview such as:
-
-    ![Table](https://i.imgur.com/7FHyuqc.png)
-
-    ----
-
-    ![Line](https://i.imgur.com/UnVryDK.png)
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, TickerOptionsVolume, str]
+        Union[ErrorMessage, OffLitPriceLevel, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
-        limit=limit,
+        date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Response[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    date: Union[Unset, str] = UNSET,
+) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
+    """Off/Lit Price Levels
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
+    The price level is calculated by dividing the stock volume by the total
     ----
-    This can be used to build a ticker options overview such as:
-
-    ![Table](https://i.imgur.com/7FHyuqc.png)
-
-    ----
-
-    ![Line](https://i.imgur.com/UnVryDK.png)
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, TickerOptionsVolume, str]]
+        Response[Union[ErrorMessage, OffLitPriceLevel, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
-        limit=limit,
+        date=date,
     )
 
     response = await client.get_async_httpx_client().request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
-    limit: Union[Unset, int] = UNSET,
-) -> Optional[Union[ErrorMessage, TickerOptionsVolume, str]]:
-    """Options Volume
+    date: Union[Unset, str] = UNSET,
+) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
+    """Off/Lit Price Levels
 
-     Returns the options volume & premium for all trade executions
-    that happened on a given trading date for the given ticker.
+     Returns the lit & off lit stock volume per price level for the given ticker.
 
+    The price level is calculated by dividing the stock volume by the total
     ----
-    This can be used to build a ticker options overview such as:
-
-    ![Table](https://i.imgur.com/7FHyuqc.png)
-
-    ----
-
-    ![Line](https://i.imgur.com/UnVryDK.png)
+    Important: The volume does **NOT** represent the full market dialy volume. It
+    only represents the volume of executed trades on exchanges operated by Nasdaq
+    and FINRA off lit exchanges.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
-        limit (Union[Unset, int]): How many items to return. Default: 1. Max: 500. Min: 1.
-            Example: 10.
+        date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
+            This is optional and by default the last trading date.
+             Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, TickerOptionsVolume, str]
+        Union[ErrorMessage, OffLitPriceLevel, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
-            limit=limit,
+            date=date,
         )
     ).parsed
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_spot_exposures_by_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_spot_exposures_one_minute.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_stock_volume_price_level.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_volume_open_interest_by_expiry.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.error_message import ErrorMessage
-from ...models.off_lit_price_level import OffLitPriceLevel
+from ...models.volume_oi_per_expiry import VolumeOIPerExpiry
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
@@ -19,26 +19,26 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/stock-volume-price-levels",
+        "url": f"/api/stock/{ticker}/option/volume-oi-expiry",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = OffLitPriceLevel.from_dict(response.json())
+        response_200 = VolumeOIPerExpiry.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -48,50 +48,45 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
-    """Off/Lit Price Levels
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+    """Volume & OI per Expiry
 
-     Returns the lit & off lit stock volume per price level for the given ticker.
-
-    ----
-    Important: The volume does **NOT** represent the full market dialy volume. It
-    only represents the volume of executed trades on exchanges operated by Nasdaq
-    and FINRA off lit exchanges.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OffLitPriceLevel, str]]
+        Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -103,72 +98,62 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
-    """Off/Lit Price Levels
-
-     Returns the lit & off lit stock volume per price level for the given ticker.
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+    """Volume & OI per Expiry
 
-    ----
-    Important: The volume does **NOT** represent the full market dialy volume. It
-    only represents the volume of executed trades on exchanges operated by Nasdaq
-    and FINRA off lit exchanges.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OffLitPriceLevel, str]
+        Union[ErrorMessage, VolumeOIPerExpiry, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, OffLitPriceLevel, str]]:
-    """Off/Lit Price Levels
+) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+    """Volume & OI per Expiry
 
-     Returns the lit & off lit stock volume per price level for the given ticker.
-
-    ----
-    Important: The volume does **NOT** represent the full market dialy volume. It
-    only represents the volume of executed trades on exchanges operated by Nasdaq
-    and FINRA off lit exchanges.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, OffLitPriceLevel, str]]
+        Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -178,36 +163,31 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, OffLitPriceLevel, str]]:
-    """Off/Lit Price Levels
-
-     Returns the lit & off lit stock volume per price level for the given ticker.
+) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+    """Volume & OI per Expiry
 
-    ----
-    Important: The volume does **NOT** represent the full market dialy volume. It
-    only represents the volume of executed trades on exchanges operated by Nasdaq
-    and FINRA off lit exchanges.
+     Returns the total volume and open interest per expiry for the given ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, OffLitPriceLevel, str]
+        Union[ErrorMessage, VolumeOIPerExpiry, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_vol_oi_per_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_daily_expiry_breakdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
 from ...models.error_message import ErrorMessage
-from ...models.volume_oi_per_expiry import VolumeOIPerExpiry
+from ...models.expiry_breakdown import ExpiryBreakdown
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     ticker: str,
     *,
     date: Union[Unset, str] = UNSET,
@@ -19,26 +19,26 @@
 
     params["date"] = date
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": f"/api/stock/{ticker}/option/volume-oi-expiry",
+        "url": f"/api/stock/{ticker}/expiry-breakdown",
         "params": params,
     }
 
     return _kwargs
 
 
 def _parse_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = VolumeOIPerExpiry.from_dict(response.json())
+        response_200 = ExpiryBreakdown.from_dict(response.json())
 
         return response_200
     if response.status_code == HTTPStatus.UNPROCESSABLE_ENTITY:
         response_422 = ErrorMessage.from_dict(response.json())
 
         return response_422
     if response.status_code == HTTPStatus.INTERNAL_SERVER_ERROR:
@@ -48,45 +48,45 @@
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Union[AuthenticatedClient, Client], response: httpx.Response
-) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
+) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
-    """Volume & OI per Expiry
+) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
+    """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
-     Returns the total volume and open interest per expiry for the given ticker.
+     Returns all expirations for the given Trading Day for a ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]
+        Response[Union[ErrorMessage, ExpiryBreakdown, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -98,62 +98,62 @@
 
 
 def sync(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
-    """Volume & OI per Expiry
+) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
+    """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
-     Returns the total volume and open interest per expiry for the given ticker.
+     Returns all expirations for the given Trading Day for a ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, VolumeOIPerExpiry, str]
+        Union[ErrorMessage, ExpiryBreakdown, str]
     """
 
     return sync_detailed(
         ticker=ticker,
         client=client,
         date=date,
     ).parsed
 
 
 async def asyncio_detailed(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
-    """Volume & OI per Expiry
+) -> Response[Union[ErrorMessage, ExpiryBreakdown, str]]:
+    """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
-     Returns the total volume and open interest per expiry for the given ticker.
+     Returns all expirations for the given Trading Day for a ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Union[ErrorMessage, VolumeOIPerExpiry, str]]
+        Response[Union[ErrorMessage, ExpiryBreakdown, str]]
     """
 
     kwargs = _get_kwargs(
         ticker=ticker,
         date=date,
     )
 
@@ -163,31 +163,31 @@
 
 
 async def asyncio(
     ticker: str,
     *,
     client: Union[AuthenticatedClient, Client],
     date: Union[Unset, str] = UNSET,
-) -> Optional[Union[ErrorMessage, VolumeOIPerExpiry, str]]:
-    """Volume & OI per Expiry
+) -> Optional[Union[ErrorMessage, ExpiryBreakdown, str]]:
+    """Option Order Flow Grouped By Expiry on a Given Date for a Given Ticker
 
-     Returns the total volume and open interest per expiry for the given ticker.
+     Returns all expirations for the given Trading Day for a ticker.
 
     Args:
         ticker (str): A single ticker Example: AAPL.
         date (Union[Unset, str]): A trading date in the format of YYYY-MM-DD.
             This is optional and by default the last trading date.
              Example: 2024-01-18.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Union[ErrorMessage, VolumeOIPerExpiry, str]
+        Union[ErrorMessage, ExpiryBreakdown, str]
     """
 
     return (
         await asyncio_detailed(
             ticker=ticker,
             client=client,
             date=date,
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/api/websocket/public_api_socket_controller_channels.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/channels.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     )
 
 
 def sync_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Any]:
-    r"""WebSocket channels
+    r"""Unusual Whales websocket channels
 
      Returns the available WebSocket channels for connections.
 
     ## Websocket Guide
     Important: Websockets are not part of the basic API subscription. To be able to connect to
     WebSockets, please
     contact us at support@unusualwhales.com.
@@ -162,15 +162,15 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     *,
     client: Union[AuthenticatedClient, Client],
 ) -> Response[Any]:
-    r"""WebSocket channels
+    r"""Unusual Whales websocket channels
 
      Returns the available WebSocket channels for connections.
 
     ## Websocket Guide
     Important: Websockets are not part of the basic API subscription. To be able to connect to
     WebSockets, please
     contact us at support@unusualwhales.com.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/client.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,143 @@
-import os
-import python_dotenv as dotenv
 import ssl
 from typing import Any, Dict, Optional, Union
 
 import httpx
 from attrs import define, evolve, field
 
-dotenv.load_dotenv('.env')
 
-UNUSUAL_WHALES_TOKEN = os.environ.get("UNUSUAL_WHALES_TOKEN", "2bfb30b2 - 4ca1 - 4719 - 883c - ce4a01b3c47f")
+@define
+class Client:
+    """A class for keeping track of data related to the API
+
+    The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
+
+        ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
+
+        ``cookies``: A dictionary of cookies to be sent with every request
+
+        ``headers``: A dictionary of headers to be sent with every request
+
+        ``timeout``: The maximum amount of a time a request can take. API functions will raise
+        httpx.TimeoutException if this is exceeded.
+
+        ``verify_ssl``: Whether or not to verify the SSL certificate of the API server. This should be True in production,
+        but can be set to False for testing purposes.
+
+        ``follow_redirects``: Whether or not to follow redirects. Default value is False.
+
+        ``httpx_args``: A dictionary of additional arguments to be passed to the ``httpx.Client`` and ``httpx.AsyncClient`` constructor.
+
+
+    Attributes:
+        raise_on_unexpected_status: Whether or not to raise an errors.UnexpectedStatus if the API returns a
+            status code that was not documented in the source OpenAPI document. Can also be provided as a keyword
+            argument to the constructor.
+    """
+
+    raise_on_unexpected_status: bool = field(default=False, kw_only=True)
+    _base_url: str = field(alias="base_url")
+    _cookies: Dict[str, str] = field(factory=dict, kw_only=True, alias="cookies")
+    _headers: Dict[str, str] = field(factory=dict, kw_only=True, alias="headers")
+    _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True, alias="timeout")
+    _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True, alias="verify_ssl")
+    _follow_redirects: bool = field(default=False, kw_only=True, alias="follow_redirects")
+    _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True, alias="httpx_args")
+    _client: Optional[httpx.Client] = field(default=None, init=False)
+    _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
+
+    def with_headers(self, headers: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional headers"""
+        if self._client is not None:
+            self._client.headers.update(headers)
+        if self._async_client is not None:
+            self._async_client.headers.update(headers)
+        return evolve(self, headers={**self._headers, **headers})
+
+    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
+        """Get a new client matching this one with additional cookies"""
+        if self._client is not None:
+            self._client.cookies.update(cookies)
+        if self._async_client is not None:
+            self._async_client.cookies.update(cookies)
+        return evolve(self, cookies={**self._cookies, **cookies})
+
+    def with_timeout(self, timeout: httpx.Timeout) -> "Client":
+        """Get a new client matching this one with a new timeout (in seconds)"""
+        if self._client is not None:
+            self._client.timeout = timeout
+        if self._async_client is not None:
+            self._async_client.timeout = timeout
+        return evolve(self, timeout=timeout)
+
+    def set_httpx_client(self, client: httpx.Client) -> "Client":
+        """Manually the underlying httpx.Client
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._client = client
+        return self
+
+    def get_httpx_client(self) -> httpx.Client:
+        """Get the underlying httpx.Client, constructing a new one if not previously set"""
+        if self._client is None:
+            self._client = httpx.Client(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._client
+
+    def __enter__(self) -> "Client":
+        """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
+        self.get_httpx_client().__enter__()
+        return self
+
+    def __exit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for internal httpx.Client (see httpx docs)"""
+        self.get_httpx_client().__exit__(*args, **kwargs)
+
+    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "Client":
+        """Manually the underlying httpx.AsyncClient
+
+        **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
+        """
+        self._async_client = async_client
+        return self
+
+    def get_async_httpx_client(self) -> httpx.AsyncClient:
+        """Get the underlying httpx.AsyncClient, constructing a new one if not previously set"""
+        if self._async_client is None:
+            self._async_client = httpx.AsyncClient(
+                base_url=self._base_url,
+                cookies=self._cookies,
+                headers=self._headers,
+                timeout=self._timeout,
+                verify=self._verify_ssl,
+                follow_redirects=self._follow_redirects,
+                **self._httpx_args,
+            )
+        return self._async_client
+
+    async def __aenter__(self) -> "Client":
+        """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
+        await self.get_async_httpx_client().__aenter__()
+        return self
+
+    async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
+        """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
+        await self.get_async_httpx_client().__aexit__(*args, **kwargs)
 
 
 @define
-class Client:
+class AuthenticatedClient:
     """A Client which has been authenticated for use on secured endpoints
 
     The following are accepted as keyword arguments and will be used to construct httpx Clients internally:
 
         ``base_url``: The base URL for the API, all requests are made to a relative path to this URL
 
         ``cookies``: A dictionary of cookies to be sent with every request
@@ -50,45 +171,43 @@
     _timeout: Optional[httpx.Timeout] = field(default=None, kw_only=True, alias="timeout")
     _verify_ssl: Union[str, bool, ssl.SSLContext] = field(default=True, kw_only=True, alias="verify_ssl")
     _follow_redirects: bool = field(default=False, kw_only=True, alias="follow_redirects")
     _httpx_args: Dict[str, Any] = field(factory=dict, kw_only=True, alias="httpx_args")
     _client: Optional[httpx.Client] = field(default=None, init=False)
     _async_client: Optional[httpx.AsyncClient] = field(default=None, init=False)
 
-    token: str = UNUSUAL_WHALES_TOKEN
+    token: str
     prefix: str = "Bearer"
     auth_header_name: str = "Authorization"
 
-    def with_headers(self, headers: Dict[str, str]) -> "Client":
+    def with_headers(self, headers: Dict[str, str]) -> "AuthenticatedClient":
         """Get a new client matching this one with additional headers"""
-        default_header = {'Content-Type': 'application/json'}
-        default_header.update(headers)
         if self._client is not None:
-            self._client.headers.update(default_header)
+            self._client.headers.update(headers)
         if self._async_client is not None:
-            self._async_client.headers.update(default_header)
-        return evolve(self, headers={**self._headers, **default_header})
+            self._async_client.headers.update(headers)
+        return evolve(self, headers={**self._headers, **headers})
 
-    def with_cookies(self, cookies: Dict[str, str]) -> "Client":
+    def with_cookies(self, cookies: Dict[str, str]) -> "AuthenticatedClient":
         """Get a new client matching this one with additional cookies"""
         if self._client is not None:
             self._client.cookies.update(cookies)
         if self._async_client is not None:
             self._async_client.cookies.update(cookies)
         return evolve(self, cookies={**self._cookies, **cookies})
 
-    def with_timeout(self, timeout: httpx.Timeout) -> "Client":
+    def with_timeout(self, timeout: httpx.Timeout) -> "AuthenticatedClient":
         """Get a new client matching this one with a new timeout (in seconds)"""
         if self._client is not None:
             self._client.timeout = timeout
         if self._async_client is not None:
             self._async_client.timeout = timeout
         return evolve(self, timeout=timeout)
 
-    def set_httpx_client(self, client: httpx.Client) -> "Client":
+    def set_httpx_client(self, client: httpx.Client) -> "AuthenticatedClient":
         """Manually the underlying httpx.Client
 
         **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
         """
         self._client = client
         return self
 
@@ -103,24 +222,24 @@
                 timeout=self._timeout,
                 verify=self._verify_ssl,
                 follow_redirects=self._follow_redirects,
                 **self._httpx_args,
             )
         return self._client
 
-    def __enter__(self) -> "Client":
+    def __enter__(self) -> "AuthenticatedClient":
         """Enter a context manager for self.client—you cannot enter twice (see httpx docs)"""
         self.get_httpx_client().__enter__()
         return self
 
     def __exit__(self, *args: Any, **kwargs: Any) -> None:
         """Exit a context manager for internal httpx.Client (see httpx docs)"""
         self.get_httpx_client().__exit__(*args, **kwargs)
 
-    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "Client":
+    def set_async_httpx_client(self, async_client: httpx.AsyncClient) -> "AuthenticatedClient":
         """Manually the underlying httpx.AsyncClient
 
         **NOTE**: This will override any other settings on the client, including cookies, headers, and timeout.
         """
         self._async_client = async_client
         return self
 
@@ -135,15 +254,15 @@
                 timeout=self._timeout,
                 verify=self._verify_ssl,
                 follow_redirects=self._follow_redirects,
                 **self._httpx_args,
             )
         return self._async_client
 
-    async def __aenter__(self) -> "Client":
+    async def __aenter__(self) -> "AuthenticatedClient":
         """Enter a context manager for underlying httpx.AsyncClient—you cannot enter twice (see httpx docs)"""
         await self.get_async_httpx_client().__aenter__()
         return self
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         """Exit a context manager for underlying httpx.AsyncClient (see httpx docs)"""
         await self.get_async_httpx_client().__aexit__(*args, **kwargs)
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/errors.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/errors.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/__init__.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/analyst_rating.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_rating.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,38 +22,38 @@
             catalyst watch' on Microsoft into 'catalyst path'"}, {'action': 'maintained', 'analyst_name': 'Mark Rothschild',
             'firm': 'Canaccord Genuity', 'rating': '4.91', 'recommendation': 'Hold', 'sector': 'Conglomerates', 'target':
             '11.75', 'ticker': 'DRETF', 'timestamp': datetime.datetime(2023, 9, 11, 11, 11, 32,
             tzinfo=datetime.timezone.utc), 'title': 'Canaccord Genuity Keeps Their Hold Rating on Dream Office Real Estate
             Investment (DRETF)'}]}
 
     Attributes:
-        action (Union[Unset, AnalystFieldAction]): The action of the recommendation. Example: maintained.
+        action (Union[Unset, AnalystFieldAction]): The action of the recommendation. Example: upgraded.
         analyst_name (Union[Unset, str]): The name of the analyst. Example: David Vogt.
         firm (Union[Unset, str]): The firm the analyst is working for. Example: UBS.
         rating (Union[Unset, float]): The rating of the analyst. Example: 2.44.
         recommendation (Union[Unset, AnalystFieldRecommendation]): The recommendation the analyst gave out. Example:
-            Hold.
+            Buy.
         sector (Union[Unset, MarketGeneralSector]): The financial sector of the ticker. Empty if unknown or not
             applicable such as ETF/Index. Example: Technology.
-        target (Union[Unset, str]): The target price of the rating. Example: 190.0.
-        ticker (Union[Unset, Any]): A financial sector.
-        timestamp (Union[Unset, str]): The UTC timestamp, when the rating was released. Example: 2023-09-08
-            12:21:10+00:00.
+        target (Union[Unset, str]): The target price of the rating.
+        ticker (Union[Unset, str]): The stock ticker. Example: AAPL.
+        timestamp (Union[Unset, str]): The UTC timestamp as a string, when the rating was released. Example: 2023-09-11
+            11:21:12+00:00.
         title (Union[Unset, str]): The news title of the rating that went out. Example: China news could create demand
             headwind for Apple in Dec. quarter, says UBS.
     """
 
     action: Union[Unset, AnalystFieldAction] = UNSET
     analyst_name: Union[Unset, str] = UNSET
     firm: Union[Unset, str] = UNSET
     rating: Union[Unset, float] = UNSET
     recommendation: Union[Unset, AnalystFieldRecommendation] = UNSET
     sector: Union[Unset, MarketGeneralSector] = UNSET
     target: Union[Unset, str] = UNSET
-    ticker: Union[Unset, Any] = UNSET
+    ticker: Union[Unset, str] = UNSET
     timestamp: Union[Unset, str] = UNSET
     title: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         action: Union[Unset, str] = UNSET
         if not isinstance(self.action, Unset):
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/candle_data.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_data.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/country_sector_exposure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/country_sector_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/daily_market_tide.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/daily_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/darkpool_trade.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/darkpool_trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             contingent_trade.
         size (Union[Unset, int]): The size of the transaction. Example: 6400.
         ticker (Union[Unset, str]): The stock ticker. Example: AAPL.
         tracking_id (Union[Unset, int]): The tracking ID of the trade. Example: 71984388012245.
         trade_code (Union[Unset, SingleTradeTradeCode]): The trade code. Null if none applies. Example:
             derivative_priced.
         trade_settlement (Union[Unset, SingleTradeSettlement]): The kind of trade settlement. Example: cash_settlement.
-        volume (Union[Unset, int]): The volume of the ticker for the trading day. Example: 23132119.
+        volume (Union[Unset, int]): The volume of the ticker for the Trading Day. Example: 23132119.
     """
 
     canceled: Union[Unset, bool] = UNSET
     executed_at: Union[Unset, str] = UNSET
     ext_hour_sold_codes: Union[Unset, SingleTradeExternalHourSoldCode] = UNSET
     market_center: Union[Unset, str] = UNSET
     nbbo_ask: Union[Unset, float] = UNSET
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/earning.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/earning.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/economic_calendar.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/error_message.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_countries_item.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_countries_item.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_info.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,17 @@
         domicile (Union[Unset, str]): The domicile of the ETF. Example: US.
         etf_company (Union[Unset, str]): The company which oversees the ETF. Example: SPDR.
         expense_ratio (Union[Unset, str]): The expense ratio of the ETF. Example: 0.0945.
         has_options (Union[Unset, bool]): Boolean flag whether the company has options. Example: True.
         holdings_count (Union[Unset, int]): The amount of holdings the ETF has. Example: 503.
         inception_date (Union[Unset, str]): The inception date of the ETF as an ISO date. Example: 1993-01-22.
         name (Union[Unset, str]): The full name of the ETF. Example: SPDR S&P 500 ETF Trust.
-        opt_vol (Union[Unset, int]): The total options volume traded for the last trading day. Example: 533227.
+        opt_vol (Union[Unset, int]): The total options volume traded for the last Trading Day. Example: 533227.
         put_vol (Union[Unset, int]): The sum of the size of all the put transactions that executed. Example: 808326.
-        stock_vol (Union[Unset, int]): The volume of the ticker for the trading day. Example: 23132119.
+        stock_vol (Union[Unset, int]): The volume of the ticker for the Trading Day. Example: 23132119.
         website (Union[Unset, str]): A link to the website of the ETF. Example:
             https://www.ssga.com/us/en/institutional/etfs/funds/spdr-sp-500-etf-trust-spy.
     """
 
     aum: Union[Unset, str] = UNSET
     avg30_volume: Union[Unset, str] = UNSET
     call_vol: Union[Unset, int] = UNSET
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/etf_sectors_item.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_sectors_item.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/expiry_breakdown.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/fda_calendar.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_alert.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_alert_rule.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert_rule.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_per_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_expiry.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="FlowPerExpiry")
 
 
 @_attrs_define
 class FlowPerExpiry:
-    """The flow data per expiry for a trading day.
+    """The flow data per expiry for a Trading Day.
 
     Example:
         {'data': [{'call_otm_premium': '3885339', 'call_otm_trades': 10213, 'call_otm_volume': 81598, 'call_premium':
             '5839180', 'call_premium_ask_side': '2615356', 'call_premium_bid_side': '2722619', 'call_trades': 11383,
             'call_volume': 89177, 'call_volume_ask_side': 43669, 'call_volume_bid_side': 40164, 'date': datetime.date(2024,
             1, 22), 'expiry': datetime.date(2024, 1, 26), 'put_otm_premium': '632247', 'put_otm_trades': 2077,
             'put_otm_volume': 12164, 'put_premium': '4802145', 'put_premium_ask_side': '3593584', 'put_premium_bid_side':
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/flow_per_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_strike.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="FlowPerStrike")
 
 
 @_attrs_define
 class FlowPerStrike:
-    """The flow data per strike for a trading day.
+    """The flow data per strike for a Trading Day.
 
     Example:
         [{'call_otm_premium': '9908777.0', 'call_otm_trades': 6338, 'call_otm_volume': 40385, 'call_premium':
             '9908777.0', 'call_premium_ask_side': '5037703.0', 'call_premium_bid_side': '4055973.0', 'call_trades': 6338,
             'call_volume': 40385, 'call_volume_ask_side': 20145, 'call_volume_bid_side': 16923, 'date': datetime.date(2024,
             1, 22), 'put_otm_premium': '0.0', 'put_otm_trades': 0, 'put_otm_volume': 0, 'put_premium': '2746872.0',
             'put_premium_ask_side': '799873.0', 'put_premium_bid_side': '1614848.0', 'put_trades': 841, 'put_volume': 4306,
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/greeks.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greeks.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/holdings.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/holdings.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,22 +41,22 @@
             990943.
         close (Union[Unset, str]): The closing price of the candle. Example: 56.79.
         has_options (Union[Unset, bool]): Boolean flag whether the company has options. Example: True.
         high (Union[Unset, str]): The highest price of the candle. Example: 58.12.
         low (Union[Unset, str]): The lowest price of the candle. Example: 51.90.
         name (Union[Unset, str]): The name of the company. Example: APPLE INC.
         open_ (Union[Unset, str]): The opening price of the candle. Example: 54.29.
-        prev_price (Union[Unset, str]): The previous trading day's stock price of the ticker. Example: 189.70.
+        prev_price (Union[Unset, str]): The previous Trading Day's stock price of the ticker. Example: 189.70.
         put_premium (Union[Unset, str]): The sum of the premium of all the put transactions that executed. Example:
             163537151.
         put_volume (Union[Unset, int]): The sum of the size of all the put transactions that executed. Example: 808326.
         sector (Union[Unset, MarketGeneralSector]): The financial sector of the ticker. Empty if unknown or not
             applicable such as ETF/Index. Example: Technology.
         ticker (Union[Unset, str]): The stock ticker. Example: AAPL.
-        volume (Union[Unset, int]): The volume of the ticker for the trading day. Example: 23132119.
+        volume (Union[Unset, int]): The volume of the ticker for the Trading Day. Example: 23132119.
         week_52_high (Union[Unset, str]): The 52 week high stock price of the ticker. Example: 198.23.
         week_52_low (Union[Unset, str]): The 52 week low stock price of the ticker. Example: 124.17.
     """
 
     avg30_volume: Union[Unset, str] = UNSET
     bearish_premium: Union[Unset, str] = UNSET
     bullish_premium: Union[Unset, str] = UNSET
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/imbalances_volume.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/imbalances_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/insider_statistics.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_statistics.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_general_sector.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_holidays.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_holidays.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/market_options_volume.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/max_pain.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/max_pain.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/net_prem_tick_response.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/net_prem_tick_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/off_lit_price_level.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/off_lit_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/oi_change.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/oi_change.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_chains_response.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contract.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,29 @@
             'date': datetime.date(2023, 5, 26), 'floor_volume': 0, 'high_price': '0.03', 'implied_volatility':
             '0.310502942482285', 'iv_high': '0.675815680048166', 'iv_low': '0.310502942482285', 'last_price': '0.01',
             'last_tape_time': datetime.datetime(2023, 5, 26, 21, 30, 29, tzinfo=datetime.timezone.utc), 'low_price': '0.01',
             'mid_volume': 0, 'multi_leg_volume': 393, 'neutral_volume': 2, 'open_interest': 15907, 'stock_multi_leg_volume':
             0, 'sweep_volume': 752, 'total_premium': '3613.00', 'trades': 244, 'volume': 2655}]}
 
     Attributes:
-        ask_volume (Union[Unset, int]): The amount of volume that happened on the ask side. Ask side is defined as (ask + bid) / 2 < fill price. Example: 119403.
-        avg_price (Union[Unset, str]): The volume weighted average fill price of the contract. Example: 1.0465802437910297887119234370.
-        bid_volume (Union[Unset, int]): The amount of volume that happened on the bid side. Bid side is defined as (ask + bid) / 2 > fill price. Example: 122789.
-        cross_volume (Union[Unset, int]): The amount of cross volume. Cross volume consists of all transaction that have the cross trade code.
+        ask_volume (Union[Unset, int]): The amount of volume that happened on the ask side.
+
+            Ask side is defined as (ask + bid) / 2 < fill price.
+             Example: 119403.
+        avg_price (Union[Unset, str]): The volume weighted average fill price of the contract. Example:
+            1.0465802437910297887119234370.
+        bid_volume (Union[Unset, int]): The amount of volume that happened on the bid side.
+
+            Bid side is defined as (ask + bid) / 2 > fill price.
+             Example: 122789.
+        cross_volume (Union[Unset, int]): The amount of cross volume.
+            Cross volume consists of all transaction that have the cross trade code.
         date (Union[Unset, str]): A trading date in ISO format YYYY-MM-DD Example: 2023-09-08.
-        floor_volume (Union[Unset, int]): The amount of floor volume. Floor volume consists of all transaction that have the floor trade code.
+        floor_volume (Union[Unset, int]): The amount of floor volume.
+            Floor volume consists of all transaction that have the floor trade code.
              Example: 142.
         high_price (Union[Unset, str]): The highest fill on that contract. Example: 2.95.
         implied_volatility (Union[Unset, str]): The implied volatility for the last transaction. Example:
             0.675815680048166.
         iv_high (Union[Unset, str]): The highest implied volatility at which a transaction occurred. Example:
             0.675815680048166.
         iv_low (Union[Unset, str]): The lowest implied volatility at which a transaction occurred. Example:
@@ -83,40 +92,60 @@
     total_premium: Union[Unset, str] = UNSET
     trades: Union[Unset, int] = UNSET
     volume: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         ask_volume = self.ask_volume
+
         avg_price = self.avg_price
+
         bid_volume = self.bid_volume
+
         cross_volume = self.cross_volume
+
         date = self.date
+
         floor_volume = self.floor_volume
+
         high_price = self.high_price
+
         implied_volatility = self.implied_volatility
+
         iv_high = self.iv_high
+
         iv_low = self.iv_low
+
         last_price = self.last_price
+
         last_tape_time = self.last_tape_time
+
         low_price = self.low_price
+
         mid_volume = self.mid_volume
+
         multi_leg_volume = self.multi_leg_volume
+
         no_side_volume = self.no_side_volume
+
         open_interest = self.open_interest
+
         stock_multi_leg_volume = self.stock_multi_leg_volume
+
         sweep_volume = self.sweep_volume
+
         total_premium = self.total_premium
+
         trades = self.trades
+
         volume = self.volume
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
-        
         if ask_volume is not UNSET:
             field_dict["ask_volume"] = ask_volume
         if avg_price is not UNSET:
             field_dict["avg_price"] = avg_price
         if bid_volume is not UNSET:
             field_dict["bid_volume"] = bid_volume
         if cross_volume is not UNSET:
@@ -160,34 +189,55 @@
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         ask_volume = d.pop("ask_volume", UNSET)
+
         avg_price = d.pop("avg_price", UNSET)
+
         bid_volume = d.pop("bid_volume", UNSET)
+
         cross_volume = d.pop("cross_volume", UNSET)
+
         date = d.pop("date", UNSET)
+
         floor_volume = d.pop("floor_volume", UNSET)
+
         high_price = d.pop("high_price", UNSET)
+
         implied_volatility = d.pop("implied_volatility", UNSET)
+
         iv_high = d.pop("iv_high", UNSET)
+
         iv_low = d.pop("iv_low", UNSET)
+
         last_price = d.pop("last_price", UNSET)
+
         last_tape_time = d.pop("last_tape_time", UNSET)
+
         low_price = d.pop("low_price", UNSET)
+
         mid_volume = d.pop("mid_volume", UNSET)
+
         multi_leg_volume = d.pop("multi_leg_volume", UNSET)
+
         no_side_volume = d.pop("no_side_volume", UNSET)
+
         open_interest = d.pop("open_interest", UNSET)
+
         stock_multi_leg_volume = d.pop("stock_multi_leg_volume", UNSET)
+
         sweep_volume = d.pop("sweep_volume", UNSET)
+
         total_premium = d.pop("total_premium", UNSET)
+
         trades = d.pop("trades", UNSET)
+
         volume = d.pop("volume", UNSET)
 
         option_contract = cls(
             ask_volume=ask_volume,
             avg_price=avg_price,
             bid_volume=bid_volume,
             cross_volume=cross_volume,
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contract_screener_response.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_screener_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
              Example: 119403.
         avg_price (Union[Unset, str]): The volume weighted average fill price of the contract. Example:
             1.0465802437910297887119234370.
         bid_side_volume (Union[Unset, int]): The amount of volume that happened on the bid side.
 
             Bid side is defined as (ask + bid) / 2 > fill price.
              Example: 122789.
-        chain_prev_close (Union[Unset, str]): The previous trading day's contract price. Example: 1.29.
+        chain_prev_close (Union[Unset, str]): The previous Trading Day's contract price. Example: 1.29.
         close (Union[Unset, str]): The last fill on the contract. Example: 0.03.
         cross_volume (Union[Unset, int]): The amount of cross volume.
             Cross volume consists of all transaction that have the cross trade code.
         er_time (Union[Unset, StockEarningsTime]): The time when the earnings will be released. Example: premarket.
         floor_volume (Union[Unset, int]): The amount of floor volume.
             Floor volume consists of all transaction that have the floor trade code.
              Example: 142.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_contracts.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         open_interest (Union[Unset, int]): The open interest for the contract. Example: 18680.
         option_symbol (Union[Unset, str]): The option symbol of the contract.
 
             You can use the following regex to extract underlying ticker, option type, expiry & strike:
             `^(?<symbol>[\w]*)(?<expiry>(\d{2})(\d{2})(\d{2}))(?<type>[PC])(?<strike>\d{8})$`
 
             Keep in mind that the strike needs to be multiplied by 1,000.
-        prev_oi (Union[Unset, int]): The previous trading day's open interest. Example: 18680.
+        prev_oi (Union[Unset, int]): The previous Trading Day's open interest. Example: 18680.
         stock_multi_leg_volume (Union[Unset, int]): The amount of volume that happened as part of a stock transaction
             and possibly other option contracts.
             This can be covered calls and more.
              Example: 52.
         sweep_volume (Union[Unset, int]): The amount of sweep volume.
             Sweep volume consists of all transaction that have the sweep trade code.
              Example: 18260.
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/option_price_level.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/screener_order_by_field.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_market.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_market.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_monthly.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_monthly.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_performers.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performers.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/seasonality_year_month.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_year_month.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/sector.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/sector_etf.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector_etf.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,21 +38,21 @@
         close (Union[Unset, str]): The closing price of the candle. Example: 56.79.
         full_name (Union[Unset, str]): The name/sector of the SPDR sector ETF. Example: S&P 500 Index.
         high (Union[Unset, str]): The highest price of the candle. Example: 58.12.
         low (Union[Unset, str]): The lowest price of the candle. Example: 51.90.
         marketcap (Union[Unset, str]): The marketcap of the underlying ticker. If the issue type of the ticker is ETF
             then the marketcap represents the AUM. Example: 2965813810400.
         open_ (Union[Unset, str]): The opening price of the candle. Example: 54.29.
-        prev_close (Union[Unset, str]): The previous trading day's stock price of the ticker. Example: 189.70.
-        prev_date (Union[Unset, str]): The date of the previous trading day in ISO format. Example: 2023-09-07.
+        prev_close (Union[Unset, str]): The previous Trading Day's stock price of the ticker. Example: 189.70.
+        prev_date (Union[Unset, str]): The date of the previous Trading Day in ISO format. Example: 2023-09-07.
         put_premium (Union[Unset, str]): The sum of the premium of all the put transactions that executed. Example:
             163537151.
         put_volume (Union[Unset, int]): The sum of the size of all the put transactions that executed. Example: 808326.
         ticker (Union[Unset, str]): The stock ticker. Example: AAPL.
-        volume (Union[Unset, int]): The volume of the ticker for the trading day. Example: 23132119.
+        volume (Union[Unset, int]): The volume of the ticker for the Trading Day. Example: 23132119.
         week_52_high (Union[Unset, str]): The 52 week high stock price of the ticker. Example: 198.23.
         week_52_low (Union[Unset, str]): The 52 week low stock price of the ticker. Example: 124.17.
     """
 
     avg30_stock_volume: Union[Unset, str] = UNSET
     avg_30_day_call_volume: Union[Unset, str] = UNSET
     avg_30_day_put_volume: Union[Unset, str] = UNSET
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/senate_stock.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/senate_stock.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/single_sector.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spike_value.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spike_value.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/stock_screener_response.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_screener_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             is included, then the implied move is for the nearest end of the week expiration (the nearest monthly expiration
             if there are no weekly contracts). Example: 2.2398043036460877.
         implied_move_perc (Union[Unset, str]): The implied move as a percentage of the underlying stock price. Example:
             0.012247398860706955.
         is_index (Union[Unset, bool]): Indicator, whether the ticker is an index. Example: True.
         issue_type (Union[Unset, StockIssueType]): The issue type of the ticker. Example: Common Stock.
         iv30d (Union[Unset, str]): The 30 day implied volatility. Example: 0.2038053572177887.
-        iv30d_1d (Union[Unset, str]): The previous trading day's 30 day implied volatility. Example:
+        iv30d_1d (Union[Unset, str]): The previous Trading Day's 30 day implied volatility. Example:
             0.18791808187961578.
         iv30d_1m (Union[Unset, str]): The implied volatility relative to the implied volatility throughout the previous
             year. A rank of 0 indicates that the implied volatility is the lowest it has been within the past year. A rank
             of 100 indicates that the implied volatility is the highest it has been within the past year. Example:
             13.52369891956068210400.
         iv30d_1w (Union[Unset, str]): The 30 day implied volatility from 1 week ago. Example: 0.18398597836494446.
         iv_rank (Union[Unset, str]): The implied volatility relative to the implied volatility throughout the previous
@@ -82,17 +82,17 @@
             -29138464.
         net_put_premium (Union[Unset, str]): Defined as (put premium ask side) - (put premium bid side). Example:
             23924325.
         next_dividend_date (Union[Unset, datetime.date]): The next dividend date of the ticker. Null if either unknown
             as of now or the stock does not pay dividends. Example: 2023-10-26.
         next_earnings_date (Union[Unset, datetime.date]): The next earnings date of the ticker. Null if either unknown
             as of now or if the ticker does not have any earnings such as an ETF Example: 2023-10-26.
-        prev_call_oi (Union[Unset, int]): The call open interest of the previous trading day. Example: 3994750.
-        prev_close (Union[Unset, str]): The previous trading day's stock price of the ticker. Example: 189.70.
-        prev_put_oi (Union[Unset, int]): The put open interest of the previous trading day. Example: 3679410.
+        prev_call_oi (Union[Unset, int]): The call open interest of the previous Trading Day. Example: 3994750.
+        prev_close (Union[Unset, str]): The previous Trading Day's stock price of the ticker. Example: 189.70.
+        prev_put_oi (Union[Unset, int]): The put open interest of the previous Trading Day. Example: 3679410.
         put_call_ratio (Union[Unset, str]): The put call ratio which is defined as put volume / call volume. Example:
             0.815713920982337.
         put_open_interest (Union[Unset, int]): The sum of the open interest of all the put options. Example: 3564153.
         put_premium (Union[Unset, str]): The sum of the premium of all the put transactions that executed. Example:
             163537151.
         put_volume (Union[Unset, int]): The sum of the size of all the put transactions that executed. Example: 808326.
         put_volume_ask_side (Union[Unset, int]): The sum of the size of all the put transactions that executed on the
```

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/ticker_info.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/ticker_options_volume.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/unusual_whales_api_client/types.py` & `unusual_whales_api_client-1.0.1/unusual_whales_api_client/types.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-0.0.1/PKG-INFO` & `unusual_whales_api_client-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unusual-whales-api-client
-Version: 0.0.1
+Version: 1.0.1
 Summary: A client library for accessing Unusual Whales API
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

