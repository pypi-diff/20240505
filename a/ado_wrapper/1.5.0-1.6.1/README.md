# Comparing `tmp/ado_wrapper-1.5.0.tar.gz` & `tmp/ado_wrapper-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ado_wrapper-1.5.0.tar", max compression
+gzip compressed data, was "ado_wrapper-1.6.1.tar", max compression
```

## Comparing `ado_wrapper-1.5.0.tar` & `ado_wrapper-1.6.1.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.5.0/LICENSE
--rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.5.0/README.md
--rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.5.0/ado_wrapper/__init__.py
--rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.5.0/ado_wrapper/__main__.py
--rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.5.0/ado_wrapper/client.py
--rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.5.0/ado_wrapper/dumps.py
--rw-r--r--   0        0        0     3378 2024-05-02 10:50:48.977836 ado_wrapper-1.5.0/ado_wrapper/generate_docs.py
--rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.5.0/ado_wrapper/plan_resources/__init__.py
--rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.5.0/ado_wrapper/plan_resources/colours.py
--rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.5.0/ado_wrapper/plan_resources/mapping.py
--rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_repo.py
--rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_resource.py
--rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_state_manager.py
--rw-r--r--   0        0        0     1082 2024-05-02 12:12:40.876620 ado_wrapper-1.5.0/ado_wrapper/resources/__init__.py
--rw-r--r--   0        0        0     3710 2024-05-02 12:34:44.409220 ado_wrapper-1.5.0/ado_wrapper/resources/agent_pools.py
--rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.5.0/ado_wrapper/resources/annotated_tags.py
--rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.5.0/ado_wrapper/resources/branches.py
--rw-r--r--   0        0        0    14870 2024-05-03 16:42:18.453223 ado_wrapper-1.5.0/ado_wrapper/resources/builds.py
--rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.5.0/ado_wrapper/resources/commits.py
--rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.5.0/ado_wrapper/resources/environment.py
--rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.5.0/ado_wrapper/resources/groups.py
--rw-r--r--   0        0        0    15327 2024-05-03 16:42:42.079759 ado_wrapper-1.5.0/ado_wrapper/resources/merge_policies.py
--rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.5.0/ado_wrapper/resources/projects.py
--rw-r--r--   0        0        0    14012 2024-05-03 16:42:47.416430 ado_wrapper-1.5.0/ado_wrapper/resources/pull_requests.py
--rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.5.0/ado_wrapper/resources/releases.py
--rw-r--r--   0        0        0    10450 2024-05-03 16:43:21.984943 ado_wrapper-1.5.0/ado_wrapper/resources/repo.py
--rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.5.0/ado_wrapper/resources/searches.py
--rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.5.0/ado_wrapper/resources/service_endpoint.py
--rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.5.0/ado_wrapper/resources/teams.py
--rw-r--r--   0        0        0     8295 2024-04-21 14:56:46.799706 ado_wrapper-1.5.0/ado_wrapper/resources/users.py
--rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.5.0/ado_wrapper/resources/variable_groups.py
--rw-r--r--   0        0        0     9437 2024-05-03 16:43:45.994580 ado_wrapper-1.5.0/ado_wrapper/state_managed_abc.py
--rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.5.0/ado_wrapper/state_manager.py
--rw-r--r--   0        0        0     4806 2024-05-02 12:13:10.282768 ado_wrapper-1.5.0/ado_wrapper/utils.py
--rw-r--r--   0        0        0     2760 2024-05-03 16:45:03.092106 ado_wrapper-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-03-12 15:09:12.939731 ado_wrapper-1.6.1/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-09 08:14:25.263935 ado_wrapper-1.6.1/README.md
+-rw-r--r--   0        0        0      118 2024-04-20 14:42:40.460346 ado_wrapper-1.6.1/ado_wrapper/__init__.py
+-rw-r--r--   0        0        0     6516 2024-04-21 14:56:46.791401 ado_wrapper-1.6.1/ado_wrapper/__main__.py
+-rw-r--r--   0        0        0     2325 2024-05-03 16:43:39.046186 ado_wrapper-1.6.1/ado_wrapper/client.py
+-rw-r--r--   0        0        0    25691 2024-04-21 11:28:27.535399 ado_wrapper-1.6.1/ado_wrapper/dumps.py
+-rw-r--r--   0        0        0     3427 2024-05-04 17:24:03.055237 ado_wrapper-1.6.1/ado_wrapper/generate_docs.py
+-rw-r--r--   0        0        0       58 2024-04-05 11:26:35.622666 ado_wrapper-1.6.1/ado_wrapper/plan_resources/__init__.py
+-rw-r--r--   0        0        0      343 2024-04-09 09:48:22.014467 ado_wrapper-1.6.1/ado_wrapper/plan_resources/colours.py
+-rw-r--r--   0        0        0      296 2024-04-21 14:56:46.792465 ado_wrapper-1.6.1/ado_wrapper/plan_resources/mapping.py
+-rw-r--r--   0        0        0     1067 2024-04-21 14:56:46.792911 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_repo.py
+-rw-r--r--   0        0        0     1820 2024-04-21 14:56:46.793288 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_resource.py
+-rw-r--r--   0        0        0      809 2024-04-23 08:39:40.317360 ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_state_manager.py
+-rw-r--r--   0        0        0     1173 2024-05-05 12:45:05.895693 ado_wrapper-1.6.1/ado_wrapper/resources/__init__.py
+-rw-r--r--   0        0        0     3704 2024-05-04 17:23:41.003500 ado_wrapper-1.6.1/ado_wrapper/resources/agent_pools.py
+-rw-r--r--   0        0        0     4763 2024-04-24 08:14:16.703798 ado_wrapper-1.6.1/ado_wrapper/resources/annotated_tags.py
+-rw-r--r--   0        0        0     3387 2024-04-22 11:52:18.509396 ado_wrapper-1.6.1/ado_wrapper/resources/branches.py
+-rw-r--r--   0        0        0    14870 2024-05-03 16:42:18.453223 ado_wrapper-1.6.1/ado_wrapper/resources/builds.py
+-rw-r--r--   0        0        0     6621 2024-05-03 16:39:20.096468 ado_wrapper-1.6.1/ado_wrapper/resources/commits.py
+-rw-r--r--   0        0        0     7397 2024-04-23 08:38:52.950096 ado_wrapper-1.6.1/ado_wrapper/resources/environment.py
+-rw-r--r--   0        0        0     3308 2024-04-21 14:56:46.796388 ado_wrapper-1.6.1/ado_wrapper/resources/groups.py
+-rw-r--r--   0        0        0    15327 2024-05-03 16:42:42.079759 ado_wrapper-1.6.1/ado_wrapper/resources/merge_policies.py
+-rw-r--r--   0        0        0     2135 2024-05-02 08:38:58.564678 ado_wrapper-1.6.1/ado_wrapper/resources/projects.py
+-rw-r--r--   0        0        0    14012 2024-05-03 16:42:47.416430 ado_wrapper-1.6.1/ado_wrapper/resources/pull_requests.py
+-rw-r--r--   0        0        0    12487 2024-04-21 14:56:46.797975 ado_wrapper-1.6.1/ado_wrapper/resources/releases.py
+-rw-r--r--   0        0        0    10450 2024-05-05 11:05:13.008884 ado_wrapper-1.6.1/ado_wrapper/resources/repo.py
+-rw-r--r--   0        0        0    10496 2024-05-05 13:08:03.080705 ado_wrapper-1.6.1/ado_wrapper/resources/repo_user_permission.py
+-rw-r--r--   0        0        0     2853 2024-04-29 16:33:17.512344 ado_wrapper-1.6.1/ado_wrapper/resources/searches.py
+-rw-r--r--   0        0        0     5973 2024-04-23 09:01:01.373067 ado_wrapper-1.6.1/ado_wrapper/resources/service_endpoint.py
+-rw-r--r--   0        0        0     4557 2024-04-21 14:56:46.799334 ado_wrapper-1.6.1/ado_wrapper/resources/teams.py
+-rw-r--r--   0        0        0     8314 2024-05-04 20:57:42.347047 ado_wrapper-1.6.1/ado_wrapper/resources/users.py
+-rw-r--r--   0        0        0     4828 2024-04-21 14:56:46.800092 ado_wrapper-1.6.1/ado_wrapper/resources/variable_groups.py
+-rw-r--r--   0        0        0     9437 2024-05-03 16:43:45.994580 ado_wrapper-1.6.1/ado_wrapper/state_managed_abc.py
+-rw-r--r--   0        0        0     8129 2024-05-03 16:44:33.762863 ado_wrapper-1.6.1/ado_wrapper/state_manager.py
+-rw-r--r--   0        0        0     4929 2024-05-05 09:30:08.198011 ado_wrapper-1.6.1/ado_wrapper/utils.py
+-rw-r--r--   0        0        0     2760 2024-05-05 13:08:28.204945 ado_wrapper-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 ado_wrapper-1.6.1/PKG-INFO
```

### Comparing `ado_wrapper-1.5.0/LICENSE` & `ado_wrapper-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/README.md` & `ado_wrapper-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/__main__.py` & `ado_wrapper-1.6.1/ado_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/client.py` & `ado_wrapper-1.6.1/ado_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/dumps.py` & `ado_wrapper-1.6.1/ado_wrapper/dumps.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/generate_docs.py` & `ado_wrapper-1.6.1/ado_wrapper/generate_docs.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 def format_return_type(return_type: str) -> str | None:
     """Returns the value, formatted, and = if it's not None, makes list[`object`] also be called `objects`"""
     return_type = pascal_to_snake(return_type.split(" | ")[0])
     if "." in return_type:
         return_type = return_type.split(".")[-1].removesuffix(">").removeprefix("_")
     if return_type == "str":
