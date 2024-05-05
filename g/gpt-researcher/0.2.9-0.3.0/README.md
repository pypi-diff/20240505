# Comparing `tmp/gpt-researcher-0.2.9.tar.gz` & `tmp/gpt-researcher-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-researcher-0.2.9.tar", last modified: Thu Apr 25 09:21:51 2024, max compression
+gzip compressed data, was "gpt-researcher-0.3.0.tar", last modified: Sun May  5 07:06:29 2024, max compression
```

## Comparing `gpt-researcher-0.2.9.tar` & `gpt-researcher-0.3.0.tar`

### file list

```diff
@@ -1,119 +1,103 @@
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.918215 gpt-researcher-0.2.9/
--rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/LICENSE
--rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 09:21:51.917205 gpt-researcher-0.2.9/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     9295 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/README.md
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.851778 gpt-researcher-0.2.9/backend/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.852675 gpt-researcher-0.2.9/backend/report_type/
--rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/report_type/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.853976 gpt-researcher-0.2.9/backend/report_type/basic_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/report_type/basic_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/report_type/basic_report/basic_report.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.855232 gpt-researcher-0.2.9/backend/report_type/detailed_report/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/report_type/detailed_report/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/report_type/detailed_report/detailed_report.py
--rw-r--r--   0 assafel    (501) staff       (20)     2130 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/server.py
--rw-r--r--   0 assafel    (501) staff       (20)     2396 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/backend/websocket_manager.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.856291 gpt-researcher-0.2.9/gpt_researcher/
--rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.2.9/gpt_researcher/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.861101 gpt-researcher-0.2.9/gpt_researcher/config/
--rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.2.9/gpt_researcher/config/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/config/config.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.863940 gpt-researcher-0.2.9/gpt_researcher/context/
--rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.2.9/gpt_researcher/context/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/context/compression.py
--rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.2.9/gpt_researcher/context/retriever.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.864854 gpt-researcher-0.2.9/gpt_researcher/llm_provider/
--rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.866251 gpt-researcher-0.2.9/gpt_researcher/llm_provider/azureopenai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/azureopenai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/azureopenai/azureopenai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.867555 gpt-researcher-0.2.9/gpt_researcher/llm_provider/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.868733 gpt-researcher-0.2.9/gpt_researcher/llm_provider/openai/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/openai/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/llm_provider/openai/openai.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.872174 gpt-researcher-0.2.9/gpt_researcher/master/
--rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.2.9/gpt_researcher/master/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     8909 2024-04-25 07:55:48.000000 gpt-researcher-0.2.9/gpt_researcher/master/agent.py
--rw-r--r--   0 assafel    (501) staff       (20)    12199 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/master/functions.py
--rw-r--r--   0 assafel    (501) staff       (20)    13310 2024-04-25 09:21:17.000000 gpt-researcher-0.2.9/gpt_researcher/master/prompts.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.873695 gpt-researcher-0.2.9/gpt_researcher/memory/
--rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.2.9/gpt_researcher/memory/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/memory/embeddings.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.874529 gpt-researcher-0.2.9/gpt_researcher/retrievers/
--rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.875903 gpt-researcher-0.2.9/gpt_researcher/retrievers/bing/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/bing/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/bing/bing.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.877307 gpt-researcher-0.2.9/gpt_researcher/retrievers/duckduckgo/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/duckduckgo/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.878731 gpt-researcher-0.2.9/gpt_researcher/retrievers/google/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/google/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/google/google.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.880620 gpt-researcher-0.2.9/gpt_researcher/retrievers/searx/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/searx/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/searx/searx.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.882065 gpt-researcher-0.2.9/gpt_researcher/retrievers/serpapi/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/serpapi/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/serpapi/serpapi.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.883713 gpt-researcher-0.2.9/gpt_researcher/retrievers/serper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/serper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/serper/serper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.885819 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_news/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_news/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_news/tavily_news.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.887796 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_search/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_search/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_search/tavily_search.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.890482 gpt-researcher-0.2.9/gpt_researcher/scraper/
--rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.891881 gpt-researcher-0.2.9/gpt_researcher/scraper/arxiv/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/arxiv/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/arxiv/arxiv.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.893290 gpt-researcher-0.2.9/gpt_researcher/scraper/beautiful_soup/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/beautiful_soup/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.894802 gpt-researcher-0.2.9/gpt_researcher/scraper/newspaper/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/newspaper/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/newspaper/newspaper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.896103 gpt-researcher-0.2.9/gpt_researcher/scraper/pymupdf/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/pymupdf/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/pymupdf/pymupdf.py
--rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/scraper.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.897713 gpt-researcher-0.2.9/gpt_researcher/scraper/web_base_loader/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/web_base_loader/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.2.9/gpt_researcher/scraper/web_base_loader/web_base_loader.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.901289 gpt-researcher-0.2.9/gpt_researcher/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.2.9/gpt_researcher/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/utils/enum.py
--rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/utils/llm.py
--rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/gpt_researcher/utils/validators.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.859536 gpt-researcher-0.2.9/gpt_researcher.egg-info/
--rw-r--r--   0 assafel    (501) staff       (20)    10018 2024-04-25 09:21:51.000000 gpt-researcher-0.2.9/gpt_researcher.egg-info/PKG-INFO
--rw-r--r--   0 assafel    (501) staff       (20)     3134 2024-04-25 09:21:51.000000 gpt-researcher-0.2.9/gpt_researcher.egg-info/SOURCES.txt
--rw-r--r--   0 assafel    (501) staff       (20)        1 2024-04-25 09:21:51.000000 gpt-researcher-0.2.9/gpt_researcher.egg-info/dependency_links.txt
--rw-r--r--   0 assafel    (501) staff       (20)      331 2024-04-25 09:21:51.000000 gpt-researcher-0.2.9/gpt_researcher.egg-info/requires.txt
--rw-r--r--   0 assafel    (501) staff       (20)       36 2024-04-25 09:21:51.000000 gpt-researcher-0.2.9/gpt_researcher.egg-info/top_level.txt
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.902702 gpt-researcher-0.2.9/multi_agents/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:48:05.000000 gpt-researcher-0.2.9/multi_agents/__init__.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.914258 gpt-researcher-0.2.9/multi_agents/agents/
--rw-r--r--   0 assafel    (501) staff       (20)      396 2024-04-24 07:58:50.000000 gpt-researcher-0.2.9/multi_agents/agents/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     1727 2024-03-19 10:01:22.000000 gpt-researcher-0.2.9/multi_agents/agents/critique.py
--rw-r--r--   0 assafel    (501) staff       (20)     1666 2024-03-19 10:01:22.000000 gpt-researcher-0.2.9/multi_agents/agents/curator.py
--rw-r--r--   0 assafel    (501) staff       (20)     2351 2024-04-24 15:50:47.000000 gpt-researcher-0.2.9/multi_agents/agents/editor.py
--rw-r--r--   0 assafel    (501) staff       (20)     2482 2024-04-25 07:27:33.000000 gpt-researcher-0.2.9/multi_agents/agents/master.py
--rw-r--r--   0 assafel    (501) staff       (20)     1082 2024-04-25 08:05:29.000000 gpt-researcher-0.2.9/multi_agents/agents/publisher.py
--rw-r--r--   0 assafel    (501) staff       (20)     2477 2024-04-25 07:44:43.000000 gpt-researcher-0.2.9/multi_agents/agents/researcher.py
--rw-r--r--   0 assafel    (501) staff       (20)      361 2024-04-22 12:37:36.000000 gpt-researcher-0.2.9/multi_agents/agents/reviser.py
-drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-04-25 09:21:51.916120 gpt-researcher-0.2.9/multi_agents/agents/utils/
--rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-25 07:20:14.000000 gpt-researcher-0.2.9/multi_agents/agents/utils/__init__.py
--rw-r--r--   0 assafel    (501) staff       (20)     2410 2024-04-25 07:24:00.000000 gpt-researcher-0.2.9/multi_agents/agents/utils/file_utils.py
--rw-r--r--   0 assafel    (501) staff       (20)     2693 2024-04-25 08:06:44.000000 gpt-researcher-0.2.9/multi_agents/agents/writer.py
--rw-r--r--   0 assafel    (501) staff       (20)      366 2024-04-25 08:55:58.000000 gpt-researcher-0.2.9/multi_agents/main.py
--rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-22 11:21:41.000000 gpt-researcher-0.2.9/pyproject.toml
--rw-r--r--   0 assafel    (501) staff       (20)       38 2024-04-25 09:21:51.918451 gpt-researcher-0.2.9/setup.cfg
--rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-04-25 09:21:45.000000 gpt-researcher-0.2.9/setup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.857440 gpt-researcher-0.3.0/
+-rw-r--r--   0 assafel    (501) staff       (20)     1069 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/LICENSE
+-rw-r--r--   0 assafel    (501) staff       (20)    10552 2024-05-05 07:06:29.856570 gpt-researcher-0.3.0/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     9829 2024-05-01 07:22:17.000000 gpt-researcher-0.3.0/README.md
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.788803 gpt-researcher-0.3.0/backend/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.789859 gpt-researcher-0.3.0/backend/report_type/
+-rw-r--r--   0 assafel    (501) staff       (20)      165 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.791400 gpt-researcher-0.3.0/backend/report_type/basic_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/basic_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      777 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/basic_report/basic_report.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.793029 gpt-researcher-0.3.0/backend/report_type/detailed_report/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/detailed_report/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     6012 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/report_type/detailed_report/detailed_report.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2327 2024-04-30 14:44:06.000000 gpt-researcher-0.3.0/backend/server.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2689 2024-04-30 14:43:31.000000 gpt-researcher-0.3.0/backend/utils.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2822 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/backend/websocket_manager.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.794044 gpt-researcher-0.3.0/gpt_researcher/
+-rw-r--r--   0 assafel    (501) staff       (20)      100 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.799909 gpt-researcher-0.3.0/gpt_researcher/config/
+-rw-r--r--   0 assafel    (501) staff       (20)       48 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/config/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2094 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/config/config.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.804047 gpt-researcher-0.3.0/gpt_researcher/context/
+-rw-r--r--   0 assafel    (501) staff       (20)      140 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/context/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1812 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/context/compression.py
+-rw-r--r--   0 assafel    (501) staff       (20)      801 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/context/retriever.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.805315 gpt-researcher-0.3.0/gpt_researcher/llm_provider/
+-rw-r--r--   0 assafel    (501) staff       (20)      226 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.807450 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3068 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.809572 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3670 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.811729 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2091 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/openai.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.816261 gpt-researcher-0.3.0/gpt_researcher/master/
+-rw-r--r--   0 assafel    (501) staff       (20)       61 2023-11-13 18:29:19.000000 gpt-researcher-0.3.0/gpt_researcher/master/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     8928 2024-05-05 07:01:28.000000 gpt-researcher-0.3.0/gpt_researcher/master/agent.py
+-rw-r--r--   0 assafel    (501) staff       (20)    12476 2024-05-05 07:01:28.000000 gpt-researcher-0.3.0/gpt_researcher/master/functions.py
+-rw-r--r--   0 assafel    (501) staff       (20)    13399 2024-05-05 06:59:59.000000 gpt-researcher-0.3.0/gpt_researcher/master/prompts.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.818637 gpt-researcher-0.3.0/gpt_researcher/memory/
+-rw-r--r--   0 assafel    (501) staff       (20)       31 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/memory/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1047 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/memory/embeddings.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.819959 gpt-researcher-0.3.0/gpt_researcher/retrievers/
+-rw-r--r--   0 assafel    (501) staff       (20)      510 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.821473 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-08 11:24:31.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2240 2023-12-08 11:24:31.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/bing.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.823144 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      479 2024-04-12 11:24:29.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/duckduckgo/duckduckgo.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.825330 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2535 2023-11-19 07:01:11.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/google/google.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.827634 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1294 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/searx.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.829744 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2232 2023-11-25 13:46:26.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/serpapi.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.831965 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     2117 2023-11-25 13:46:26.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/serper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.834300 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1281 2023-12-18 08:18:37.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/tavily_news.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.836685 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1506 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/tavily_search.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.839407 gpt-researcher-0.3.0/gpt_researcher/scraper/
+-rw-r--r--   0 assafel    (501) staff       (20)      398 2024-03-17 08:29:46.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/__init__.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.841497 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      762 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/arxiv.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.843839 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1992 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.846041 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1312 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/newspaper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.848111 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      640 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/pymupdf.py
+-rw-r--r--   0 assafel    (501) staff       (20)     3111 2024-03-17 08:29:46.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/scraper.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.850280 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)     1074 2024-03-12 13:09:58.000000 gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.855037 gpt-researcher-0.3.0/gpt_researcher/utils/
+-rw-r--r--   0 assafel    (501) staff       (20)        0 2023-11-28 09:06:52.000000 gpt-researcher-0.3.0/gpt_researcher/utils/__init__.py
+-rw-r--r--   0 assafel    (501) staff       (20)      274 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/enum.py
+-rw-r--r--   0 assafel    (501) staff       (20)     5108 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/llm.py
+-rw-r--r--   0 assafel    (501) staff       (20)      216 2024-04-22 11:21:41.000000 gpt-researcher-0.3.0/gpt_researcher/utils/validators.py
+drwxr-xr-x   0 assafel    (501) staff       (20)        0 2024-05-05 07:06:29.798035 gpt-researcher-0.3.0/gpt_researcher.egg-info/
+-rw-r--r--   0 assafel    (501) staff       (20)    10552 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/PKG-INFO
+-rw-r--r--   0 assafel    (501) staff       (20)     2727 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/SOURCES.txt
+-rw-r--r--   0 assafel    (501) staff       (20)        1 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/dependency_links.txt
+-rw-r--r--   0 assafel    (501) staff       (20)      342 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/requires.txt
+-rw-r--r--   0 assafel    (501) staff       (20)       23 2024-05-05 07:06:29.000000 gpt-researcher-0.3.0/gpt_researcher.egg-info/top_level.txt
+-rw-r--r--   0 assafel    (501) staff       (20)     1156 2024-04-27 17:11:32.000000 gpt-researcher-0.3.0/pyproject.toml
+-rw-r--r--   0 assafel    (501) staff       (20)       38 2024-05-05 07:06:29.857689 gpt-researcher-0.3.0/setup.cfg
+-rw-r--r--   0 assafel    (501) staff       (20)     1176 2024-05-05 07:05:54.000000 gpt-researcher-0.3.0/setup.py
```

### Comparing `gpt-researcher-0.2.9/LICENSE` & `gpt-researcher-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/PKG-INFO` & `gpt-researcher-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.9
+Version: 0.3.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,18 @@
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
-- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
+
+## Demo
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -56,18 +59,14 @@
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
-## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
-
-
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
@@ -84,14 +83,15 @@
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
+### Installation
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 > **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
@@ -109,15 +109,15 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
 
 ```bash
@@ -132,14 +132,33 @@
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
 **To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
+### Run as PIP package
+```bash
+pip install gpt-researcher
+```
+
+```python
+from gpt_researcher import GPTResearcher
+
+query = "why is Nvidia stock going up?"
+researcher = GPTResearcher(query=query, report_type="research_report")
+# Conduct research on the given query
+await researcher.conduct_research()
+# Write the report
+report = await researcher.write_report()
+```
+
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+
+
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
```

