# Comparing `tmp/snapquery-0.0.3.tar.gz` & `tmp/snapquery-0.0.4.tar.gz`

## Comparing `snapquery-0.0.3.tar` & `snapquery-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.3/.project
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.3/.pydevproject
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.3/.github/workflows/build.yml
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.3/.github/workflows/upload-to-pypi.yml
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/blackisort
--rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/install
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.3/scripts/test
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/__init__.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_cmd.py
--rw-r--r--   0        0        0    13540 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_core.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_view.py
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/snapquery_webserver.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.3/snapquery/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_endpoints.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_namedqueries.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 snapquery-0.0.3/tests/test_restful_api.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.3/LICENSE
--rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.3/README.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 snapquery-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 snapquery-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 snapquery-0.0.4/.project
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 snapquery-0.0.4/.pydevproject
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snapquery-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 snapquery-0.0.4/.github/workflows/upload-to-pypi.yml
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/blackisort
+-rwxr-xr-x   0        0        0       42 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/install
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snapquery-0.0.4/scripts/test
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/scholia.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_cmd.py
+-rw-r--r--   0        0        0    15268 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_core.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_view.py
+-rw-r--r--   0        0        0     7292 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/snapquery_webserver.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 snapquery-0.0.4/snapquery/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_cmdline.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_namedqueries.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_restful_api.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_scholia.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 snapquery-0.0.4/tests/test_wd_query_parsing.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 snapquery-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snapquery-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 snapquery-0.0.4/README.md
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 snapquery-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 snapquery-0.0.4/PKG-INFO
```

### Comparing `snapquery-0.0.3/.github/workflows/build.yml` & `snapquery-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.3/.github/workflows/upload-to-pypi.yml` & `snapquery-0.0.4/.github/workflows/upload-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.3/snapquery/snapquery_cmd.py` & `snapquery-0.0.4/snapquery/snapquery_cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+
 import sys
 from argparse import ArgumentParser
 
-from lodstorage.query import EndpointManager, Format, Query
+from lodstorage.query import EndpointManager, Format
 from ngwidgets.cmd import WebserverCmd
 
 from snapquery.snapquery_core import NamedQueryManager
 from snapquery.snapquery_webserver import SnapQueryWebServer
 
 
 class SnapQueryCmd(WebserverCmd):
@@ -30,27 +31,30 @@
             default=None,
             help="path to yaml file to configure endpoints to use for queries",
         )
         parser.add_argument(
             "-en",
             "--endpointName",
             default="wikidata",
-            help=f"Name of the endpoint to use for queries - use --listEndpoints to list available endpoints",
+            help="Name of the endpoint to use for queries - use --listEndpoints to list available endpoints",
         )
         parser.add_argument(
             "-le",
             "--listEndpoints",
             action="store_true",
             help="show the list of available endpoints",
         )
         parser.add_argument(
             "--limit", type=int, default=None, help="set limit parameter of query"
         )
         parser.add_argument(
-            "--namespace", type=str, default="wikidata-examples", help="namespace to filter queries"
+            "--namespace",
+            type=str,
+            default="wikidata-examples",
+            help="namespace to filter queries",
         )
         parser.add_argument("-qn", "--queryName", help="run a named query")
         parser.add_argument("-f", "--format", type=Format, choices=list(Format))
         return parser
 
     def handle_args(self) -> bool:
         """
@@ -62,21 +66,28 @@
         # Check if listing of endpoints is requested
         if self.args.listEndpoints:
             # List endpoints
             for endpoint in endpoints.values():
                 print(endpoint)
             handled = True  # Operation handled
         elif self.args.queryName is not None:
-            nqm = NamedQueryManager()
-            namespace=self.args.namespace
+            nqm = NamedQueryManager.from_samples()
+            namespace = self.args.namespace
             name = self.args.queryName
             endpoint_name = self.args.endpointName
             r_format = self.args.format
-            limit=self.args.limit
-            formatted_result=nqm.formatted_query(name, namespace=namespace,endpoint_name=endpoint_name, r_format=r_format,limit=limit)
+            limit = self.args.limit
+            qb = nqm.get_query(
+                name=name, namespace=namespace, endpoint_name=endpoint_name, limit=limit
+            )
+            if r_format==Format.raw:
+                formatted_result=qb.raw_query()
+            else:
+                qlod = qb.get_lod()
+                formatted_result = qb.format_result(qlod=qlod, r_format=r_format)
             print(formatted_result)
             return handled
 
 
 def main(argv: list = None):
     """
     main call
