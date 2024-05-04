# Comparing `tmp/sysrev-1.3.5.tar.gz` & `tmp/sysrev-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.3.5.tar", last modified: Sat Apr 20 01:04:13 2024, max compression
+gzip compressed data, was "sysrev-1.3.6.tar", last modified: Sat May  4 23:39:59 2024, max compression
```

## Comparing `sysrev-1.3.5.tar` & `sysrev-1.3.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 01:04:13.198064 sysrev-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-20 01:04:07.000000 sysrev-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 01:04:13.198064 sysrev-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-20 01:04:07.000000 sysrev-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.194064 sysrev-1.3.5/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 01:04:07.000000 sysrev-1.3.5/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-04-20 01:04:07.000000 sysrev-1.3.5/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-20 01:04:13.000000 sysrev-1.3.5/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:04:13.198064 sysrev-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-20 01:04:07.000000 sysrev-1.3.5/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-20 01:04:07.000000 sysrev-1.3.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:39:59.815853 sysrev-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 23:39:59.815853 sysrev-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-04 23:39:54.000000 sysrev-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 23:39:59.815853 sysrev-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-04 23:39:54.000000 sysrev-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:39:59.815853 sysrev-1.3.6/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 23:39:54.000000 sysrev-1.3.6/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-05-04 23:39:54.000000 sysrev-1.3.6/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:39:59.815853 sysrev-1.3.6/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-04 23:39:59.000000 sysrev-1.3.6/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 23:39:59.815853 sysrev-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-04 23:39:54.000000 sysrev-1.3.6/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-04 23:39:54.000000 sysrev-1.3.6/tests/test_utils.py
```

### Comparing `sysrev-1.3.5/PKG-INFO` & `sysrev-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.5
+Version: 1.3.6
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.5/setup.py` & `sysrev-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.3.5',
+    version='1.3.6',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.3.5/sysrev/client.py` & `sysrev-1.3.6/sysrev/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,99 @@
         if label_type == 'boolean':
             return self.handle_boolean(label_value)
         elif label_type in ['categorical', 'string']:
             return self.handle_categorical_or_string(label_value)
         else:
             raise ValueError("Invalid label type")
 