### Comparing `gpt-researcher-0.2.9/README.md` & `gpt-researcher-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
-- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
+
+## Demo
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -38,18 +41,14 @@
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
-## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
-
-
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
@@ -66,14 +65,15 @@
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
+### Installation
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 > **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
@@ -91,15 +91,15 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
 
 ```bash
@@ -114,14 +114,33 @@
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
 **To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
+### Run as PIP package
+```bash
+pip install gpt-researcher
+```
+
+```python
+from gpt_researcher import GPTResearcher
+
+query = "why is Nvidia stock going up?"
+researcher = GPTResearcher(query=query, report_type="research_report")
+# Conduct research on the given query
+await researcher.conduct_research()
+# Write the report
+report = await researcher.write_report()
+```
+
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+
+
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
```

### Comparing `gpt-researcher-0.2.9/backend/report_type/basic_report/basic_report.py` & `gpt-researcher-0.3.0/backend/report_type/basic_report/basic_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/backend/report_type/detailed_report/detailed_report.py` & `gpt-researcher-0.3.0/backend/report_type/detailed_report/detailed_report.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/backend/server.py` & `gpt-researcher-0.3.0/backend/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from fastapi import FastAPI, Request, WebSocket, WebSocketDisconnect
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from pydantic import BaseModel
+from backend.websocket_manager import WebSocketManager
+from backend.utils import write_md_to_pdf, write_md_to_word, write_text_to_md
+import time
 import json
 import os