```

### Comparing `snapquery-0.0.3/snapquery/snapquery_core.py` & `snapquery-0.0.4/snapquery/snapquery_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+
 import json
-import re
 import os
+import re
+import requests
 from dataclasses import field
 from pathlib import Path
 from typing import Any, Dict, List, Optional
 
 from lodstorage.csv import CSV
 from lodstorage.query import Endpoint, EndpointManager, Format, Query
 from lodstorage.sparql import SPARQL
@@ -34,29 +36,34 @@
 
     query_id: str = field(init=False)
 
     # namespace
     namespace: str
     # name/id
     name: str
-    # one line title
-    title: str
-    # multiline description
-    description: str
     # sparql query (to be hidden later)
     sparql: str
-
+    # the url of the source code of the query 
+    url: Optional[str]=None
+    # one line title
+    title: Optional[str]=None
+    # multiline description
+    description: Optional[str]=None
+  
     def __post_init__(self):
         """
         Post-initialization processing to construct a unique identifier for the query
         based on its namespace and name.
         """
         self.query_id = f"{self.namespace}.{self.name}"
 
     def as_link(self) -> str:
+        """
+        get me as a link
+        """
         url = f"/query/{self.namespace}/{self.name}"
         text = self.name
         tooltip = "query details"
         link = Link.create(url, text, tooltip)
         return link
 
     @classmethod
@@ -64,30 +71,156 @@
         """
         Class method to instantiate NamedQuery from a dictionary record.
         """
         return cls(
             namespace=record["namespace"],
             name=record["name"],
             title=record["title"],
+            url=record["url"],
             description=record["description"],
             sparql=record["sparql"],
         )
+        
+    def as_record(self)->Dict:
+        record = {
+            "namespace": self.namespace,
+            "name": self.name,
+            "url": self.url,
+            "title": self.title,
+            "description": self.description,
+            "sparql": self.sparql,
+        }
+        return record
 
     def as_viewrecord(self) -> Dict:
         """
         Return a dictionary representing the NamedQuery with keys ordered as Name, Namespace, Title, Description.
         """
         return {
             "name": self.as_link(),
             "namespace": self.namespace,
             "title": self.title,
             "description": self.description,
+            "url": self.url
         }
 
 
