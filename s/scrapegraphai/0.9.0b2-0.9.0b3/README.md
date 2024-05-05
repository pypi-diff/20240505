# Comparing `tmp/scrapegraphai-0.9.0b2.tar.gz` & `tmp/scrapegraphai-0.9.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.9.0b2.tar", max compression
+gzip compressed data, was "scrapegraphai-0.9.0b3.tar", max compression
```

## Comparing `scrapegraphai-0.9.0b2.tar` & `scrapegraphai-0.9.0b3.tar`

### file list

```diff
@@ -1,60 +1,61 @@
--rw-r--r--   0        0        0     1065 2024-05-05 00:05:42.608618 scrapegraphai-0.9.0b2/LICENSE
--rw-r--r--   0        0        0    10242 2024-05-05 00:05:42.608618 scrapegraphai-0.9.0b2/README.md
--rw-r--r--   0        0        0     1792 2024-05-05 00:06:01.604670 scrapegraphai-0.9.0b2/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      449 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0    10984 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3738 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/pdf_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     2068 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      342 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      579 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/bedrock.py
--rw-r--r--   0        0        0      463 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      736 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-05 00:05:42.636618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6987 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py
--rw-r--r--   0        0        0     6639 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     4464 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     2140 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-05 00:05:42.640618 scrapegraphai-0.9.0b2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-05 00:19:51.770133 scrapegraphai-0.9.0b3/LICENSE
+-rw-r--r--   0        0        0    10242 2024-05-05 00:19:51.770133 scrapegraphai-0.9.0b3/README.md
+-rw-r--r--   0        0        0     1792 2024-05-05 00:20:18.554206 scrapegraphai-0.9.0b3/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      449 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0    11402 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-05 00:19:51.798133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/pdf_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     2068 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      369 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      479 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/claude.py
+-rw-r--r--   0        0        0      487 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      736 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6987 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py
+-rw-r--r--   0        0        0     6639 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     4464 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     2140 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-05 00:19:51.802133 scrapegraphai-0.9.0b3/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    12183 1970-01-01 00:00:00.000000 scrapegraphai-0.9.0b3/PKG-INFO
```

### Comparing `scrapegraphai-0.9.0b2/LICENSE` & `scrapegraphai-0.9.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/README.md` & `scrapegraphai-0.9.0b3/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/pyproject.toml` & `scrapegraphai-0.9.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.9.0b2"
+version = "0.9.0b3"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.9.0b3/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/abstract_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 from typing import Optional
 
 from langchain_aws.embeddings.bedrock import BedrockEmbeddings
 from langchain_community.embeddings import HuggingFaceHubEmbeddings, OllamaEmbeddings
 from langchain_openai import AzureOpenAIEmbeddings, OpenAIEmbeddings
 
 from ..helpers import models_tokens
-from ..models import AzureOpenAI, Bedrock, Gemini, Groq, HuggingFace, Ollama, OpenAI
+from ..models import AzureOpenAI, Bedrock, Gemini, Groq, HuggingFace, Ollama, OpenAI, Claude
 
 
 class AbstractGraph(ABC):
     """
     Scaffolding class for creating a graph representation and executing it.
 
     Attributes:
         prompt (str): The prompt for the graph.
         source (str): The source of the graph.
         config (dict): Configuration parameters for the graph.
         llm_model: An instance of a language model client, configured for generating answers.
-        embedder_model: An instance of an embedding model client, configured for generating embeddings.
+        embedder_model: An instance of an embedding model client,
+                        configured for generating embeddings.
         verbose (bool): A flag indicating whether to show print statements during execution.
         headless (bool): A flag indicating whether to run the graph in headless mode.
 
     Args:
         prompt (str): The prompt for the graph.
         config (dict): Configuration parameters for the graph.
         source (str, optional): The source of the graph.
@@ -43,45 +44,43 @@
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
 
         self.prompt = prompt
         self.source = source
         self.config = config
         self.llm_model = self._create_llm(config["llm"], chat=True)
-        self.embedder_model = self._create_default_embedder(    
-            ) if "embeddings" not in config else self._create_embedder(
+        self.embedder_model = self._create_default_embedder(
+        ) if "embeddings" not in config else self._create_embedder(
             config["embeddings"])
 
         # Set common configuration parameters
         self.verbose = True if config is None else config.get("verbose", False)
         self.headless = True if config is None else config.get(
             "headless", True)
 
         # Create the graph
         self.graph = self._create_graph()
         self.final_state = None
         self.execution_info = None
 
-
     def _set_model_token(self, llm):
 
         if 'Azure' in str(type(llm)):
             try:
                 self.model_token = models_tokens["azure"][llm.model_name]
             except KeyError:
                 raise KeyError("Model not supported")
-            
+                
         elif 'HuggingFaceEndpoint' in str(type(llm)):
             if 'mistral' in llm.repo_id:
                 try:
                     self.model_token = models_tokens['mistral'][llm.repo_id]
                 except KeyError:
                     raise KeyError("Model not supported")
 
-
     def _create_llm(self, llm_config: dict, chat=False) -> object:
         """
         Create a large language model instance based on the configuration provided.
 
         Args:
             llm_config (dict): Configuration parameters for the language model.
 