-from backend.websocket_manager import WebSocketManager
-from backend.utils import write_md_to_pdf, write_md_to_word
 
 
 class ResearchRequest(BaseModel):
     task: str
     report_type: str
     agent: str
 
@@ -42,21 +43,23 @@
     try:
         while True:
             data = await websocket.receive_text()
             if data.startswith("start"):
                 json_data = json.loads(data[6:])
                 task = json_data.get("task")
                 report_type = json_data.get("report_type")
+                filename = f"task_{int(time.time())}_{task}"
                 if task and report_type:
                     report = await manager.start_streaming(task, report_type, websocket)
                     # Saving report as pdf
-                    pdf_path = await write_md_to_pdf(report)
+                    pdf_path = await write_md_to_pdf(report, filename)
                     # Saving report as docx
-                    docx_path = await write_md_to_word(report)
+                    docx_path = await write_md_to_word(report, filename)
                     # Returning the path of saved report files
-                    await websocket.send_json({"type": "path", "output": {"pdf": pdf_path, "docx": docx_path}})
+                    md_path = await write_text_to_md(report, filename)
+                    await websocket.send_json({"type": "path", "output": {"pdf": pdf_path, "docx": docx_path, "md": md_path}})
                 else:
                     print("Error: not enough parameters provided.")
 
     except WebSocketDisconnect:
         await manager.disconnect(websocket)