+class QueryBundle:
+    """
+    Bundles a named query, a query, and an endpoint into a single manageable object, facilitating the execution of SPARQL queries.
+
+    Attributes:
+        named_query (NamedQuery): The named query object, which includes metadata about the query.
+        query (Query): The actual query object that contains the SPARQL query string.
+        endpoint (Endpoint): The endpoint object where the SPARQL query should be executed.
+        sparql (SPARQL): A SPARQL service object initialized with the endpoint URL.
+    """
+
+    def __init__(self, named_query: NamedQuery, query: Query, endpoint: Endpoint):
+        """
+        Initializes a new instance of the QueryBundle class.
+
+        Args:
+            named_query (NamedQuery): An instance of NamedQuery that provides a named reference to the query.
+            query (Query): An instance of Query containing the SPARQL query string.
+            endpoint (Endpoint): An instance of Endpoint representing the SPARQL endpoint URL.
+        """
+        self.named_query = named_query
+        self.query = query
+        self.endpoint = endpoint
+        self.sparql = SPARQL(endpoint.endpoint)
+        
+    def raw_query(self,resultFormat, mime_type:str=None, timeout:float=10.0):
+        """
+        returns raw result of the endpoint
+
+        Args:
+            resultFormat(str): format of the result
+            mime_type(str): mime_type to use (if any)
+            timeout(float): timeout in seconds
+
+        Returns:
+            raw result of the query
+        """
+        params = {"query": self.query.query, "format": resultFormat}
+        payload = {}
+        if mime_type:
+            headers = {"Accept": mime_type}
+        else:
+            headers = {}
+        endpoint_url = self.endpoint.endpoint
+        method = self.endpoint.method
+        response = requests.request(
+            method, endpoint_url, headers=headers, data=payload, params=params,timeout=timeout
+        )
+        return response.text
+
+    def get_lod(self) -> List[dict]:
+        """
+        Executes the stored query using the SPARQL service and returns the results as a list of dictionaries.
+
+        Returns:
+            List[dict]: A list where each dictionary represents a row of results from the SPARQL query.
+        """
+        lod = self.sparql.queryAsListOfDicts(self.query.query)
+        return lod
+
+    def format_result(
+        self,
+        qlod: List[Dict[str, Any]] = None,
+        r_format: Format = Format.json,
+    ) -> Optional[str]:
+        """
+        Formats the query results based on the specified format and prints them.
+
+        Args:
+            qlod (List[Dict[str, Any]]): The list of dictionaries that represent the query results.
+            query (Query): The query object which contains details like the endpoint and the database.
+            r_format(Format): The format in which to print the results.
+
+        Returns:
+            Optional[str]: The formatted string representation of the query results, or None if printed directly.
+        """
+        if qlod is None:
+            qlod = self.get_lod()
+        if r_format is None:
+            r_format = Format.json
+        if r_format == Format.csv:
+            csv_output = CSV.toCSV(qlod)
+            return csv_output
+        elif r_format in [Format.latex, Format.github, Format.mediawiki, Format.html]:
+            doc = self.query.documentQueryResult(
+                qlod, tablefmt=str(r_format), floatfmt=".0f"
+            )
+            return doc.asText()
+        elif r_format == Format.json:
+            return json.dumps(qlod, indent=2, sort_keys=True, default=str)
+        return None  # In case no format is matched or needed
+
+    def set_limit(self, limit: int = None):
+        """
+        set the limit of my query
+        
+        Args:
+            limit(int): the limit to set - default: None
+        """
+        if limit:
+            sparql_query = self.query.query
+            # @TODO - this is too naive for cases where
+            # there are SPARQL elements hat have a "limit" in the name e.g. "height_limit"
+            # or if there is a LIMIT in a subquery
+            if "limit" in sparql_query or "LIMIT" in sparql_query:
+                sparql_query = re.sub(
+                    r"(limit|LIMIT)\s+(\d+)", f"LIMIT {limit}", sparql_query
+                )
+            else:
+                sparql_query += f"\nLIMIT {limit}"
+            self.query.query = sparql_query
+
+
 class NamedQueryManager:
     """
     Manages the storage, retrieval, and execution of named SPARQL queries.
     """
 
     def __init__(self, db_path: str = None, debug: bool = False):
         """
@@ -132,54 +265,66 @@
         """
         if db_path is None:
             db_path = cls.get_cache_path()
 
         nqm = NamedQueryManager(debug=debug)
         path_obj = Path(db_path)
         if not path_obj.exists() or path_obj.stat().st_size == 0:
-            sample_queries = cls.get_samples()
-            list_of_records = []
-            for _query_name, named_query in sample_queries.items():
-                record = {
-                    "namespace": named_query.namespace,
-                    "name": named_query.name,
-                    "title": named_query.title,
-                    "description": named_query.description,
-                    "sparql": named_query.sparql,
-                }
-                list_of_records.append(record)
+            sample_records=cls.get_sample_records()
             entityInfo = EntityInfo(
-                list_of_records, name="NamedQuery", primaryKey="query_id"
+                sample_records, name="NamedQuery", primaryKey="query_id"
             )
-            nqm.sql_db.createTable(list_of_records, "NamedQuery", withDrop=True)
-            nqm.sql_db.store(list_of_records, entityInfo)
+            nqm.sql_db.createTable(sample_records, "NamedQuery", withDrop=True)
+            nqm.sql_db.store(sample_records, entityInfo)
         return nqm