-        return f"string_var = "
+        return "string_var = "
     if return_type.startswith("dict"):
-        return f"dictionary = "
+        return "dictionary = "
     if return_type.startswith("none"):
         return ""
     if "state_managed_resource" in return_type:
         return None
     if return_type.startswith("list[_"):
         return_type = return_type.removeprefix("list[_").removesuffix("]")+"s"
     return f"{return_type} = "
 
-def dataclass_attributes(cls) -> list[str]:
+def dataclass_attributes(cls) -> list[str]:  # type: ignore[no-untyped-def]
     return [x for x in dir(cls) if x in cls.__dataclass_fields__.keys()]
 
 sorted_pairs = dict(sorted({string: value for string, value in globals().items() if string[0].isupper()}.items()))
 
 for class_name, value in sorted_pairs.items():
     # if class_name != "Build":
     #     continue
@@ -73,11 +73,11 @@
             continue  # For things inheritting from update, for the time being before we remap to _update
         single_args_formatted = [x if i==0 else f"<{x}>" for i, x in enumerate(function_args)]
         function_args_formatted = ", ".join(single_args_formatted)
         string += f"# {comment}\n{return_type}{class_name if ' = ' in return_type else pascal_to_snake(class_name)}.{function_name}({function_args_formatted})\n\n"
 
     string += "\n```\n</details>\n\n"
 