+        
+class Client():
+    
+    def __init__(self, api_key, base_url="https://www.sysrev.com"):
+        self.api_key = api_key
+        self.base_url = base_url
+        
+    def sync(self, project_id):
+        Synchronizer().sync(self, project_id)
+    
+    def get_project_info(self, project_id):
+        endpoint = f"{self.base_url}/api-json/project-info"
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        response = requests.get(endpoint, headers=headers, params={"project-id": project_id})
+        return response.json()
+    
+    def get_labels(self, project_id):
+        raw_labels = self.get_project_info(project_id)['result']['project']['labels']
+        labels = [{"label_id": label_id} | raw_labels[label_id] for label_id in raw_labels.keys()]
+        return labels
+    
+    def set_labels(self, project_id, article_id, label_ids, label_values, label_types, confirm=False, change=False, resolve=False):
+        endpoint = f"{self.base_url}/api-json/set-labels"
+        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        
+        assert len(label_ids) == len(label_values) == len(label_types), "Length of label_ids, label_values, and label_types should be the same."
+        
+        # construct label_values_dict
+        tf = LabelTransformer()
+        label_values_dict = {label_ids[i]: tf.transform_label(label_types[i], label_values[i]) for i in range(len(label_ids))}    
+        
+        # Constructing the data payload as per the server's expectation
+        data = {"project-id": project_id, "article-id": article_id, "label-values": label_values_dict}
+        data.update({ "confirm?": confirm, "change?": change, "resolve?": resolve })
+        
+        # Sending a POST request to the server
+        response = requests.post(endpoint, json=data, headers=headers)
+        return response.json()
+    
+    def get_project_articles(self, project_id, offset=0, limit=10, sort_by=None, sort_dir=None):
+        endpoint = f"{self.base_url}/api-json/project-articles"
+        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        body = {"project-id": project_id, "n-offset": offset, "n-count": limit}
+        
+        # Add optional sorting keys if provided
+        if sort_by: body["sort-by"] = sort_by
+        if sort_dir: body["sort-dir"] = sort_dir
+
+        # Make the POST request with the simplified body
+        response = requests.post(endpoint, headers=headers, json=body)
+        return response.json()
+    
+    def fetch_all_articles(self, project_id, limit=10, sort_by=None, sort_dir=None):
+        offset = 0
+        while True:
+            result = self.get_project_articles(project_id, offset=offset, limit=limit, sort_by=sort_by, sort_dir=sort_dir)
+            articles = result.get('result', [])
+            if not articles:
+                break  # Stop iteration if no articles are left
+            yield from articles  # Yield each article in the current batch
+            offset += len(articles)
+    
+    def get_article_info(self, project_id, article_id):
+        endpoint = f"{self.base_url}/api-json/article-info/{article_id}"
+        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+        body = {"project-id": project_id,}
+        response = requests.get(endpoint, headers=headers, json=body)
+        return response.json()['result']
+                   
+    def upload_jsonlines(self, file_path, project_id):
+        url = f"{self.base_url}/api-json/import-files/{project_id}"
+        headers = {"Authorization": f"Bearer {self.api_key}"}
+        
+        # Prepare the file for upload
+        with open(file_path, 'rb') as f:
+            files = {'file': (file_path.split('/')[-1], f, 'application/octet-stream')}
+            # Let requests handle "Content-Type"
+            response = requests.post(url, headers=headers, files=files)
+        
+        return response
+    
+    def get_article_file(self, project_id, article_id, hash):
+        url = f"{self.base_url}/api-json/files/{project_id}/article/{article_id}/download/{hash}"
+        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+
 class Synchronizer:
     
     def create_sqlite_db(self):
         pathlib.Path(".sr").mkdir(exist_ok=True)
         conn = sqlite3.connect('.sr/sr.sqlite')
         c = conn.cursor()
 
@@ -89,41 +174,36 @@
         c.execute('CREATE INDEX IF NOT EXISTS idx_labels_project_id ON labels (project_id);')
         c.execute('CREATE INDEX IF NOT EXISTS idx_article_label_user_id ON article_label (user_id);')
 
         # Commit changes and close connection
         conn.commit()
         conn.close()
 
-    # TODO - this could be made more efficient by checking sqlite state and updating the sysrev api
-    def sync(self, client, project_id):
-        
-        if not pathlib.Path('.sr/sr.sqlite').exists():
-            self.create_sqlite_db()
-            
-        project_info = client.get_project_info(project_id)
-        
-        labels = client.get_labels(project_id)
-        labels_df = pd.DataFrame(labels)
-        labels_df['definition'] = labels_df['definition'].apply(json.dumps)
+    def write_df(self, df, name, db_path='.sr/sr.sqlite'):
+        """
+        Writes the given DataFrame to a SQLite database.
+        
+        Parameters:
+            df (pandas.DataFrame): The DataFrame to be written to the database.
+            name (str): The name of the table in which the DataFrame should be stored.
+            db_path (str): Path to the SQLite database file.
+        """
+        # Connect to the SQLite database
+        conn = sqlite3.connect(db_path)
         
-        n_articles = project_info['result']['project']['stats']['articles']
-        articles = [resp for resp in tqdm.tqdm(client.fetch_all_articles(project_id), total=n_articles)]
-        
-        article_labels = [a['labels'] for a in articles if a['labels'] is not None]
-        article_labels = [lbl for lbls in article_labels for lbl in lbls]
-        article_label_df = pd.DataFrame(article_labels)
-        article_label_df['answer'] = article_label_df['answer'].apply(json.dumps)
-        
-        article_data = [{k: v for k, v in a.items() if k != 'labels'} for a in articles]
-        article_data_df = pd.DataFrame(article_data)
-        article_data_df['notes'] = article_data_df['notes'].apply(json.dumps)
-        article_data_df['resolve'] = article_data_df['resolve'].apply(json.dumps)
-            
+        try:
+            df.columns = df.columns.str.replace('-', '_')
+            df = df.loc[:, ~df.columns.duplicated()]
+            df.to_sql(name, conn, if_exists='replace', index=False) if not df.empty else None
+        finally:
+            conn.close()
+    
+    def sync_article_info(self, client:Client, project_id, article_ids):
         article_info = []