+    
+    def store(self,lod):
+        """
+        store the given list of dicts
+        """
+        sample_records=NamedQueryManager.get_sample_records()
+        entityInfo = EntityInfo(
+            sample_records, name="NamedQuery", primaryKey="query_id"
+        )
+        self.sql_db.store(lod, entityInfo,fixNone=True,replace=True)
+        
+    @classmethod
+    def get_sample_records(cls):
+        sample_queries = cls.get_samples()
+        list_of_records = []
+        for _query_name, named_query in sample_queries.items():
+            record=named_query.as_record()
+            list_of_records.append(record)
+        return list_of_records
+
 
     @classmethod
     def get_samples(cls) -> dict[str, NamedQuery]:
         """
         get samples
         """
         samples = {
             "wikidata-examples.cats": NamedQuery(
                 namespace="wikidata-examples",
                 name="cats",
+                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Cats",
                 title="Cats on Wikidata",
                 description="This query retrieves all items classified under 'house cat' (Q146) on Wikidata.",
                 sparql="""
 SELECT ?item ?itemLabel
 WHERE {
   ?item wdt:P31 wd:Q146. # Must be a cat
   SERVICE wikibase:label { bd:serviceParam wikibase:language "[AUTO_LANGUAGE],en". }
 }
 """,
             ),
             "wikidata-examples.horses": NamedQuery(
                 namespace="wikidata-examples",
                 name="horses",
+                url="https://www.wikidata.org/wiki/Wikidata:SPARQL_query_service/queries/examples#Horses_(showing_some_info_about_them)",
                 title="Horses on Wikidata",
                 description="This query retrieves information about horses, including parents, gender, and approximate birth and death years.",
                 sparql="""
 SELECT DISTINCT ?horse ?horseLabel ?mother ?motherLabel ?father ?fatherLabel 
 (year(?birthdate) as ?birthyear) (year(?deathdate) as ?deathyear) ?genderLabel
 WHERE {
   ?horse wdt:P31/wdt:P279* wd:Q726 .     # Instance and subclasses of horse (Q726)
@@ -194,22 +339,28 @@
 }
 ORDER BY ?horse
 """,
             ),
         }
         return samples
 
-    def get_sparql(
-        self,
-        name: str,
-        namespace: str = "wikidata-examples",
-        endpoint_name: str = "wikidata",
-    ) -> str:
-        sql_query = f"""SELECT 
-    sparql 
+    def lookup(self, name: str, namespace: str) -> NamedQuery:
+        """
+        lookup the named query for the given name and namespace
+
+
+        Args:
+            name (str): The name of the named query to execute.
+            namespace (str): The namespace of the named query, default is 'wikidata-examples'.
+
+        Returns:
+            NamedQuery: the named query
+        """
+        sql_query = """SELECT 
+    *
 FROM 
     NamedQuery 
 WHERE 
     name = ? AND namespace = ?"""
         query_records = self.sql_db.query(sql_query, (name, namespace))
 
         if not query_records:
@@ -217,138 +368,53 @@
             raise ValueError(msg)
 
         query_count = len(query_records)
         if query_count != 1:
             msg = f"multiple entries ({query_count}) for name '{name}' and namespace '{namespace}'"
             raise ValueError(msg)
 
-        sparql_query = query_records[0]["sparql"]
-        return sparql_query
+        record = query_records[0]
+        named_query = NamedQuery.from_record(record)
+        return named_query
 
-    def query(
+    def get_query(
         self,
         name: str,
         namespace: str = "wikidata-examples",
         endpoint_name: str = "wikidata",
-        limit:int=None
-    ):
+        limit: int = None,
+    ) -> QueryBundle:
         """
-        Execute a named SPARQL query using a specified endpoint and return the results.
+        get the query for the given parameters
 
         Args:
             name (str): The name of the named query to execute.
             namespace (str): The namespace of the named query, default is 'wikidata-examples'.
             endpoint_name (str): The name of the endpoint to send the SPARQL query to, default is 'wikidata'.
             limit(int): the query limit (if any)
 
         Returns:
