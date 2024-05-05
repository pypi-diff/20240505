# Comparing `tmp/wtfis-0.9.0.tar.gz` & `tmp/wtfis-0.9.1.tar.gz`

## Comparing `wtfis-0.9.0.tar` & `wtfis-0.9.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wtfis-0.9.0/.env.wtfis.example
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.9.0/.flake8
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.9.0/Dockerfile
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.9.0/Makefile
--rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/demo-old.gif
--rw-r--r--   0        0        0   132990 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/demo.gif
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-abuseipdb.png
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-greynoise.png
--rw-r--r--   0        0        0   100708 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-ip.png
--rw-r--r--   0        0        0    58474 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-no-color.png
--rw-r--r--   0        0        0   110694 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-one-column.png
--rw-r--r--   0        0        0    29089 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-shodan.png
--rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 wtfis-0.9.0/imgs/example-urlhaus.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_cli.py
--rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_clients.py
--rw-r--r--   0        0        0    23993 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_handlers.py
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_models_vt.py
--rw-r--r--   0        0        0    54609 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_ui_domain_view.py
--rw-r--r--   0        0        0    28862 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_ui_ip_view.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_green.json
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_raw.json
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_red.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_1.1.1.1_yellow.json
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/abuseipdb_one.json
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1.json
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1_malicious.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_1.1.1.1_unknown.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/greynoise_one.json
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ip2whois_whois_bbc.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ip2whois_whois_hotmail.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_1.1.1.1.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_gist.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/ipwhois_raw_10.0.0.1.json
--rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_passive_dns_gist.json
--rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/pt_whois_gist.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_1.1.1.1.json
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_gist.json
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_gist_2.json
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_one.json
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/shodan_wired.json
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/urlhaus_1.1.1.1.json
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/urlhaus_gist.json
--rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_gist.json
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_google.json
--rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_domain_tucows.json
--rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_ip_1.1.1.1.json
--rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_ip_142.251.220.110.json
--rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_gist.json
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_one.json
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_resolutions_wired.json
--rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_1.1.1.1.json
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_bbc.json
--rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_example.json
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_example_2.json
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_foo.json
--rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.9.0/tests/test_data/vt_whois_gist.json
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/__init__.py
--rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/main.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/types.py
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/utils.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/__init__.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/abuseipdb.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/base.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/greynoise.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/ip2whois.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/ipwhois.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/passivetotal.py
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/shodan.py
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/urlhaus.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/clients/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/__init__.py
--rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/base.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/domain.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/handlers/ip.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/__init__.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/abuseipdb.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/common.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/greynoise.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/ip2whois.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/ipwhois.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/passivetotal.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/shodan.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/urlhaus.py
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/models/virustotal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/__init__.py
--rw-r--r--   0        0        0    19498 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/base.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/progress.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/theme.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wtfis-0.9.0/wtfis/ui/view.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 wtfis-0.9.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.0/LICENSE
--rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 wtfis-0.9.0/README.md
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 wtfis-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11547 2020-02-02 00:00:00.000000 wtfis-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wtfis-0.9.1/.env.wtfis.example
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 wtfis-0.9.1/.flake8
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 wtfis-0.9.1/Dockerfile
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 wtfis-0.9.1/Makefile
+-rw-r--r--   0        0        0    80106 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/demo-old.gif
+-rw-r--r--   0        0        0   132990 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/demo.gif
+-rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-abuseipdb.png
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-greynoise.png
+-rw-r--r--   0        0        0   100708 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-ip.png
+-rw-r--r--   0        0        0    58474 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-no-color.png
+-rw-r--r--   0        0        0   110694 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-one-column.png
+-rw-r--r--   0        0        0    29089 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-shodan.png
+-rw-r--r--   0        0        0    23045 2020-02-02 00:00:00.000000 wtfis-0.9.1/imgs/example-urlhaus.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_cli.py
+-rw-r--r--   0        0        0     8351 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_clients.py
+-rw-r--r--   0        0        0    23993 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_handlers.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_models_vt.py
+-rw-r--r--   0        0        0    54155 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_ui_domain_view.py
+-rw-r--r--   0        0        0    28376 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_ui_ip_view.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/abuseipdb_1.1.1.1_green.json
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/abuseipdb_1.1.1.1_raw.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/abuseipdb_1.1.1.1_red.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/abuseipdb_1.1.1.1_yellow.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/abuseipdb_one.json
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/greynoise_1.1.1.1.json
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/greynoise_1.1.1.1_malicious.json
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/greynoise_1.1.1.1_unknown.json
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/greynoise_one.json
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/ip2whois_whois_bbc.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/ip2whois_whois_hotmail.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/ipwhois_1.1.1.1.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/ipwhois_gist.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/ipwhois_raw_10.0.0.1.json
+-rw-r--r--   0        0        0     9733 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/pt_passive_dns_gist.json
+-rw-r--r--   0        0        0    10017 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/pt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/pt_whois_gist.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/shodan_1.1.1.1.json
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/shodan_gist.json
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/shodan_gist_2.json
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/shodan_one.json
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/shodan_wired.json
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/urlhaus_1.1.1.1.json
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/urlhaus_gist.json
+-rw-r--r--   0        0        0    18175 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_domain_gist.json
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_domain_google.json
+-rw-r--r--   0        0        0    17624 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_domain_tucows.json
+-rw-r--r--   0        0        0    17725 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_ip_1.1.1.1.json
+-rw-r--r--   0        0        0    11171 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_ip_142.251.220.110.json
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_resolutions_gist.json
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_resolutions_one.json
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_resolutions_wired.json
+-rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_1.1.1.1.json
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_bbc.json
+-rw-r--r--   0        0        0    14040 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_example.json
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_example_2.json
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_foo.json
+-rw-r--r--   0        0        0    18644 2020-02-02 00:00:00.000000 wtfis-0.9.1/tests/test_data/vt_whois_gist.json
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/__init__.py
+-rw-r--r--   0        0        0     8239 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/main.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/types.py
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/utils.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/__init__.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/abuseipdb.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/base.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/greynoise.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/ip2whois.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/ipwhois.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/passivetotal.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/shodan.py
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/urlhaus.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/clients/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/handlers/__init__.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/handlers/base.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/handlers/domain.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/handlers/ip.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/__init__.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/abuseipdb.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/common.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/greynoise.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/ip2whois.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/ipwhois.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/passivetotal.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/shodan.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/urlhaus.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/models/virustotal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/ui/__init__.py
+-rw-r--r--   0        0        0    19526 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/ui/base.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/ui/progress.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/ui/theme.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wtfis-0.9.1/wtfis/ui/view.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 wtfis-0.9.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 wtfis-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10744 2020-02-02 00:00:00.000000 wtfis-0.9.1/README.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 wtfis-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11547 2020-02-02 00:00:00.000000 wtfis-0.9.1/PKG-INFO
```

### Comparing `wtfis-0.9.0/Dockerfile` & `wtfis-0.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/demo-old.gif` & `wtfis-0.9.1/imgs/demo-old.gif`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/demo.gif` & `wtfis-0.9.1/imgs/demo.gif`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-abuseipdb.png` & `wtfis-0.9.1/imgs/example-abuseipdb.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-greynoise.png` & `wtfis-0.9.1/imgs/example-greynoise.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-ip.png` & `wtfis-0.9.1/imgs/example-ip.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-no-color.png` & `wtfis-0.9.1/imgs/example-no-color.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-one-column.png` & `wtfis-0.9.1/imgs/example-one-column.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-shodan.png` & `wtfis-0.9.1/imgs/example-shodan.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/imgs/example-urlhaus.png` & `wtfis-0.9.1/imgs/example-urlhaus.png`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/conftest.py` & `wtfis-0.9.1/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,29 +15,35 @@
 class TestTheme:
     """ Expected theme values for the tests """
     panel_title = "bold yellow"
     heading_h1 = "bold bright_green on dark_green"
     heading_h2 = "bold yellow"
     table_field = "bold bright_magenta"
     table_value = "not bold default"
+    popularity_source = "bright_cyan"
+    inline_stat = "cyan"
+    vendor_list = "cyan"
     nameserver_list = "bright_blue"
-    timestamp_date = "not bold default"
-    timestamp_t = "dim bright_white"
-    timestamp_time = "dim default"
-    timestamp_z = "dim bright_white"
-    asn_org = "bright_white"
-    whois_org = "bright_cyan"
     disclaimer = "italic white on red"
     tags = "bright_white on black"
     tags_green = "bright_green on black"
     tags_red = "bright_red on black"
+    product = "orange_red1"
+    port = "bright_cyan"
+    transport = "cyan"
     footer = "cyan"
     info = "bold green"
     warn = "bold yellow"
     error = "bold red"
+    timestamp_date = "not bold default"
+    timestamp_t = "dim bright_white"
+    timestamp_time = "dim default"
+    timestamp_z = "dim bright_white"
+    asn_org = "bright_white"
+    whois_org = "bright_cyan"
     urlhaus_bl_name = "bright_cyan"
     urlhaus_bl_low = "bright_white on green"
     urlhaus_bl_med = "black on yellow"
     urlhaus_bl_high = "bright_white on red"
 
 
 def open_test_data(fname: str) -> str:
```

