# Comparing `tmp/recommender-agent-0.2.1.tar.gz` & `tmp/recommender-agent-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommender-agent-0.2.1.tar", last modified: Mon Apr 15 18:31:34 2024, max compression
+gzip compressed data, was "recommender-agent-0.3.0.tar", last modified: Sun May  5 00:27:49 2024, max compression
```

## Comparing `recommender-agent-0.2.1.tar` & `recommender-agent-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:31:34.040792 recommender-agent-0.2.1/
--rw-rw-rw-   0        0        0     1093 2024-04-14 17:54:09.000000 recommender-agent-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     3947 2024-04-15 18:31:34.040792 recommender-agent-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     3386 2024-04-14 22:00:49.000000 recommender-agent-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 18:31:34.005794 recommender-agent-0.2.1/recommender_agent/
--rw-rw-rw-   0        0        0       66 2024-04-14 21:07:45.000000 recommender-agent-0.2.1/recommender_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:31:34.039791 recommender-agent-0.2.1/recommender_agent/components/
--rw-rw-rw-   0        0        0      130 2024-04-14 22:08:44.000000 recommender-agent-0.2.1/recommender_agent/components/__init__.py
--rw-rw-rw-   0        0        0     9045 2024-04-12 23:09:28.000000 recommender-agent-0.2.1/recommender_agent/components/agent.py
--rw-rw-rw-   0        0        0     3116 2024-04-15 18:30:32.000000 recommender-agent-0.2.1/recommender_agent/components/vectorStoreClient.py
--rw-rw-rw-   0        0        0     3333 2024-04-15 18:21:53.000000 recommender-agent-0.2.1/recommender_agent/recommenderSystem.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:31:34.035796 recommender-agent-0.2.1/recommender_agent.egg-info/
--rw-rw-rw-   0        0        0     3947 2024-04-15 18:31:33.000000 recommender-agent-0.2.1/recommender_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-15 18:31:33.000000 recommender-agent-0.2.1/recommender_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:31:33.000000 recommender-agent-0.2.1/recommender_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2024-04-15 18:31:33.000000 recommender-agent-0.2.1/recommender_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 18:31:33.000000 recommender-agent-0.2.1/recommender_agent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-15 18:31:34.043795 recommender-agent-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1088 2024-04-15 18:28:38.000000 recommender-agent-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 00:27:49.889896 recommender-agent-0.3.0/
+-rw-rw-rw-   0        0        0     1093 2024-04-14 17:54:09.000000 recommender-agent-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4601 2024-05-05 00:27:49.891900 recommender-agent-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4064 2024-05-05 00:12:09.000000 recommender-agent-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 00:27:49.849665 recommender-agent-0.3.0/recommender_agent/
+-rw-rw-rw-   0        0        0       66 2024-04-14 21:07:45.000000 recommender-agent-0.3.0/recommender_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 00:27:49.888896 recommender-agent-0.3.0/recommender_agent/components/
+-rw-rw-rw-   0        0        0      130 2024-04-14 22:08:44.000000 recommender-agent-0.3.0/recommender_agent/components/__init__.py
+-rw-rw-rw-   0        0        0     6865 2024-05-04 23:05:23.000000 recommender-agent-0.3.0/recommender_agent/components/agent.py
+-rw-rw-rw-   0        0        0     3126 2024-05-04 22:58:22.000000 recommender-agent-0.3.0/recommender_agent/components/vectorStoreClient.py
+-rw-rw-rw-   0        0        0     2639 2024-05-04 23:43:05.000000 recommender-agent-0.3.0/recommender_agent/recommenderSystem.py
+drwxrwxrwx   0        0        0        0 2024-05-05 00:27:49.885896 recommender-agent-0.3.0/recommender_agent.egg-info/
+-rw-rw-rw-   0        0        0     4601 2024-05-05 00:27:49.000000 recommender-agent-0.3.0/recommender_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      438 2024-05-05 00:27:49.000000 recommender-agent-0.3.0/recommender_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 00:27:49.000000 recommender-agent-0.3.0/recommender_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      232 2024-05-05 00:27:49.000000 recommender-agent-0.3.0/recommender_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-05 00:27:49.000000 recommender-agent-0.3.0/recommender_agent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-05 00:27:49.900118 recommender-agent-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2024-05-04 23:13:43.000000 recommender-agent-0.3.0/setup.py
```

### Comparing `recommender-agent-0.2.1/LICENSE` & `recommender-agent-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recommender-agent-0.2.1/PKG-INFO` & `recommender-agent-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 Metadata-Version: 2.1
 Name: recommender-agent
-Version: 0.2.1
+Version: 0.3.0
 Summary: En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
 Home-page: https://github.com/johansquintero/recommender-agent
 Author: Johan sebastian quintero rojas
 Author-email: metalium144@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sistema de recomendaciÃ³n con agente langchain
+# Sistema de recomendación con agente langchain
 
-<!-- ABOUT THE PROJECT -->
 ## Acerca del proyecto
-En el presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el sistema permite recomendar recursos a travÃ©s del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
+En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
 
 
 ## Procesos 
 
-* ConfiguraciÃ³n de ChromaDb - Vector Similarity
-* CreaciÃ³n del mÃ³dulo de generaciÃ³n de embeddings ya sea por openAi o algun otro modelo
-* MÃ³dulo de recomendaciÃ³n generativo con agentes langchain y llms
+* Configuración y creacion del modulo de la base de datos vectorial con ChromaDb
+* Creación del módulo y configuracion del agente Langchain
+* Módulo principal de recomendación el cual gestiona e integrar los dos anteriores modulos
 