-            Dict[str, Any]: The results of the SPARQL query in JSON format.
-
-        Raises:
-            ValueError: If no named query matches the given name and namespace.
-            Exception: If the SPARQL query execution fails or the endpoint returns an error.
+            QueryBundle: named_query, query and endpoint
         """
-        sparql_query = self.get_sparql(name, namespace, endpoint_name)
-
-        if not endpoint_name in self.endpoints:
+        named_query = self.lookup(name, namespace)
+        if endpoint_name not in self.endpoints:
             msg = f"Invalid endpoint {endpoint_name}"
             ValueError(msg)
         endpoint = self.endpoints.get(endpoint_name)
-        self.query = Query(name=name, query=sparql_query, lang="sparql",limit=limit)
- 
-        sparql = SPARQL(endpoint.endpoint)
-        if limit: 
-            # @TODO - this is to naive for cases where there are 
-            # SPARQL elements hat have a "limit" in the name e.g. "height_limit"
-            if "limit" in sparql_query or "LIMIT" in sparql_query:
-                sparql_query = re.sub(
-                    r"(limit|LIMIT)\s+(\d+)", f"LIMIT {limit}", sparql_query
-                )
-            else:
-                sparql_query += f"\nLIMIT {limit}"
-        lod = sparql.queryAsListOfDicts(sparql_query)
-        return lod
-    
-    def formatted_query(self,
-        name: str,
-        namespace: str = "wikidata-examples",
-        endpoint_name: str = "wikidata",
-        r_format: Format = Format.html,
-        limit:int=None)->str:
-        """
-        Execute a named SPARQL query using a specified endpoint and return the results formatted .
-
-        Args:
-            name (str): The name of the named query to execute.
-            namespace (str): The namespace of the named query, default is 'wikidata-examples'.
-            endpoint_name (str): The name of the endpoint to send the SPARQL query to, default is 'wikidata'.
-            r_format: (Format): the format to result should be returned in
-            limit(int): the query limit (if any)
-        Returns:
-            str: The results of the SPARQL query in the given format.
-
-        Raises:
-            ValueError: If no named query matches the given name and namespace.
-            Exception: If the SPARQL query execution fails or the endpoint returns an error.
-        """
-        qlod = self.query(endpoint_name=endpoint_name, name=name,namespace=namespace,limit=limit)
-        formatted_result=self.format_result(qlod=qlod, query=self.query, r_format=r_format, endpoint_name=endpoint_name)
-        return formatted_result
-
-    def format_result(
-        self,
-        qlod: List[Dict[str, Any]],
-        query: Query,
-        r_format: Format,
-        endpoint_name: str = "wikidata",
-    ) -> Optional[str]:
-        """
-        Formats the query results based on the specified format and prints them.
-
-        Args:
-            qlod (List[Dict[str, Any]]): The list of dictionaries that represent the query results.
-            query (Query): The query object which contains details like the endpoint and the database.
-            r_format_str(Format): The format in which to print the results.
-            endpoint_name (str): The name of the endpoint to be used, defaults to "wikidata".
-
-        Returns:
-            Optional[str]: The formatted string representation of the query results, or None if printed directly.
-        """
-        # Retrieve endpoint configuration using the provided endpoint name
+        sparql_query = named_query.sparql
+        query = Query(
+            name=name,
+            query=sparql_query,
+            lang="sparql",
+            endpoint=endpoint.endpoint,
+            limit=limit,
+        )
         endpointConf = self.endpoints.get(endpoint_name, Endpoint.getDefault())
         query.tryItUrl = endpointConf.website
         query.database = endpointConf.database
-
-        if r_format == Format.csv:
-            csv_output = CSV.toCSV(qlod)
-            return csv_output
-        elif r_format in [Format.latex, Format.github, Format.mediawiki, Format.html]:
-            doc = query.documentQueryResult(
-                qlod, tablefmt=str(r_format), floatfmt=".0f"
-            )
-            return doc.asText()
-        elif r_format == Format.json:
-            return json.dumps(qlod, indent=2, sort_keys=True, default=str)
-        return None  # In case no format is matched or needed
-
-    def print_result(
-        self,
-        qlod: List[Dict[str, Any]],
-        query: Query,
-        r_format_str: str,
-        endpoint_name: str = "wikidata",
-    ) -> None:
-        """
-        Prints the formatted results of a query.
-
-        Args:
-            qlod (List[Dict[str, Any]]): The list of dictionaries that represent the query results.
-            query (Query): The query object which contains details such as the endpoint and the database.
-            r_format_str: The format in which to print the results.
-            endpoint_name (str): The name of the endpoint to be used, defaults to "wikidata".
-
-        Returns:
-            None
-        """
-        result_str = self.format_result(qlod, query, r_format_str, endpoint_name)
-        if result_str is not None:
-            print(result_str)
+        query_bundle = QueryBundle(
+            named_query=named_query, 
+            query=query, 
+            endpoint=endpoint
+        )
+        query_bundle.set_limit(limit)
+        return query_bundle
```

### Comparing `snapquery-0.0.3/snapquery/snapquery_webserver.py` & `snapquery-0.0.4/snapquery/snapquery_webserver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Created on 2024-05-03
 @author: wf
 """