```

### Comparing `gpt-researcher-0.2.9/backend/utils.py` & `gpt-researcher-0.3.0/backend/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,65 +15,75 @@
     """
     # Convert text to UTF-8, replacing any problematic characters
     text_utf8 = text.encode('utf-8', errors='replace').decode('utf-8')
 
     async with aiofiles.open(filename, "w", encoding='utf-8') as file:
         await file.write(text_utf8)
 
-async def write_md_to_pdf(text: str) -> str:
+async def write_text_to_md(text: str, filename: str = "") -> str:
+    """Writes text to a Markdown file and returns the file path.
+
+    Args:
+        text (str): Text to write to the Markdown file.
+
+    Returns:
+        str: The file path of the generated Markdown file.
+    """
+    file_path = f"outputs/{filename}.md"
+    await write_to_file(file_path, text)
+    return file_path
+
+async def write_md_to_pdf(text: str, filename: str = "") -> str:
     """Converts Markdown text to a PDF file and returns the file path.
 
     Args:
         text (str): Markdown text to convert.
 
     Returns:
         str: The encoded file path of the generated PDF.
     """
-    task = uuid.uuid4().hex
-    file_path = f"outputs/{task}"
-    await write_to_file(f"{file_path}.md", text)
+    file_path = f"outputs/{filename}.pdf"
 
     try:
-        md2pdf(f"{file_path}.pdf",
-               md_content=None,
-               md_file_path=f"{file_path}.md",
+        md2pdf(file_path,
+               md_content=text,
+               #md_file_path=f"{file_path}.md",
                css_file_path="./frontend/pdf_styles.css",
                base_url=None)
         print(f"Report written to {file_path}.pdf")
     except Exception as e:
         print(f"Error in converting Markdown to PDF: {e}")
         return ""
 
-    encoded_file_path = urllib.parse.quote(f"{file_path}.pdf")
+    encoded_file_path = urllib.parse.quote(file_path)
     return encoded_file_path
 
-async def write_md_to_word(text: str) -> str:
+async def write_md_to_word(text: str, filename: str = "") -> str:
     """Converts Markdown text to a DOCX file and returns the file path.
 
     Args:
         text (str): Markdown text to convert.
 
     Returns:
         str: The encoded file path of the generated DOCX.
     """
-    task = uuid.uuid4().hex
-    file_path = f"outputs/{task}"
+    file_path = f"outputs/{filename}.docx"
 
     try:
         # Convert report markdown to HTML
         html = mistune.html(text)
         # Create a document object
         doc = Document()
         # Convert the html generated from the report to document format
         HtmlToDocx().add_html_to_document(html, doc)
 
         # Saving the docx document to file_path
-        doc.save(f"{file_path}.docx")
+        doc.save(file_path)
         
-        print(f"Report written to {file_path}.docx")
+        print(f"Report written to {file_path}")
 
-        encoded_file_path = urllib.parse.quote(f"{file_path}.docx")
+        encoded_file_path = urllib.parse.quote(file_path)
         return encoded_file_path
     
     except Exception as e:
         print(f"Error in converting Markdown to DOCX: {e}")
         return ""
```

### Comparing `gpt-researcher-0.2.9/backend/websocket_manager.py` & `gpt-researcher-0.3.0/backend/websocket_manager.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/config/config.py` & `gpt-researcher-0.3.0/gpt_researcher/config/config.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/context/compression.py` & `gpt-researcher-0.3.0/gpt_researcher/context/compression.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/context/retriever.py` & `gpt-researcher-0.3.0/gpt_researcher/context/retriever.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/llm_provider/azureopenai/azureopenai.py` & `gpt-researcher-0.3.0/gpt_researcher/llm_provider/azureopenai/azureopenai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/llm_provider/google/google.py` & `gpt-researcher-0.3.0/gpt_researcher/llm_provider/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/llm_provider/openai/openai.py` & `gpt-researcher-0.3.0/gpt_researcher/llm_provider/openai/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/master/agent.py` & `gpt-researcher-0.3.0/gpt_researcher/master/agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         """
         Runs the GPT Researcher to conduct research
         """
         print(f"🔎 Running research for '{self.query}'...")
         
         # Generate Agent
         if not (self.agent and self.role):
-            self.agent, self.role = await choose_agent(self.query, self.cfg)
+            self.agent, self.role = await choose_agent(self.query, self.cfg, self.parent_query)
         await stream_output("logs", self.agent, self.websocket)
 
         # If specified, the researcher will use the given urls as the context for the research.
         if self.source_urls:
             self.context = await self.get_context_by_urls(self.source_urls)
         else:
             self.context = await self.get_context_by_search(self.query)
```

### Comparing `gpt-researcher-0.2.9/gpt_researcher/master/functions.py` & `gpt-researcher-0.3.0/gpt_researcher/master/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,25 +47,28 @@
 
         case _:
             raise Exception("Retriever not found.")
 
     return retriever
 
 
-async def choose_agent(query, cfg):
+async def choose_agent(query, cfg, parent_query=None):
     """
     Chooses the agent automatically
     Args:
+        parent_query: In some cases the research is conducted on a subtopic from the main query.
+        Tge parent query allows the agent to know the main context for better reasoning.
         query: original query
         cfg: Config
 
     Returns:
         agent: Agent name
         agent_role_prompt: Agent role prompt
     """
+    query = f"{parent_query} - {query}" if parent_query else f"{query}"
     try:
         response = await create_chat_completion(
             model=cfg.smart_llm_model,
             messages=[
                 {"role": "system", "content": f"{auto_agent_instructions()}"},
                 {"role": "user", "content": f"task: {query}"}],
             temperature=0,
```

### Comparing `gpt-researcher-0.2.9/gpt_researcher/master/prompts.py` & `gpt-researcher-0.3.0/gpt_researcher/master/prompts.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             f"Cite search results using inline notations. Only cite the most \
             relevant results that answer the query accurately. Place these citations at the end \
             of the sentence or paragraph that reference them.\n"\
             f"Please do your best, this is very important to my career. " \
             f"Assume that the current date is {datetime.now().strftime('%B %d, %Y')}"
 
 
-def generate_resource_report_prompt(question, context, report_format="apa", total_words=1000):
+def generate_resource_report_prompt(question, context, report_format="apa", total_words=700):
     """Generates the resource report prompt for the given question and research summary.
 
     Args:
         question (str): The question to generate the resource report prompt for.
         context (str): The research summary to generate the resource report prompt for.
 
     Returns:
@@ -71,34 +71,34 @@
     """
     return f'"""{context}"""\n\nBased on the above information, generate a bibliography recommendation report for the following' \
            f' question or topic: "{question}". The report should provide a detailed analysis of each recommended resource,' \
            ' explaining how each source can contribute to finding answers to the research question.\n' \
            'Focus on the relevance, reliability, and significance of each source.\n' \
            'Ensure that the report is well-structured, informative, in-depth, and follows Markdown syntax.\n' \
            'Include relevant facts, figures, and numbers whenever available.\n' \
-           'The report should have a minimum length of 700 words.\n' \
+           f'The report should have a minimum length of {total_words} words.\n' \
         'You MUST include all relevant source urls.'\
         'Every url should be hyperlinked: [url website](url)'
 
 
 def generate_custom_report_prompt(query_prompt, context, report_format="apa", total_words=1000):
     return f'"{context}"\n\n{query_prompt}'
 
 
-def generate_outline_report_prompt(question, context, report_format="apa", total_words=1000):
+def generate_outline_report_prompt(question, context, report_format="apa", total_words=1200):
     """ Generates the outline report prompt for the given question and research summary.
     Args: question (str): The question to generate the outline report prompt for
             research_summary (str): The research summary to generate the outline report prompt for
     Returns: str: The outline report prompt for the given question and research summary
     """
 
     return f'"""{context}""" Using the above information, generate an outline for a research report in Markdown syntax' \
            f' for the following question or topic: "{question}". The outline should provide a well-structured framework' \
            ' for the research report, including the main sections, subsections, and key points to be covered.' \
-           ' The research report should be detailed, informative, in-depth, and a minimum of 1,200 words.' \
+           f' The research report should be detailed, informative, in-depth, and a minimum of {total_words} words.' \
            ' Use appropriate Markdown syntax to format the outline and ensure readability.'
 
 
 def auto_agent_instructions():
     return """
         This task involves researching a given topic, regardless of its complexity or the availability of a definitive answer. The research is conducted by a specific server, defined by its type and role, with each server requiring distinct instructions.
         Agent
@@ -206,14 +206,15 @@
     "Date":
     Assume the current date is {datetime.now(timezone.utc).strftime('%B %d, %Y')} if required.
     
     "IMPORTANT!":
     - The focus MUST be on the main topic! You MUST Leave out any information un-related to it!
     - Must NOT have any introduction, conclusion, summary or reference section.
     - You MUST include hyperlinks with markdown syntax ([url website](url)) related to the sentences wherever necessary.