### Comparing `wtfis-0.9.0/tests/test_cli.py` & `wtfis-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_clients.py` & `wtfis-0.9.1/tests/test_clients.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_handlers.py` & `wtfis-0.9.1/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_models_vt.py` & `wtfis-0.9.1/tests/test_models_vt.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_ui_domain_view.py` & `wtfis-0.9.1/tests/test_ui_domain_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -334,15 +334,15 @@
             "Categories:",
             "Updated:",
             "Last Seen:",
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             Text("0"),
             Text(
                 "Majestic (532)\nCisco Umbrella (39463)",
                 spans=[
                     Span(0, 8, "bright_cyan"),
                     Span(10, 13, "cyan"),
                     Span(15, 29, "bright_cyan"),
@@ -403,15 +403,15 @@
             "ASN:",
             "ISP:",
             "Location:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2022-08-06T14:56:20Z"),
             Text(
                 "16509 (Amazon Data Services India)",
                 spans=[Span(7, 33, theme.asn_org)]
             ),
             "Amazon.com, Inc.",
             Text(
@@ -447,15 +447,15 @@
             "ASN:",
             "ISP:",
             "Location:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("1/94 malicious"),
+            Text("1/94 malicious", spans=[Span(0, 14, theme.error)]),
             display_timestamp("2022-06-21T18:10:54Z"),
             Text(
                 "36459 (GitHub, Inc.)",
                 spans=[Span(7, 19, theme.asn_org)]
             ),
             "GitHub, Inc.",
             Text(
@@ -494,15 +494,15 @@
             "ASN:",
             "ISP:",
             "Location:",
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2015-08-17T07:11:53Z"),
             Text(
                 "16509 (Amazon Data Services India)",
                 spans=[Span(7, 33, theme.asn_org)]
             ),
             "Amazon.com, Inc.",
             Text(
@@ -648,15 +648,15 @@
                 spans=[Span(0, 8, 'link https://virustotal.com/gui/ip-address/13.234.210.38')],
             ),
             "Resolved:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2022-08-06T14:56:20Z"),
         ]
 
         # Spacing and remaining count footer
         assert res.renderable.renderables[2] == ""
         assert str(footer) == "+36 more"
         assert footer.spans[0].style.startswith(f"{theme.footer} link https://virustotal.com/gui/domain/")
@@ -776,15 +776,15 @@
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "1/94 malicious\nCyble",
                 spans=[
-                    Span(15, 20, ""),
+                    Span(0, 14, theme.error),
                     Span(15, 20, "cyan"),
                 ]
             ),
             Text("448"),
             Text(
                 "Majestic (1)\nStatvoo (1)\nAlexa (1)\nCisco Umbrella (2)\nQuantcast (1)",
                 spans=[
@@ -856,15 +856,15 @@
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "1/94 malicious\nDr.Web",
                 spans=[
-                    Span(15, 21, ""),
+                    Span(0, 14, theme.error),
                     Span(15, 21, "cyan"),
                 ]
             ),
             Text("-1"),
             Text(
                 (
                     "ads/analytics, dynamic dns and isp sites, hosting, information technology, "
@@ -953,15 +953,15 @@
             ),
             "Tags:",
             "Last Scan:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2022-08-06T14:56:20Z"),
             Text(
                 "16509 (Amazon Data Services India)",
                 spans=[Span(7, 33, theme.asn_org)]
             ),
             "Amazon.com, Inc.",
             Text(
@@ -969,25 +969,22 @@
                 spans=[
                     Span(6, 8, "default"),
                 ]
             ),
             Text(
                 "22/tcp, 80/tcp, 443/tcp",
                 spans=[
-                    Span(0, 6, ""),
-                    Span(0, 2, "bright_cyan"),
-                    Span(2, 6, "cyan"),
+                    Span(0, 2, theme.port),
+                    Span(2, 6, theme.transport),
                     Span(6, 8, "default"),
-                    Span(8, 14, ""),
-                    Span(8, 10, "bright_cyan"),
-                    Span(10, 14, "cyan"),
+                    Span(8, 10, theme.port),
+                    Span(10, 14, theme.transport),
                     Span(14, 16, "default"),
-                    Span(16, 23, ""),
-                    Span(16, 19, "bright_cyan"),
-                    Span(19, 23, "cyan"),
+                    Span(16, 19, theme.port),
+                    Span(19, 23, theme.transport),
                 ]
             ),
             Text(
                 "cloud",
                 spans=[
                     Span(0, 5, 'bright_white on black')
                 ]
@@ -1024,15 +1021,15 @@
                 spans=[Span(0, 8, "link https://www.shodan.io/host/192.30.255.113")]
             ),
             "Last Scan:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("1/94 malicious"),
+            Text("1/94 malicious", spans=[Span(0, 14, theme.error)]),
             display_timestamp("2022-06-21T18:10:54Z"),
             Text(
                 "36459 (GitHub, Inc.)",
                 spans=[Span(7, 19, theme.asn_org)]
             ),
             "GitHub, Inc.",
             Text(
@@ -1040,25 +1037,22 @@
                 spans=[
                     Span(7, 9, "default"),
                 ]
             ),
             Text(
                 "22/tcp, 80/tcp, 443/tcp",
                 spans=[
-                    Span(0, 6, ""),
-                    Span(0, 2, "bright_cyan"),
-                    Span(2, 6, "cyan"),
+                    Span(0, 2, theme.port),
+                    Span(2, 6, theme.transport),
                     Span(6, 8, "default"),
-                    Span(8, 14, ""),
-                    Span(8, 10, "bright_cyan"),
-                    Span(10, 14, "cyan"),
+                    Span(8, 10, theme.port),
+                    Span(10, 14, theme.transport),
                     Span(14, 16, "default"),
-                    Span(16, 23, ""),
-                    Span(16, 19, "bright_cyan"),
-                    Span(19, 23, "cyan")
+                    Span(16, 19, theme.port),
+                    Span(19, 23, theme.transport)
                 ]
             ),
             display_timestamp("2022-08-21T22:33:53Z")
         ]
 
         # Spacing
         assert res.renderable.renderables[4] == ""
