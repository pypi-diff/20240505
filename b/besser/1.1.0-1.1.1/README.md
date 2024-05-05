# Comparing `tmp/besser-1.1.0.tar.gz` & `tmp/besser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besser-1.1.0.tar", last modified: Wed May  1 21:35:02 2024, max compression
+gzip compressed data, was "besser-1.1.1.tar", last modified: Sun May  5 18:41:06 2024, max compression
```

## Comparing `besser-1.1.0.tar` & `besser-1.1.1.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.115845 besser-1.1.0/
--rw-rw-rw-   0        0        0     3777 2024-05-01 21:35:02.114846 besser-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2804 2024-04-29 14:01:22.000000 besser-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.007321 besser-1.1.0/besser/
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.016795 besser-1.1.0/besser/BUML/
--rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.1.0/besser/BUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.018792 besser-1.1.0/besser/BUML/metamodel/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.0/besser/BUML/metamodel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.020788 besser-1.1.0/besser/BUML/metamodel/gui/
--rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.1.0/besser/BUML/metamodel/gui/__init__.py
--rw-rw-rw-   0        0        0    25750 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/gui/graphical_ui.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.023560 besser-1.1.0/besser/BUML/metamodel/object/
--rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.1.0/besser/BUML/metamodel/object/__init__.py
--rw-rw-rw-   0        0        0    10058 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/object/object.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.025909 besser-1.1.0/besser/BUML/metamodel/ocl/
--rw-rw-rw-   0        0        0       20 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/ocl/__init__.py
--rw-rw-rw-   0        0        0    18910 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/ocl/rules.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.028244 besser-1.1.0/besser/BUML/metamodel/structural/
--rw-rw-rw-   0        0        0       25 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/metamodel/structural/__init__.py
--rw-rw-rw-   0        0        0    42656 2024-05-01 21:18:56.000000 besser-1.1.0/besser/BUML/metamodel/structural/structural.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.030734 besser-1.1.0/besser/BUML/notations/
--rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.0/besser/BUML/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.036732 besser-1.1.0/besser/BUML/notations/objectPlantUML/
--rw-rw-rw-   0        0        0     5938 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODLexer.py
--rw-rw-rw-   0        0        0     4994 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODListener.py
--rw-rw-rw-   0        0        0    25828 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/ODParser.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/objectPlantUML/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.050327 besser-1.1.0/besser/BUML/notations/ocl/
--rw-rw-rw-   0        0        0    23268 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLLexer.py
--rw-rw-rw-   0        0        0    41633 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLListener.py
--rw-rw-rw-   0        0        0   212929 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/BOCLParser.py
--rw-rw-rw-   0        0        0     4732 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/FactoryInstance.py
--rw-rw-rw-   0        0        0     1080 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/OCLWrapper.py
--rw-rw-rw-   0        0        0    12723 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/RootHandler.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/ocl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.058329 besser-1.1.0/besser/BUML/notations/structuralPlantUML/
--rw-rw-rw-   0        0        0    10331 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
--rw-rw-rw-   0        0        0     6394 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
--rw-rw-rw-   0        0        0    51575 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
--rw-rw-rw-   0        0        0      203 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/__init__.py
--rw-rw-rw-   0        0        0     9121 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
--rw-rw-rw-   0        0        0     1432 2024-04-29 14:01:22.000000 besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
--rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.1.0/besser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.060328 besser-1.1.0/besser/generators/
--rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.1.0/besser/generators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.063330 besser-1.1.0/besser/generators/backend/
--rw-rw-rw-   0        0        0       32 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/backend/__init__.py
--rw-rw-rw-   0        0        0     3276 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/backend/backend_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.065330 besser-1.1.0/besser/generators/django/
--rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/django/__init__.py
--rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.1.0/besser/generators/django/django_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.068330 besser-1.1.0/besser/generators/django/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/django/templates/__init__.py
--rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/django/templates/django_fields.py.j2
--rw-rw-rw-   0        0        0     3580 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/django/templates/django_template.py.j2
--rw-rw-rw-   0        0        0     1166 2024-04-29 14:01:22.000000 besser-1.1.0/besser/generators/generator_interface.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.072329 besser-1.1.0/besser/generators/pydantic_classes/
--rw-rw-rw-   0        0        0       41 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/__init__.py
--rw-rw-rw-   0        0        0     2593 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/pydantic_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.074330 besser-1.1.0/besser/generators/pydantic_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     3409 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.077334 besser-1.1.0/besser/generators/python_classes/
--rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.1.0/besser/generators/python_classes/__init__.py
--rw-rw-rw-   0        0        0     1722 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/python_classes/python_classes_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.081335 besser-1.1.0/besser/generators/python_classes/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/python_classes/templates/__init__.py
--rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.1.0/besser/generators/python_classes/templates/class_parameters.py.j2
--rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.1.0/besser/generators/python_classes/templates/python_classes_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.083335 besser-1.1.0/besser/generators/rest_api/
--rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.1.0/besser/generators/rest_api/__init__.py
--rw-rw-rw-   0        0        0     4716 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/rest_api_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.087335 besser-1.1.0/besser/generators/rest_api/templates/
--rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.1.0/besser/generators/rest_api/templates/__init__.py
--rw-rw-rw-   0        0        0    11014 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/templates/backend_fast_api_template.py.j2
--rw-rw-rw-   0        0        0     4987 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/rest_api/templates/fast_api_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.089334 besser-1.1.0/besser/generators/sql/
--rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.1.0/besser/generators/sql/__init__.py
--rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.1.0/besser/generators/sql/sql_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.092845 besser-1.1.0/besser/generators/sql/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/sql/templates/__init__.py
--rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/sql/templates/sql_dialects.sql.j2
--rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.1.0/besser/generators/sql/templates/sql_template.sql.j2
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.094845 besser-1.1.0/besser/generators/sql_alchemy/
--rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.1.0/besser/generators/sql_alchemy/__init__.py
--rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.1.0/besser/generators/sql_alchemy/sql_alchemy_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.096844 besser-1.1.0/besser/generators/sql_alchemy/templates/
--rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.0/besser/generators/sql_alchemy/templates/__init__.py
--rw-rw-rw-   0        0        0     3695 2024-05-01 21:18:56.000000 besser-1.1.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.100845 besser-1.1.0/besser/utilities/
--rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.1.0/besser/utilities/__init__.py
--rw-rw-rw-   0        0        0     2897 2024-05-01 21:18:56.000000 besser-1.1.0/besser/utilities/image_to_buml.py
--rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.1.0/besser/utilities/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.113847 besser-1.1.0/besser.egg-info/
--rw-rw-rw-   0        0        0     3777 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3529 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      263 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-01 21:35:01.000000 besser-1.1.0/besser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      277 2024-05-01 21:18:56.000000 besser-1.1.0/requirements.txt
--rw-rw-rw-   0        0        0      659 2024-05-01 21:35:02.116848 besser-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.101845 besser-1.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.103845 besser-1.1.0/tests/gui/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/gui/__init__.py
--rw-rw-rw-   0        0        0     2479 2024-05-01 21:33:29.000000 besser-1.1.0/tests/gui/gui_model.py
--rw-rw-rw-   0        0        0     5271 2024-04-29 14:01:22.000000 besser-1.1.0/tests/gui/test_gui.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.105846 besser-1.1.0/tests/notations/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/notations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.108845 besser-1.1.0/tests/object/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/__init__.py
--rw-rw-rw-   0        0        0    10547 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/library_object.py
--rw-rw-rw-   0        0        0     3879 2024-04-29 14:01:22.000000 besser-1.1.0/tests/object/test_object_mm.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.109845 besser-1.1.0/tests/ocl/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/ocl/__init__.py
--rw-rw-rw-   0        0        0     7566 2024-04-29 14:01:22.000000 besser-1.1.0/tests/ocl/test_ocl_parser.py
-drwxrwxrwx   0        0        0        0 2024-05-01 21:35:02.111845 besser-1.1.0/tests/structural/
--rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.0/tests/structural/__init__.py
--rw-rw-rw-   0        0        0    10194 2024-01-15 16:18:42.000000 besser-1.1.0/tests/structural/test_structural.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.841696 besser-1.1.1/
+-rw-rw-rw-   0        0        0     3777 2024-05-05 18:41:06.840693 besser-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2804 2024-04-29 14:01:22.000000 besser-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.722524 besser-1.1.1/besser/
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.733037 besser-1.1.1/besser/BUML/
+-rw-rw-rw-   0        0        0        0 2023-11-29 15:43:44.000000 besser-1.1.1/besser/BUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.735037 besser-1.1.1/besser/BUML/metamodel/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.1/besser/BUML/metamodel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.737200 besser-1.1.1/besser/BUML/metamodel/gui/
+-rw-rw-rw-   0        0        0       29 2024-03-07 10:53:16.000000 besser-1.1.1/besser/BUML/metamodel/gui/__init__.py
+-rw-rw-rw-   0        0        0    25750 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/gui/graphical_ui.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.740326 besser-1.1.1/besser/BUML/metamodel/object/
+-rw-rw-rw-   0        0        0       21 2024-03-07 08:52:50.000000 besser-1.1.1/besser/BUML/metamodel/object/__init__.py
+-rw-rw-rw-   0        0        0    10058 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/object/object.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.743325 besser-1.1.1/besser/BUML/metamodel/ocl/
+-rw-rw-rw-   0        0        0       20 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/ocl/__init__.py
+-rw-rw-rw-   0        0        0    18910 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/ocl/rules.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.747325 besser-1.1.1/besser/BUML/metamodel/structural/
+-rw-rw-rw-   0        0        0       25 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/metamodel/structural/__init__.py
+-rw-rw-rw-   0        0        0    42620 2024-05-03 13:04:47.000000 besser-1.1.1/besser/BUML/metamodel/structural/structural.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.749157 besser-1.1.1/besser/BUML/notations/
+-rw-rw-rw-   0        0        0        0 2023-10-23 15:26:16.000000 besser-1.1.1/besser/BUML/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.755179 besser-1.1.1/besser/BUML/notations/objectPlantUML/
+-rw-rw-rw-   0        0        0     5938 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODLexer.py
+-rw-rw-rw-   0        0        0     4976 2024-05-03 13:06:20.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODListener.py
+-rw-rw-rw-   0        0        0    25828 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/ODParser.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/objectPlantUML/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.766948 besser-1.1.1/besser/BUML/notations/ocl/
+-rw-rw-rw-   0        0        0    23268 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLLexer.py
+-rw-rw-rw-   0        0        0    41633 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLListener.py
+-rw-rw-rw-   0        0        0   212929 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/BOCLParser.py
+-rw-rw-rw-   0        0        0     4732 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/FactoryInstance.py
+-rw-rw-rw-   0        0        0     1080 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/OCLWrapper.py
+-rw-rw-rw-   0        0        0    12723 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/RootHandler.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/ocl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.777205 besser-1.1.1/besser/BUML/notations/structuralPlantUML/
+-rw-rw-rw-   0        0        0    10331 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py
+-rw-rw-rw-   0        0        0     6394 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py
+-rw-rw-rw-   0        0        0    51575 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py
+-rw-rw-rw-   0        0        0      203 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/__init__.py
+-rw-rw-rw-   0        0        0     9094 2024-05-03 13:06:20.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py
+-rw-rw-rw-   0        0        0     1432 2024-04-29 14:01:22.000000 besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py
+-rw-rw-rw-   0        0        0        0 2024-01-15 16:06:49.000000 besser-1.1.1/besser/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.780209 besser-1.1.1/besser/generators/
+-rw-rw-rw-   0        0        0       34 2023-10-23 15:26:16.000000 besser-1.1.1/besser/generators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.783205 besser-1.1.1/besser/generators/backend/
+-rw-rw-rw-   0        0        0       32 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/backend/__init__.py
+-rw-rw-rw-   0        0        0     3276 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/backend/backend_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.785205 besser-1.1.1/besser/generators/django/
+-rw-rw-rw-   0        0        0       31 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/django/__init__.py
+-rw-rw-rw-   0        0        0     1756 2024-01-15 16:11:55.000000 besser-1.1.1/besser/generators/django/django_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.788900 besser-1.1.1/besser/generators/django/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/django/templates/__init__.py
+-rw-rw-rw-   0        0        0      608 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/django/templates/django_fields.py.j2
+-rw-rw-rw-   0        0        0     3580 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/django/templates/django_template.py.j2
+-rw-rw-rw-   0        0        0     1166 2024-04-29 14:01:22.000000 besser-1.1.1/besser/generators/generator_interface.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.793002 besser-1.1.1/besser/generators/pydantic_classes/
+-rw-rw-rw-   0        0        0       41 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/__init__.py
+-rw-rw-rw-   0        0        0     2593 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/pydantic_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.795900 besser-1.1.1/besser/generators/pydantic_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     3409 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.798001 besser-1.1.1/besser/generators/python_classes/
+-rw-rw-rw-   0        0        0       39 2023-11-03 14:54:15.000000 besser-1.1.1/besser/generators/python_classes/__init__.py
+-rw-rw-rw-   0        0        0     1722 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/python_classes/python_classes_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.801949 besser-1.1.1/besser/generators/python_classes/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/python_classes/templates/__init__.py
+-rw-rw-rw-   0        0        0     1461 2024-01-05 14:02:17.000000 besser-1.1.1/besser/generators/python_classes/templates/class_parameters.py.j2
+-rw-rw-rw-   0        0        0     1496 2024-01-04 17:15:56.000000 besser-1.1.1/besser/generators/python_classes/templates/python_classes_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.804900 besser-1.1.1/besser/generators/rest_api/
+-rw-rw-rw-   0        0        0       33 2024-03-07 08:29:25.000000 besser-1.1.1/besser/generators/rest_api/__init__.py
+-rw-rw-rw-   0        0        0     4716 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/rest_api_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.808899 besser-1.1.1/besser/generators/rest_api/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-07 08:29:25.000000 besser-1.1.1/besser/generators/rest_api/templates/__init__.py
+-rw-rw-rw-   0        0        0    11014 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/templates/backend_fast_api_template.py.j2
+-rw-rw-rw-   0        0        0     4987 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/rest_api/templates/fast_api_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.811900 besser-1.1.1/besser/generators/sql/
+-rw-rw-rw-   0        0        0       28 2023-11-03 14:54:15.000000 besser-1.1.1/besser/generators/sql/__init__.py
+-rw-rw-rw-   0        0        0     2191 2024-01-15 16:14:26.000000 besser-1.1.1/besser/generators/sql/sql_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.815900 besser-1.1.1/besser/generators/sql/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/sql/templates/__init__.py
+-rw-rw-rw-   0        0        0     4633 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/sql/templates/sql_dialects.sql.j2
+-rw-rw-rw-   0        0        0     3608 2023-11-24 11:35:33.000000 besser-1.1.1/besser/generators/sql/templates/sql_template.sql.j2
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.817998 besser-1.1.1/besser/generators/sql_alchemy/
+-rw-rw-rw-   0        0        0       36 2023-11-23 14:47:36.000000 besser-1.1.1/besser/generators/sql_alchemy/__init__.py
+-rw-rw-rw-   0        0        0     1994 2024-01-15 16:14:45.000000 besser-1.1.1/besser/generators/sql_alchemy/sql_alchemy_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.819900 besser-1.1.1/besser/generators/sql_alchemy/templates/
+-rw-rw-rw-   0        0        0        0 2024-01-05 16:17:26.000000 besser-1.1.1/besser/generators/sql_alchemy/templates/__init__.py
+-rw-rw-rw-   0        0        0     3695 2024-05-01 21:18:56.000000 besser-1.1.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.823901 besser-1.1.1/besser/utilities/
+-rw-rw-rw-   0        0        0       50 2024-01-04 13:03:26.000000 besser-1.1.1/besser/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2897 2024-05-01 21:18:56.000000 besser-1.1.1/besser/utilities/image_to_buml.py
+-rw-rw-rw-   0        0        0     2106 2024-01-15 16:16:07.000000 besser-1.1.1/besser/utilities/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.838686 besser-1.1.1/besser.egg-info/
+-rw-rw-rw-   0        0        0     3777 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3529 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      263 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-05 18:41:06.000000 besser-1.1.1/besser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       97 2023-10-23 15:26:16.000000 besser-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      277 2024-05-01 21:18:56.000000 besser-1.1.1/requirements.txt
+-rw-rw-rw-   0        0        0      659 2024-05-05 18:41:06.842695 besser-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.824900 besser-1.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.828901 besser-1.1.1/tests/gui/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/gui/__init__.py
+-rw-rw-rw-   0        0        0     2461 2024-05-03 13:07:26.000000 besser-1.1.1/tests/gui/gui_model.py
+-rw-rw-rw-   0        0        0     5244 2024-05-03 13:07:26.000000 besser-1.1.1/tests/gui/test_gui.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.829900 besser-1.1.1/tests/notations/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/notations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.833133 besser-1.1.1/tests/object/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/object/__init__.py
+-rw-rw-rw-   0        0        0    10448 2024-05-03 13:07:26.000000 besser-1.1.1/tests/object/library_object.py
+-rw-rw-rw-   0        0        0     3843 2024-05-03 13:07:26.000000 besser-1.1.1/tests/object/test_object_mm.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.835146 besser-1.1.1/tests/ocl/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/ocl/__init__.py
+-rw-rw-rw-   0        0        0     7566 2024-04-29 14:01:22.000000 besser-1.1.1/tests/ocl/test_ocl_parser.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:41:06.837599 besser-1.1.1/tests/structural/
+-rw-rw-rw-   0        0        0        0 2024-04-29 14:01:22.000000 besser-1.1.1/tests/structural/__init__.py
+-rw-rw-rw-   0        0        0    10023 2024-05-03 13:07:26.000000 besser-1.1.1/tests/structural/test_structural.py
```

### Comparing `besser-1.1.0/PKG-INFO` & `besser-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.1.0
+Version: 1.1.1
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
```

### Comparing `besser-1.1.0/README.md` & `besser-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/metamodel/gui/graphical_ui.py` & `besser-1.1.1/besser/BUML/metamodel/gui/graphical_ui.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/metamodel/object/object.py` & `besser-1.1.1/besser/BUML/metamodel/object/object.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/metamodel/ocl/rules.py` & `besser-1.1.1/besser/BUML/metamodel/ocl/rules.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/metamodel/structural/structural.py` & `besser-1.1.1/besser/BUML/metamodel/structural/structural.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,38 +292,38 @@
 class Property(TypedElement):
     """A property can represents an attribute of a class or an end of an association.
 
     Properties are owned by a class or an association.
 
     Args:
         name (str): The name of the property.
-        property_type (Type): The type of the property.
+        type (Type): The type of the property.
         owner (Type): The type that owns the property.
         multiplicity (Multiplicity): The multiplicity of the property.
         visibility (str): The visibility of the property ('public', 'private', etc.).
         is_composite (bool): Indicates whether the property is a composite.
         is_navigable (bool): Indicates whether the property is navigable in a relationship.
         is_id (bool): Indicates whether the property is an id.
         is_read_only (bool): Indicates whether the property is read only.
 
     Attributes:
         name (str): Inherited from TypedElement, represents the name of the property.
-        property_type (Type): Inherited from TypedElement, represents the type of the property.
+        type (Type): Inherited from TypedElement, represents the type of the property.
         owner (Type): The type that owns the property.
         multiplicity (Multiplicity): The multiplicity of the property.
         visibility (str): Inherited from TypedElement, represents the visibility of the property.
         is_composite (bool): Indicates whether the property is a composite.
         is_navigable (bool): Indicates whether the property is navigable in a relationship.
         is_id (bool): Indicates whether the property is an id.
         is_read_only (bool): Indicates whether the property is read only.
     """
     