+
 from fastapi import HTTPException
 from fastapi.responses import HTMLResponse, PlainTextResponse
-from lodstorage.query import Query, Format
+from lodstorage.query import Format
 from ngwidgets.input_webserver import InputWebserver, InputWebSolution, WebserverConfig
-from nicegui import app
+from nicegui import app, ui
 from nicegui.client import Client
 
 from snapquery.snapquery_core import NamedQueryManager
-from snapquery.snapquery_view import NamedQuerySearch
+from snapquery.snapquery_view import NamedQuerySearch, NamedQueryView
 from snapquery.version import Version
 
 
 class SnapQueryWebServer(InputWebserver):
     """
     server to supply named Queries
     """
@@ -36,84 +37,129 @@
         return server_config
 
     def __init__(self):
         """Constructs all the necessary attributes for the WebServer object."""
         InputWebserver.__init__(self, config=SnapQueryWebServer.get_config())
         self.nqm = NamedQueryManager.from_samples()
 
-        @app.get("/sparql/{namespace}/{name}")
-        def sparql(namespace: str, name: str) -> PlainTextResponse:
+        @ui.page("/query/{namespace}/{name}")
+        async def query_page(
+            client: Client,
+            namespace: str,
+            name: str,
+            endpoint_name: str = "wikidata",
+            limit: int = None,
+            format: str = "html",
+        ):
+            """
+            show the query page for the given namespace and name
+            """
+            return await self.page(
+                client,
+                SnapQuerySolution.query_page,
+                namespace=namespace,
+                name=name,
+                endpoint_name=endpoint_name,
+                limit=limit,
+                r_format_str=format,
+            )
+
+        @app.get("/api/sparql/{namespace}/{name}")
+        def sparql(
+            namespace: str,
+            name: str,
+            endpoint_name: str = "wikidata",
+            limit: int = None,
+        ) -> PlainTextResponse:
             """
             Gets a SPARQL query by name within a specified namespace
 
             Args:
                 namespace (str): The namespace identifying the group or category of the query.
                 name (str): The specific name of the query to be executed.
-
+                endpoint_name(str): the name of the endpoint to use
+                limit(int): a limit to set, default=None
             Returns:
                 HTMLResponse: The plain text SPARQL code
 
             Raises:
                 HTTPException: If the query cannot be found or fails to execute.
             """
-            endpoint_name = "wikidata"
-            sparql_query = self.nqm.get_sparql(name, namespace, endpoint_name)
+            qb = self.nqm.get_query(name, namespace, endpoint_name, limit)
+            sparql_query = qb.query.query
             return PlainTextResponse(sparql_query)
 
-        @app.get("/query/{namespace}/{name}")
-        def query(namespace: str, name: str) -> HTMLResponse:
+        @app.get("/api/query/{namespace}/{name}")
+        def query(
+            namespace: str,
+            name: str,
+            endpoint_name: str = "wikidata",
+            limit: int = None,
+        ) -> HTMLResponse:
             """
             Executes a SPARQL query by name within a specified namespace, formats the results, and returns them as an HTML response.
 
             Args:
                 namespace (str): The namespace identifying the group or category of the query.
                 name (str): The specific name of the query to be executed.
+                endpoint_name(str): the name of the endpoint to use
+                limit(int): a limit to set, default=None
 
             Returns:
                 HTMLResponse: The HTML formatted response containing the results of the query execution.
 
             Raises:
                 HTTPException: If the query cannot be found or fails to execute.
             """
-            content = self.query(namespace, name)
+            content = self.query(
+                namespace, name, endpoint_name=endpoint_name, limit=limit
+            )
             if not content:
                 raise HTTPException(status_code=500, detail="Could not create result")
 
             # Return the content as an HTML response
             return HTMLResponse(content)
 
