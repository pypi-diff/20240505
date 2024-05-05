# Comparing `tmp/mp2c-0.0.1.tar.gz` & `tmp/mp2c-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mp2c-0.0.1.tar", last modified: Sun Mar 31 14:44:15 2024, max compression
+gzip compressed data, was "mp2c-0.0.2.tar", last modified: Sun May  5 15:01:06 2024, max compression
```

## Comparing `mp2c-0.0.1.tar` & `mp2c-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 14:44:15.967200 mp2c-0.0.1/
--rw-rw-rw-   0        0        0      117 2024-03-31 14:44:15.966200 mp2c-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-03-30 02:15:52.000000 mp2c-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 14:44:15.959677 mp2c-0.0.1/mp2c/
--rw-rw-rw-   0        0        0       56 2024-03-31 03:17:04.000000 mp2c-0.0.1/mp2c/__init__.py
--rw-rw-rw-   0        0        0     4811 2024-03-31 03:19:44.000000 mp2c-0.0.1/mp2c/parser.py
-drwxrwxrwx   0        0        0        0 2024-03-31 14:44:15.965195 mp2c-0.0.1/mp2c.egg-info/
--rw-rw-rw-   0        0        0      117 2024-03-31 14:44:15.000000 mp2c-0.0.1/mp2c.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2024-03-31 14:44:15.000000 mp2c-0.0.1/mp2c.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 14:44:15.000000 mp2c-0.0.1/mp2c.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-31 14:44:15.000000 mp2c-0.0.1/mp2c.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 14:44:15.967200 mp2c-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      430 2024-03-31 14:43:43.000000 mp2c-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.909753 mp2c-0.0.2/
+-rw-rw-rw-   0        0        0      117 2024-05-05 15:01:06.908262 mp2c-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-03-30 02:15:52.000000 mp2c-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.903206 mp2c-0.0.2/mp2c/
+-rw-rw-rw-   0        0        0      168 2024-05-05 14:30:01.000000 mp2c-0.0.2/mp2c/__init__.py
+-rw-rw-rw-   0        0        0    12644 2024-04-13 09:26:13.000000 mp2c-0.0.2/mp2c/compiler.py
+-rw-rw-rw-   0        0        0     4818 2024-05-05 13:04:09.000000 mp2c-0.0.2/mp2c/context.py
+-rw-rw-rw-   0        0        0      685 2024-05-05 14:30:00.000000 mp2c-0.0.2/mp2c/converter.py
+-rw-rw-rw-   0        0        0     4691 2024-05-04 03:46:19.000000 mp2c-0.0.2/mp2c/rules.py
+-rw-rw-rw-   0        0        0     1492 2024-05-05 14:24:40.000000 mp2c-0.0.2/mp2c/utils.py
+-rw-rw-rw-   0        0        0    31962 2024-05-05 14:42:11.000000 mp2c-0.0.2/mp2c/visitors.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.907085 mp2c-0.0.2/mp2c.egg-info/
+-rw-rw-rw-   0        0        0      117 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-05 15:01:06.000000 mp2c-0.0.2/mp2c.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 15:01:06.909753 mp2c-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      430 2024-05-05 14:59:10.000000 mp2c-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 15:01:06.907085 mp2c-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-13 14:05:25.000000 mp2c-0.0.2/test/test_visitors.py
```

### Comparing `mp2c-0.0.1/mp2c/parser.py` & `mp2c-0.0.2/mp2c/rules.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,110 @@
-from typing import Any
-import lark
-from lark import Lark, Transformer, v_args
-rules=r"""
-%import common.DIGIT
-%import common.LETTER
-%import common.WS
+rules = r"""
 programstruct            : program_head ";" program_body "."
-program_head              : "program" id "(" idlist ")"
-                          | "program" id
+program_head             : "program" id "(" idlist ")"
+                         | "program" id
 idlist                   : id
-                          | idlist "," id
+                         | idlist "," id
 program_body             : const_declarations var_declarations subprogram_declarations compound_statement
 const_declarations       : empty
-                          | "const" const_declaration ";"
-const_declaration        : id "=" const_value
-                          | const_declaration ";" id "=" const_value
-const_value              : "+" num
-                          | "-" num
-                          | num
-                          | "'" LETTER "'"
+                         | "const" const_declaration ";"
+const_declaration        : id "=" const_value (";" id "=" const_value)*
+const_value              : PLUS num
+                         | MINUS num
+                         | num
+                         | "'" LETTER "'"
+PLUS                     : "+"
+MINUS                    : "-"        
 var_declarations         : empty
-                          | "var" var_declaration ";"
+                         | "var" var_declaration ";"
 var_declaration          : idlist ":" type
-                          | var_declaration ";" idlist ":" type
+                         | var_declaration ";" idlist ":" type
 type                     : basic_type
-                          | "array" "[" period "]" "of" basic_type
-basic_type               : "integer"
-                          | "real"
-                          | "boolean"
-                          | "char"
-period                   : digits ".." digits
-                          | period "," digits ".." digits
-
+                         | "array" "[" period "]" "of" basic_type
+basic_type               : INTEGER
+                         | REAL
+                         | BOOLEAN
+                         | CHAR
+period                   : DIGITS ".." DIGITS
+                         | period "," DIGITS ".." DIGITS
 subprogram_declarations  : empty