@@ -1093,15 +1087,15 @@
             ),
             "Tags:",
             "Last Scan:",
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2015-08-17T07:11:53Z"),
             Text(
                 "16509 (Amazon Data Services India)",
                 spans=[Span(7, 33, theme.asn_org)]
             ),
             "Amazon.com, Inc.",
             Text(
@@ -1109,25 +1103,22 @@
                 spans=[
                     Span(6, 8, "default"),
                 ]
             ),
             Text(
                 "22/tcp, 80/tcp, 443/tcp",
                 spans=[
-                    Span(0, 6, ""),
-                    Span(0, 2, "bright_cyan"),
-                    Span(2, 6, "cyan"),
+                    Span(0, 2, theme.port),
+                    Span(2, 6, theme.transport),
                     Span(6, 8, "default"),
-                    Span(8, 14, ""),
-                    Span(8, 10, "bright_cyan"),
-                    Span(10, 14, "cyan"),
+                    Span(8, 10, theme.port),
+                    Span(10, 14, theme.transport),
                     Span(14, 16, "default"),
-                    Span(16, 23, ""),
-                    Span(16, 19, "bright_cyan"),
-                    Span(19, 23, "cyan"),
+                    Span(16, 19, theme.port),
+                    Span(19, 23, theme.transport),
                 ]
             ),
             Text(
                 "cloud",
                 spans=[
                     Span(0, 5, 'bright_white on black')
                 ]
@@ -1185,15 +1176,15 @@
             ),
             "Tags:",
             "Last Scan:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("0/93 malicious"),