@@ -99,89 +98,94 @@
         llm_params = {**llm_defaults, **llm_config}
 
         # If model instance is passed directly instead of the model details
         if 'model_instance' in llm_params:
             if chat:
                 self._set_model_token(llm_params['model_instance'])
             return llm_params['model_instance']
-        
+
         # Instantiate the language model based on the model name
         if "gpt-" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return OpenAI(llm_params)
 
         elif "azure" in llm_params["model"]:
             # take the model after the last dash
             llm_params["model"] = llm_params["model"].split("/")[-1]
             try:
                 self.model_token = models_tokens["azure"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return AzureOpenAI(llm_params)
 
         elif "gemini" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["gemini"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return Gemini(llm_params)
-
+        elif "claude" in llm_params["model"]:
+            try:
+                self.model_token = models_tokens["claude"][llm_params["model"]]
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
+            return Claude(llm_params)
         elif "ollama" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             # allow user to set model_tokens in config
             try:
                 if "model_tokens" in llm_params:
                     self.model_token = llm_params["model_tokens"]
                 elif llm_params["model"] in models_tokens["ollama"]:
                     try:
                         self.model_token = models_tokens["ollama"][llm_params["model"]]
-                    except KeyError:
-                        raise KeyError("Model not supported")
+                    except KeyError as exc:
+                        raise KeyError("Model not supported") from exc
                 else:
                     self.model_token = 8192
             except AttributeError:
                 self.model_token = 8192
 
             return Ollama(llm_params)
         elif "hugging_face" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["hugging_face"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return HuggingFace(llm_params)
         elif "groq" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
 
             try:
                 self.model_token = models_tokens["groq"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return Groq(llm_params)
         elif "bedrock" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
             model_id = llm_params["model"]
 
             try:
                 self.model_token = models_tokens["bedrock"][llm_params["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return Bedrock({
                 "model_id": model_id,
                 "model_kwargs": {
                     "temperature": llm_params["temperature"],
                 }
             })
         else:
             raise ValueError(
                 "Model provided by the configuration not supported")
-    
+
     def _create_default_embedder(self) -> object:
         """
         Create an embedding model instance based on the chosen llm model.
 
         Returns:
             object: An instance of the embedding model client.
 
@@ -204,15 +208,15 @@
             return OllamaEmbeddings(**params)
         elif isinstance(self.llm_model, HuggingFace):
             return HuggingFaceHubEmbeddings(model=self.llm_model.model)
         elif isinstance(self.llm_model, Bedrock):
             return BedrockEmbeddings(client=None, model_id=self.llm_model.model_id)
         else:
             raise ValueError("Embedding Model missing or not supported")
-        
+
     def _create_embedder(self, embedder_config: dict) -> object:
         """
         Create an embedding model instance based on the configuration provided.
 
         Args:
             embedder_config (dict): Configuration parameters for the embedding model.
 
@@ -233,35 +237,35 @@
         elif "azure" in embedder_config["model"]:
             return AzureOpenAIEmbeddings()
 
         elif "ollama" in embedder_config["model"]:
             embedder_config["model"] = embedder_config["model"].split("/")[-1]
             try:
                 models_tokens["ollama"][embedder_config["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return OllamaEmbeddings(**embedder_config)
-        
+
         elif "hugging_face" in embedder_config["model"]:
             try:
                 models_tokens["hugging_face"][embedder_config["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported")from exc
             return HuggingFaceHubEmbeddings(model=embedder_config["model"])
-        
+
         elif "bedrock" in embedder_config["model"]:
             embedder_config["model"] = embedder_config["model"].split("/")[-1]
             try:
                 models_tokens["bedrock"][embedder_config["model"]]
-            except KeyError:
-                raise KeyError("Model not supported")
+            except KeyError as exc:
+                raise KeyError("Model not supported") from exc
             return BedrockEmbeddings(client=None, model_id=embedder_config["model"])
         else:
             raise ValueError(
-                "Model provided by the configuration not supported") 
+                "Model provided by the configuration not supported")
 
     def get_state(self, key=None) -> dict:
         """""
         Get the final state of the graph.
 
         Args:
             key (str, optional): The key of the final state to retrieve.
@@ -277,15 +281,15 @@
     def get_execution_info(self):
         """
         Returns the execution information of the graph.
 
         Returns:
             dict: The execution information of the graph.
         """
-        
+
         return self.execution_info
 
     @abstractmethod
     def _create_graph(self):
         """
         Abstract method to create a graph representation.
         """
@@ -293,8 +297,7 @@
 
     @abstractmethod
     def run(self) -> str:
         """
         Abstract method to execute the graph and return the result.
         """
         pass
-
```

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/pdf_scraper_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/pdf_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.9.0b3/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.9.0b3/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.9.0b3/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.9.0b3/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/models/bedrock.py` & `scrapegraphai-0.9.0b3/scrapegraphai/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.9.0b3/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.9.0b3/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_answer_pdf_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_answer_pdf_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.9.0b3/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/remover.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.9.0b3/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.9.0b2/PKG-INFO` & `scrapegraphai-0.9.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.9.0b2
+Version: 0.9.0b3
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

