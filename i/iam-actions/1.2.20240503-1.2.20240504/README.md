# Comparing `tmp/iam_actions-1.2.20240503.tar.gz` & `tmp/iam_actions-1.2.20240504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240503.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240504.tar", max compression
```

## Comparing `iam_actions-1.2.20240503.tar` & `iam_actions-1.2.20240504.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/LICENSE
--rw-r--r--   0        0        0     2302 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/README.md
--rw-r--r--   0        0        0      228 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/__init__.py
--rw-r--r--   0        0        0  4825636 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-05-03 02:21:09.387521 iam_actions-1.2.20240503/iam_actions/generate/services.py
--rw-r--r--   0        0        0   627685 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/policies.json
--rw-r--r--   0        0        0   209301 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   609078 2024-05-03 02:23:06.800053 iam_actions-1.2.20240503/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-05-03 02:23:07.448056 iam_actions-1.2.20240503/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240503/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240503/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/LICENSE
+-rw-r--r--   0        0        0     2302 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/README.md
+-rw-r--r--   0        0        0      228 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4826508 2024-05-04 02:18:07.698048 iam_actions-1.2.20240504/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-05-04 02:16:40.204450 iam_actions-1.2.20240504/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-05-04 02:16:40.208450 iam_actions-1.2.20240504/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-05-04 02:16:40.208450 iam_actions-1.2.20240504/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-05-04 02:16:40.208450 iam_actions-1.2.20240504/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-05-04 02:16:40.208450 iam_actions-1.2.20240504/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-05-04 02:16:40.208450 iam_actions-1.2.20240504/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   627782 2024-05-04 02:18:07.698048 iam_actions-1.2.20240504/iam_actions/policies.json
+-rw-r--r--   0        0        0   209301 2024-05-04 02:18:07.698048 iam_actions-1.2.20240504/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   609172 2024-05-04 02:18:07.698048 iam_actions-1.2.20240504/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-05-04 02:18:08.442062 iam_actions-1.2.20240504/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240504/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240504/PKG-INFO
```

### Comparing `iam_actions-1.2.20240503/LICENSE` & `iam_actions-1.2.20240504/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/README.md` & `iam_actions-1.2.20240504/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/actions.json` & `iam_actions-1.2.20240504/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999483236336919%*

 * *Differences: {"'connect'": "{'AdminGetEmergencyAccessToken': OrderedDict([('access_level', 'Undocumented'), "*

 * *              "('action', 'AdminGetEmergencyAccessToken'), ('condition_keys', []), ('description', "*

 * *              "'Not Documented by AWS'), ('orphan', False), ('resources', [])])}",*

 * * "'personalize'": "{'CreateDataDeletionJob': OrderedDict([('access_level', 'Undocumented'), "*

 * *                  "('action', 'CreateDataDeletionJob'), ('condition_keys', []), ('description', "*

 * *                  "'Not Documented by A […]*

```diff
@@ -34226,14 +34226,22 @@
             ],
             "description": "Grants permission to activate an evaluation form in the specified Amazon Connect instance. After the evaluation form is activated, it is available to start new evaluations based on the form",
             "orphan": false,
             "resources": [
                 "evaluation-form"
             ]
         },
+        "AdminGetEmergencyAccessToken": {
+            "access_level": "Undocumented",
+            "action": "AdminGetEmergencyAccessToken",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "AssociateApprovedOrigin": {
             "access_level": "Write",
             "action": "AssociateApprovedOrigin",
             "condition_keys": [
                 "connect:InstanceId"
             ],
             "description": "Grants permission to associate approved origin for an existing Amazon Connect instance",
@@ -120011,14 +120019,22 @@
             "condition_keys": [],
             "description": "Grants permission to create a campaign",
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         },
+        "CreateDataDeletionJob": {
+            "access_level": "Undocumented",
+            "action": "CreateDataDeletionJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateDataInsightsJob": {
             "access_level": "Write",
             "action": "CreateDataInsightsJob",
             "condition_keys": [],
             "description": "Grants permission to create a data insights job",
             "orphan": false,
             "resources": [
@@ -120261,14 +120277,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe a campaign",
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         },
+        "DescribeDataDeletionJob": {
+            "access_level": "Undocumented",
+            "action": "DescribeDataDeletionJob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDataInsightsJob": {
             "access_level": "Read",
             "action": "DescribeDataInsightsJob",
             "condition_keys": [],
             "description": "Grants permission to describe a data insights job",
             "orphan": false,
             "resources": [
@@ -120475,14 +120499,22 @@
             "access_level": "List",
             "action": "ListCampaigns",
             "condition_keys": [],
             "description": "Grants permission to list campaigns",
             "orphan": false,
             "resources": []
         },
+        "ListDataDeletionJobs": {
+            "access_level": "Undocumented",
+            "action": "ListDataDeletionJobs",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDataInsightsJobs": {
             "access_level": "List",
             "action": "ListDataInsightsJobs",
             "condition_keys": [],
             "description": "Grants permission to list data insights jobs",
             "orphan": false,
             "resources": []
```

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240504/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240504/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/generate.py` & `iam_actions-1.2.20240504/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240504/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240504/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/generate/services.py` & `iam_actions-1.2.20240504/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/policies.json` & `iam_actions-1.2.20240504/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999994731654993%*

 * *Differences: {"'serviceMap'": "{'Amazon Connect': {'Actions': {insert: [(1, 'AdminGetEmergencyAccessToken')], "*

 * *                 "delete: [110]}}, 'Amazon Personalize': {'Actions': {insert: [(3, "*

 * *                 "'CreateDataDeletionJob'), (29, 'DescribeDataDeletionJob'), (52, "*

 * *                 "'ListDataDeletionJobs')]}}}"}*

```diff
@@ -13039,14 +13039,15 @@
             ]
         },
         "Amazon Connect": {
             "ARNFormat": "arn:aws:connect:${Region}:${Account}:instance/${InstanceId}",
             "ARNRegex": "^arn:aws:connect:.+:.+:instance/.+",
             "Actions": [
                 "ActivateEvaluationForm",
+                "AdminGetEmergencyAccessToken",
                 "AssociateApprovedOrigin",
                 "AssociateBot",
                 "AssociateCustomerProfilesDomain",
                 "AssociateDefaultVocabulary",
                 "AssociateFlow",
                 "AssociateInstanceStorageConfig",
                 "AssociateLambdaFunction",
@@ -13148,15 +13149,14 @@
                 "DisassociateTrafficDistributionGroupUser",
                 "DisassociateUserProficiencies",
                 "DismissUserContact",
                 "GetContactAttributes",
                 "GetCurrentMetricData",
                 "GetCurrentUserData",
                 "GetFederationToken",
-                "GetFederationTokens",
                 "GetFlowAssociation",
                 "GetMetricData",
                 "GetMetricDataV2",
                 "GetPromptFile",
                 "GetTaskTemplate",
                 "GetTrafficDistribution",
                 "ImportPhoneNumber",
@@ -18427,14 +18427,15 @@
         "Amazon Personalize": {
             "ARNFormat": "arn:aws:personalize:${Region}:${Account}:${Resourcename}/${ResourceId}",
             "ARNRegex": "^arn:aws:personalize:.+:.+:.+",
             "Actions": [
                 "CreateBatchInferenceJob",
                 "CreateBatchSegmentJob",
                 "CreateCampaign",
+                "CreateDataDeletionJob",
                 "CreateDataInsightsJob",
                 "CreateDataset",
                 "CreateDatasetExportJob",
                 "CreateDatasetGroup",
                 "CreateDatasetImportJob",
                 "CreateEventTracker",
                 "CreateFilter",
@@ -18452,14 +18453,15 @@
                 "DeleteRecommender",
                 "DeleteSchema",
                 "DeleteSolution",
                 "DescribeAlgorithm",
                 "DescribeBatchInferenceJob",
                 "DescribeBatchSegmentJob",
                 "DescribeCampaign",
+                "DescribeDataDeletionJob",
                 "DescribeDataInsightsJob",
                 "DescribeDataset",
                 "DescribeDatasetExportJob",
                 "DescribeDatasetGroup",
                 "DescribeDatasetImportJob",
                 "DescribeEventTracker",
                 "DescribeFeatureTransformation",
@@ -18474,14 +18476,15 @@
                 "GetDataInsights",
                 "GetPersonalizedRanking",
                 "GetRecommendations",
                 "GetSolutionMetrics",
                 "ListBatchInferenceJobs",
                 "ListBatchSegmentJobs",
                 "ListCampaigns",
+                "ListDataDeletionJobs",
                 "ListDataInsightsJobs",
                 "ListDatasetExportJobs",
                 "ListDatasetGroups",
                 "ListDatasetImportJobs",
                 "ListDatasets",
                 "ListEventTrackers",
                 "ListFilters",
```

### Comparing `iam_actions-1.2.20240503/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240504/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240503/iam_actions/services.json` & `iam_actions-1.2.20240504/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999952661278645%*

 * *Differences: {"'connect'": "{'Actions': {insert: [(1, 'AdminGetEmergencyAccessToken')], delete: [110]}}",*

 * * "'personalize'": "{'Actions': {insert: [(3, 'CreateDataDeletionJob'), (29, "*

 * *                  "'DescribeDataDeletionJob'), (52, 'ListDataDeletionJobs')]}}"}*

```diff
@@ -5222,14 +5222,15 @@
             "arn:aws:connect:${Region}:${Account}:instance/${InstanceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:connect:.+:.+:instance/.+"
         ],
         "Actions": [
             "ActivateEvaluationForm",
+            "AdminGetEmergencyAccessToken",
             "AssociateApprovedOrigin",
             "AssociateBot",
             "AssociateCustomerProfilesDomain",
             "AssociateDefaultVocabulary",
             "AssociateFlow",
             "AssociateInstanceStorageConfig",
             "AssociateLambdaFunction",
@@ -5331,15 +5332,14 @@
             "DisassociateTrafficDistributionGroupUser",
             "DisassociateUserProficiencies",
             "DismissUserContact",
             "GetContactAttributes",
             "GetCurrentMetricData",
             "GetCurrentUserData",
             "GetFederationToken",
-            "GetFederationTokens",
             "GetFlowAssociation",
             "GetMetricData",
             "GetMetricDataV2",
             "GetPromptFile",
             "GetTaskTemplate",
             "GetTrafficDistribution",
             "ImportPhoneNumber",
@@ -16877,14 +16877,15 @@
         "ARNRegexes": [
             "^arn:aws:personalize:.+:.+:.+"
         ],
         "Actions": [
             "CreateBatchInferenceJob",
             "CreateBatchSegmentJob",
             "CreateCampaign",
+            "CreateDataDeletionJob",
             "CreateDataInsightsJob",
             "CreateDataset",
             "CreateDatasetExportJob",
             "CreateDatasetGroup",
             "CreateDatasetImportJob",
             "CreateEventTracker",
             "CreateFilter",
@@ -16902,14 +16903,15 @@
             "DeleteRecommender",
             "DeleteSchema",
             "DeleteSolution",
             "DescribeAlgorithm",
             "DescribeBatchInferenceJob",
             "DescribeBatchSegmentJob",
             "DescribeCampaign",
+            "DescribeDataDeletionJob",
             "DescribeDataInsightsJob",
             "DescribeDataset",
             "DescribeDatasetExportJob",
             "DescribeDatasetGroup",
             "DescribeDatasetImportJob",
             "DescribeEventTracker",
             "DescribeFeatureTransformation",
@@ -16924,14 +16926,15 @@
             "GetDataInsights",
             "GetPersonalizedRanking",
             "GetRecommendations",
             "GetSolutionMetrics",
             "ListBatchInferenceJobs",
             "ListBatchSegmentJobs",
             "ListCampaigns",
+            "ListDataDeletionJobs",
             "ListDataInsightsJobs",
             "ListDatasetExportJobs",
             "ListDatasetGroups",
             "ListDatasetImportJobs",
             "ListDatasets",
             "ListEventTrackers",
             "ListFilters",
```

### Comparing `iam_actions-1.2.20240503/pyproject.toml` & `iam_actions-1.2.20240504/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240503"
+version = "1.2.20240504"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240503/setup.py` & `iam_actions-1.2.20240504/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240503',
+    'version': '1.2.20240504',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240503/PKG-INFO` & `iam_actions-1.2.20240504/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240503
+Version: 1.2.20240504
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