+            Text("0/93 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2022-06-03T22:32:19Z"),
             Text(
                 "54113 (Fastly, Inc.)",
                 spans=[Span(7, 19, theme.asn_org)]
             ),
             "Fastly, Inc.",
             Text(
@@ -1201,24 +1192,20 @@
                 spans=[
                     Span(7, 9, "default"),
                 ]
             ),
             Text(
                 "Varnish HTTP Cache (80/tcp)\nOther (443/tcp)",
                 spans=[
-                    Span(0, 18, "orange_red1"),
-                    Span(20, 26, ""),
-                    Span(20, 26, ""),
-                    Span(20, 22, "bright_cyan"),
-                    Span(22, 26, "cyan"),
-                    Span(28, 33, "orange_red1"),
-                    Span(35, 42, ""),
-                    Span(35, 42, ""),
-                    Span(35, 38, "bright_cyan"),
-                    Span(38, 42, "cyan"),
+                    Span(0, 18, theme.product),
+                    Span(20, 22, theme.port),
+                    Span(22, 26, theme.transport),
+                    Span(28, 33, theme.product),
+                    Span(35, 38, theme.port),
+                    Span(38, 42, theme.transport),
                 ]
             ),
             Text(
                 "cdn",
                 spans=[
                     Span(0, 3, 'bright_white on black'),
                 ]
@@ -1284,15 +1271,15 @@
                 "AbuseIPDB:",
                 spans=[Span(0, 9, "link https://www.abuseipdb.com/check/1.0.0.1")]
             ),
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
-            Text("2/94 malicious"),
+            Text("2/94 malicious", spans=[Span(0, 14, theme.error)]),
             display_timestamp("2020-08-01T22:07:20Z"),
             Text(
                 "13335 (APNIC and Cloudflare DNS Resolver project)",
                 spans=[Span(7, 48, theme.asn_org)],
             ),
             "Cloudflare, Inc.",
             Text(
@@ -1303,52 +1290,41 @@
             ),
             Text(
                 (
                     "CloudFlare (80/tcp, 8080/tcp)\nOther (53/tcp, 53/udp, 443/tcp, 2082/tcp, "
                     "2086/tcp, 2087/tcp, 8443/tcp)"
                 ),
                 spans=[
-                    Span(0, 10, "orange_red1"),
-                    Span(12, 28, ""),
-                    Span(12, 18, ""),
-                    Span(12, 14, "bright_cyan"),
-                    Span(14, 18, "cyan"),
+                    Span(0, 10, theme.product),
+                    Span(12, 14, theme.port),
+                    Span(14, 18, theme.transport),
                     Span(18, 20, "default"),
-                    Span(20, 28, ""),
-                    Span(20, 24, "bright_cyan"),
-                    Span(24, 28, "cyan"),
-                    Span(30, 35, "orange_red1"),
-                    Span(37, 100, ""),
-                    Span(37, 43, ""),
-                    Span(37, 39, "bright_cyan"),
-                    Span(39, 43, "cyan"),
+                    Span(20, 24, theme.port),
+                    Span(24, 28, theme.transport),
+                    Span(30, 35, theme.product),
+                    Span(37, 39, theme.port),
+                    Span(39, 43, theme.transport),
                     Span(43, 45, "default"),
-                    Span(45, 51, ""),
-                    Span(45, 47, "bright_cyan"),
-                    Span(47, 51, "cyan"),
+                    Span(45, 47, theme.port),
+                    Span(47, 51, theme.transport),
                     Span(51, 53, "default"),
-                    Span(53, 60, ""),
-                    Span(53, 56, "bright_cyan"),
-                    Span(56, 60, "cyan"),
+                    Span(53, 56, theme.port),
+                    Span(56, 60, theme.transport),
                     Span(60, 62, "default"),
-                    Span(62, 70, ""),
-                    Span(62, 66, "bright_cyan"),
-                    Span(66, 70, "cyan"),
+                    Span(62, 66, theme.port),
+                    Span(66, 70, theme.transport),
                     Span(70, 72, "default"),
-                    Span(72, 80, ""),
-                    Span(72, 76, "bright_cyan"),
-                    Span(76, 80, "cyan"),
+                    Span(72, 76, theme.port),
+                    Span(76, 80, theme.transport),
                     Span(80, 82, "default"),
-                    Span(82, 90, ""),
-                    Span(82, 86, "bright_cyan"),
-                    Span(86, 90, "cyan"),
+                    Span(82, 86, theme.port),
+                    Span(86, 90, theme.transport),
                     Span(90, 92, "default"),
-                    Span(92, 100, ""),
-                    Span(92, 96, "bright_cyan"),
-                    Span(96, 100, "cyan"),
+                    Span(92, 96, theme.port),
+                    Span(96, 100, theme.transport),
                 ]
             ),
             display_timestamp("2022-08-22T02:35:34Z"),
             Text(
                 "✓ riot  ✗ noise  ✓ benign",
                 spans=[
                     Span(0, 1, theme.info),
@@ -1435,15 +1411,15 @@
             "Location:",
             "Tags:",
             "Last Scan:",
         ]
         assert group[1].columns[1].style == theme.table_value
         assert group[1].columns[1].justify == "left"
         assert group[1].columns[1]._cells == [
-            Text("0/94 malicious"),
+            Text("0/94 malicious", spans=[Span(0, 14, theme.info)]),
             display_timestamp("2022-08-06T14:56:20Z"),
             Text(
                 "16509 (Amazon Data Services India)",
                 spans=[Span(7, 33, theme.asn_org)]
             ),
             "Amazon.com, Inc.",
             Text(
@@ -1451,15 +1427,15 @@
                 spans=[
                     Span(6, 8, "default"),
                 ]
             ),
             Text(
                 "cloud",
                 spans=[
-                    Span(0, 5, 'bright_white on black')
+                    Span(0, 5, theme.tags)
                 ]
             ),
             display_timestamp("2022-08-21T07:21:05Z")
         ]
 
 
 class TestView12:
@@ -1591,15 +1567,14 @@
                 ],
             ),
             Text(
                 "abused_legit_malware in spamhaus\nlisted in surbl",
                 spans=[
                     Span(0, 20, theme.urlhaus_bl_med),
                     Span(24, 32, theme.urlhaus_bl_name),
-                    Span(33, 48, ""),
                     Span(33, 39, theme.urlhaus_bl_high),
                     Span(43, 48, theme.urlhaus_bl_name),
                 ]
             ),
             Text(
                 "Pikabot, TA577, foo, zip",
                 spans=[
```

### Comparing `wtfis-0.9.0/tests/test_ui_ip_view.py` & `wtfis-0.9.1/tests/test_ui_ip_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,22 +236,22 @@
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "4/94 malicious\nCMC Threat Intelligence, Comodo Valkyrie Verdict, CRDF, Blueliv",
                 spans=[
-                    Span(15, 78, ''),
-                    Span(15, 38, 'cyan'),
-                    Span(38, 40, 'default'),
-                    Span(40, 63, 'cyan'),
-                    Span(63, 65, 'default'),
-                    Span(65, 69, 'cyan'),
-                    Span(69, 71, 'default'),
-                    Span(71, 78, 'cyan'),
+                    Span(0,  14, theme.error),
+                    Span(15, 38, theme.vendor_list),
+                    Span(38, 40, "default"),
+                    Span(40, 63, theme.vendor_list),
+                    Span(63, 65, "default"),
+                    Span(65, 69, theme.vendor_list),
+                    Span(69, 71, "default"),
+                    Span(71, 78, theme.vendor_list),
                 ]
             ),
             Text("134"),
             display_timestamp("2022-09-03T06:47:04Z"),
         ]
 
         #
