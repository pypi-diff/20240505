# Comparing `tmp/unusual_whales_api_client-1.0.1.tar.gz` & `tmp/unusual_whales_api_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unusual_whales_api_client-1.0.1.tar", max compression
+gzip compressed data, was "unusual_whales_api_client-1.0.2.tar", max compression
```

## Comparing `unusual_whales_api_client-1.0.1.tar` & `unusual_whales_api_client-1.0.2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusual_whales_api_client-1.0.1/LICENSE
--rw-r--r--   0        0        0     5152 2024-05-04 17:34:12.918794 unusual_whales_api_client-1.0.1/README.md
--rw-r--r--   0        0        0      604 2024-05-05 00:05:59.438598 unusual_whales_api_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-05 00:05:50.800080 unusual_whales_api_client-1.0.1/unusual_whales_api_client/.DS_Store
--rw-r--r--   0        0        0      161 2024-05-04 23:06:03.901106 unusual_whales_api_client-1.0.1/unusual_whales_api_client/__init__.py
--rw-r--r--   0        0        0    10244 2024-05-05 00:05:42.270268 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/.DS_Store
--rw-r--r--   0        0        0       45 2024-05-04 23:06:03.900019 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.254843 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/__init__.py
--rw-r--r--   0        0        0     6567 2024-05-04 23:06:03.899211 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trade_report.py
--rw-r--r--   0        0        0     7572 2024-05-04 23:06:03.899581 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trades.py
--rw-r--r--   0        0        0     6538 2024-05-04 23:06:03.899164 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congressional_trades.py
--rw-r--r--   0        0        0     6549 2024-05-04 23:06:03.898428 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_recent_late_reports.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.292207 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/__init__.py
--rw-r--r--   0        0        0     5711 2024-05-04 23:06:03.901311 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_atm_contracts_for_expiries.py
--rw-r--r--   0        0        0     5666 2024-05-04 23:06:03.902527 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_contract_price_history.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.271540 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/__init__.py
--rw-r--r--   0        0        0     6057 2024-05-04 23:06:03.901371 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades.py
--rw-r--r--   0        0        0     7133 2024-05-04 23:06:03.900367 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades_by_ticker.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.272908 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/__init__.py
--rw-r--r--   0        0        0     5739 2024-05-04 23:06:03.898240 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_after_hours_earnings.py
--rw-r--r--   0        0        0     4463 2024-05-04 23:06:03.899179 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_earnings_history.py
--rw-r--r--   0        0        0     5730 2024-05-04 23:06:03.899777 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_premarket_earnings.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.275749 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/__init__.py
--rw-r--r--   0        0        0     3778 2024-05-04 23:06:03.902152 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_holdings.py
--rw-r--r--   0        0        0     4445 2024-05-04 23:06:03.903125 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_info.py
--rw-r--r--   0        0        0     4727 2024-05-04 23:06:03.897476 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_sector_country_weights.py
--rw-r--r--   0        0        0     3914 2024-05-04 23:06:03.897841 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_ticker_exposure_by_etf.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.285035 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/__init__.py
--rw-r--r--   0        0        0     8758 2024-05-04 23:06:03.897691 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_contract_flow.py
--rw-r--r--   0        0        0     6018 2024-05-04 23:06:03.897497 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_daily_expiry_breakdown.py
--rw-r--r--   0        0        0     4221 2024-05-04 23:06:03.897850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_expiry.py
--rw-r--r--   0        0        0     4716 2024-05-04 23:06:03.897790 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_strike.py
--rw-r--r--   0        0        0     3110 2024-05-04 23:06:03.897218 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_full_tape.py
--rw-r--r--   0        0        0     5518 2024-05-04 23:06:03.899198 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_order_flow_alerts.py
--rw-r--r--   0        0        0    28988 2024-05-04 23:06:03.897976 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_ticker_order_flow.py
--rw-r--r--   0        0        0     7172 2024-05-04 23:06:03.898647 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/public_api_ticker_controller_flow_recent.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.331076 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/__init__.py
--rw-r--r--   0        0        0    14016 2024-05-04 23:06:03.898820 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures.py
--rw-r--r--   0        0        0    14437 2024-05-04 23:06:03.898171 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures_by_strike.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.277994 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/__init__.py
--rw-r--r--   0        0        0     3714 2024-05-04 23:06:03.901870 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_economic_calendar.py
--rw-r--r--   0        0        0     3688 2024-05-04 23:06:03.903282 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_fda_calendar.py
--rw-r--r--   0        0        0     3663 2024-05-04 23:06:03.900776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_holidays.py
--rw-r--r--   0        0        0     3735 2024-05-04 23:06:03.903362 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_imbalances.py
--rw-r--r--   0        0        0     5585 2024-05-04 23:06:03.903037 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_insider_trades.py
--rw-r--r--   0        0        0     6092 2024-05-04 23:06:03.901315 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_options_volume.py
--rw-r--r--   0        0        0    12539 2024-05-04 23:06:03.902895 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide.py
--rw-r--r--   0        0        0     6888 2024-05-04 23:06:03.900097 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide_by_etf.py
--rw-r--r--   0        0        0     4441 2024-05-04 23:06:03.900893 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_sector_stats.py
--rw-r--r--   0        0        0     5668 2024-05-04 23:06:03.901797 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_spike.py
--rw-r--r--   0        0        0     7443 2024-05-04 23:06:03.899547 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.319520 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/__init__.py
--rw-r--r--   0        0        0    14029 2024-05-04 23:06:03.904164 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure.py
--rw-r--r--   0        0        0     6143 2024-05-04 23:06:03.899839 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_expiry.py
--rw-r--r--   0        0        0     6211 2024-05-04 23:06:03.903029 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6713 2024-05-04 23:06:03.903077 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike_expiry.py
--rw-r--r--   0        0        0     6286 2024-05-04 23:06:03.903697 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greeks_by_strike_expiry.py
--rw-r--r--   0        0        0     4566 2024-05-04 23:06:03.903668 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_max_pain.py
--rw-r--r--   0        0        0    10450 2024-05-04 23:06:03.899392 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_net_premium_ticks.py
--rw-r--r--   0        0        0     7629 2024-05-04 23:06:03.904034 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_open_interest_change.py
--rw-r--r--   0        0        0     7213 2024-05-04 23:06:03.904169 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_chains.py
--rw-r--r--   0        0        0    10684 2024-05-04 23:06:03.903715 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_contracts.py
--rw-r--r--   0        0        0     5861 2024-05-04 23:06:03.903627 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_volume_by_price_level.py
--rw-r--r--   0        0        0     5856 2024-05-04 23:06:03.903933 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_options_volume.py
--rw-r--r--   0        0        0     5909 2024-05-04 23:06:03.904024 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_volume_open_interest_by_expiry.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.293446 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/__init__.py
--rw-r--r--   0        0        0     8900 2024-05-04 23:06:03.901873 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_analyst_ratings.py
--rw-r--r--   0        0        0    45475 2024-05-04 23:06:03.902568 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_option_contracts.py
--rw-r--r--   0        0        0    64194 2024-05-04 23:06:03.901278 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_stocks.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.304536 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/__init__.py
--rw-r--r--   0        0        0     4129 2024-05-04 23:06:03.902965 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_market_average_returns_by_month.py
--rw-r--r--   0        0        0     4674 2024-05-04 23:06:03.903285 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_average_returns.py
--rw-r--r--   0        0        0    13580 2024-05-04 23:06:03.900876 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_top_performers.py
--rw-r--r--   0        0        0     4800 2024-05-04 23:06:03.901739 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_price_changes_by_month_and_year.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.308574 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/__init__.py
--rw-r--r--   0        0        0     8976 2024-05-04 23:06:03.898970 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_candles.py
--rw-r--r--   0        0        0     4905 2024-05-04 23:06:03.899798 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_insider_trades.py
--rw-r--r--   0        0        0     4561 2024-05-04 23:06:03.898188 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_sector_tickers.py
--rw-r--r--   0        0        0     6260 2024-05-04 23:06:03.899956 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volatility_term_structure.py
--rw-r--r--   0        0        0     7026 2024-05-04 23:06:03.899490 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volume_by_price_level.py
--rw-r--r--   0        0        0     6101 2024-05-04 23:06:03.897503 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.330040 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/__init__.py
--rw-r--r--   0        0        0     8884 2024-05-04 23:06:03.900700 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/get_risk_reversal_skew.py
--rw-r--r--   0        0        0        0 2024-05-04 23:06:03.307484 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/__init__.py
--rw-r--r--   0        0        0    10067 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/channels.py
--rw-r--r--   0        0        0    12417 2024-05-04 23:06:03.901552 unusual_whales_api_client-1.0.1/unusual_whales_api_client/client.py
--rw-r--r--   0        0        0      546 2024-05-04 23:06:03.897133 unusual_whales_api_client-1.0.1/unusual_whales_api_client/errors.py
--rw-r--r--   0        0        0     6501 2024-05-04 23:06:03.901695 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-04 23:06:03.880396 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_action.py
--rw-r--r--   0        0        0      267 2024-05-04 23:06:03.873332 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_field_action.py
--rw-r--r--   0        0        0      183 2024-05-04 23:06:03.872281 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_field_recommendation.py
--rw-r--r--   0        0        0     6697 2024-05-04 23:06:03.899197 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_rating.py
--rw-r--r--   0        0        0      178 2024-05-04 23:06:03.867691 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_recommendation.py
--rw-r--r--   0        0        0      428 2024-05-04 23:06:03.871869 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_sector.py
--rw-r--r--   0        0        0     5399 2024-05-04 23:06:03.897314 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_data.py
--rw-r--r--   0        0        0      251 2024-05-04 23:06:03.868214 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_size.py
--rw-r--r--   0        0        0     5200 2024-05-04 23:06:03.899759 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/country_sector_exposure.py
--rw-r--r--   0        0        0     3869 2024-05-04 23:06:03.899833 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/daily_market_tide.py
--rw-r--r--   0        0        0    10341 2024-05-04 23:06:03.903785 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/darkpool_trade.py
--rw-r--r--   0        0        0     8919 2024-05-04 23:06:03.901180 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/earning.py
--rw-r--r--   0        0        0     4185 2024-05-04 23:06:03.901806 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_calendar.py
--rw-r--r--   0        0        0      189 2024-05-04 23:06:03.868741 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_type.py
--rw-r--r--   0        0        0     2673 2024-05-04 23:06:03.897366 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message.py
--rw-r--r--   0        0        0     1779 2024-05-04 23:06:03.902052 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
--rw-r--r--   0        0        0     2063 2024-05-04 23:06:03.897630 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_countries_item.py
--rw-r--r--   0        0        0     7575 2024-05-04 23:06:03.901157 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_info.py
--rw-r--r--   0        0        0     2044 2024-05-04 23:06:03.901145 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_sectors_item.py
--rw-r--r--   0        0        0     2953 2024-05-04 23:06:03.903989 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/expiry_breakdown.py
--rw-r--r--   0        0        0     5086 2024-05-04 23:06:03.898753 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/fda_calendar.py
--rw-r--r--   0        0        0    10635 2024-05-04 23:06:03.899489 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert.py
--rw-r--r--   0        0        0      590 2024-05-04 23:06:03.871726 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert_rule.py
--rw-r--r--   0        0        0    12800 2024-05-04 23:06:03.904343 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_expiry.py
--rw-r--r--   0        0        0    12688 2024-05-04 23:06:03.898718 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_strike.py
--rw-r--r--   0        0        0     6320 2024-05-04 23:06:03.899850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure.py
--rw-r--r--   0        0        0     6349 2024-05-04 23:06:03.898856 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6808 2024-05-04 23:06:03.903104 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py
--rw-r--r--   0        0        0     9046 2024-05-04 23:06:03.899966 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greeks.py
--rw-r--r--   0        0        0     2535 2024-05-04 23:06:03.900308 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py
--rw-r--r--   0        0        0    10020 2024-05-04 23:06:03.900599 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/holdings.py
--rw-r--r--   0        0        0     4229 2024-05-04 23:06:03.899326 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/imbalances_volume.py
--rw-r--r--   0        0        0     4426 2024-05-04 23:06:03.900807 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py
--rw-r--r--   0        0        0     3678 2024-05-04 23:06:03.898099 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_statistics.py
--rw-r--r--   0        0        0      190 2024-05-04 23:06:03.870716 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_trades_member_type.py
--rw-r--r--   0        0        0      345 2024-05-04 23:06:03.872052 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_trades_transaction_type.py
--rw-r--r--   0        0        0      164 2024-05-04 23:06:03.875455 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_event.py
--rw-r--r--   0        0        0      165 2024-05-04 23:06:03.877003 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_side.py
--rw-r--r--   0        0        0      213 2024-05-04 23:06:03.876685 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_imbalance_type.py
--rw-r--r--   0        0        0      168 2024-05-04 23:06:03.868907 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_market_time.py
--rw-r--r--   0        0        0      528 2024-05-04 23:06:03.878990 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_sector.py
--rw-r--r--   0        0        0     4512 2024-05-04 23:06:03.898435 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_holidays.py
--rw-r--r--   0        0        0     3378 2024-05-04 23:06:03.902850 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_options_volume.py
--rw-r--r--   0        0        0     2680 2024-05-04 23:06:03.901776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/max_pain.py
--rw-r--r--   0        0        0     5964 2024-05-04 23:06:03.898508 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/net_prem_tick_response.py
--rw-r--r--   0        0        0     2494 2024-05-04 23:06:03.901791 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/off_lit_price_level.py
--rw-r--r--   0        0        0    11261 2024-05-04 23:06:03.900810 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/oi_change.py
--rw-r--r--   0        0        0     1742 2024-05-04 23:06:03.898550 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_chains_response.py
--rw-r--r--   0        0        0    10940 2024-05-04 23:06:03.898496 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract.py
--rw-r--r--   0        0        0    14886 2024-05-04 23:06:03.898299 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_screener_response.py
--rw-r--r--   0        0        0      157 2024-05-04 23:06:03.875604 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_type.py
--rw-r--r--   0        0        0    11268 2024-05-04 23:06:03.900558 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contracts.py
--rw-r--r--   0        0        0     2522 2024-05-04 23:06:03.899171 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_price_level.py
--rw-r--r--   0        0        0      149 2024-05-04 23:06:03.877920 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_type.py
--rw-r--r--   0        0        0      153 2024-05-04 23:06:03.870845 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/order_direction.py
--rw-r--r--   0        0        0      949 2024-05-04 23:06:03.878579 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py
--rw-r--r--   0        0        0     1401 2024-05-04 23:06:03.877776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_order_by_field.py
--rw-r--r--   0        0        0     5330 2024-05-04 23:06:03.902577 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_market.py
--rw-r--r--   0        0        0     5009 2024-05-04 23:06:03.897915 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_monthly.py
--rw-r--r--   0        0        0      412 2024-05-04 23:06:03.871752 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performance_order_by.py
--rw-r--r--   0        0        0     6634 2024-05-04 23:06:03.898503 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performers.py
--rw-r--r--   0        0        0     3121 2024-05-04 23:06:03.903851 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_year_month.py
--rw-r--r--   0        0        0      515 2024-05-04 23:06:03.867719 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector.py
--rw-r--r--   0        0        0    10842 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector_etf.py
--rw-r--r--   0        0        0     5674 2024-05-04 23:06:03.897567 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/senate_stock.py
--rw-r--r--   0        0        0      173 2024-05-04 23:06:03.867695 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/side.py
--rw-r--r--   0        0        0      206 2024-05-04 23:06:03.867692 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_issue_type.py
--rw-r--r--   0        0        0      343 2024-05-04 23:06:03.879664 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_month_number.py
--rw-r--r--   0        0        0      521 2024-05-04 23:06:03.869738 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_sector.py
--rw-r--r--   0        0        0      334 2024-05-04 23:06:03.870776 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_external_hour_sold_code.py
--rw-r--r--   0        0        0      312 2024-05-04 23:06:03.879928 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_sale_cond_code.py
--rw-r--r--   0        0        0      304 2024-05-04 23:06:03.871735 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_settlement.py
--rw-r--r--   0        0        0      275 2024-05-04 23:06:03.871914 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_trade_trade_code.py
--rw-r--r--   0        0        0     2304 2024-05-04 23:06:03.903870 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spike_value.py
--rw-r--r--   0        0        0     7769 2024-05-04 23:06:03.901158 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py
--rw-r--r--   0        0        0     8339 2024-05-04 23:06:03.900787 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py
--rw-r--r--   0        0        0      202 2024-05-04 23:06:03.869883 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_earnings_time.py
--rw-r--r--   0        0        0      205 2024-05-04 23:06:03.874468 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_issue_type.py
--rw-r--r--   0        0        0    24207 2024-05-04 23:06:03.900228 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_screener_response.py
--rw-r--r--   0        0        0     8648 2024-05-04 23:06:03.899314 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_info.py
--rw-r--r--   0        0        0    11609 2024-05-04 23:06:03.901548 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_options_volume.py
--rw-r--r--   0        0        0     2436 2024-05-04 23:06:03.900259 unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py
--rw-r--r--   0        0        0       25 2024-05-04 23:06:03.164456 unusual_whales_api_client-1.0.1/unusual_whales_api_client/py.typed
--rw-r--r--   0        0        0      985 2024-05-04 23:06:03.897220 unusual_whales_api_client-1.0.1/unusual_whales_api_client/types.py
--rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 unusual_whales_api_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusual_whales_api_client-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5152 2024-05-04 17:34:12.918794 unusual_whales_api_client-1.0.2/README.md
+-rw-r--r--   0        0        0      580 2024-05-05 00:53:03.026567 unusual_whales_api_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-05 00:05:50.800080 unusual_whales_api_client-1.0.2/unusualwhales/.DS_Store
+-rw-r--r--   0        0        0      161 2024-05-04 23:06:03.901106 unusual_whales_api_client-1.0.2/unusualwhales/__init__.py
+-rw-r--r--   0        0        0    10244 2024-05-05 00:05:42.270268 unusual_whales_api_client-1.0.2/unusualwhales/api/.DS_Store
+-rw-r--r--   0        0        0       45 2024-05-04 23:06:03.900019 unusual_whales_api_client-1.0.2/unusualwhales/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.254843 unusual_whales_api_client-1.0.2/unusualwhales/api/congress/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-04 23:06:03.899211 unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congress_member_trade_report.py
+-rw-r--r--   0        0        0     7572 2024-05-04 23:06:03.899581 unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congress_member_trades.py
+-rw-r--r--   0        0        0     6538 2024-05-04 23:06:03.899164 unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congressional_trades.py
+-rw-r--r--   0        0        0     6549 2024-05-04 23:06:03.898428 unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_recent_late_reports.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.292207 unusual_whales_api_client-1.0.2/unusualwhales/api/contract/__init__.py
+-rw-r--r--   0        0        0     5711 2024-05-04 23:06:03.901311 unusual_whales_api_client-1.0.2/unusualwhales/api/contract/get_atm_contracts_for_expiries.py
+-rw-r--r--   0        0        0     5666 2024-05-04 23:06:03.902527 unusual_whales_api_client-1.0.2/unusualwhales/api/contract/get_contract_price_history.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.271540 unusual_whales_api_client-1.0.2/unusualwhales/api/darkpool/__init__.py
+-rw-r--r--   0        0        0     6057 2024-05-04 23:06:03.901371 unusual_whales_api_client-1.0.2/unusualwhales/api/darkpool/get_darkpool_trades.py
+-rw-r--r--   0        0        0     7133 2024-05-04 23:06:03.900367 unusual_whales_api_client-1.0.2/unusualwhales/api/darkpool/get_darkpool_trades_by_ticker.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.272908 unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/__init__.py
+-rw-r--r--   0        0        0     5739 2024-05-04 23:06:03.898240 unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_after_hours_earnings.py
+-rw-r--r--   0        0        0     4463 2024-05-04 23:06:03.899179 unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_earnings_history.py
+-rw-r--r--   0        0        0     5730 2024-05-04 23:06:03.899777 unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_premarket_earnings.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.275749 unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/__init__.py
+-rw-r--r--   0        0        0     3778 2024-05-04 23:06:03.902152 unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_holdings.py
+-rw-r--r--   0        0        0     4445 2024-05-04 23:06:03.903125 unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_info.py
+-rw-r--r--   0        0        0     4727 2024-05-04 23:06:03.897476 unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_sector_country_weights.py
+-rw-r--r--   0        0        0     3914 2024-05-04 23:06:03.897841 unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_ticker_exposure_by_etf.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.285035 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/__init__.py
+-rw-r--r--   0        0        0     8758 2024-05-04 23:06:03.897691 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_contract_flow.py
+-rw-r--r--   0        0        0     6018 2024-05-04 23:06:03.897497 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_daily_expiry_breakdown.py
+-rw-r--r--   0        0        0     4221 2024-05-04 23:06:03.897850 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_flow_by_expiry.py
+-rw-r--r--   0        0        0     4716 2024-05-04 23:06:03.897790 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_flow_by_strike.py
+-rw-r--r--   0        0        0     3110 2024-05-04 23:06:03.897218 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_full_tape.py
+-rw-r--r--   0        0        0     5518 2024-05-04 23:06:03.899198 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_order_flow_alerts.py
+-rw-r--r--   0        0        0    28988 2024-05-04 23:06:03.897976 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_ticker_order_flow.py
+-rw-r--r--   0        0        0     7172 2024-05-04 23:06:03.898647 unusual_whales_api_client-1.0.2/unusualwhales/api/flow/public_api_ticker_controller_flow_recent.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.331076 unusual_whales_api_client-1.0.2/unusualwhales/api/gex/__init__.py
+-rw-r--r--   0        0        0    14016 2024-05-04 23:06:03.898820 unusual_whales_api_client-1.0.2/unusualwhales/api/gex/get_spot_exposures.py
+-rw-r--r--   0        0        0    14437 2024-05-04 23:06:03.898171 unusual_whales_api_client-1.0.2/unusualwhales/api/gex/get_spot_exposures_by_strike.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.277994 unusual_whales_api_client-1.0.2/unusualwhales/api/market/__init__.py
+-rw-r--r--   0        0        0     3714 2024-05-04 23:06:03.901870 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_economic_calendar.py
+-rw-r--r--   0        0        0     3688 2024-05-04 23:06:03.903282 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_fda_calendar.py
+-rw-r--r--   0        0        0     3663 2024-05-04 23:06:03.900776 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_holidays.py
+-rw-r--r--   0        0        0     3735 2024-05-04 23:06:03.903362 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_imbalances.py
+-rw-r--r--   0        0        0     5585 2024-05-04 23:06:03.903037 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_insider_trades.py
+-rw-r--r--   0        0        0     6092 2024-05-04 23:06:03.901315 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_options_volume.py
+-rw-r--r--   0        0        0    12539 2024-05-04 23:06:03.902895 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_tide.py
+-rw-r--r--   0        0        0     6888 2024-05-04 23:06:03.900097 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_tide_by_etf.py
+-rw-r--r--   0        0        0     4441 2024-05-04 23:06:03.900893 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_sector_stats.py
+-rw-r--r--   0        0        0     5668 2024-05-04 23:06:03.901797 unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_spike.py
+-rw-r--r--   0        0        0     7443 2024-05-04 23:06:03.899547 unusual_whales_api_client-1.0.2/unusualwhales/api/market/public_api_market_controller_oi_change.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.319520 unusual_whales_api_client-1.0.2/unusualwhales/api/option/__init__.py
+-rw-r--r--   0        0        0    14029 2024-05-04 23:06:03.904164 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure.py
+-rw-r--r--   0        0        0     6143 2024-05-04 23:06:03.899839 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_expiry.py
+-rw-r--r--   0        0        0     6211 2024-05-04 23:06:03.903029 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6713 2024-05-04 23:06:03.903077 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_strike_expiry.py
+-rw-r--r--   0        0        0     6286 2024-05-04 23:06:03.903697 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greeks_by_strike_expiry.py
+-rw-r--r--   0        0        0     4566 2024-05-04 23:06:03.903668 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_max_pain.py
+-rw-r--r--   0        0        0    10450 2024-05-04 23:06:03.899392 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_net_premium_ticks.py
+-rw-r--r--   0        0        0     7629 2024-05-04 23:06:03.904034 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_open_interest_change.py
+-rw-r--r--   0        0        0     7213 2024-05-04 23:06:03.904169 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_chains.py
+-rw-r--r--   0        0        0    10684 2024-05-04 23:06:03.903715 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_contracts.py
+-rw-r--r--   0        0        0     5861 2024-05-04 23:06:03.903627 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_volume_by_price_level.py
+-rw-r--r--   0        0        0     5856 2024-05-04 23:06:03.903933 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_options_volume.py
+-rw-r--r--   0        0        0     5909 2024-05-04 23:06:03.904024 unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_volume_open_interest_by_expiry.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.293446 unusual_whales_api_client-1.0.2/unusualwhales/api/screener/__init__.py
+-rw-r--r--   0        0        0     8900 2024-05-04 23:06:03.901873 unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_analyst_ratings.py
+-rw-r--r--   0        0        0    45475 2024-05-04 23:06:03.902568 unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_option_contracts.py
+-rw-r--r--   0        0        0    64194 2024-05-04 23:06:03.901278 unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_stocks.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.304536 unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/__init__.py
+-rw-r--r--   0        0        0     4129 2024-05-04 23:06:03.902965 unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_market_average_returns_by_month.py
+-rw-r--r--   0        0        0     4674 2024-05-04 23:06:03.903285 unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_monthly_average_returns.py
+-rw-r--r--   0        0        0    13580 2024-05-04 23:06:03.900876 unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_monthly_top_performers.py
+-rw-r--r--   0        0        0     4800 2024-05-04 23:06:03.901739 unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.308574 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/__init__.py
+-rw-r--r--   0        0        0     8976 2024-05-04 23:06:03.898970 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_candles.py
+-rw-r--r--   0        0        0     4905 2024-05-04 23:06:03.899798 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_insider_trades.py
+-rw-r--r--   0        0        0     4561 2024-05-04 23:06:03.898188 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_sector_tickers.py
+-rw-r--r--   0        0        0     6260 2024-05-04 23:06:03.899956 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_volatility_term_structure.py
+-rw-r--r--   0        0        0     7026 2024-05-04 23:06:03.899490 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_volume_by_price_level.py
+-rw-r--r--   0        0        0     6101 2024-05-04 23:06:03.897503 unusual_whales_api_client-1.0.2/unusualwhales/api/stock/public_api_ticker_controller_info.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.330040 unusual_whales_api_client-1.0.2/unusualwhales/api/volatility/__init__.py
+-rw-r--r--   0        0        0     8884 2024-05-04 23:06:03.900700 unusual_whales_api_client-1.0.2/unusualwhales/api/volatility/get_risk_reversal_skew.py
+-rw-r--r--   0        0        0        0 2024-05-04 23:06:03.307484 unusual_whales_api_client-1.0.2/unusualwhales/api/websocket/__init__.py
+-rw-r--r--   0        0        0    10067 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.2/unusualwhales/api/websocket/channels.py
+-rw-r--r--   0        0        0    12417 2024-05-04 23:06:03.901552 unusual_whales_api_client-1.0.2/unusualwhales/client.py
+-rw-r--r--   0        0        0      546 2024-05-04 23:06:03.897133 unusual_whales_api_client-1.0.2/unusualwhales/errors.py
+-rw-r--r--   0        0        0     6501 2024-05-04 23:06:03.901695 unusual_whales_api_client-1.0.2/unusualwhales/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-04 23:06:03.880396 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_action.py
+-rw-r--r--   0        0        0      267 2024-05-04 23:06:03.873332 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_field_action.py
+-rw-r--r--   0        0        0      183 2024-05-04 23:06:03.872281 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_field_recommendation.py
+-rw-r--r--   0        0        0     6697 2024-05-04 23:06:03.899197 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_rating.py
+-rw-r--r--   0        0        0      178 2024-05-04 23:06:03.867691 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_recommendation.py
+-rw-r--r--   0        0        0      428 2024-05-04 23:06:03.871869 unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_sector.py
+-rw-r--r--   0        0        0     5399 2024-05-04 23:06:03.897314 unusual_whales_api_client-1.0.2/unusualwhales/models/candle_data.py
+-rw-r--r--   0        0        0      251 2024-05-04 23:06:03.868214 unusual_whales_api_client-1.0.2/unusualwhales/models/candle_size.py
+-rw-r--r--   0        0        0     5200 2024-05-04 23:06:03.899759 unusual_whales_api_client-1.0.2/unusualwhales/models/country_sector_exposure.py
+-rw-r--r--   0        0        0     3869 2024-05-04 23:06:03.899833 unusual_whales_api_client-1.0.2/unusualwhales/models/daily_market_tide.py
+-rw-r--r--   0        0        0    10341 2024-05-04 23:06:03.903785 unusual_whales_api_client-1.0.2/unusualwhales/models/darkpool_trade.py
+-rw-r--r--   0        0        0     8919 2024-05-04 23:06:03.901180 unusual_whales_api_client-1.0.2/unusualwhales/models/earning.py
+-rw-r--r--   0        0        0     4185 2024-05-04 23:06:03.901806 unusual_whales_api_client-1.0.2/unusualwhales/models/economic_calendar.py
+-rw-r--r--   0        0        0      189 2024-05-04 23:06:03.868741 unusual_whales_api_client-1.0.2/unusualwhales/models/economic_type.py
+-rw-r--r--   0        0        0     2673 2024-05-04 23:06:03.897366 unusual_whales_api_client-1.0.2/unusualwhales/models/error_message.py
+-rw-r--r--   0        0        0     1779 2024-05-04 23:06:03.902052 unusual_whales_api_client-1.0.2/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
+-rw-r--r--   0        0        0     2063 2024-05-04 23:06:03.897630 unusual_whales_api_client-1.0.2/unusualwhales/models/etf_countries_item.py
+-rw-r--r--   0        0        0     7575 2024-05-04 23:06:03.901157 unusual_whales_api_client-1.0.2/unusualwhales/models/etf_info.py
+-rw-r--r--   0        0        0     2044 2024-05-04 23:06:03.901145 unusual_whales_api_client-1.0.2/unusualwhales/models/etf_sectors_item.py
+-rw-r--r--   0        0        0     2953 2024-05-04 23:06:03.903989 unusual_whales_api_client-1.0.2/unusualwhales/models/expiry_breakdown.py
+-rw-r--r--   0        0        0     5086 2024-05-04 23:06:03.898753 unusual_whales_api_client-1.0.2/unusualwhales/models/fda_calendar.py
+-rw-r--r--   0        0        0    10635 2024-05-04 23:06:03.899489 unusual_whales_api_client-1.0.2/unusualwhales/models/flow_alert.py
+-rw-r--r--   0        0        0      590 2024-05-04 23:06:03.871726 unusual_whales_api_client-1.0.2/unusualwhales/models/flow_alert_rule.py
+-rw-r--r--   0        0        0    12800 2024-05-04 23:06:03.904343 unusual_whales_api_client-1.0.2/unusualwhales/models/flow_per_expiry.py
+-rw-r--r--   0        0        0    12688 2024-05-04 23:06:03.898718 unusual_whales_api_client-1.0.2/unusualwhales/models/flow_per_strike.py
+-rw-r--r--   0        0        0     6320 2024-05-04 23:06:03.899850 unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure.py
+-rw-r--r--   0        0        0     6349 2024-05-04 23:06:03.898856 unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6808 2024-05-04 23:06:03.903104 unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure_by_strike_and_expiry.py
+-rw-r--r--   0        0        0     9046 2024-05-04 23:06:03.899966 unusual_whales_api_client-1.0.2/unusualwhales/models/greeks.py
+-rw-r--r--   0        0        0     2535 2024-05-04 23:06:03.900308 unusual_whales_api_client-1.0.2/unusualwhales/models/historical_risk_reversal_skew.py
+-rw-r--r--   0        0        0    10020 2024-05-04 23:06:03.900599 unusual_whales_api_client-1.0.2/unusualwhales/models/holdings.py
+-rw-r--r--   0        0        0     4229 2024-05-04 23:06:03.899326 unusual_whales_api_client-1.0.2/unusualwhales/models/imbalances_volume.py
+-rw-r--r--   0        0        0     4426 2024-05-04 23:06:03.900807 unusual_whales_api_client-1.0.2/unusualwhales/models/implied_volatility_term_structure.py
+-rw-r--r--   0        0        0     3678 2024-05-04 23:06:03.898099 unusual_whales_api_client-1.0.2/unusualwhales/models/insider_statistics.py
+-rw-r--r--   0        0        0      190 2024-05-04 23:06:03.870716 unusual_whales_api_client-1.0.2/unusualwhales/models/insider_trades_member_type.py
+-rw-r--r--   0        0        0      345 2024-05-04 23:06:03.872052 unusual_whales_api_client-1.0.2/unusualwhales/models/insider_trades_transaction_type.py
+-rw-r--r--   0        0        0      164 2024-05-04 23:06:03.875455 unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_imbalance_event.py
+-rw-r--r--   0        0        0      165 2024-05-04 23:06:03.877003 unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_imbalance_side.py
+-rw-r--r--   0        0        0      213 2024-05-04 23:06:03.876685 unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_imbalance_type.py
+-rw-r--r--   0        0        0      168 2024-05-04 23:06:03.868907 unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_market_time.py
+-rw-r--r--   0        0        0      528 2024-05-04 23:06:03.878990 unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_sector.py
+-rw-r--r--   0        0        0     4512 2024-05-04 23:06:03.898435 unusual_whales_api_client-1.0.2/unusualwhales/models/market_holidays.py
+-rw-r--r--   0        0        0     3378 2024-05-04 23:06:03.902850 unusual_whales_api_client-1.0.2/unusualwhales/models/market_options_volume.py
+-rw-r--r--   0        0        0     2680 2024-05-04 23:06:03.901776 unusual_whales_api_client-1.0.2/unusualwhales/models/max_pain.py
+-rw-r--r--   0        0        0     5964 2024-05-04 23:06:03.898508 unusual_whales_api_client-1.0.2/unusualwhales/models/net_prem_tick_response.py
+-rw-r--r--   0        0        0     2494 2024-05-04 23:06:03.901791 unusual_whales_api_client-1.0.2/unusualwhales/models/off_lit_price_level.py
+-rw-r--r--   0        0        0    11261 2024-05-04 23:06:03.900810 unusual_whales_api_client-1.0.2/unusualwhales/models/oi_change.py
+-rw-r--r--   0        0        0     1742 2024-05-04 23:06:03.898550 unusual_whales_api_client-1.0.2/unusualwhales/models/option_chains_response.py
+-rw-r--r--   0        0        0    10940 2024-05-04 23:06:03.898496 unusual_whales_api_client-1.0.2/unusualwhales/models/option_contract.py
+-rw-r--r--   0        0        0    14886 2024-05-04 23:06:03.898299 unusual_whales_api_client-1.0.2/unusualwhales/models/option_contract_screener_response.py
+-rw-r--r--   0        0        0      157 2024-05-04 23:06:03.875604 unusual_whales_api_client-1.0.2/unusualwhales/models/option_contract_type.py
+-rw-r--r--   0        0        0    11268 2024-05-04 23:06:03.900558 unusual_whales_api_client-1.0.2/unusualwhales/models/option_contracts.py
+-rw-r--r--   0        0        0     2522 2024-05-04 23:06:03.899171 unusual_whales_api_client-1.0.2/unusualwhales/models/option_price_level.py
+-rw-r--r--   0        0        0      149 2024-05-04 23:06:03.877920 unusual_whales_api_client-1.0.2/unusualwhales/models/option_type.py
+-rw-r--r--   0        0        0      153 2024-05-04 23:06:03.870845 unusual_whales_api_client-1.0.2/unusualwhales/models/order_direction.py
+-rw-r--r--   0        0        0      949 2024-05-04 23:06:03.878579 unusual_whales_api_client-1.0.2/unusualwhales/models/screener_contract_order_by_field.py
+-rw-r--r--   0        0        0     1401 2024-05-04 23:06:03.877776 unusual_whales_api_client-1.0.2/unusualwhales/models/screener_order_by_field.py
+-rw-r--r--   0        0        0     5330 2024-05-04 23:06:03.902577 unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_market.py
+-rw-r--r--   0        0        0     5009 2024-05-04 23:06:03.897915 unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_monthly.py
+-rw-r--r--   0        0        0      412 2024-05-04 23:06:03.871752 unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_performance_order_by.py
+-rw-r--r--   0        0        0     6634 2024-05-04 23:06:03.898503 unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_performers.py
+-rw-r--r--   0        0        0     3121 2024-05-04 23:06:03.903851 unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_year_month.py
+-rw-r--r--   0        0        0      515 2024-05-04 23:06:03.867719 unusual_whales_api_client-1.0.2/unusualwhales/models/sector.py
+-rw-r--r--   0        0        0    10842 2024-05-04 23:06:03.902044 unusual_whales_api_client-1.0.2/unusualwhales/models/sector_etf.py
+-rw-r--r--   0        0        0     5674 2024-05-04 23:06:03.897567 unusual_whales_api_client-1.0.2/unusualwhales/models/senate_stock.py
+-rw-r--r--   0        0        0      173 2024-05-04 23:06:03.867695 unusual_whales_api_client-1.0.2/unusualwhales/models/side.py
+-rw-r--r--   0        0        0      206 2024-05-04 23:06:03.867692 unusual_whales_api_client-1.0.2/unusualwhales/models/single_issue_type.py
+-rw-r--r--   0        0        0      343 2024-05-04 23:06:03.879664 unusual_whales_api_client-1.0.2/unusualwhales/models/single_month_number.py
+-rw-r--r--   0        0        0      521 2024-05-04 23:06:03.869738 unusual_whales_api_client-1.0.2/unusualwhales/models/single_sector.py
+-rw-r--r--   0        0        0      334 2024-05-04 23:06:03.870776 unusual_whales_api_client-1.0.2/unusualwhales/models/single_trade_external_hour_sold_code.py
+-rw-r--r--   0        0        0      312 2024-05-04 23:06:03.879928 unusual_whales_api_client-1.0.2/unusualwhales/models/single_trade_sale_cond_code.py
+-rw-r--r--   0        0        0      304 2024-05-04 23:06:03.871735 unusual_whales_api_client-1.0.2/unusualwhales/models/single_trade_settlement.py
+-rw-r--r--   0        0        0      275 2024-05-04 23:06:03.871914 unusual_whales_api_client-1.0.2/unusualwhales/models/single_trade_trade_code.py
+-rw-r--r--   0        0        0     2304 2024-05-04 23:06:03.903870 unusual_whales_api_client-1.0.2/unusualwhales/models/spike_value.py
+-rw-r--r--   0        0        0     7769 2024-05-04 23:06:03.901158 unusual_whales_api_client-1.0.2/unusualwhales/models/spot_gex_exposures_per_1_min.py
+-rw-r--r--   0        0        0     8339 2024-05-04 23:06:03.900787 unusual_whales_api_client-1.0.2/unusualwhales/models/spot_greek_exposures_by_strike.py
+-rw-r--r--   0        0        0      202 2024-05-04 23:06:03.869883 unusual_whales_api_client-1.0.2/unusualwhales/models/stock_earnings_time.py
+-rw-r--r--   0        0        0      205 2024-05-04 23:06:03.874468 unusual_whales_api_client-1.0.2/unusualwhales/models/stock_issue_type.py
+-rw-r--r--   0        0        0    24207 2024-05-04 23:06:03.900228 unusual_whales_api_client-1.0.2/unusualwhales/models/stock_screener_response.py
+-rw-r--r--   0        0        0     8648 2024-05-04 23:06:03.899314 unusual_whales_api_client-1.0.2/unusualwhales/models/ticker_info.py
+-rw-r--r--   0        0        0    11609 2024-05-04 23:06:03.901548 unusual_whales_api_client-1.0.2/unusualwhales/models/ticker_options_volume.py
+-rw-r--r--   0        0        0     2436 2024-05-04 23:06:03.900259 unusual_whales_api_client-1.0.2/unusualwhales/models/volume_oi_per_expiry.py
+-rw-r--r--   0        0        0       25 2024-05-04 23:06:03.164456 unusual_whales_api_client-1.0.2/unusualwhales/py.typed
+-rw-r--r--   0        0        0      985 2024-05-04 23:06:03.897220 unusual_whales_api_client-1.0.2/unusualwhales/types.py
+-rw-r--r--   0        0        0     5819 1970-01-01 00:00:00.000000 unusual_whales_api_client-1.0.2/PKG-INFO
```

### Comparing `unusual_whales_api_client-1.0.1/LICENSE` & `unusual_whales_api_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/README.md` & `unusual_whales_api_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/pyproject.toml` & `unusual_whales_api_client-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "unusual-whales-api-client"
-version = "1.0.1"
+version = "1.0.2"
 description = "A client library for accessing Unusual Whales API"
 authors = []
 readme = "README.md"
 packages = [
-    {include = "unusual_whales_api_client"},
+    {include = "unusualwhales"},
 ]