-with open("examples.md", "w") as file:
+with open("examples.md", "w", encoding="utf-8") as file:
     file.write(string.replace("\n\n\n", "\n"))
 
-# All the functions which have NotImplementedError
+# All the functions which have NotImplementedError
```

### Comparing `ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_repo.py` & `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_resource.py` & `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_resource.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/plan_resources/plan_state_manager.py` & `ado_wrapper-1.6.1/ado_wrapper/plan_resources/plan_state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/__init__.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,13 +9,14 @@
     MergeBranchPolicy,
     MergePolicies,
     MergePolicyDefaultReviewer,
 )
 from ado_wrapper.resources.projects import Project
 from ado_wrapper.resources.pull_requests import PullRequest
 from ado_wrapper.resources.releases import Release, ReleaseDefinition
+from ado_wrapper.resources.repo_user_permission import RepoUserPermissions, UserPermission
 from ado_wrapper.resources.repo import BuildRepository, Repo
 from ado_wrapper.resources.searches import Search
 from ado_wrapper.resources.service_endpoint import ServiceEndpoint
 from ado_wrapper.resources.teams import Team
 from ado_wrapper.resources.users import AdoUser, Member, Reviewer, TeamMember
 from ado_wrapper.resources.variable_groups import VariableGroup
```

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/agent_pools.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/agent_pools.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,52 +34,52 @@
         created_by = Member.from_request_payload(data["createdBy"])
         return cls(
             str(data["id"]), data["agentCloudId"], data["name"], data["size"], data["targetSize"], data["autoSize"], data["autoUpdate"],
             data["autoProvision"], data["isHosted"], data["scope"], from_ado_date_string(data["createdOn"]), created_by  # fmt: skip
         )
 
     @classmethod
-    def get_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> AgentPool:  # type: ignore[override]
+    def get_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> AgentPool:
         return super().get_by_url(
             ado_client,
             f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     @classmethod
-    def create(cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,
-               auto_update: bool, is_hosted: bool, size: int, target_size: int | None) -> AgentPool:  # type: ignore[override]
+    def create(cls, ado_client: AdoClient, name: str, agent_cloud_id: str | None, auto_provision: bool, auto_size: bool,  # type: ignore[override]
+               auto_update: bool, is_hosted: bool, size: int, target_size: int | None) -> AgentPool:
         raise NotImplementedError
         PAYLOAD = {
             "name": name, "agentCloudId": agent_cloud_id, "autoProvision": auto_provision, "autoSize": auto_size,
             "autoUpdate": auto_update, "isHosted": is_hosted, "size": size, "targetSize": target_size,
         }
         return super().create(
             ado_client,
-            f"/_apis/distributedtask/pools?api-version=7.1-preview.1",
+            "/_apis/distributedtask/pools?api-version=7.1-preview.1",
             payload=PAYLOAD,
-        )  # type: ignore[return-value]
+        )
 
     # def update(self) -> None:
     #     raise NotImplementedError
     #     # PATCH https://dev.azure.com/{organization}/_apis/distributedtask/pools/{poolId}?api-version=7.1-preview.1
 
     @classmethod
-    def delete_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> None:
+    def delete_by_id(cls, ado_client: AdoClient, agent_pool_id: str) -> None:  # type: ignore[override]
         raise NotImplementedError
         return super().delete_by_id(
             ado_client,
             f"/_apis/distributedtask/pools/{agent_pool_id}?api-version=7.1-preview.1",
             agent_pool_id
         )
 
     @classmethod
-    def get_all(cls, ado_client: AdoClient) -> list[AgentPool]:
+    def get_all(cls, ado_client: AdoClient) -> list[AgentPool]:  # type: ignore[override]
         return super().get_all(
             ado_client,
-            f"/_apis/distributedtask/pools?api-version=7.1-preview.1",
+            "/_apis/distributedtask/pools?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
 
     # ============ End of requirement set by all state managed resources ================== #
     # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
     # =============== Start of additional methods included with class ===================== #
 
     @classmethod
```

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/annotated_tags.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/annotated_tags.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/branches.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/branches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/builds.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/builds.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/commits.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/commits.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/environment.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/environment.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/groups.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/merge_policies.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/merge_policies.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/projects.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/projects.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/pull_requests.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/pull_requests.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/releases.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/releases.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/repo.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/repo.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/searches.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/searches.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/service_endpoint.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/service_endpoint.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/teams.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/teams.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/users.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/users.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,27 +25,27 @@
     """https://learn.microsoft.com/en-us/rest/api/azure/devops/graph/users?view=azure-devops-rest-7.1"""
 
     descriptor_id: str = field(metadata={"is_id_field": True})
     display_name: str
     email: str
     origin: str
     origin_id: str  # DON'T USE THIS, USE `descriptor_id` INSTEAD