@@ -322,15 +322,14 @@
                 ]
             ),
             Text(
                 "not listed in spamhaus\nnot listed in surbl",
                 spans=[
                     Span(0, 10, theme.urlhaus_bl_low),
                     Span(14, 22, theme.urlhaus_bl_name),
-                    Span(23, 42, ""),
                     Span(23, 33, theme.urlhaus_bl_low),
                     Span(37, 42, theme.urlhaus_bl_name),
                 ]
             ),
             Text(
                 "elf, mirai",
                 spans=[
@@ -484,22 +483,22 @@
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
             Text(
                 "4/94 malicious\nCMC Threat Intelligence, Comodo Valkyrie Verdict, CRDF, Blueliv",
                 spans=[
-                    Span(15, 78, ''),
-                    Span(15, 38, 'cyan'),
-                    Span(38, 40, 'default'),
-                    Span(40, 63, 'cyan'),
-                    Span(63, 65, 'default'),
-                    Span(65, 69, 'cyan'),
-                    Span(69, 71, 'default'),
-                    Span(71, 78, 'cyan'),
+                    Span(0, 14, theme.error),
+                    Span(15, 38, theme.vendor_list),
+                    Span(38, 40, "default"),
+                    Span(40, 63, theme.vendor_list),
+                    Span(63, 65, "default"),
+                    Span(65, 69, theme.vendor_list),
+                    Span(69, 71, "default"),
+                    Span(71, 78, theme.vendor_list),
                 ]
             ),
             Text("134"),
             display_timestamp("2022-09-03T06:47:04Z"),
         ]
 
         #
@@ -540,70 +539,53 @@
             Text(
                 (
                     "Cisco router tftpd (69/udp)\nCloudFlare (80/tcp, 8080/tcp, 8880/tcp)\n"
                     "DrayTek Vigor Router (443/tcp)\nOther (53/tcp, 53/udp, 161/udp, "
                     "2082/tcp, 2083/tcp, 2086/tcp, 2087/tcp, 8443/tcp)"
                 ),
                 spans=[
-                    Span(0, 18, "orange_red1"),
-                    Span(20, 26, ""),
-                    Span(20, 26, ""),
-                    Span(20, 22, "bright_cyan"),
-                    Span(22, 26, "cyan"),
-                    Span(28, 38, "orange_red1"),
-                    Span(40, 66, ""),
-                    Span(40, 46, ""),
-                    Span(40, 42, "bright_cyan"),
-                    Span(42, 46, "cyan"),
+                    Span(0, 18, theme.product),
+                    Span(20, 22, theme.port),
+                    Span(22, 26, theme.transport),
+                    Span(28, 38, theme.product),
+                    Span(40, 42, theme.port),
+                    Span(42, 46, theme.transport),
                     Span(46, 48, "default"),
-                    Span(48, 56, ""),
-                    Span(48, 52, "bright_cyan"),
-                    Span(52, 56, "cyan"),
+                    Span(48, 52, theme.port),
+                    Span(52, 56, theme.transport),
                     Span(56, 58, "default"),
-                    Span(58, 66, ""),
-                    Span(58, 62, "bright_cyan"),
-                    Span(62, 66, "cyan"),
-                    Span(68, 88, "orange_red1"),
-                    Span(90, 97, ""),
-                    Span(90, 97, ""),
-                    Span(90, 93, "bright_cyan"),
-                    Span(93, 97, "cyan"),
-                    Span(99, 104, "orange_red1"),
-                    Span(106, 179, ""),
-                    Span(106, 112, ""),
-                    Span(106, 108, "bright_cyan"),
-                    Span(108, 112, "cyan"),
+                    Span(58, 62, theme.port),
+                    Span(62, 66, theme.transport),
+                    Span(68, 88, theme.product),
+                    Span(90, 93, theme.port),
+                    Span(93, 97, theme.transport),
+                    Span(99, 104, theme.product),
+                    Span(106, 108, theme.port),
+                    Span(108, 112, theme.transport),
                     Span(112, 114, "default"),
-                    Span(114, 120, ""),
-                    Span(114, 116, "bright_cyan"),
-                    Span(116, 120, "cyan"),
+                    Span(114, 116, theme.port),
+                    Span(116, 120, theme.transport),
                     Span(120, 122, "default"),
-                    Span(122, 129, ""),
-                    Span(122, 125, "bright_cyan"),
-                    Span(125, 129, "cyan"),
+                    Span(122, 125, theme.port),
+                    Span(125, 129, theme.transport),
                     Span(129, 131, "default"),
-                    Span(131, 139, ""),
-                    Span(131, 135, "bright_cyan"),
-                    Span(135, 139, "cyan"),
+                    Span(131, 135, theme.port),
+                    Span(135, 139, theme.transport),
                     Span(139, 141, "default"),
-                    Span(141, 149, ""),
-                    Span(141, 145, "bright_cyan"),
-                    Span(145, 149, "cyan"),
+                    Span(141, 145, theme.port),
+                    Span(145, 149, theme.transport),
                     Span(149, 151, "default"),
-                    Span(151, 159, ""),
-                    Span(151, 155, "bright_cyan"),
-                    Span(155, 159, "cyan"),
+                    Span(151, 155, theme.port),
+                    Span(155, 159, theme.transport),
                     Span(159, 161, "default"),
-                    Span(161, 169, ""),
-                    Span(161, 165, "bright_cyan"),
-                    Span(165, 169, "cyan"),
+                    Span(161, 165, theme.port),
+                    Span(165, 169, theme.transport),
                     Span(169, 171, "default"),
-                    Span(171, 179, ""),
-                    Span(171, 175, "bright_cyan"),
-                    Span(175, 179, "cyan"),
+                    Span(171, 175, theme.port),
+                    Span(175, 179, theme.transport),
                 ]
             ),
             display_timestamp("2022-09-04T01:03:56Z"),
         ]
 
         #
         # Other section