-    def query(self, namespace: str, name: str):
-        """ """
-        endpoint_name = "wikidata"
+    def query(
+        self,
+        namespace: str,
+        name: str,
+        endpoint_name: str = "wikidata",
+        limit: int = None,
+    ) -> str:
+        """
+        Queries an external API to retrieve data based on a given namespace and name.
+
+        Args:
+            namespace (str): The namespace to which the query belongs. It helps in categorizing the data.
+            name (str): The name identifier of the data to be queried.
+            endpoint_name (str): The name of the endpoint to be used for the query. Defaults to 'wikidata'.
+            limit(int): the limit for the query default: None
+
+            Returns:
+                str: the content retrieved
+        """
         # content negotiation
         # Determine response format by extension in the name or Accept header
         if "." in name:
             r_format_str = name.split(".")[-1]
             name = name[: name.rfind(".")]
         else:
             r_format_str = "html"
 
-        # Retrieve the SPARQL query string using the namespace and name.
         try:
-            sparql_query = self.nqm.get_sparql(name, namespace, endpoint_name)
-            qlod = self.nqm.query(
-                name=name, namespace=namespace, endpoint_name=endpoint_name
-            )
-            query = Query(name=name, query=sparql_query, lang="sparql")
+            r_format = Format[r_format_str]
+            qb = self.nqm.get_query(name, namespace, endpoint_name, limit)
+            qlod = qb.get_lod()
+            content = qb.format_result(qlod, r_format)
+            return content
         except Exception as e:
             # Handling specific exceptions can be more detailed based on what nqm.get_sparql and nqm.query can raise
             raise HTTPException(status_code=404, detail=str(e))
 
-        # Format the results and generate HTML content
-        r_format = Format[r_format_str]
-        content = self.nqm.format_result(
-            qlod, query, r_format, endpoint_name=endpoint_name
-        )
-        return content
-
 
 class SnapQuerySolution(InputWebSolution):
     """
     the Snap Query solution
     """
 
     def __init__(self, webserver: SnapQueryWebServer, client: Client):
@@ -146,7 +192,23 @@
     async def home(
         self,
     ):
         """Generates the home page with a selection of examples and
         svg display
         """
         await self.setup_content_div(self.setup_ui)
+
+    async def query_page(
+        self,
+        namespace: str,
+        name: str,
+        endpoint_name: str = "wikidata",
+        limit: int = None,
+        r_format_str: str = "html",
+    ):
+        def show():
+            query_bundle = self.nqm.get_query(name, namespace, endpoint_name, limit)
+            self.named_query_view = NamedQueryView(
+                self, query_bundle=query_bundle, r_format_str=r_format_str
+            )
+
+        await self.setup_content_div(show)
```

### Comparing `snapquery-0.0.3/snapquery/version.py` & `snapquery-0.0.4/snapquery/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 2024-05-01
 
 @author: wf
 """
+
 from dataclasses import dataclass
 
 import snapquery
 
 
 @dataclass
 class Version:
@@ -22,15 +23,15 @@
 
     authors = "Wolfgang Fahl"
 
     doc_url = "https://wiki.bitplan.com/index.php/snapquery"
     chat_url = "https://github.com/WolfgangFahl/snapquery/discussions"
     cm_url = "https://github.com/WolfgangFahl/snapquery"
 
-    license = f"""Copyright 2024 contributors. All rights reserved.
+    license = """Copyright 2024 contributors. All rights reserved.
 
   Licensed under the Apache License 2.0
   http://www.apache.org/licenses/LICENSE-2.0
 
   Distributed on an "AS IS" basis without warranties
   or conditions of any kind, either express or implied."""
```

### Comparing `snapquery-0.0.3/tests/test_endpoints.py` & `snapquery-0.0.4/tests/test_endpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+
 from lodstorage.query import EndpointManager
 from ngwidgets.basetest import Basetest
 
 
 class TestEndpoints(Basetest):
     """
     test endpoint handling according to https://github.com/WolfgangFahl/snapquery/issues/1
```

### Comparing `snapquery-0.0.3/tests/test_namedqueries.py` & `snapquery-0.0.4/tests/test_namedqueries.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+
 import json
 
 from ngwidgets.basetest import Basetest
 
 from snapquery.snapquery_core import NamedQueryManager
 
 
 class TestNamedQueryManager(Basetest):
     """