-    def __init__(self, name: str, property_type: Type, owner: Type = None, multiplicity: Multiplicity = Multiplicity(1, 1), 
+    def __init__(self, name: str, type: Type, owner: Type = None, multiplicity: Multiplicity = Multiplicity(1, 1), 
                  visibility: str = 'public', is_composite: bool = False, is_navigable: bool = True, is_id: bool = False, is_read_only: bool = False):
-        super().__init__(name, property_type, visibility)
+        super().__init__(name, type, visibility)
         self.owner: Type = owner
         self.multiplicity: Multiplicity = multiplicity
         self.is_composite: bool = is_composite
         self.is_navigable: bool = is_navigable
         self.is_id: bool = is_id
         self.is_read_only: bool = is_read_only
```

### Comparing `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODLexer.py` & `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODListener.py` & `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODListener.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     # Exit a parse tree produced by ODParser#property.
     def exitProperty(self, ctx:ODParser.PropertyContext):
         pass
 
 
     # Enter a parse tree produced by ODParser#propertyName.
     def enterPropertyName(self, ctx:ODParser.PropertyNameContext):
-        self.property = Property(name = ctx.getText(),property_type='NP')
+        self.property = Property(name = ctx.getText(),type='NP')
         pass
 
     # Exit a parse tree produced by ODParser#propertyName.
     def exitPropertyName(self, ctx:ODParser.PropertyNameContext):
         pass
 
 
@@ -104,15 +104,15 @@
 
     # Exit a parse tree produced by ODParser#linkDeclaration.
     def exitLinkDeclaration(self, ctx:ODParser.LinkDeclarationContext):
         linkParts = ctx.getText().split(":")[0].split(self.linkType)
         linkName = ctx.getText().split(":")[1]
         obj1 = self.getObject(linkParts[0])
         obj2 = self.getObject(linkParts[1])
-        prop = Property(name = linkName, property_type= 'NF')
+        prop = Property(name = linkName, type= 'NF')
         linkEndLeft = LinkEnd(linkName,prop, obj1)
         linkEndRight = LinkEnd(linkName,prop, obj2)
         link = Link(linkName, None, [linkEndLeft,linkEndRight])
         obj1._add_link(link)
         obj2._add_link(link)
```

### Comparing `besser-1.1.0/besser/BUML/notations/objectPlantUML/ODParser.py` & `besser-1.1.1/besser/BUML/notations/objectPlantUML/ODParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/BOCLLexer.py` & `besser-1.1.1/besser/BUML/notations/ocl/BOCLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/BOCLListener.py` & `besser-1.1.1/besser/BUML/notations/ocl/BOCLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/BOCLParser.py` & `besser-1.1.1/besser/BUML/notations/ocl/BOCLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/FactoryInstance.py` & `besser-1.1.1/besser/BUML/notations/ocl/FactoryInstance.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/OCLWrapper.py` & `besser-1.1.1/besser/BUML/notations/ocl/OCLWrapper.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/ocl/RootHandler.py` & `besser-1.1.1/besser/BUML/notations/ocl/RootHandler.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py` & `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLLexer.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py` & `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLListener.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py` & `besser-1.1.1/besser/BUML/notations/structuralPlantUML/PlantUMLParser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py` & `besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantUML_buml_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         text += ")\n\n"
         self.output.write(text)
         self.__classes.append(ctx.ID().getText())
 
     def enterAttribute(self, ctx: PlantUMLParser.AttributeContext):
         attribute_name = ctx.parentCtx.ID().getText() + "_" + ctx.ID().getText()
         text = attribute_name + ": Property = Property(name=\"" + ctx.ID().getText() + \
-            "\", property_type="+ ctx.primitiveData().getText() +"_type"
+            "\", type="+ ctx.primitiveData().getText() +"_type"
         if ctx.visibility():
             text += ", visibility=\"" + self.visibility[ctx.visibility().getText()] + "\""
         text += ")\n"
         self.output.write(text)
         self.__attr_list.append(attribute_name)
         self.__dtypes.add(ctx.primitiveData().getText())
 
@@ -57,16 +57,16 @@
         cl_name_2 = ctx.ID(1).getText()
         if ctx.ID(2) is None:
             raise ValueError("All the associations in the model must have a name")
         assoc_name = ctx.ID(2).getText()
         if assoc_name in self.__relations:
             raise ValueError("The model cannot have two associations with the same name")
         text = assoc_name + ": BinaryAssociation = BinaryAssociation(name=\"" + assoc_name + "\", ends={\n\
-        Property(name=\"" + assoc_name + "\", property_type=" + cl_name_1 + ", multiplicity=" + getMultiplicity(ctx.c_left) + self.__ends[0] + "),\n\
-        Property(name=\"" + assoc_name + "\", property_type=" + cl_name_2 + ", multiplicity=" + getMultiplicity(ctx.c_right) + self.__ends[1] + ")})\n"
+        Property(name=\"" + assoc_name + "\", type=" + cl_name_1 + ", multiplicity=" + getMultiplicity(ctx.c_left) + self.__ends[0] + "),\n\
+        Property(name=\"" + assoc_name + "\", type=" + cl_name_2 + ", multiplicity=" + getMultiplicity(ctx.c_right) + self.__ends[1] + ")})\n"
         self.__relations[assoc_name] = text
         self.__relation_classes.append(cl_name_1)
         self.__relation_classes.append(cl_name_2)
 
     def enterBidirectional(self, ctx: PlantUMLParser.BidirectionalContext):
         self.__ends = ["", ""]
```

### Comparing `besser-1.1.0/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py` & `besser-1.1.1/besser/BUML/notations/structuralPlantUML/plantuml_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/backend/backend_generator.py` & `besser-1.1.1/besser/generators/backend/backend_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/django/django_generator.py` & `besser-1.1.1/besser/generators/django/django_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/django/templates/django_fields.py.j2` & `besser-1.1.1/besser/generators/django/templates/django_fields.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/django/templates/django_template.py.j2` & `besser-1.1.1/besser/generators/django/templates/django_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/generator_interface.py` & `besser-1.1.1/besser/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/pydantic_classes/pydantic_classes_generator.py` & `besser-1.1.1/besser/generators/pydantic_classes/pydantic_classes_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2` & `besser-1.1.1/besser/generators/pydantic_classes/templates/pydantic_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/python_classes/python_classes_generator.py` & `besser-1.1.1/besser/generators/python_classes/python_classes_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/python_classes/templates/class_parameters.py.j2` & `besser-1.1.1/besser/generators/python_classes/templates/class_parameters.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/python_classes/templates/python_classes_template.py.j2` & `besser-1.1.1/besser/generators/python_classes/templates/python_classes_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/rest_api/rest_api_generator.py` & `besser-1.1.1/besser/generators/rest_api/rest_api_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/rest_api/templates/backend_fast_api_template.py.j2` & `besser-1.1.1/besser/generators/rest_api/templates/backend_fast_api_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/rest_api/templates/fast_api_template.py.j2` & `besser-1.1.1/besser/generators/rest_api/templates/fast_api_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/sql/sql_generator.py` & `besser-1.1.1/besser/generators/sql/sql_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/sql/templates/sql_dialects.sql.j2` & `besser-1.1.1/besser/generators/sql/templates/sql_dialects.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/sql/templates/sql_template.sql.j2` & `besser-1.1.1/besser/generators/sql/templates/sql_template.sql.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/sql_alchemy/sql_alchemy_generator.py` & `besser-1.1.1/besser/generators/sql_alchemy/sql_alchemy_generator.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2` & `besser-1.1.1/besser/generators/sql_alchemy/templates/sql_alchemy_template.py.j2`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/utilities/image_to_buml.py` & `besser-1.1.1/besser/utilities/image_to_buml.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser/utilities/utils.py` & `besser-1.1.1/besser/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/besser.egg-info/PKG-INFO` & `besser-1.1.1/besser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besser
-Version: 1.1.0
+Version: 1.1.1
 Summary: BESSER
 Author: Luxembourg Institute of Science and Technology
 License: MIT
 Project-URL: Documentation, https://besser.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BESSER-PEARL/BESSER
 Project-URL: Bug Tracker, https://github.com/BESSER-PEARL/BESSER/issues
 Keywords: uml,code generation,python
```

### Comparing `besser-1.1.0/besser.egg-info/SOURCES.txt` & `besser-1.1.1/besser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/setup.cfg` & `besser-1.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6573 7365 720d 0a76 6572 7369   = besser..versi
-00000020: 6f6e 203d 2031 2e31 2e30 0d0a 6175 7468  on = 1.1.0..auth
+00000020: 6f6e 203d 2031 2e31 2e31 0d0a 6175 7468  on = 1.1.1..auth
 00000030: 6f72 203d 204c 7578 656d 626f 7572 6720  or = Luxembourg 
 00000040: 496e 7374 6974 7574 6520 6f66 2053 6369  Institute of Sci
 00000050: 656e 6365 2061 6e64 2054 6563 686e 6f6c  ence and Technol
 00000060: 6f67 790d 0a64 6573 6372 6970 7469 6f6e  ogy..description
 00000070: 203d 2042 4553 5345 520d 0a6c 6f6e 675f   = BESSER..long_
 00000080: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 00000090: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
```

### Comparing `besser-1.1.0/tests/gui/gui_model.py` & `besser-1.1.1/tests/gui/gui_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 #   Library class - structural model definition   #
 ###################################################
 
 # Primitive DataTypes
 t_str: PrimitiveDataType = PrimitiveDataType("str")
 
 # Library definition
-library_name: Property = Property(name="name", property_type=t_str)
-address: Property = Property(name="address", property_type=t_str)
+library_name: Property = Property(name="name", type=t_str)
+address: Property = Property(name="address", type=t_str)
 library: Class = Class (name="Library", attributes={library_name, address})
 
 ##################################
 #      GUI model definition      #
 ##################################
 
 #DataSource definition
```

### Comparing `besser-1.1.0/tests/gui/test_gui.py` & `besser-1.1.1/tests/gui/test_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,20 +49,20 @@
         list_duplicate: List = List(name="list1", description="", list_sources={})
         screen1.components={list1, list2, list_duplicate}
         module1.screens = {screen1}
         assert "A screen cannot have two lists with the same name" in str(excinfo.value)
 
 # Test: Do not have two fields with the same name in a list item.
 def test_unique_field_names():
-    field1: Property = Property(name="field1", property_type="")
-    field2: Property = Property(name="field2", property_type="")
+    field1: Property = Property(name="field1", type="")
+    field2: Property = Property(name="field2", type="")
     modelElement: ModelElement = ModelElement(name="item1", dataSourceClass="", fields={field1, field2})
     with pytest.raises(ValueError) as excinfo:
         # Try to create a field with the same name as field1
-        field_duplicate: Property = Property(name="field1", property_type="")
+        field_duplicate: Property = Property(name="field1", type="")
         modelElement.fields={field1, field2, field_duplicate}
         assert "A list item cannot have two fields with the same name" in str(excinfo.value)
 
 # Test: Do not have two items with the same name in a list.
 def test_unique_item_names():
     item1: ModelElement = ModelElement(name="item1", dataSourceClass="", fields={})
     item2: ModelElement = ModelElement(name="item2", dataSourceClass="", fields={})
```

### Comparing `besser-1.1.0/tests/object/library_object.py` & `besser-1.1.1/tests/object/library_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,40 +10,40 @@
 
 # Primitive DataTypes
 t_int: PrimitiveDataType = PrimitiveDataType("int")
 t_str: PrimitiveDataType = PrimitiveDataType("str")
 t_date: PrimitiveDataType = PrimitiveDataType("date")
 
 # Library attributes definition
-library_name: Property = Property(name="name", property_type=t_str)
-address: Property = Property(name="address", property_type=t_str)
+library_name: Property = Property(name="name", type=t_str)
+address: Property = Property(name="address", type=t_str)
 # Library class definition
 library: Class = Class (name="Library", attributes={library_name, address})
 
 # Book attributes definition
-title: Property = Property(name="title", property_type=t_str)
-pages: Property = Property(name="pages", property_type=t_int)
-release: Property = Property(name="release", property_type=t_date)
+title: Property = Property(name="title", type=t_str)
+pages: Property = Property(name="pages", type=t_int)
+release: Property = Property(name="release", type=t_date)
 # Book class definition
 book: Class = Class (name="Book", attributes={title, pages, release})
 
 # Author attributes definition
-author_name: Property = Property(name="name", property_type=t_str)
-email: Property = Property(name="email", property_type=t_str)
+author_name: Property = Property(name="name", type=t_str)
+email: Property = Property(name="email", type=t_str)
 # Author class definition
 author: Class = Class (name="Author", attributes={author_name, email})
 
 # Library-Book association definition
-located_in: Property = Property(name="locatedIn",property_type=library, multiplicity=Multiplicity(1, 1))
-has: Property = Property(name="has", property_type=book, multiplicity=Multiplicity(0, "*"))
+located_in: Property = Property(name="locatedIn",type=library, multiplicity=Multiplicity(1, 1))
+has: Property = Property(name="has", type=book, multiplicity=Multiplicity(0, "*"))
 lib_book_association: BinaryAssociation = BinaryAssociation(name="lib_book_assoc", ends={located_in, has})
 
 # Book-Author association definition
-publishes: Property = Property(name="publishes", property_type=book, multiplicity=Multiplicity(0, "*"))
-writed_by: Property = Property(name="writedBy", property_type=author, multiplicity=Multiplicity(1, "*"))
+publishes: Property = Property(name="publishes", type=book, multiplicity=Multiplicity(0, "*"))
+writed_by: Property = Property(name="writedBy", type=author, multiplicity=Multiplicity(1, "*"))
 book_author_association: BinaryAssociation = BinaryAssociation(name="book_author_assoc", ends={writed_by, publishes})
 
 constraintPageNumber: Constraint = Constraint(name = "libraryPageNumber",context=library,expression="context Library inv inv1: self.has ->forAll(b:Book|b.pages>0)",language="OCL")
 
 constraintBookPageNumber: Constraint = Constraint(name = "BookPageNumber",context=book,expression="context Book inv inv2: self.pages>0",language="OCL")
 
 constraintTitleIncorrect: Constraint = Constraint(name = "BookTitleInc",context=book,expression="context Book inv inv2: self.title= 'NI')",language="OCL")
```

### Comparing `besser-1.1.0/tests/object/test_object_mm.py` & `besser-1.1.1/tests/object/test_object_mm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from besser.BUML.metamodel.object import *
 from besser.BUML.metamodel.structural import *
 
 ########################
 #   Structural model   #
 ########################
 
-attribute1: Property = Property(name="A1", property_type=PrimitiveDataType("int"))
-attribute2: Property = Property(name="A2", property_type=PrimitiveDataType("str"))
+attribute1: Property = Property(name="A1", type=PrimitiveDataType("int"))
+attribute2: Property = Property(name="A2", type=PrimitiveDataType("str"))
 class1: Class = Class(name="class1", attributes={attribute1, attribute2})
 class2: Class = Class(name="class2", attributes=set())
-aend1: Property = Property(name="end1", property_type=class1, multiplicity=Multiplicity(0, 1))
-aend2: Property = Property(name="end2", property_type=class2, multiplicity=Multiplicity(0, "*"))
+aend1: Property = Property(name="end1", type=class1, multiplicity=Multiplicity(0, 1))
+aend2: Property = Property(name="end2", type=class2, multiplicity=Multiplicity(0, "*"))
 association1: BinaryAssociation = BinaryAssociation(name="association1", ends={aend1, aend2})
 
 ##########################
 #   Object model tests   #
 ##########################
 
 # Testing model initialization
```

### Comparing `besser-1.1.0/tests/ocl/test_ocl_parser.py` & `besser-1.1.1/tests/ocl/test_ocl_parser.py`

 * *Files identical despite different names*

### Comparing `besser-1.1.0/tests/structural/test_structural.py` & `besser-1.1.1/tests/structural/test_structural.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,112 +27,112 @@
         model: DomainModel = DomainModel(name="mymodel", types={class1, class2}, associations = None, packages = None, constraints = None)
         assert "same name" in str(excinfo.value)
 
 
 # Testing attributes initialization
 def test_attribute_initialization():
     class1: Type = Type(name="name1")
-    attribute1: Property = Property(name="attribute1", owner = class1, property_type=PrimitiveDataType("int"),
+    attribute1: Property = Property(name="attribute1", owner = class1, type=PrimitiveDataType("int"),
                                     multiplicity=Multiplicity(0, 1))
     # assert attributes has proper type and multiplicity
     assert attribute1.type.name == "int"
     assert attribute1.multiplicity.min == 0
     assert attribute1.multiplicity.max == 1
 
 
 # Testing attribute multiplicity and data type violations
 def test_attribute_type_and_multiplicity_violation():
     with pytest.raises(ValueError) as excinfo:
-        attribute1: Property = Property(name="attribute1", property_type=PrimitiveDataType("int"),
+        attribute1: Property = Property(name="attribute1", type=PrimitiveDataType("int"),
                                         multiplicity=Multiplicity(0, -1))
         assert "Invalid max multiplicity" in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
-        attribute1: Property = Property(name="attribute1", property_type=PrimitiveDataType("int"),
+        attribute1: Property = Property(name="attribute1", type=PrimitiveDataType("int"),
                                         multiplicity=Multiplicity(-1, 1))
         assert "Invalid min multiplicity" in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
-        attribute1: Property = Property(name="attribute1", property_type=PrimitiveDataType("int"),
+        attribute1: Property = Property(name="attribute1", type=PrimitiveDataType("int"),
                                         multiplicity=Multiplicity(2, 1))
         assert "Invalid max multiplicity" in str(excinfo.value)
 
     with pytest.raises(ValueError) as excinfo:
-        attribute1: Property = Property(name="attribute1", property_type=PrimitiveDataType("invented_type"),
+        attribute1: Property = Property(name="attribute1", type=PrimitiveDataType("invented_type"),
                                         multiplicity=Multiplicity(2, 1))
         assert "Invalid primitive data type" in str(excinfo.value)
 
 
 # Testing class initialization
 def test_class_initialization():
     class1: Class = Class(name="classA", attributes=set())
     class2: Class
-    attribute1: Property = Property(name="attribute1", owner=None, property_type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
-    attribute2: Property = Property(name="attribute2", owner=None, property_type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
-    reference1: Property = Property(name="reference1", owner=None, property_type=class1, multiplicity=Multiplicity(0, 1))
+    attribute1: Property = Property(name="attribute1", owner=None, type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
+    attribute2: Property = Property(name="attribute2", owner=None, type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
+    reference1: Property = Property(name="reference1", owner=None, type=class1, multiplicity=Multiplicity(0, 1))
     class2: Class = Class(name="classB", attributes={attribute1, attribute2})
     assert len(class2.attributes) == 2
     print(class2)
 
 
 # Testing no duplicated names in class attributes
 def test_duplicated_name_class():
     with pytest.raises(ValueError) as excinfo:
         class1 : Class
-        attribute1: Property = Property(name="attribute1", owner=None, property_type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
-        attribute2: Property = Property(name="attribute1", owner=None, property_type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
+        attribute1: Property = Property(name="attribute1", owner=None, type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
+        attribute2: Property = Property(name="attribute1", owner=None, type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
         class1 = Class(name="name1", attributes={attribute1, attribute2})
         assert "A class cannot have two attributes with the same name" in str(excinfo.value)
 
 # Testing for no more than one id attribute in class
 def test_more_than_one_id_class():
     with pytest.raises(ValueError) as excinfo:
         class1 : Class
-        attribute1: Property = Property(name="attribute1", property_type=PrimitiveDataType("int"), is_id=True)
-        attribute2: Property = Property(name="attribute2", property_type=PrimitiveDataType("int"), is_id=True)
+        attribute1: Property = Property(name="attribute1", type=PrimitiveDataType("int"), is_id=True)
+        attribute2: Property = Property(name="attribute2", type=PrimitiveDataType("int"), is_id=True)
         class1 = Class(name="name1", attributes={attribute1, attribute2})
         assert "A class cannot have two id attributes" in str(excinfo.value)
 
 def test_association_initialization():
     class1: Class = Class(name="name1", attributes=set())
     class2: Class = Class(name="name2", attributes=set())
-    aend1: Property = Property(name="end1", owner=None, property_type=class1, multiplicity=Multiplicity(0, 1))
-    aend2: Property = Property(name="end2", owner=None, property_type=class2, multiplicity=Multiplicity(0, 1))
+    aend1: Property = Property(name="end1", owner=None, type=class1, multiplicity=Multiplicity(0, 1))
+    aend2: Property = Property(name="end2", owner=None, type=class2, multiplicity=Multiplicity(0, 1))
     association: BinaryAssociation = BinaryAssociation(name="association1", ends={aend1, aend2})
     assert len(association.ends) == 2
     assert aend1 in association.ends
     assert aend1.owner == association
     assert class1.associations == {association}
     assert class1.association_ends() == {aend2}
 
 # Testing the creation of a binary association cannot have more than two ends
 def test_binary_association():
     with pytest.raises(ValueError) as excinfo:
         class1: Type = Type(name="name1")
-        aend: Property = Property(name="end1", owner=None, property_type=class1, multiplicity=Multiplicity(0, 1))
+        aend: Property = Property(name="end1", owner=None, type=class1, multiplicity=Multiplicity(0, 1))
         association: BinaryAssociation = BinaryAssociation(name="association1", ends={aend})
         assert "A binary association should have two ends" in str(excinfo.value)
 
 
 # Testing the creation of an association class with an attribute
 def test_association_class():
     class1: Class = Class(name="name1", attributes=None)
     class2: Class = Class(name="name2", attributes=None)
-    aend1: Property = Property(name="end1", owner=None, property_type=class1, multiplicity=Multiplicity(0, 1))
-    aend2: Property = Property(name="end2", owner=None, property_type=class2, multiplicity=Multiplicity(0, 1))
+    aend1: Property = Property(name="end1", owner=None, type=class1, multiplicity=Multiplicity(0, 1))
+    aend2: Property = Property(name="end2", owner=None, type=class2, multiplicity=Multiplicity(0, 1))
     association: BinaryAssociation = BinaryAssociation(name="association1", ends={aend1, aend2})
-    attribute1: Property = Property(name="attribute1", owner=None, property_type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
+    attribute1: Property = Property(name="attribute1", owner=None, type=PrimitiveDataType("int"), multiplicity=Multiplicity(0, 1))
     association_class: AssociationClass = AssociationClass(name="association_class1", attributes={attribute1}, association=association)
     assert len(association_class.attributes) == 1
     assert attribute1 in association_class.attributes
     assert association_class.association.name == "association1"
 
 
 def test_generalization_initialization():
-    attribute1: Property = Property(name="attribute1", owner = None, property_type=PrimitiveDataType("int"),
+    attribute1: Property = Property(name="attribute1", owner = None, type=PrimitiveDataType("int"),
                                     multiplicity=Multiplicity(0, 1))
     class1: Class = Class(name="name1", attributes={attribute1})
     class2: Class = Class(name="name2", attributes=None)
     generalization: Generalization = Generalization(general=class1, specific=class2)
     assert generalization.general == class1
     assert generalization.specific == class2
     assert class2.generalizations == {generalization}
```