@@ -743,15 +725,15 @@
             ),
             "Reputation:",
             "Updated:",
         ]
         assert table.columns[1].style == theme.table_value
         assert table.columns[1].justify == "left"
         assert table.columns[1]._cells == [
-            Text("0/93 malicious"),
+            Text("0/93 malicious", spans=[Span(0, 14, theme.info)]),
             Text("0"),
             display_timestamp("2022-09-03T16:58:45Z"),
         ]
 
 
 class TestView05:
     def test_ip_panel_greynoise_only(self, view05, theme):
```

### Comparing `wtfis-0.9.0/tests/test_utils.py` & `wtfis-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/ip2whois_whois_bbc.json` & `wtfis-0.9.1/tests/test_data/ip2whois_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/ip2whois_whois_hotmail.json` & `wtfis-0.9.1/tests/test_data/ip2whois_whois_hotmail.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/ipwhois_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/ipwhois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/ipwhois_gist.json` & `wtfis-0.9.1/tests/test_data/ipwhois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/pt_passive_dns_gist.json` & `wtfis-0.9.1/tests/test_data/pt_passive_dns_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/pt_whois_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/pt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/pt_whois_gist.json` & `wtfis-0.9.1/tests/test_data/pt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/shodan_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/shodan_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/shodan_gist.json` & `wtfis-0.9.1/tests/test_data/shodan_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/shodan_gist_2.json` & `wtfis-0.9.1/tests/test_data/shodan_gist_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/shodan_one.json` & `wtfis-0.9.1/tests/test_data/shodan_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/shodan_wired.json` & `wtfis-0.9.1/tests/test_data/shodan_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/urlhaus_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/urlhaus_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/urlhaus_gist.json` & `wtfis-0.9.1/tests/test_data/urlhaus_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_domain_gist.json` & `wtfis-0.9.1/tests/test_data/vt_domain_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_domain_google.json` & `wtfis-0.9.1/tests/test_data/vt_domain_google.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_domain_tucows.json` & `wtfis-0.9.1/tests/test_data/vt_domain_tucows.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_ip_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/vt_ip_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_ip_142.251.220.110.json` & `wtfis-0.9.1/tests/test_data/vt_ip_142.251.220.110.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_resolutions_gist.json` & `wtfis-0.9.1/tests/test_data/vt_resolutions_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_resolutions_one.json` & `wtfis-0.9.1/tests/test_data/vt_resolutions_one.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_resolutions_wired.json` & `wtfis-0.9.1/tests/test_data/vt_resolutions_wired.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_whois_1.1.1.1.json` & `wtfis-0.9.1/tests/test_data/vt_whois_1.1.1.1.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_whois_bbc.json` & `wtfis-0.9.1/tests/test_data/vt_whois_bbc.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_whois_example.json` & `wtfis-0.9.1/tests/test_data/vt_whois_example.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_whois_example_2.json` & `wtfis-0.9.1/tests/test_data/vt_whois_example_2.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/tests/test_data/vt_whois_gist.json` & `wtfis-0.9.1/tests/test_data/vt_whois_gist.json`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/main.py` & `wtfis-0.9.1/wtfis/main.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/utils.py` & `wtfis-0.9.1/wtfis/utils.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/abuseipdb.py` & `wtfis-0.9.1/wtfis/clients/abuseipdb.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/base.py` & `wtfis-0.9.1/wtfis/clients/base.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/greynoise.py` & `wtfis-0.9.1/wtfis/clients/greynoise.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/ip2whois.py` & `wtfis-0.9.1/wtfis/clients/ip2whois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/ipwhois.py` & `wtfis-0.9.1/wtfis/clients/ipwhois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/passivetotal.py` & `wtfis-0.9.1/wtfis/clients/passivetotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/shodan.py` & `wtfis-0.9.1/wtfis/clients/shodan.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/urlhaus.py` & `wtfis-0.9.1/wtfis/clients/urlhaus.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/clients/virustotal.py` & `wtfis-0.9.1/wtfis/clients/virustotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/handlers/base.py` & `wtfis-0.9.1/wtfis/handlers/base.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/handlers/domain.py` & `wtfis-0.9.1/wtfis/handlers/domain.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/handlers/ip.py` & `wtfis-0.9.1/wtfis/handlers/ip.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/abuseipdb.py` & `wtfis-0.9.1/wtfis/models/abuseipdb.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/common.py` & `wtfis-0.9.1/wtfis/models/common.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/ip2whois.py` & `wtfis-0.9.1/wtfis/models/ip2whois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/ipwhois.py` & `wtfis-0.9.1/wtfis/models/ipwhois.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/passivetotal.py` & `wtfis-0.9.1/wtfis/models/passivetotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/shodan.py` & `wtfis-0.9.1/wtfis/models/shodan.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/urlhaus.py` & `wtfis-0.9.1/wtfis/models/urlhaus.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/models/virustotal.py` & `wtfis-0.9.1/wtfis/models/virustotal.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/ui/base.py` & `wtfis-0.9.1/wtfis/ui/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,16 @@
         # Custom style
         stats_style = self.theme.error if stats.malicious >= 1 else self.theme.info
 
         # Total count
         total = stats.harmless + stats.malicious + stats.suspicious + stats.timeout + stats.undetected
 
         # Text
-        text = Text(f"{stats.malicious}/{total} malicious", style=stats_style)
+        text = Text()
+        text.append(Text(f"{stats.malicious}/{total} malicious", style=stats_style))
 
         # Include list of vendors that flagged malicious
         if vendors:
             text.append("\n")
             text.append(smart_join(*vendors, style=self.theme.vendor_list))
 
         return text
```