+    - The report should have a minimum length of {total_words} words.
     """
 
 
 def generate_report_introduction(question: str, research_summary: str = "") -> str:
     return f"""{research_summary}\n 
         Using the above latest information, Prepare a detailed report introduction on the topic -- {question}.
         - The introduction should be succinct, well-structured, informative with markdown syntax.
```

### Comparing `gpt-researcher-0.2.9/gpt_researcher/memory/embeddings.py` & `gpt-researcher-0.3.0/gpt_researcher/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/bing/bing.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/bing/bing.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/google/google.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/google/google.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/searx/searx.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/searx/searx.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/serpapi/serpapi.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/serpapi/serpapi.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/serper/serper.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/serper/serper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_news/tavily_news.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_news/tavily_news.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/retrievers/tavily_search/tavily_search.py` & `gpt-researcher-0.3.0/gpt_researcher/retrievers/tavily_search/tavily_search.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/arxiv/arxiv.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/arxiv/arxiv.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/beautiful_soup/beautiful_soup.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/newspaper/newspaper.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/newspaper/newspaper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/pymupdf/pymupdf.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/pymupdf/pymupdf.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/scraper.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/scraper/web_base_loader/web_base_loader.py` & `gpt-researcher-0.3.0/gpt_researcher/scraper/web_base_loader/web_base_loader.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher/utils/llm.py` & `gpt-researcher-0.3.0/gpt_researcher/utils/llm.py`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/gpt_researcher.egg-info/PKG-INFO` & `gpt-researcher-0.3.0/gpt_researcher.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-researcher
-Version: 0.2.9
+Version: 0.3.0
 Summary: GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.
 Home-page: https://github.com/assafelovic/gpt-researcher
 Author: Assaf Elovic
 Author-email: assaf.elovic@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,18 @@
 **Our mission is to empower individuals and organizations with accurate, unbiased, and factual information by leveraging the power of AI.**
 
 ## Why GPT Researcher?
 
 - To form objective conclusions for manual research tasks can take time, sometimes weeks to find the right resources and information.
 - Current LLMs are trained on past and outdated information, with heavy risks of hallucinations, making them almost irrelevant for research tasks.
 - Services that enable web search (such as ChatGPT + Web Plugin), only consider limited sources and content that in some cases result in superficial and biased answers.
-- Using only a selection of web sources can create bias in determining the right conclusions for research tasks. 
+- Using only a selection of web sources can create bias in determining the right conclusions for research tasks.
+
+## Demo
+https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
 
 ## Architecture
 The main idea is to run "planner" and "execution" agents, whereas the planner generates questions to research, and the execution agents seek the most related information based on each generated research question. Finally, the planner filters and aggregates all related information and creates a research report. <br /> <br /> 
 The agents leverage both gpt3.5-turbo and gpt-4-turbo (128K context) to complete a research task. We optimize for costs using each only when necessary. **The average research task takes around 3 minutes to complete, and costs ~$0.1.**
 
 <div align="center">
 <img align="center" height="500" src="https://cowriter-images.s3.amazonaws.com/architecture.png">
@@ -56,18 +59,14 @@
 More specifically:
 * Create a domain specific agent based on research query or task.
 * Generate a set of research questions that together form an objective opinion on any given task. 
 * For each research question, trigger a crawler agent that scrapes online resources for information relevant to the given task.
 * For each scraped resources, summarize based on relevant information and keep track of its sources.
 * Finally, filter and aggregate all summarized sources and generate a final research report.
 
-## Demo
-https://github.com/assafelovic/gpt-researcher/assets/13554167/dd6cf08f-b31e-40c6-9907-1915f52a7110
-
-
 ## Tutorials
  - [How it Works](https://docs.tavily.com/blog/building-gpt-researcher)
  - [How to Install](https://www.loom.com/share/04ebffb6ed2a4520a27c3e3addcdde20?sid=da1848e8-b1f1-42d1-93c3-5b0b9c3b24ea)
  - [Live Demo](https://www.loom.com/share/6a3385db4e8747a1913dd85a7834846f?sid=a740fd5b-2aa3-457e-8fb7-86976f59f9b8)
 
 ## Features
 - 📝 Generate research, outlines, resources and lessons reports
@@ -84,14 +83,15 @@
 
 - Getting started (installation, setting up the environment, simple examples)
 - Customization and configuration
 - How-To examples (demos, integrations, docker support)
 - Reference (full API docs)
 
 ## ⚙️ Getting Started
+### Installation
 > **Step 0** - Install Python 3.11 or later. [See here](https://www.tutorialsteacher.com/python/install-python) for a step-by-step guide.
 
 > **Step 1** - Download the project and navigate to its directory
 
 ```bash
 git clone https://github.com/assafelovic/gpt-researcher.git
 cd gpt-researcher