-    test the named query Manage
+    test the named query Manager
     """
 
     def setUp(self, debug=False, profile=True):
         Basetest.setUp(self, debug=debug, profile=profile)
 
     def testNamedQueries(self):
         """
         test getting a named query manager
         """
         db_path = "/tmp/named_queries.db"
         nqm = NamedQueryManager.from_samples(db_path=db_path)
         for name, ex_count in [("x-invalid", -1), ("cats", 223)]:
             try:
-                lod = nqm.query(name)
+                query_bundle = nqm.get_query(name)
+                lod = query_bundle.get_lod()
                 if self.debug:
                     print(f"{name}:")
                     print(json.dumps(lod, default=str, indent=2))
                 self.assertEqual(ex_count, len(lod))
             except Exception as ex:
                 if self.debug:
                     print(f"{name}:Exception {str(ex)}")
```

### Comparing `snapquery-0.0.3/tests/test_restful_api.py` & `snapquery-0.0.4/tests/test_restful_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Created on 2024-05-03
 
 @author: wf
 """
+
 from ngwidgets.webserver_test import WebserverTest
 
 from snapquery.snapquery_cmd import SnapQueryCmd
 from snapquery.snapquery_webserver import SnapQueryWebServer
 
 
 class TestRestFulApi(WebserverTest):
@@ -28,22 +29,22 @@
         self.assertTrue("Swagger" in html)
 
     def testSparqlApi(self):
         """
         test the plaintext SPARQL API
         """
         for example in ["cats", "horses"]:
-            path = f"/sparql/wikidata-examples/{example}"
+            path = f"/api/sparql/wikidata-examples/{example}?limit=10"
             sparql_query = self.getHtml(path)
             if self.debug:
                 print(sparql_query)
             self.assertTrue("SELECT" in sparql_query)
 
     def testQueryApi(self):
         """
         test the RESTFul Query API
         """
-        for r_format in ["mediawiki", "github", "latex", "html"]:
-            path = f"/query/wikidata-examples/cats.{r_format}"
-            html = self.getHtml(path)
+        for r_format in ["mediawiki", "github", "latex", "html", "json"]:
+            path = f"/api/query/wikidata-examples/cats.{r_format}?limit=10"
+            result = self.getHtml(path)
             if self.debug:
-                print(html)
+                print(result)
```

### Comparing `snapquery-0.0.3/.gitignore` & `snapquery-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.3/LICENSE` & `snapquery-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.3/README.md` & `snapquery-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `snapquery-0.0.3/pyproject.toml` & `snapquery-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,18 @@
   { name = "Wolfgang Fahl", email = "wf@WolfgangFahl.com" },
 ]
 readme = "README.md"
 license = {text = "Apache-2.0"}
 dependencies = [
 	# https://github.com/WolfgangFahl/nicegui_widgets
 	"ngwidgets>=0.14.2",
-  # https://pypi.org/project/pyLodStorage/
-  "pyLodStorage>=0.10.4"
+    # https://pypi.org/project/pyLodStorage/
+    "pyLodStorage>=0.10.5",
+    "wikitextparser",
+    "requests"
 ]
 
 requires-python = ">=3.9"
 classifiers=[
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `snapquery-0.0.3/PKG-INFO` & `snapquery-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snapquery
-Version: 0.0.3
+Version: 0.0.4
 Summary: snapquery: Introduce Named Queries and Named Query Middleware to wikidata
 Project-URL: Home, https://github.com/WolfgangFahl/snapquery
 Project-URL: Documentation, https://wiki.bitplan.com/index.php/snapquery
 Project-URL: Source, https://github.com/WolfgangFahl/snapquery
 Author-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 Maintainer-email: Wolfgang Fahl <wf@WolfgangFahl.com>
 License: Apache-2.0
@@ -21,15 +21,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.9
 Requires-Dist: ngwidgets>=0.14.2
-Requires-Dist: pylodstorage>=0.10.4
+Requires-Dist: pylodstorage>=0.10.5
+Requires-Dist: requests
+Requires-Dist: wikitextparser
 Provides-Extra: test
 Requires-Dist: green; extra == 'test'
 Description-Content-Type: text/markdown
 
 # snapQuery
 Tool that helps users preview, annotate, rate, comment, run and explore Wikidata queries on different sparql backends seamlessly. 
 It enhances the user experience by storing the results and comparing the results from different backends and comparing over time.
```