### Comparing `wtfis-0.9.0/wtfis/ui/theme.py` & `wtfis-0.9.1/wtfis/ui/theme.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/wtfis/ui/view.py` & `wtfis-0.9.1/wtfis/ui/view.py`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/.gitignore` & `wtfis-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/LICENSE` & `wtfis-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/README.md` & `wtfis-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `wtfis-0.9.0/pyproject.toml` & `wtfis-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,19 +25,19 @@
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Topic :: Security",
 ]
 dependencies = [
-    "pydantic~=2.0.3",
-    "python-dotenv~=1.0.0",
+    "pydantic~=2.7.0",
+    "python-dotenv~=1.0.1",
     "requests~=2.31.0",
-    "rich~=13.4.2",
-    "shodan~=1.29.1",
+    "rich~=13.7.1",
+    "shodan~=1.31.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/pirxthepilot/wtfis"
 
 [project.scripts]
@@ -56,15 +56,15 @@
 [tool.hatch.publish.index]
 disable = true
 
 # Hatch default env
 [tool.hatch.envs.default]
 dependencies = [
     "bandit",
-    "flake8>=6.0.0",
+    "flake8>=7.0.0",
     "freezegun",
     "mypy",
     "pytest",
     "pytest-cov",
     "types-requests~=2.31.0",
 ]
 [tool.hatch.envs.default.scripts]
@@ -74,15 +74,15 @@
 test-all = [
     "typecheck",
     "test-cov",
 ]
 
 # Hatch test env
 [[tool.hatch.envs.test.matrix]]
-python = ["38", "39", "310", "311"]
+python = ["38", "39", "310", "311", "312"]
 
 # Hatch lint env
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [  # Make sure the respective versions are synced with default!
     "bandit",
     "flake8>=6.0.0",
```

### Comparing `wtfis-0.9.0/PKG-INFO` & `wtfis-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.3
 Name: wtfis
-Version: 0.9.0
+Version: 0.9.1
 Summary: Passive hostname, domain and IP lookup tool for non-robots
 Project-URL: Homepage, https://github.com/pirxthepilot/wtfis
 Author-email: pirxthepilot <pirxthepilot@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ipinfo,osint,passive lookup,passivetotal,security,shodan,virustotal,whois
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Python: >=3.8
-Requires-Dist: pydantic~=2.0.3
-Requires-Dist: python-dotenv~=1.0.0
+Requires-Dist: pydantic~=2.7.0
+Requires-Dist: python-dotenv~=1.0.1
 Requires-Dist: requests~=2.31.0
-Requires-Dist: rich~=13.4.2
-Requires-Dist: shodan~=1.29.1
+Requires-Dist: rich~=13.7.1
+Requires-Dist: shodan~=1.31.0
 Description-Content-Type: text/markdown
 
 # wtfis
 
 [![Tests](https://github.com/pirxthepilot/wtfis/actions/workflows/tests.yml/badge.svg)](https://github.com/pirxthepilot/wtfis/actions/workflows/tests.yml)
 [![PyPI](https://img.shields.io/pypi/v/wtfis?color=blue&logo=pypi&logoColor=gold)](https://pypi.org/project/wtfis/)
```