-include = ["CHANGELOG.md", "unusual_whales_api_client/py.typed"]
+include = ["CHANGELOG.md", "unusualwhales/py.typed"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.20.0,<0.28.0"
 attrs = ">=21.3.0"
 python-dateutil = "^2.8.0"
```

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/.DS_Store` & `unusual_whales_api_client-1.0.2/unusualwhales/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/.DS_Store` & `unusual_whales_api_client-1.0.2/unusualwhales/api/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trade_report.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congress_member_trade_report.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congress_member_trades.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congress_member_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_congressional_trades.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_congressional_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/congress/get_recent_late_reports.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/congress/get_recent_late_reports.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_atm_contracts_for_expiries.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/contract/get_atm_contracts_for_expiries.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/contract/get_contract_price_history.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/contract/get_contract_price_history.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/darkpool/get_darkpool_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/darkpool/get_darkpool_trades_by_ticker.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/darkpool/get_darkpool_trades_by_ticker.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_after_hours_earnings.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_after_hours_earnings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_earnings_history.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_earnings_history.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/earnings/get_premarket_earnings.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/earnings/get_premarket_earnings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_holdings.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_holdings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_info.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_sector_country_weights.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_sector_country_weights.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/etfs/get_ticker_exposure_by_etf.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/etfs/get_ticker_exposure_by_etf.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_contract_flow.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_contract_flow.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_daily_expiry_breakdown.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_daily_expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_flow_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_flow_by_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_flow_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_full_tape.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_full_tape.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_order_flow_alerts.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_order_flow_alerts.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/get_ticker_order_flow.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/get_ticker_order_flow.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/flow/public_api_ticker_controller_flow_recent.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/flow/public_api_ticker_controller_flow_recent.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/gex/get_spot_exposures.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/gex/get_spot_exposures_by_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/gex/get_spot_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_economic_calendar.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_fda_calendar.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_holidays.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_holidays.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_imbalances.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_imbalances.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_insider_trades.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_options_volume.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_market_tide_by_etf.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_market_tide_by_etf.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_sector_stats.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_sector_stats.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/get_spike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/get_spike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/market/public_api_market_controller_oi_change.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/market/public_api_market_controller_oi_change.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greek_exposure_by_strike_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greek_exposure_by_strike_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_greeks_by_strike_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_greeks_by_strike_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_max_pain.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_max_pain.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_net_premium_ticks.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_net_premium_ticks.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_open_interest_change.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_open_interest_change.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_chains.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_chains.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_contracts.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_option_volume_by_price_level.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_option_volume_by_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_options_volume.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/option/get_volume_open_interest_by_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/option/get_volume_open_interest_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_analyst_ratings.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_option_contracts.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/screener/get_stocks.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/screener/get_stocks.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_market_average_returns_by_month.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_market_average_returns_by_month.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_average_returns.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_monthly_average_returns.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_monthly_top_performers.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_monthly_top_performers.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/seasonality/get_price_changes_by_month_and_year.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_candles.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_candles.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_insider_trades.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_sector_tickers.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_sector_tickers.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volatility_term_structure.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/get_volume_by_price_level.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/get_volume_by_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/stock/public_api_ticker_controller_info.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/stock/public_api_ticker_controller_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/volatility/get_risk_reversal_skew.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/volatility/get_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/api/websocket/channels.py` & `unusual_whales_api_client-1.0.2/unusualwhales/api/websocket/channels.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/client.py` & `unusual_whales_api_client-1.0.2/unusualwhales/client.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/errors.py` & `unusual_whales_api_client-1.0.2/unusualwhales/errors.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/__init__.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/analyst_rating.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/analyst_rating.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/candle_data.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/candle_data.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/country_sector_exposure.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/country_sector_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/daily_market_tide.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/daily_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/darkpool_trade.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/darkpool_trade.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/earning.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/earning.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/economic_calendar.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/error_message.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_countries_item.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/etf_countries_item.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_info.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/etf_sectors_item.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/etf_sectors_item.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/expiry_breakdown.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/fda_calendar.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/flow_alert.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_alert_rule.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/flow_alert_rule.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/flow_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/flow_per_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/flow_per_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greek_exposure_by_strike_and_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/greek_exposure_by_strike_and_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/greeks.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/greeks.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/historical_risk_reversal_skew.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/historical_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/holdings.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/holdings.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/imbalances_volume.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/imbalances_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/implied_volatility_term_structure.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/implied_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/insider_statistics.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/insider_statistics.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_general_sector.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/market_general_sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_holidays.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/market_holidays.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/market_options_volume.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/max_pain.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/max_pain.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/net_prem_tick_response.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/net_prem_tick_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/off_lit_price_level.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/off_lit_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/oi_change.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/oi_change.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_chains_response.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/option_contract.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contract_screener_response.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/option_contract_screener_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_contracts.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/option_price_level.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/option_price_level.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_contract_order_by_field.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/screener_contract_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/screener_order_by_field.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/screener_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_market.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_market.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_monthly.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_monthly.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_performers.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_performers.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/seasonality_year_month.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/seasonality_year_month.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/sector_etf.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/sector_etf.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/senate_stock.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/senate_stock.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/single_sector.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/single_sector.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spike_value.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/spike_value.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_gex_exposures_per_1_min.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/spot_gex_exposures_per_1_min.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/spot_greek_exposures_by_strike.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/spot_greek_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/stock_screener_response.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/stock_screener_response.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_info.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/ticker_info.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/ticker_options_volume.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/ticker_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/models/volume_oi_per_expiry.py` & `unusual_whales_api_client-1.0.2/unusualwhales/models/volume_oi_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/unusual_whales_api_client/types.py` & `unusual_whales_api_client-1.0.2/unusualwhales/types.py`

 * *Files identical despite different names*

### Comparing `unusual_whales_api_client-1.0.1/PKG-INFO` & `unusual_whales_api_client-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unusual-whales-api-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: A client library for accessing Unusual Whales API
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