@@ -109,15 +109,15 @@
 For a more permanent setup, create a `.env` file in the current `gpt-researcher` directory and input the keys as follows:
 
 ```bash
 OPENAI_API_KEY={Your OpenAI API Key here}
 TAVILY_API_KEY={Your Tavily API Key here}
 ```
 
-- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/guides/adapters/openai), simply change the llm model and provider in config/config.py. 
+- **For LLM, we recommend [OpenAI GPT](https://platform.openai.com/docs/guides/gpt)**, but you can use any other LLM model (including open sources) supported by [Langchain Adapter](https://python.langchain.com/docs/integrations/adapters/openai/), simply change the llm model and provider in config/config.py. 
 - **For web search API, we recommend [Tavily Search API](https://app.tavily.com)**, but you can also refer to other search APIs of your choice by changing the search provider in config/config.py to `"duckduckgo"`, `"googleAPI"`, `"bing"`, `"googleSerp"`, `"searx"` and more. Then add the corresponding env API key as seen in the config.py file.
 
 ### Quickstart
 
 > **Step 1** - Install dependencies
 
 ```bash
@@ -132,14 +132,33 @@
 
 > **Step 3** - Go to http://localhost:8000 on any browser and enjoy researching!
 
 <br />
 
 **To learn how to get started with [Docker](https://docs.tavily.com/docs/gpt-researcher/getting-started#try-it-with-docker), [Poetry](https://docs.tavily.com/docs/gpt-researcher/getting-started#poetry) or a [virtual environment](https://docs.tavily.com/docs/gpt-researcher/getting-started#virtual-environment) check out the [documentation](https://docs.tavily.com/docs/gpt-researcher/getting-started) page.**
 
+### Run as PIP package
+```bash
+pip install gpt-researcher
+```
+
+```python
+from gpt_researcher import GPTResearcher
+
+query = "why is Nvidia stock going up?"
+researcher = GPTResearcher(query=query, report_type="research_report")
+# Conduct research on the given query
+await researcher.conduct_research()
+# Write the report
+report = await researcher.write_report()
+```
+
+**For more examples and configurations, please refer to the [PIP documentation](https://docs.tavily.com/docs/gpt-researcher/pip-package) page.**
+
+
 ## 🚀 Contributing
 We highly welcome contributions! Please check out [contributing](CONTRIBUTING.md) if you're interested.
 
 Please check out our [roadmap](https://trello.com/b/3O7KBePw/gpt-researcher-roadmap) page and reach out to us via our [Discord community](https://discord.gg/2pFkc83fRq) if you're interested in joining our mission.
 
 ## ✉️ Support / Contact us
 - [Community Discord](https://discord.gg/spBgZmm3Xe)
```

### Comparing `gpt-researcher-0.2.9/gpt_researcher.egg-info/SOURCES.txt` & `gpt-researcher-0.3.0/gpt_researcher.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -63,21 +63,8 @@
 gpt_researcher/scraper/pymupdf/__init__.py
 gpt_researcher/scraper/pymupdf/pymupdf.py
 gpt_researcher/scraper/web_base_loader/__init__.py
 gpt_researcher/scraper/web_base_loader/web_base_loader.py
 gpt_researcher/utils/__init__.py
 gpt_researcher/utils/enum.py
 gpt_researcher/utils/llm.py
-gpt_researcher/utils/validators.py
-multi_agents/__init__.py
-multi_agents/main.py
-multi_agents/agents/__init__.py
-multi_agents/agents/critique.py
-multi_agents/agents/curator.py
-multi_agents/agents/editor.py
-multi_agents/agents/master.py
-multi_agents/agents/publisher.py
-multi_agents/agents/researcher.py
-multi_agents/agents/reviser.py
-multi_agents/agents/writer.py
-multi_agents/agents/utils/__init__.py
-multi_agents/agents/utils/file_utils.py
+gpt_researcher/utils/validators.py
```

### Comparing `gpt-researcher-0.2.9/pyproject.toml` & `gpt-researcher-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-researcher-0.2.9/setup.py` & `gpt-researcher-0.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
 
 with open("requirements.txt", "r") as f:
     reqs = [line.strip() for line in f if ('selenium' not in line and 'webdriver' not in line)]
 
 setup(
     name="gpt-researcher",
-    version="0.2.9",
+    version="0.3.0",
     description="GPT Researcher is an autonomous agent designed for comprehensive online research on a variety of tasks.",
     package_dir={'gpt_researcher': 'gpt_researcher'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/assafelovic/gpt-researcher",
     author="Assaf Elovic",
```