+    domain_container_id: str  # Ignore this
     # "subjectKind": "user",
     # "metaType": "member",
     # "directoryAlias": "MiryabblliS",
-    # "domain": "68283f3b-8487-4c86-adb3-a5228f18b893",
     # "url": "https://vssps.dev.azure.com/{ado_client.}/_apis/Graph/Users/aad.M2Q5NDlkZTgtZDI2Yi03MGQ3LWEyYjItMDAwYTQzYTdlNzFi",
 
     def __str__(self) -> str:
         return f"{self.display_name} ({self.email})"
 
     @classmethod
     def from_request_payload(cls, data: dict[str, str]) -> AdoUser:
         return cls(data["descriptor"], data["displayName"], data["mailAddress"].removeprefix("vstfs:///Classification/TeamProject/"),
-                   data["origin"], data["originId"])  # fmt: skip
+                   data["origin"], data["originId"], data.get("domain", "UNKNOWN"))  # fmt: skip
 
     @classmethod
     def get_by_id(cls, ado_client: AdoClient, descriptor_id: str) -> AdoUser:
         return super().get_by_url(
             ado_client,  # Preview required
             f"https://vssps.dev.azure.com/{ado_client.ado_org}/_apis/graph/users/{descriptor_id}?api-version=7.1-preview.1",
         )  # type: ignore[return-value]