-                          | subprogram_declarations subprogram ";"
-subprogram                : subprogram_head ";" subprogram_body
-subprogram_head           : "procedure" id formal_parameter
-                          | "function" id formal_parameter ":" basic_type
-formal_parameter         : empty
-                          | "(" parameter_list ")"
-parameter_list           : parameter
-                          | parameter_list ";" parameter
+                         | subprogram_declarations subprogram ";"
+subprogram               : subprogram_head ";" subprogram_body
+subprogram_head          : "procedure" id formal_parameter
+                         | "function" id formal_parameter ":" basic_type
+formal_parameter         : "(" parameter_list ")"
+parameter_list           : empty
+                         | parameter (";" parameter)*
 parameter                : var_parameter
-                          | value_parameter
+                         | value_parameter
 var_parameter            : "var" value_parameter
 value_parameter          : idlist ":" basic_type
 subprogram_body          : const_declarations var_declarations compound_statement
 compound_statement       : "begin" statement_list "end"
-statement_list           : statement
-                          | statement_list ";" statement
+statement_list           : statement (";" statement)*
 statement                : empty
-                          | variable assignop expression
-                          | func_id assignop expression
-                          | procedure_call
-                          | compound_statement
-                          | "if" expression "then" statement else_part
-                          | "for" id assignop expression "to" expression "do" statement
-                          | "while" expression "do" statement
-                          | "read\(" variable_list ")"
-                          | "write\(" expression_list ")"
-variable_list            : variable
-                          | variable_list "," variable
+                         | assign_statement
+                         | procedure_call
+                         | compound_statement
+                         | if_else_statement
+                         | for_statement
+                         | while_statement
+assign_statement         : variable ASSIGNOP expression
+                         | func_id ASSIGNOP expression
+if_else_statement        : "if" expression "then" statement else_part
+for_statement            : "for" id ASSIGNOP expression "to" expression "do" statement
+while_statement          : "while" expression "do" statement
+variable_list            : variable ("," variable)*
 variable                 : id id_varpart
 id_varpart               : empty
-                          | "[" expression_list "]"
+                         | "[" expression_list "]"
 procedure_call           : id
-                          | id "(" expression_list ")"
+                         | id "(" expression_list ")"
 else_part                : empty
-                          | "else" statement
-expression_list          : expression
-                          | expression_list "," expression
+                         | "else" statement
+expression_list          : expression ("," expression)*
 expression               : simple_expression
-                          | simple_expression relop simple_expression
+                         | simple_expression RELOP simple_expression
 simple_expression        : term
-                          | simple_expression addop term
+                         | simple_expression ADDOP term
 term                     : factor
-                          | term mulop factor
+                         | term MULOP factor
 factor                   : num
-                          | variable
-                          | "(" expression ")"
-                          | "not" factor
-                          | uminus factor
-                          | func_id "(" expression_list ")"
-
-digits                   : DIGIT+
-id                     : LETTER (LETTER | DIGIT)*
-optional_fraction     : empty
-                        | "." digits
-num                   : digits optional_fraction
-relop                 : "="
-                        | "<>"
-                        | "<"
-                        | "<="
-                        | ">"
-                        | ">="
-addop                 : "+"
-                        | "-"
-                        | "or"
-mulop                 : "*"
-                        |"/"
-                        | "div"
-                        | "mod"
-                        | "and"
-assignop              : ":="
-empty                 : WS*
-func_id               : id
-uminus                : "-"
-
+                         | variable
+                         | "(" expression ")"
+                         | NOT factor
+                         | UMINUS factor
+                         | function_call
+function_call            : func_id "(" expression_list ")"
+NOT                      : "not"
+DIGITS                   : DIGIT+
+id                       : IDENTIFIER_TOKEN
+optional_fraction        : "." DIGITS
+num                      : DIGITS optional_fraction?
+RELOP                    : "="
+                         | "<>"
+                         | "<"
+                         | "<="
+                         | ">"
+                         | ">="
+ADDOP                    : "+"
+                         | "-"
+                         | "or"
+MULOP                    : "*"
+                         | "/"
+                         | "div"
+                         | "mod"
+                         | "and"
+ASSIGNOP                 : ":="
+empty                    : WS*
+func_id                  : id
+UMINUS                   : "-"
+IDENTIFIER_TOKEN         : /[a-zA-Z_][a-zA-Z0-9_]*/
+INTEGER                  : "integer"
+REAL                     : "real"
+BOOLEAN                  : "boolean"
+CHAR                     : "char"
+%import common.DIGIT
+%import common.LETTER
+%import common.WS
 %ignore WS
-"""
-class MP2CParser():
-    def __init__(self):
-        self.parser = Lark(rules, start='programstruct')
-
-    def __call__(self, code) -> Any:
-        return self.parser.parse(code).pretty()
-
-    
+"""
```