-<!-- GETTING STARTED -->
-## TecnologÃ­as
+## Tecnologías
 
 * Python
 * ChromaDB
 * Langchain
 * Llama
 * HugginFace
 * pytorch
 * OpenAI
+* Groq
 * Embeddings
-* Mistral
-* GPT
+* LLM
 
 
 ## Prerequisitos
-
 * Instalar Python (<a href="https://www.python.org/downloads/">https://www.python.org/downloads/</a>).
-* Obtener el API KEY de OpenAI (opcional) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de OpenAI (opcional si se va a utilizar Groq) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de groq (opcional si se va a utilizar OpenAI) (<a href="https://console.groq.com/keys">https://console.groq.com/keys</a>)
 
-## Inicializacion manual
+## Instalacion manual desde el repositorio
 
 * Clonar el repositorio
   ```sh
   git clone https://github.com/johansquintero/recommender-agent
   ```
 
 * Crear el entorno virtual
@@ -82,25 +80,33 @@
 ```python
 books["id"] = books.index + 1
 ```
 #### Se convierte a diccionario el dataset
 ```python
 books_dict = books.to_dict(orient='records') 
 ```
-#### Si se cuenta con una api key de openai se agrega en este apartado
+### la libreria dispone de dos alternativas para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe recalcar que es obligatorio contar con alguna de estas 2 apis
+
+#### Si se cuenta con una api key de openai este seria el proceso
 ```python
 openai_api_key = ""
 ```
 #### Se inicializa la instancia el recomendador
 ```python
-recommender = CoreRecommendation(openai_key=openai_api_key)
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key)
 ```
 #### De la intancia anterior se crea ruta de persistencia de los recursos
 ```python
-recommender.init_components(collection_name="books",resources=books_dict)
+recommender_open_ai.init_components(collection_name="books",resources=books_dict)
+```
+#### El el caso de usar groq este es el metodo
+```python
+groq_api_key=""
+recommender_groq = CoreRecommendation(groq_key=groq_api_key)
+recommender_groq.init_components(collection_name="books",resources=books_dict)
 ```
 #### Usuario de prueba en formato JSON
 ```python
 user = {
   "user": {
     "id": 234567,
     "name": "Carlos Rodriguez",
@@ -109,15 +115,15 @@
       "street": "Calle Principal",
       "city": "Barcelona",
       "state": "Spain",
       "postal_code": "08001"
     },
     "preferences": {
       "genres": ["Philosophy","Novels", "History"],
-      "favorite_authors": ["Dan Brown", "Ken Follett", "RenÃ© Descartes"]
+      "favorite_authors": ["Dan Brown", "Ken Follett", "René Descartes"]
     },
     "purchase_history": [
       {
         "book": "The Da Vinci Code",
         "author": "Dan Brown",
         "price": 17.99,
         "purchase_date": "2023-12-12"
@@ -130,12 +136,14 @@
       }
     ]
   }
 }
 ```
 #### Se ejecuta el recomendador con la informacion del usuario
 ```python
-print(recommender.get_recommendation(user=user))
+response = recommender_groq.get_recommendation(user=user)
+print(f"Usuario={response['user']} \n") 
+print(f"Recomendaciones= {response['rec']}")
 ```
```

#### html2text {}

```diff
@@ -1,47 +1,56 @@
-Metadata-Version: 2.1 Name: recommender-agent Version: 0.2.1 Summary: En el
+Metadata-Version: 2.1 Name: recommender-agent Version: 0.3.0 Summary: En el
 presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el
 sistema permite recomendar recursos a travÃ©s del uso de mecanismos de
 Procesamiento de lenguaje natura como agentes langchain, IA generatica y
 embeddings. Home-page: https://github.com/johansquintero/recommender-agent
 Author: Johan sebastian quintero rojas Author-email: metalium144@gmail.com
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE #
-Sistema de recomendaciÃÂ³n con agente langchain ## Acerca del proyecto En el
-presente proyecto muestro la construcciÃÂ³n de una sistema de
-recomendaciÃÂ³n, el sistema permite recomendar recursos a travÃÂ©s del uso de
-mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA
-generatica y embeddings. ## Procesos * ConfiguraciÃÂ³n de ChromaDb - Vector
-Similarity * CreaciÃÂ³n del mÃÂ³dulo de generaciÃÂ³n de embeddings ya sea
-por openAi o algun otro modelo * MÃÂ³dulo de recomendaciÃÂ³n generativo con
-agentes langchain y llms ## TecnologÃÂ­as * Python * ChromaDB * Langchain *
-Llama * HugginFace * pytorch * OpenAI * Embeddings * Mistral * GPT ##
-Prerequisitos * Instalar Python (_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener
-el API KEY de OpenAI (opcional) (_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). ## Inicializacion manual
-* Clonar el repositorio ```sh git clone https://github.com/johansquintero/
-recommender-agent ``` * Crear el entorno virtual ```sh python -m venv env ``` *
-Activar entorno virtual (windows): ```sh env\Scripts\activate ``` * Instalar
-las dependencias del proyecto: ```sh pip install -r requirements.txt ``` ##
-Instalando con pip ```sh pip install recommender-agent ``` # Ejemplo de
-implementacion del sistema #### Imports ```python from
-recommender_agent.recommenderSystem import CoreRecommendation import pandas as
-pd ``` #### Se importa el dataset de la ruta donde este ubicado ```python books
-= pd.read_csv("../dataset_books/Books2.csv") books = books.fillna('')
-books.drop(columns=["isbn13","thumbnail","subtitle"],axis=1,inplace=True) ```
-#### Un requisito es que cada uno de los elementos tengan un id ```python books
-["id"] = books.index + 1 ``` #### Se convierte a diccionario el dataset
-```python books_dict = books.to_dict(orient='records') ``` #### Si se cuenta
-con una api key de openai se agrega en este apartado ```python openai_api_key =
-"" ``` #### Se inicializa la instancia el recomendador ```python recommender =
-CoreRecommendation(openai_key=openai_api_key) ``` #### De la intancia anterior
-se crea ruta de persistencia de los recursos ```python
-recommender.init_components(collection_name="books",resources=books_dict) ```
-#### Usuario de prueba en formato JSON ```python user = { "user": { "id":
-234567, "name": "Carlos Rodriguez", "email": "carlos_rodriguez@email.com",
-"address": { "street": "Calle Principal", "city": "Barcelona", "state":
-"Spain", "postal_code": "08001" }, "preferences": { "genres":
-["Philosophy","Novels", "History"], "favorite_authors": ["Dan Brown", "Ken
-Follett", "RenÃÂ© Descartes"] }, "purchase_history": [ { "book": "The Da Vinci
-Code", "author": "Dan Brown", "price": 17.99, "purchase_date": "2023-12-12" },
-{ "book": "The Pillars of the Earth", "author": "Ken Follett", "price": 22.99,
-"purchase_date": "2024-01-05" } ] } } ``` #### Se ejecuta el recomendador con
-la informacion del usuario ```python print(recommender.get_recommendation
-(user=user)) ```
+Sistema de recomendaciÃ³n con agente langchain ## Acerca del proyecto En el
+presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el
+sistema permite recomendar recursos a travÃ©s del uso de mecanismos de
+Procesamiento de lenguaje natura como agentes langchain, IA generatica y
+embeddings. ## Procesos * ConfiguraciÃ³n y creacion del modulo de la base de
+datos vectorial con ChromaDb * CreaciÃ³n del mÃ³dulo y configuracion del agente
+Langchain * MÃ³dulo principal de recomendaciÃ³n el cual gestiona e integrar los
+dos anteriores modulos ## TecnologÃ­as * Python * ChromaDB * Langchain * Llama
+* HugginFace * pytorch * OpenAI * Groq * Embeddings * LLM ## Prerequisitos *
+Instalar Python (_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener una API KEY de
+OpenAI (opcional si se va a utilizar Groq) (_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). * Obtener una
+API KEY de groq (opcional si se va a utilizar OpenAI) (_h_t_t_p_s_:_/_/
+_c_o_n_s_o_l_e_._g_r_o_q_._c_o_m_/_k_e_y_s) ## Instalacion manual desde el repositorio * Clonar el
+repositorio ```sh git clone https://github.com/johansquintero/recommender-agent
+``` * Crear el entorno virtual ```sh python -m venv env ``` * Activar entorno
+virtual (windows): ```sh env\Scripts\activate ``` * Instalar las dependencias
+del proyecto: ```sh pip install -r requirements.txt ``` ## Instalando con pip
+```sh pip install recommender-agent ``` # Ejemplo de implementacion del sistema
+#### Imports ```python from recommender_agent.recommenderSystem import
+CoreRecommendation import pandas as pd ``` #### Se importa el dataset de la
+ruta donde este ubicado ```python books = pd.read_csv("../dataset_books/
+Books2.csv") books = books.fillna('') books.drop(columns=
+["isbn13","thumbnail","subtitle"],axis=1,inplace=True) ``` #### Un requisito es
+que cada uno de los elementos tengan un id ```python books["id"] = books.index
++ 1 ``` #### Se convierte a diccionario el dataset ```python books_dict =
+books.to_dict(orient='records') ``` ### la libreria dispone de dos alternativas
+para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe
+recalcar que es obligatorio contar con alguna de estas 2 apis #### Si se cuenta
+con una api key de openai este seria el proceso ```python openai_api_key = ""
+``` #### Se inicializa la instancia el recomendador ```python
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key) ``` #### De
+la intancia anterior se crea ruta de persistencia de los recursos ```python
+recommender_open_ai.init_components
+(collection_name="books",resources=books_dict) ``` #### El el caso de usar groq
+este es el metodo ```python groq_api_key="" recommender_groq =
+CoreRecommendation(groq_key=groq_api_key) recommender_groq.init_components
+(collection_name="books",resources=books_dict) ``` #### Usuario de prueba en
+formato JSON ```python user = { "user": { "id": 234567, "name": "Carlos
+Rodriguez", "email": "carlos_rodriguez@email.com", "address": { "street":
+"Calle Principal", "city": "Barcelona", "state": "Spain", "postal_code":
+"08001" }, "preferences": { "genres": ["Philosophy","Novels", "History"],
+"favorite_authors": ["Dan Brown", "Ken Follett", "RenÃ© Descartes"] },
+"purchase_history": [ { "book": "The Da Vinci Code", "author": "Dan Brown",
+"price": 17.99, "purchase_date": "2023-12-12" }, { "book": "The Pillars of the
+Earth", "author": "Ken Follett", "price": 22.99, "purchase_date": "2024-01-05"
+} ] } } ``` #### Se ejecuta el recomendador con la informacion del usuario
+```python response = recommender_groq.get_recommendation(user=user) print
+(f"Usuario={response['user']} \n") print(f"Recomendaciones= {response['rec']}")
+```
```

### Comparing `recommender-agent-0.2.1/README.md` & `recommender-agent-0.3.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # Sistema de recomendación con agente langchain
 
-<!-- ABOUT THE PROJECT -->
 ## Acerca del proyecto
 En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
 
 
 ## Procesos 
 
-* Configuración de ChromaDb - Vector Similarity
-* Creación del módulo de generación de embeddings ya sea por openAi o algun otro modelo
-* Módulo de recomendación generativo con agentes langchain y llms
+* Configuración y creacion del modulo de la base de datos vectorial con ChromaDb
+* Creación del módulo y configuracion del agente Langchain
+* Módulo principal de recomendación el cual gestiona e integrar los dos anteriores modulos
 
-<!-- GETTING STARTED -->
 ## Tecnologías
 
 * Python
 * ChromaDB
 * Langchain
 * Llama
 * HugginFace
 * pytorch
 * OpenAI
+* Groq
 * Embeddings
-* Mistral
-* GPT
+* LLM
 
 
 ## Prerequisitos
-
 * Instalar Python (<a href="https://www.python.org/downloads/">https://www.python.org/downloads/</a>).
-* Obtener el API KEY de OpenAI (opcional) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de OpenAI (opcional si se va a utilizar Groq) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de groq (opcional si se va a utilizar OpenAI) (<a href="https://console.groq.com/keys">https://console.groq.com/keys</a>)
 
-## Inicializacion manual
+## Instalacion manual desde el repositorio
 
 * Clonar el repositorio
   ```sh
   git clone https://github.com/johansquintero/recommender-agent
   ```
 
 * Crear el entorno virtual
@@ -71,25 +69,33 @@
 ```python
 books["id"] = books.index + 1
 ```
 #### Se convierte a diccionario el dataset
 ```python
 books_dict = books.to_dict(orient='records') 
 ```
-#### Si se cuenta con una api key de openai se agrega en este apartado
+### la libreria dispone de dos alternativas para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe recalcar que es obligatorio contar con alguna de estas 2 apis
+
+#### Si se cuenta con una api key de openai este seria el proceso
 ```python
 openai_api_key = ""
 ```
 #### Se inicializa la instancia el recomendador
 ```python
-recommender = CoreRecommendation(openai_key=openai_api_key)
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key)
 ```
 #### De la intancia anterior se crea ruta de persistencia de los recursos
 ```python
-recommender.init_components(collection_name="books",resources=books_dict)
+recommender_open_ai.init_components(collection_name="books",resources=books_dict)
+```
+#### El el caso de usar groq este es el metodo
+```python
+groq_api_key=""
+recommender_groq = CoreRecommendation(groq_key=groq_api_key)
+recommender_groq.init_components(collection_name="books",resources=books_dict)
 ```
 #### Usuario de prueba en formato JSON
 ```python
 user = {
   "user": {
     "id": 234567,
     "name": "Carlos Rodriguez",
@@ -119,12 +125,14 @@
       }
     ]
   }
 }
 ```
 #### Se ejecuta el recomendador con la informacion del usuario
 ```python
-print(recommender.get_recommendation(user=user))
+response = recommender_groq.get_recommendation(user=user)
+print(f"Usuario={response['user']} \n") 
+print(f"Recomendaciones= {response['rec']}")
 ```
```

#### html2text {}

```diff
@@ -1,39 +1,49 @@
 # Sistema de recomendaciÃ³n con agente langchain ## Acerca del proyecto En el
 presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el
 sistema permite recomendar recursos a travÃ©s del uso de mecanismos de
 Procesamiento de lenguaje natura como agentes langchain, IA generatica y
-embeddings. ## Procesos * ConfiguraciÃ³n de ChromaDb - Vector Similarity *
-CreaciÃ³n del mÃ³dulo de generaciÃ³n de embeddings ya sea por openAi o algun
-otro modelo * MÃ³dulo de recomendaciÃ³n generativo con agentes langchain y llms
-## TecnologÃ­as * Python * ChromaDB * Langchain * Llama * HugginFace * pytorch
-* OpenAI * Embeddings * Mistral * GPT ## Prerequisitos * Instalar Python
-(_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener el API KEY de OpenAI (opcional)
-(_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). ## Inicializacion manual * Clonar el repositorio ```sh
-git clone https://github.com/johansquintero/recommender-agent ``` * Crear el
-entorno virtual ```sh python -m venv env ``` * Activar entorno virtual
-(windows): ```sh env\Scripts\activate ``` * Instalar las dependencias del
-proyecto: ```sh pip install -r requirements.txt ``` ## Instalando con pip ```sh
-pip install recommender-agent ``` # Ejemplo de implementacion del sistema ####
-Imports ```python from recommender_agent.recommenderSystem import
+embeddings. ## Procesos * ConfiguraciÃ³n y creacion del modulo de la base de
+datos vectorial con ChromaDb * CreaciÃ³n del mÃ³dulo y configuracion del agente
+Langchain * MÃ³dulo principal de recomendaciÃ³n el cual gestiona e integrar los
+dos anteriores modulos ## TecnologÃ­as * Python * ChromaDB * Langchain * Llama
+* HugginFace * pytorch * OpenAI * Groq * Embeddings * LLM ## Prerequisitos *
+Instalar Python (_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener una API KEY de
+OpenAI (opcional si se va a utilizar Groq) (_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). * Obtener una
+API KEY de groq (opcional si se va a utilizar OpenAI) (_h_t_t_p_s_:_/_/
+_c_o_n_s_o_l_e_._g_r_o_q_._c_o_m_/_k_e_y_s) ## Instalacion manual desde el repositorio * Clonar el
+repositorio ```sh git clone https://github.com/johansquintero/recommender-agent
+``` * Crear el entorno virtual ```sh python -m venv env ``` * Activar entorno
+virtual (windows): ```sh env\Scripts\activate ``` * Instalar las dependencias
+del proyecto: ```sh pip install -r requirements.txt ``` ## Instalando con pip
+```sh pip install recommender-agent ``` # Ejemplo de implementacion del sistema
+#### Imports ```python from recommender_agent.recommenderSystem import
 CoreRecommendation import pandas as pd ``` #### Se importa el dataset de la
 ruta donde este ubicado ```python books = pd.read_csv("../dataset_books/
 Books2.csv") books = books.fillna('') books.drop(columns=
 ["isbn13","thumbnail","subtitle"],axis=1,inplace=True) ``` #### Un requisito es
 que cada uno de los elementos tengan un id ```python books["id"] = books.index
 + 1 ``` #### Se convierte a diccionario el dataset ```python books_dict =
-books.to_dict(orient='records') ``` #### Si se cuenta con una api key de openai
-se agrega en este apartado ```python openai_api_key = "" ``` #### Se inicializa
-la instancia el recomendador ```python recommender = CoreRecommendation
-(openai_key=openai_api_key) ``` #### De la intancia anterior se crea ruta de
-persistencia de los recursos ```python recommender.init_components
+books.to_dict(orient='records') ``` ### la libreria dispone de dos alternativas
+para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe
+recalcar que es obligatorio contar con alguna de estas 2 apis #### Si se cuenta
+con una api key de openai este seria el proceso ```python openai_api_key = ""
+``` #### Se inicializa la instancia el recomendador ```python
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key) ``` #### De
+la intancia anterior se crea ruta de persistencia de los recursos ```python
+recommender_open_ai.init_components
+(collection_name="books",resources=books_dict) ``` #### El el caso de usar groq
+este es el metodo ```python groq_api_key="" recommender_groq =
+CoreRecommendation(groq_key=groq_api_key) recommender_groq.init_components
 (collection_name="books",resources=books_dict) ``` #### Usuario de prueba en
 formato JSON ```python user = { "user": { "id": 234567, "name": "Carlos
 Rodriguez", "email": "carlos_rodriguez@email.com", "address": { "street":
 "Calle Principal", "city": "Barcelona", "state": "Spain", "postal_code":
 "08001" }, "preferences": { "genres": ["Philosophy","Novels", "History"],
 "favorite_authors": ["Dan Brown", "Ken Follett", "RenÃ© Descartes"] },
 "purchase_history": [ { "book": "The Da Vinci Code", "author": "Dan Brown",
 "price": 17.99, "purchase_date": "2023-12-12" }, { "book": "The Pillars of the
 Earth", "author": "Ken Follett", "price": 22.99, "purchase_date": "2024-01-05"
 } ] } } ``` #### Se ejecuta el recomendador con la informacion del usuario
-```python print(recommender.get_recommendation(user=user)) ```
+```python response = recommender_groq.get_recommendation(user=user) print
+(f"Usuario={response['user']} \n") print(f"Recomendaciones= {response['rec']}")
+```
```

### Comparing `recommender-agent-0.2.1/recommender_agent/components/vectorStoreClient.py` & `recommender-agent-0.3.0/recommender_agent/components/vectorStoreClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from langchain.vectorstores import Chroma
+from langchain_community.vectorstores import Chroma
 import os
 import time
 
 class Client:
     def __init__(self, resources:list[dict],collection_name):
         self.resources = resources      
         self.collection_name=collection_name
```

### Comparing `recommender-agent-0.2.1/recommender_agent/recommenderSystem.py` & `recommender-agent-0.3.0/recommender_agent/recommenderSystem.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-from langchain.embeddings import HuggingFaceEmbeddings
+from langchain_community.embeddings import HuggingFaceEmbeddings
 from recommender_agent.components.vectorStoreClient import Client
 from recommender_agent.components.agent import RecommenderAgent
-from langchain.chat_models import ChatOpenAI
-import torch, subprocess
+from langchain_openai import ChatOpenAI
+from langchain_groq import ChatGroq
+import torch
 
 EMBEDDING_MODEL_NAME = "BAAI/bge-base-en-v1.5"
 ENCODE_KWARGS = {'normalize_embeddings': True} # set True to compute cosine similarity
 MODEL_KWARGS = {'device': 'cuda' if torch.cuda.is_available() else 'cpu'}#si esta cuda habilitado se crearan los embeddings con este
 
 HUGGINFACE_MODEL_NAME = "TheBloke/Mistral-7B-OpenOrca-GGUF"
 HUGGINFACE_BASENAME = "mistral-7b-openorca.Q4_K_M.gguf"
 
 OPENAI_MODEL_NAME = "gpt-3.5-turbo-1106"
 
+GROQ_MODEL_NAME = "llama3-70b-8192"
 
 class CoreRecommendation:
-    def __init__(self,openai_key='') -> None:
+    def __init__(self,openai_key='',groq_key='') -> None:
         self.openai_key=openai_key
         self.embeddingModel = HuggingFaceEmbeddings(
             model_name=EMBEDDING_MODEL_NAME,
             encode_kwargs=ENCODE_KWARGS,
             model_kwargs=MODEL_KWARGS
         )
         if(openai_key!=''):
-            print(f"model name = {OPENAI_MODEL_NAME}")
+            print(f"OpenAi model name = {OPENAI_MODEL_NAME}")
             self.llm = ChatOpenAI(temperature=0.3, model_name=OPENAI_MODEL_NAME,api_key = openai_key)
-        else:
-            from langchain.callbacks.manager import CallbackManager
-            from langchain.callbacks.streaming_stdout import StreamingStdOutCallbackHandler
-            from huggingface_hub import hf_hub_download           
-            
-            if torch.cuda.is_available():
-                import os
-                os.system(f"CMAKE_ARGS='-DLLAMA_CUBLAS=on' FORCE_CMAKE=1 pip install llama-cpp-python==0.2.23")
-                                            
-            from langchain.llms import LlamaCpp            
-
-            model_path = hf_hub_download(repo_id=HUGGINFACE_MODEL_NAME, filename=HUGGINFACE_BASENAME)
-            callback_manager = CallbackManager([StreamingStdOutCallbackHandler()])
-            self.llm = LlamaCpp(
-                model_path=model_path,
-                callback_manager=callback_manager,
-                verbose=True, # Verbose is required to pass to the callback manager
-                temperature=0.0,
-                n_batch=2,
-                n_ctx=8000#15000
-            )
+        if(groq_key!=''):
+            print(f"Groq model name = {GROQ_MODEL_NAME}")
+            self.llm = ChatGroq(temperature=0.5, groq_api_key=groq_key, model_name=GROQ_MODEL_NAME)
             
 
     def init_components(self,collection_name:str,resources:list[dict]):
         self.resourcesClient = Client(resources=resources,collection_name=collection_name)
         vectordb = self.resourcesClient.create_collection(embedding_model=self.embeddingModel)
         self.agent = RecommenderAgent(vectordb=vectordb,llm=self.llm)
         self.agent.initAgent()
     
     def get_recommendation(self,user):
         text = self.get_text_for_user(user=user)
         response = self.agent.executeAgent(string=text)
-        return tuple((user, response))
+        
+        user_rec = {
+            "user":user, 
+            "rec":response['output']
+        }
+        return user_rec
     
     def get_recommendatios(self,users):
         responses = []
         for user in users:
             response = self.get_recommendation(user=user)
             responses.append(response)
         return responses
```

### Comparing `recommender-agent-0.2.1/recommender_agent.egg-info/PKG-INFO` & `recommender-agent-0.3.0/recommender_agent.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,50 @@
 Metadata-Version: 2.1
 Name: recommender-agent
-Version: 0.2.1
+Version: 0.3.0
 Summary: En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
 Home-page: https://github.com/johansquintero/recommender-agent
 Author: Johan sebastian quintero rojas
 Author-email: metalium144@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Sistema de recomendaciÃ³n con agente langchain
+# Sistema de recomendación con agente langchain
 
-<!-- ABOUT THE PROJECT -->
 ## Acerca del proyecto
-En el presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el sistema permite recomendar recursos a travÃ©s del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
+En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.
 
 
 ## Procesos 
 
-* ConfiguraciÃ³n de ChromaDb - Vector Similarity
-* CreaciÃ³n del mÃ³dulo de generaciÃ³n de embeddings ya sea por openAi o algun otro modelo
-* MÃ³dulo de recomendaciÃ³n generativo con agentes langchain y llms
+* Configuración y creacion del modulo de la base de datos vectorial con ChromaDb
+* Creación del módulo y configuracion del agente Langchain
+* Módulo principal de recomendación el cual gestiona e integrar los dos anteriores modulos
 
-<!-- GETTING STARTED -->
-## TecnologÃ­as
+## Tecnologías
 
 * Python
 * ChromaDB
 * Langchain
 * Llama
 * HugginFace
 * pytorch
 * OpenAI
+* Groq
 * Embeddings
-* Mistral
-* GPT
+* LLM
 
 
 ## Prerequisitos
-
 * Instalar Python (<a href="https://www.python.org/downloads/">https://www.python.org/downloads/</a>).
-* Obtener el API KEY de OpenAI (opcional) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de OpenAI (opcional si se va a utilizar Groq) (<a href="https://openai.com/">https://openai.com/</a>).
+* Obtener una API KEY de groq (opcional si se va a utilizar OpenAI) (<a href="https://console.groq.com/keys">https://console.groq.com/keys</a>)
 
-## Inicializacion manual
+## Instalacion manual desde el repositorio
 
 * Clonar el repositorio
   ```sh
   git clone https://github.com/johansquintero/recommender-agent
   ```
 
 * Crear el entorno virtual
@@ -82,25 +80,33 @@
 ```python
 books["id"] = books.index + 1
 ```
 #### Se convierte a diccionario el dataset
 ```python
 books_dict = books.to_dict(orient='records') 
 ```
-#### Si se cuenta con una api key de openai se agrega en este apartado
+### la libreria dispone de dos alternativas para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe recalcar que es obligatorio contar con alguna de estas 2 apis
+
+#### Si se cuenta con una api key de openai este seria el proceso
 ```python
 openai_api_key = ""
 ```
 #### Se inicializa la instancia el recomendador
 ```python
-recommender = CoreRecommendation(openai_key=openai_api_key)
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key)
 ```
 #### De la intancia anterior se crea ruta de persistencia de los recursos
 ```python
-recommender.init_components(collection_name="books",resources=books_dict)
+recommender_open_ai.init_components(collection_name="books",resources=books_dict)
+```
+#### El el caso de usar groq este es el metodo
+```python
+groq_api_key=""
+recommender_groq = CoreRecommendation(groq_key=groq_api_key)
+recommender_groq.init_components(collection_name="books",resources=books_dict)
 ```
 #### Usuario de prueba en formato JSON
 ```python
 user = {
   "user": {
     "id": 234567,
     "name": "Carlos Rodriguez",
@@ -109,15 +115,15 @@
       "street": "Calle Principal",
       "city": "Barcelona",
       "state": "Spain",
       "postal_code": "08001"
     },
     "preferences": {
       "genres": ["Philosophy","Novels", "History"],
-      "favorite_authors": ["Dan Brown", "Ken Follett", "RenÃ© Descartes"]
+      "favorite_authors": ["Dan Brown", "Ken Follett", "René Descartes"]
     },
     "purchase_history": [
       {
         "book": "The Da Vinci Code",
         "author": "Dan Brown",
         "price": 17.99,
         "purchase_date": "2023-12-12"
@@ -130,12 +136,14 @@
       }
     ]
   }
 }
 ```
 #### Se ejecuta el recomendador con la informacion del usuario
 ```python
-print(recommender.get_recommendation(user=user))
+response = recommender_groq.get_recommendation(user=user)
+print(f"Usuario={response['user']} \n") 
+print(f"Recomendaciones= {response['rec']}")
 ```
```

#### html2text {}

```diff
@@ -1,47 +1,56 @@
-Metadata-Version: 2.1 Name: recommender-agent Version: 0.2.1 Summary: En el
+Metadata-Version: 2.1 Name: recommender-agent Version: 0.3.0 Summary: En el
 presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el
 sistema permite recomendar recursos a travÃ©s del uso de mecanismos de
 Procesamiento de lenguaje natura como agentes langchain, IA generatica y
 embeddings. Home-page: https://github.com/johansquintero/recommender-agent
 Author: Johan sebastian quintero rojas Author-email: metalium144@gmail.com
 License: MIT Description-Content-Type: text/markdown License-File: LICENSE #
-Sistema de recomendaciÃÂ³n con agente langchain ## Acerca del proyecto En el
-presente proyecto muestro la construcciÃÂ³n de una sistema de
-recomendaciÃÂ³n, el sistema permite recomendar recursos a travÃÂ©s del uso de
-mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA
-generatica y embeddings. ## Procesos * ConfiguraciÃÂ³n de ChromaDb - Vector
-Similarity * CreaciÃÂ³n del mÃÂ³dulo de generaciÃÂ³n de embeddings ya sea
-por openAi o algun otro modelo * MÃÂ³dulo de recomendaciÃÂ³n generativo con
-agentes langchain y llms ## TecnologÃÂ­as * Python * ChromaDB * Langchain *
-Llama * HugginFace * pytorch * OpenAI * Embeddings * Mistral * GPT ##
-Prerequisitos * Instalar Python (_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener
-el API KEY de OpenAI (opcional) (_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). ## Inicializacion manual
-* Clonar el repositorio ```sh git clone https://github.com/johansquintero/
-recommender-agent ``` * Crear el entorno virtual ```sh python -m venv env ``` *
-Activar entorno virtual (windows): ```sh env\Scripts\activate ``` * Instalar
-las dependencias del proyecto: ```sh pip install -r requirements.txt ``` ##
-Instalando con pip ```sh pip install recommender-agent ``` # Ejemplo de
-implementacion del sistema #### Imports ```python from
-recommender_agent.recommenderSystem import CoreRecommendation import pandas as
-pd ``` #### Se importa el dataset de la ruta donde este ubicado ```python books
-= pd.read_csv("../dataset_books/Books2.csv") books = books.fillna('')
-books.drop(columns=["isbn13","thumbnail","subtitle"],axis=1,inplace=True) ```
-#### Un requisito es que cada uno de los elementos tengan un id ```python books
-["id"] = books.index + 1 ``` #### Se convierte a diccionario el dataset
-```python books_dict = books.to_dict(orient='records') ``` #### Si se cuenta
-con una api key de openai se agrega en este apartado ```python openai_api_key =
-"" ``` #### Se inicializa la instancia el recomendador ```python recommender =
-CoreRecommendation(openai_key=openai_api_key) ``` #### De la intancia anterior
-se crea ruta de persistencia de los recursos ```python
-recommender.init_components(collection_name="books",resources=books_dict) ```
-#### Usuario de prueba en formato JSON ```python user = { "user": { "id":
-234567, "name": "Carlos Rodriguez", "email": "carlos_rodriguez@email.com",
-"address": { "street": "Calle Principal", "city": "Barcelona", "state":
-"Spain", "postal_code": "08001" }, "preferences": { "genres":
-["Philosophy","Novels", "History"], "favorite_authors": ["Dan Brown", "Ken
-Follett", "RenÃÂ© Descartes"] }, "purchase_history": [ { "book": "The Da Vinci
-Code", "author": "Dan Brown", "price": 17.99, "purchase_date": "2023-12-12" },
-{ "book": "The Pillars of the Earth", "author": "Ken Follett", "price": 22.99,
-"purchase_date": "2024-01-05" } ] } } ``` #### Se ejecuta el recomendador con
-la informacion del usuario ```python print(recommender.get_recommendation
-(user=user)) ```
+Sistema de recomendaciÃ³n con agente langchain ## Acerca del proyecto En el
+presente proyecto muestro la construcciÃ³n de una sistema de recomendaciÃ³n, el
+sistema permite recomendar recursos a travÃ©s del uso de mecanismos de
+Procesamiento de lenguaje natura como agentes langchain, IA generatica y
+embeddings. ## Procesos * ConfiguraciÃ³n y creacion del modulo de la base de
+datos vectorial con ChromaDb * CreaciÃ³n del mÃ³dulo y configuracion del agente
+Langchain * MÃ³dulo principal de recomendaciÃ³n el cual gestiona e integrar los
+dos anteriores modulos ## TecnologÃ­as * Python * ChromaDB * Langchain * Llama
+* HugginFace * pytorch * OpenAI * Groq * Embeddings * LLM ## Prerequisitos *
+Instalar Python (_h_t_t_p_s_:_/_/_w_w_w_._p_y_t_h_o_n_._o_r_g_/_d_o_w_n_l_o_a_d_s_/). * Obtener una API KEY de
+OpenAI (opcional si se va a utilizar Groq) (_h_t_t_p_s_:_/_/_o_p_e_n_a_i_._c_o_m_/). * Obtener una
+API KEY de groq (opcional si se va a utilizar OpenAI) (_h_t_t_p_s_:_/_/
+_c_o_n_s_o_l_e_._g_r_o_q_._c_o_m_/_k_e_y_s) ## Instalacion manual desde el repositorio * Clonar el
+repositorio ```sh git clone https://github.com/johansquintero/recommender-agent
+``` * Crear el entorno virtual ```sh python -m venv env ``` * Activar entorno
+virtual (windows): ```sh env\Scripts\activate ``` * Instalar las dependencias
+del proyecto: ```sh pip install -r requirements.txt ``` ## Instalando con pip
+```sh pip install recommender-agent ``` # Ejemplo de implementacion del sistema
+#### Imports ```python from recommender_agent.recommenderSystem import
+CoreRecommendation import pandas as pd ``` #### Se importa el dataset de la
+ruta donde este ubicado ```python books = pd.read_csv("../dataset_books/
+Books2.csv") books = books.fillna('') books.drop(columns=
+["isbn13","thumbnail","subtitle"],axis=1,inplace=True) ``` #### Un requisito es
+que cada uno de los elementos tengan un id ```python books["id"] = books.index
++ 1 ``` #### Se convierte a diccionario el dataset ```python books_dict =
+books.to_dict(orient='records') ``` ### la libreria dispone de dos alternativas
+para aplicar un LLM uno por la api de OpenAI y el otro por la api de Groq, cabe
+recalcar que es obligatorio contar con alguna de estas 2 apis #### Si se cuenta
+con una api key de openai este seria el proceso ```python openai_api_key = ""
+``` #### Se inicializa la instancia el recomendador ```python
+recommender_open_ai = CoreRecommendation(openai_key=openai_api_key) ``` #### De
+la intancia anterior se crea ruta de persistencia de los recursos ```python
+recommender_open_ai.init_components
+(collection_name="books",resources=books_dict) ``` #### El el caso de usar groq
+este es el metodo ```python groq_api_key="" recommender_groq =
+CoreRecommendation(groq_key=groq_api_key) recommender_groq.init_components
+(collection_name="books",resources=books_dict) ``` #### Usuario de prueba en
+formato JSON ```python user = { "user": { "id": 234567, "name": "Carlos
+Rodriguez", "email": "carlos_rodriguez@email.com", "address": { "street":
+"Calle Principal", "city": "Barcelona", "state": "Spain", "postal_code":
+"08001" }, "preferences": { "genres": ["Philosophy","Novels", "History"],
+"favorite_authors": ["Dan Brown", "Ken Follett", "RenÃ© Descartes"] },
+"purchase_history": [ { "book": "The Da Vinci Code", "author": "Dan Brown",
+"price": 17.99, "purchase_date": "2023-12-12" }, { "book": "The Pillars of the
+Earth", "author": "Ken Follett", "price": 22.99, "purchase_date": "2024-01-05"
+} ] } } ``` #### Se ejecuta el recomendador con la informacion del usuario
+```python response = recommender_groq.get_recommendation(user=user) print
+(f"Usuario={response['user']} \n") print(f"Recomendaciones= {response['rec']}")
+```
```

### Comparing `recommender-agent-0.2.1/setup.py` & `recommender-agent-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from setuptools import setup, find_packages
 
-with open("README.md", "r") as d:
+with open("README.md", "r",encoding="utf-8") as d:
     description = d.read()
 
 setup(
     name='recommender-agent',
-    version='0.2.1',
+    version='0.3.0',
     license= 'MIT',
     description="En el presente proyecto muestro la construcción de una sistema de recomendación, el sistema permite recomendar recursos a través del uso de mecanismos de Procesamiento de lenguaje natura como agentes langchain, IA generatica y embeddings.",
     long_description= description,
     long_description_content_type="text/markdown",
     author="Johan sebastian quintero rojas",
     install_requires= [
-        'numpy<1.26.0',
-        'langchain==0.0.334',
-        'chromadb==0.4.17',
-        'requests==2.31.0',
-        'huggingface_hub==0.16.4',
-        'scipy==1.9.3',
-        'pandas<2.0.0',
-        'sentence-transformers==2.2.2',
-        'openai<1.0.0',
-        'llama-cpp-python==0.2.11',
-        'torch==2.1.2'
+        'numpy==1.25.2',
+        'pandas==2.0.3',
+        'typer==0.9.4',
+        'scipy==1.11.4',
+        'langchain==0.1.17',
+        'langchain-community==0.0.36',
+        'chromadb==0.5.0',
+        'openai==1.25.1',
+        'langchain_openai==0.1.6',
+        'groq==0.5.0',
+        'langchain-groq==0.1.3',
+        'sentence-transformers==2.7.0',
+        'torch==2.3.0'
     ],
     author_email="metalium144@gmail.com",
     packages=find_packages(),
     url='https://github.com/johansquintero/recommender-agent'
 )
```