```

### Comparing `ado_wrapper-1.5.0/ado_wrapper/resources/variable_groups.py` & `ado_wrapper-1.6.1/ado_wrapper/resources/variable_groups.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/state_managed_abc.py` & `ado_wrapper-1.6.1/ado_wrapper/state_managed_abc.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/state_manager.py` & `ado_wrapper-1.6.1/ado_wrapper/state_manager.py`

 * *Files identical despite different names*

### Comparing `ado_wrapper-1.5.0/ado_wrapper/utils.py` & `ado_wrapper-1.6.1/ado_wrapper/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 
 class ConfigurationError(Exception):
     pass
 
 
 def requires_initialisation(ado_client: "AdoClient") -> None:
+    """Certain services/endpoints require the ado_project_id, which isn't set if bypass_initialisation is set to False."""
     if not ado_client.ado_project_id:
         raise ConfigurationError(
             "The client has not been initialised. Please disable `bypass_initialisation` in AdoClient before using this function."
         )
 
 
 def get_resource_variables() -> dict[str, type["StateManagedResource"]]:  # We do this to avoid circular imports
```

### Comparing `ado_wrapper-1.5.0/pyproject.toml` & `ado_wrapper-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "ado_wrapper"
 description = "A high level wrapper around the AzureDevops API including OOP principals and state management"
 authors = ["Ben Skerritt"]
-version = "1.5.0"
+version = "1.6.1"
 license = "Proprietary"
 readme = "README.md"
 packages = [{include = "ado_wrapper"}]
 
 [tool.poetry.scripts]
 ado_wrapper = "ado_wrapper.__main__:main"
```

### Comparing `ado_wrapper-1.5.0/PKG-INFO` & `ado_wrapper-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ado_wrapper
-Version: 1.5.0
+Version: 1.6.1
 Summary: A high level wrapper around the AzureDevops API including OOP principals and state management
 License: Proprietary
 Author: Ben Skerritt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