-        for article_id in tqdm.tqdm(article_data_df['article-id'], total=n_articles):
+        for article_id in tqdm.tqdm(article_ids, total=len(article_ids)):
             article_info.append(client.get_article_info(project_id, article_id))
         
         full_texts = pd.DataFrame([{**ft} for a in article_info for ft in a['article'].get('full-texts', []) ])
         full_texts.columns = [col.split('/')[-1] for col in full_texts.columns]
         
         auto_labels = pd.DataFrame([
             {**{'article-id': a['article'].get('article-id'), 'label-id': label_id}, **details} for a in article_info
@@ -133,110 +213,43 @@
         csl_citations = pd.DataFrame([
             {**{k: json.dumps(v) if isinstance(v, (dict, list)) else v for k, v in item['itemData'].items()}, 
              'article-id': a['article'].get('article-id')} 
             for a in article_info for item in a['article'].get('csl-citation', {}).get('citationItems', [])])
         csl_citations['issued'] = csl_citations['issued'].apply(json.dumps)
         csl_citations['author'] = csl_citations['author'].apply(json.dumps)
         
-        # write everything to .sr/sr.sqlite
-        conn = sqlite3.connect('.sr/sr.sqlite')
-        
-        def write_df(df,name):
-            # replace any - with _ in column names and remove duplicates
-            df.columns = df.columns.str.replace('-', '_')
-            df = df.loc[:,~df.columns.duplicated()]
-            df.to_sql(name, conn, if_exists='replace', index=False) if not df.empty else None
-                
-                
-        # Writing data to tables
-        write_df(labels_df,'labels')
-        write_df(article_label_df,'article_label')
-        write_df(article_data_df,'article_data')
-        write_df(full_texts,'full_texts')
-        write_df(auto_labels,'auto_labels')
-        write_df(csl_citations,'csl_citations')
-        
-        conn.close()
-class Client():
+        self.write_df(full_texts,'full_texts')
+        self.write_df(auto_labels,'auto_labels')
+        self.write_df(csl_citations,'csl_citations')
     
-    def __init__(self, api_key, base_url="https://www.sysrev.com"):
-        self.api_key = api_key
-        self.base_url = base_url
+    def sync_labels(self, client, project_id):
+        labels = client.get_labels(project_id)
+        labels_df = pd.DataFrame(labels)
+        labels_df['definition'] = labels_df['definition'].apply(json.dumps)
+        self.write_df(labels_df,'labels')
         
-    def sync(self, project_id):
-        Synchronizer().sync(self, project_id)
-    
-    def get_project_info(self, project_id):
-        endpoint = f"{self.base_url}/api-json/project-info"
-        headers = {"Authorization": f"Bearer {self.api_key}"}
-        response = requests.get(endpoint, headers=headers, params={"project-id": project_id})
-        return response.json()
-    
-    def get_labels(self, project_id):
-        raw_labels = self.get_project_info(project_id)['result']['project']['labels']
-        labels = [{"label_id": label_id} | raw_labels[label_id] for label_id in raw_labels.keys()]
-        return labels
-    
-    def set_labels(self, project_id, article_id, label_ids, label_values, label_types, confirm=False, change=False, resolve=False):
-        endpoint = f"{self.base_url}/api-json/set-labels"
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
+    # TODO - this could be made more efficient by checking sqlite state and updating the sysrev api
+    def sync(self, client, project_id):
         
-        assert len(label_ids) == len(label_values) == len(label_types), "Length of label_ids, label_values, and label_types should be the same."
+        if not pathlib.Path('.sr/sr.sqlite').exists():
+            self.create_sqlite_db()
+            
+        project_info = client.get_project_info(project_id)
         
-        # construct label_values_dict
-        tf = LabelTransformer()
-        label_values_dict = {label_ids[i]: tf.transform_label(label_types[i], label_values[i]) for i in range(len(label_ids))}    
+        n_articles = project_info['result']['project']['stats']['articles']
+        articles = [resp for resp in tqdm.tqdm(client.fetch_all_articles(project_id), total=n_articles)]
         
-        # Constructing the data payload as per the server's expectation
-        data = {"project-id": project_id, "article-id": article_id, "label-values": label_values_dict}
-        data.update({ "confirm?": confirm, "change?": change, "resolve?": resolve })
+        article_labels = [a['labels'] for a in articles if a['labels'] is not None]
+        article_labels = [lbl for lbls in article_labels for lbl in lbls]
+        article_label_df = pd.DataFrame(article_labels)
+        article_label_df['answer'] = article_label_df['answer'].apply(json.dumps)
         
-        # Sending a POST request to the server
-        response = requests.post(endpoint, json=data, headers=headers)
-        return response.json()
-    
-    def get_project_articles(self, project_id, offset=0, limit=10, sort_by=None, sort_dir=None):
-        endpoint = f"{self.base_url}/api-json/project-articles"
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-        body = {"project-id": project_id, "n-offset": offset, "n-count": limit}
+        article_data = [{k: v for k, v in a.items() if k != 'labels'} for a in articles]
+        article_data_df = pd.DataFrame(article_data)
+        article_data_df['notes'] = article_data_df['notes'].apply(json.dumps)
+        article_data_df['resolve'] = article_data_df['resolve'].apply(json.dumps)
         
-        # Add optional sorting keys if provided
-        if sort_by: body["sort-by"] = sort_by
-        if sort_dir: body["sort-dir"] = sort_dir
+        self.sync_article_info(client, project_id, article_data_df['article-id'])
 
-        # Make the POST request with the simplified body
-        response = requests.post(endpoint, headers=headers, json=body)
-        return response.json()
-    
-    def fetch_all_articles(self, project_id, limit=10, sort_by=None, sort_dir=None):
-        offset = 0
-        while True:
-            result = self.get_project_articles(project_id, offset=offset, limit=limit, sort_by=sort_by, sort_dir=sort_dir)
-            articles = result.get('result', [])
-            if not articles:
-                break  # Stop iteration if no articles are left
-            yield from articles  # Yield each article in the current batch
-            offset += len(articles)
-    
-    def get_article_info(self, project_id, article_id):
-        endpoint = f"{self.base_url}/api-json/article-info/{article_id}"
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-        body = {"project-id": project_id,}
-        response = requests.get(endpoint, headers=headers, json=body)
-        return response.json()['result']
-                   
-    def upload_jsonlines(self, file_path, project_id):
-        url = f"{self.base_url}/api-json/import-files/{project_id}"
-        headers = {"Authorization": f"Bearer {self.api_key}"}
-        
-        # Prepare the file for upload
-        with open(file_path, 'rb') as f:
-            files = {'file': (file_path.split('/')[-1], f, 'application/octet-stream')}
-            # Let requests handle "Content-Type"
-            response = requests.post(url, headers=headers, files=files)
-        
-        return response
-    
-    def get_article_file(self, project_id, article_id, hash):
-        url = f"{self.base_url}/api-json/files/{project_id}/article/{article_id}/download/{hash}"
-        headers = {"Authorization": f"Bearer {self.api_key}", "Content-Type": "application/json"}
-    
+        # Writing data to tables
+        self.write_df(article_label_df,'article_label')
+        self.write_df(article_data_df,'article_data')
```

### Comparing `sysrev-1.3.5/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.6/sysrev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.3.5
+Version: 1.3.6
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.3.5/tests/test_client.py` & `sysrev-1.3.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.3.5/tests/test_utils.py` & `sysrev-1.3.6/tests/test_utils.py`

 * *Files identical despite different names*

