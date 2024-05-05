# Comparing `tmp/esb-0.1.1.tar.gz` & `tmp/esb-0.1.2.tar.gz`

## Comparing `esb-0.1.1.tar` & `esb-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,41 @@
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/__init__.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/__main__.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/boiler.py
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/cli.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/config.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/dash.py
--rw-r--r--   0        0        0    11511 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/db.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/fetch.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/langs.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/paths.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/blank/.gitignore
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/blank/README.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/boilers/python/spec.json
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/boilers/python/template/main.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/__init__.py
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/base.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/fetch.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/new.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/run.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/show.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/start.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/status.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/commands/test.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/protocol/__init__.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/protocol/fireplacev1_0.py
--rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 esb-0.1.1/src/esb/protocol/metric_prefix.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 esb-0.1.1/.gitignore
--rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 esb-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     5945 2020-02-02 00:00:00.000000 esb-0.1.1/README.md
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 esb-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    47516 2020-02-02 00:00:00.000000 esb-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/__main__.py
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boiler.py
+-rw-r--r--   0        0        0     7351 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/cli.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/config.py
+-rw-r--r--   0        0        0     7745 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/dash.py
+-rw-r--r--   0        0        0    12234 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/db.py
+-rw-r--r--   0        0        0     5569 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/fetch.py
+-rw-r--r--   0        0        0     3166 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/langs.py
+-rw-r--r--   0        0        0     4003 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/paths.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/blank/.gitignore
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/blank/README.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/elixir/spec.json
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/elixir/base/.formatter.exs
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/elixir/base/.gitignore
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/elixir/base/mix.exs
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/elixir/template/lib/main.ex
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/python/spec.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/python/template/main.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/rust/spec.json
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/rust/base/.gitignore
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/rust/base/Cargo.toml
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/boilers/rust/template/src/main.rs
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/__init__.py
+-rw-r--r--   0        0        0     3701 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/base.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/dashboard.py
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/fetch.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/new.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/run.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/show.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/start.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/status.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/commands/test.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/protocol/__init__.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/protocol/fireplacev1_0.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 esb-0.1.2/src/esb/protocol/metric_prefix.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 esb-0.1.2/.gitignore
+-rw-r--r--   0        0        0    34916 2020-02-02 00:00:00.000000 esb-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 esb-0.1.2/README.md
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 esb-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    47781 2020-02-02 00:00:00.000000 esb-0.1.2/PKG-INFO
```

### Comparing `esb-0.1.1/src/esb/cli.py` & `esb-0.1.2/src/esb/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -86,26 +86,19 @@
     show = auto()
     status = auto()
     test = auto()
     run = auto()
     dashboard = auto()
 
 
-def esb_parser() -> argparse.ArgumentParser:
-    cmd_descriptions = {
-        Command.new: "Initializes the ESB repo tool",
-        Command.fetch: "Fetches problem statement and data",
-        Command.start: "Prepares boilerplate code for the given language and day",
-        Command.show: "Show problem statement and answers",
-        Command.status: "Checks progress",
-        Command.test: "Runs test cases",
-        Command.run: "Runs with real input",
-        Command.dashboard: "Rebuilds the dashboard",
-    }
+def set_arguments(parser, args, kwargs):
+    parser.add_argument(*args, **kwargs)
 
+
+def esb_parser() -> argparse.ArgumentParser:
     description = (
         "Script your way to rescue Christmas as part of the ElfScript Brigade team.\n\n"
         "`esb` is a CLI tool to help us _elves_ to save Christmas for the [Advent Of Code](https://adventofcode.com/)"
         "yearly events (Thank you [Eric 😉!](https://twitter.com/ericwastl)).\n"
         "For more information visit https://github.com/luxedo/esb"
     )
     parser = argparse.ArgumentParser(description=description)
@@ -115,61 +108,95 @@
     subparsers = parser.add_subparsers(
         title="command",
         description="What do you want to do?",
         required=True,
         dest="command",
     )
     lmap = LangMap.load()
-    parsers = {}
-    for cmd in Command:
-        parsers[cmd] = subparsers.add_parser(cmd.name, description=cmd_descriptions[cmd])
-        if cmd in {Command.fetch, Command.start}:
-            parsers[cmd].add_argument(
-                "-f",
-                "--force",
-                action="store_true",
-                help="Ignore cache and fetch again",
-            )
-
-        if cmd in {Command.fetch, Command.start, Command.show}:
-            parsers[cmd].add_argument("-y", "--year", required=True, nargs="+", type=aoc_year, help="AoC year")
-            parsers[cmd].add_argument("-d", "--day", required=True, nargs="+", type=aoc_day, help="AoC day")
-
-        if cmd == Command.start:
-            parsers[cmd].add_argument(
-                "-l",
-                "--language",
-                required=True,
-                action=AocLangAction,
-                lmap=lmap,
-                choices=lmap.names,
-            )
-
-        if cmd in {Command.test, Command.run}:
-            parsers[cmd].add_argument(
-                "-l",
-                "--language",
-                required=True,
-                action=AocLangAction,
-                lmap=lmap,
-                choices=lmap.names,
-            )
-            parsers[cmd].add_argument("-y", "--year", nargs="+", type=aoc_year, help="AoC year")
-            parsers[cmd].add_argument("-d", "--day", nargs="+", type=aoc_day, help="AoC day")
-
-        if cmd in {Command.run, Command.test}:
-            parsers[cmd].add_argument("-s", "--submit", action="store_true", help="Submits solution")
-            parsers[cmd].add_argument(
-                "-p",
-                "--parts",
-                required=True,
-                choices=get_args(FPPart),
-                type=int,
-                help="Run for part 1 or part 2",
-            )
+
+    cmd_descriptions = {
+        Command.new: "Initializes the ESB repo tool",
+        Command.fetch: "Fetches problem statement and data",
+        Command.start: "Prepares boilerplate code for the given language and day",
+        Command.show: "Show problem statement and answers",
+        Command.status: "Checks progress",
+        Command.test: "Runs test cases",
+        Command.run: "Runs with real input",
+        Command.dashboard: "Rebuilds the dashboard",
+    }
+
+    parsers = {cmd: subparsers.add_parser(cmd.name, description=cmd_descriptions[cmd]) for cmd in Command}
+
+    # Arguments
+    force_arg = (
+        ["-f", "--force"],
+        {"action": "store_true", "help": "Ignore cache and fetch again"},
+    )
+    year_arg = (
+        ["-y", "--year"],
+        {"required": True, "nargs": "+", "type": aoc_year, "help": "AoC year"},
+    )
+    day_arg = (
+        ["-d", "--day"],
+        {"required": True, "nargs": "+", "type": aoc_day, "help": "AoC day"},
+    )
+    lang_arg = (
+        ["-l", "--language"],
+        {
+            "required": True,
+            "action": AocLangAction,
+            "lmap": lmap,
+            "choices": lmap.names,
+        },
+    )
+    submit_arg = (
+        ["-s", "--submit"],
+        {"action": "store_true", "help": "Submits solution"},
+    )
+    part_arg = (
+        ["-p", "--parts"],
+        {
+            "required": True,
+            "choices": get_args(FPPart),
+            "type": int,
+            "help": "Run for part 1 or part 2",
+        },
+    )
+
+    # New
+    # Fetch
+    set_arguments(parsers[Command.fetch], *year_arg)
+    set_arguments(parsers[Command.fetch], *day_arg)
+    set_arguments(parsers[Command.fetch], *force_arg)
+
+    # Start
+    set_arguments(parsers[Command.start], *year_arg)
+    set_arguments(parsers[Command.start], *day_arg)
+    set_arguments(parsers[Command.start], *lang_arg)
+    set_arguments(parsers[Command.start], *force_arg)
+
+    # Show
+    set_arguments(parsers[Command.show], *year_arg)
+    set_arguments(parsers[Command.show], *day_arg)
+
+    # Status
+    # Test
+    set_arguments(parsers[Command.test], *year_arg)
+    set_arguments(parsers[Command.test], *day_arg)
+    set_arguments(parsers[Command.test], *lang_arg)
+    set_arguments(parsers[Command.test], *part_arg)
+
+    # Run
+    set_arguments(parsers[Command.run], *year_arg)
+    set_arguments(parsers[Command.run], *day_arg)
+    set_arguments(parsers[Command.run], *lang_arg)
+    set_arguments(parsers[Command.run], *part_arg)
+    set_arguments(parsers[Command.run], *submit_arg)
+
+    # Dashboard
 
     return parser
 
 
 ###########################################################
 # CLI main
 ###########################################################
@@ -189,18 +216,12 @@
             esb_commands.show(args.year, args.day)
         case Command.status:
             esb_commands.status()
         case Command.run:
             esb_commands.run(args.language, args.parts, args.year, args.day, submit=args.submit)
         case Command.test:
             esb_commands.test(args.language, args.parts, args.year, args.day)
+        case Command.dashboard:
+            esb_commands.dashboard()
         case _:
             message = "Should never reach here :thinking_face:"
             raise ValueError(message)
-    #     case Command.run | Command.test:
-    #         aoc_main(spec, RunMode[args.command], args.year, args.day)
-    #     case Command.fetch:
-    #         prepare_template(spec, args.year, args.day, cookie)
-    #     case Command.fetch2:
-    #         update_main_template(spec, args.year, args.day, cookie)
-    #     case _:
-    #         raise ValueError(f"Command '{args.command}' not found.")
```

### Comparing `esb-0.1.1/src/esb/config.py` & `esb-0.1.2/src/esb/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,13 +20,16 @@
     package_root = Path(__file__).parent
     blank_dir = "blank"
     solutions_dir = "solutions"
     boiler_dir = "boilers"
     cache_dir = ".cache"
     tests_dir = "tests"
     boiler_template = "template"
+    boiler_template_base = "base"
     blank_root = package_root / blank_dir
     boiler_root = package_root / boiler_dir
     spec_filename = "spec.json"
     first_year = 2015
     first_day = 1
     last_day = 25
+    max_parts = 2
+    blank_dash = package_root / blank_dir / "README.md"
```

### Comparing `esb-0.1.1/src/esb/db.py` & `esb-0.1.2/src/esb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,22 @@
         where_params = self.query_named_placeholders(where_values, sep=" AND ")
         set_params = self.query_named_placeholders(key, sep=", ")
 
         query = f"UPDATE {self.__class__.__name__} SET {set_params} WHERE {where_params}"  # noqa: S608
         self._sql.cur.execute(query, d)
         self._sql.con.commit()
 
+    @check_connection
+    def delete(self):
+        d = self.to_dict()
+        where_params = self.query_named_placeholders(d, sep=" AND ")
+        query = f"DELETE FROM {self.__class__.__name__} WHERE {where_params}"  # noqa: S608
+        self._sql.cur.execute(query, d)
+        self._sql.con.commit()
+
 
 ###########################################################
 # Main DB Interface
 ###########################################################
 @dataclass(unsafe_hash=True)
 class ECABrigadista(Table):
     brigadista_id: str
@@ -254,23 +262,30 @@
         self.started = bool(self.started)
         self.finished_pt1 = bool(self.finished_pt1)
         self.finished_pt2 = bool(self.finished_pt2)
 
     def set_solved(self, part: FPPart):
         self.update({f"finished_pt{part}": True})
         if self.day == ESBConfig.last_day:  # Day 25 has only one star
-            self.update({f"finished_pt{(part + 1) % 2}": True})
+            self.update({"finished_pt2": True})
 
     def set_unsolved(self, part: FPPart):
         self.update({f"finished_pt{part}": False})
 
 
 @dataclass(unsafe_hash=True)
+class ECAArgCache(Table):
+    year: int
+    day: int
+    language: str
+
+
+@dataclass(unsafe_hash=True)
 class ECARun(Table):
-    id: int | None  # noqa: A003
+    id: int | None
     datetime: datetime
     year: int
     day: int
     language: str
     part: FPPart
     answer: str | None = None
     time: int | None = None
@@ -316,19 +331,26 @@
                                 day INTEGER NOT NULL,
                                 language TEXT NOT NULL,
                                 part INTEGER NOT NULL,
                                 answer TEXT,
                                 time INTEGER,
                                 unit INTEGER
                             )""",
+        ECAArgCache: """CREATE TABLE {table_name} (
+                                year INTEGER NOT NULL,
+                                day INTEGER NOT NULL,
+                                language TEXT NOT NULL,
+                                PRIMARY KEY (year, day, language)
+                            )""",
     }
     ECABrigadista = ECABrigadista
     ECAPuzzle = ECAPuzzle
     ECALanguage = ECALanguage
     ECARun = ECARun
+    ECAArgCache = ECAArgCache
 
     def __init__(self, repo_root: Path):
         sqlite3.register_adapter(MetricPrefix, lambda mp: mp.value)
         self.repo_root = repo_root
         self.db_path = repo_root / ESBConfig.db_path
         if not self.db_path.parent.is_dir():
             self.db_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `esb-0.1.1/src/esb/fetch.py` & `esb-0.1.2/src/esb/fetch.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,31 +39,32 @@
 
 class RudolphFetcher:
     repo_root: Path
     cookie: str
     sess_env = "AOC_SESSION_COOKIE"
     host = "adventofcode.com"
     st_route = "/{year}/day/{day}"
-    in_route = "{st_route}/input"
-    ans_route = "{st_route}/answer"
+    in_route = "{st_route}/input"  # noqa: RUF027
+    ans_route = "{st_route}/answer"  # noqa: RUF027
 
     def __init__(self, repo_root: Path):
         self.repo_root = repo_root
-        self.cookie = self.load_cookie()
+        self.cookie = self.load_cookie(repo_root)
 
-    def load_cookie(self) -> str:
-        dotenv = self.repo_root / ".env"
+    @classmethod
+    def load_cookie(cls, repo_root) -> str:
+        dotenv = repo_root / ".env"
         if dotenv.is_file():
             with dotenv.open() as fp:
-                [dot_cookie] = [line.split("=")[1] for line in fp.read().split("\n") if line.startswith(self.sess_env)]
+                [dot_cookie] = [line.split("=")[1] for line in fp.read().split("\n") if line.startswith(cls.sess_env)]
                 return dot_cookie.removeprefix('"').removesuffix('"')
-        env_cookie: str | None = environ.get(self.sess_env)
+        env_cookie: str | None = environ.get(cls.sess_env)
         match env_cookie:
             case None:
-                message = f"Could not find {self.sess_env}"
+                message = f"Could not find {cls.sess_env}"
                 raise ValueError(message)
             case str(_):
                 return env_cookie
 
     def http_get(self, host: str, route: str) -> str:
         conn = http.client.HTTPSConnection(host)
         conn.request(
```

### Comparing `esb-0.1.1/src/esb/langs.py` & `esb-0.1.2/src/esb/langs.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,31 +8,37 @@
 [Advent Of Code](https://adventofcode.com/) yearly events
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
 from __future__ import annotations
 
 import json
+import subprocess
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 from esb.config import ESBConfig
+from esb.paths import pad_day
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from esb.paths import LangSled
 
 
 @dataclass
 class LangSpec:
     name: str
     files: dict[str, str]
-    command: list[str]
+    run_command: list[str]
     symbol: str
+    emoji: str
+    base: bool = False
+    build_command: list[str] | None = None
+    install: list[str] | None = None
 
     @classmethod
     def from_json(cls, file: str | Path):
         with open(file, encoding="utf-8") as fp:
             return cls(**json.load(fp))
 
 
@@ -59,21 +65,38 @@
 
 
 @dataclass
 class LangRunner:
     spec: LangSpec
     sled: LangSled
 
-    def build_command(self, year: int, day: int) -> list[str]:
-        return [self.replace_files(c, year, day) for c in self.spec.command]
+    def prepare_install_command(self, year: int, day: int) -> list[str]:
+        if self.spec.install is None:
+            message = f"Cannot prepare install command because it does not exists for language {self.spec.name}"
+            raise TypeError(message)
+        return self.prepare_command(self.spec.install, year, day)
+
+    def prepare_build_command(self, year: int, day: int) -> list[str]:
+        if self.spec.build_command is None:
+            message = f"Cannot prepare build command because it does not exists for language {self.spec.name}"
+            raise TypeError(message)
+        return self.prepare_command(self.spec.build_command, year, day)
+
+    def prepare_run_command(self, year: int, day: int) -> list[str]:
+        return self.prepare_command(self.spec.run_command, year, day)
+
+    def prepare_command(self, command: list[str], year: int, day: int) -> list[str]:
+        return [self.replace_files(c, year, day) for c in command]
 
     def replace_files(self, c: str, year: int, day: int) -> str:
         filenames = {k.name: v.name for k, v in self.sled.boiler_map(year, day).items()}
         replace_mapping = {
             "year": year,
-            "day": day,
+            "day": pad_day(day),
             "filenames": filenames,
         }
         return c.format_map(replace_mapping)
 
-    def working_dir(self, year: int, day: int) -> Path:
-        return self.sled.day_dir(year, day)
+    def exec_command(self, command: list[str], year: int, day: int) -> subprocess.CompletedProcess:
+        day_wd = self.sled.working_dir(year=year, day=day)
+        command = self.prepare_command(command, year=year, day=day)
+        return subprocess.run(command, cwd=day_wd, check=False)
```

### Comparing `esb-0.1.1/src/esb/paths.py` & `esb-0.1.2/src/esb/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,25 +80,30 @@
         if file not in self.files:
             message = f"Could not find path for file '{file}'"
             raise KeyError(message)
         return self.day_dir(year, day) / self.files[file].format(year=year, day=pad_day(day))
 
 
 @dataclass
-class CacheSled(YearSled):
+class CacheInputSled(YearSled):
     subdirs: SledSubdirs = field(default_factory=lambda: [ESBConfig.cache_dir])
     files: SledFiles = field(
         default_factory=lambda: {
             "statement": "day_{day}_statement.txt",
             "input": "day_{day}_input.txt",
         }
     )
 
 
 @dataclass
+class CacheTestSled(YearSled):
+    subdirs: SledSubdirs = field(default_factory=lambda: [ESBConfig.tests_dir])
+
+
+@dataclass
 class LangSled(YearSled):
     name: str
     files: SledFiles
 
     @classmethod
     def from_spec(cls, repo_root: Path, spec: LangSpec) -> Self:
         return cls(repo_root=repo_root, name=spec.name, files=spec.files)
@@ -106,23 +111,25 @@
     def __post_init__(self):
         self.subdirs = [ESBConfig.solutions_dir, self.name]
 
     @property
     def boiler_subdir(self) -> Path:
         return ESBConfig.boiler_root / self.name / ESBConfig.boiler_template
 
+    @property
+    def boiler_base_subdir(self) -> Path:
+        return self.boiler_subdir.parent / ESBConfig.boiler_template_base
+
     def boiler_source(self, filename: str) -> Path:
         return self.boiler_subdir / filename
 
     def boiler_map(self, year: int, day: int) -> dict[Path, Path]:
         return {self.boiler_source(file): self.path(file=file, year=year, day=day) for file in self.files}
 
     def copied_source(self, year: int, day: int, filename: str) -> Path:
         return self.day_dir(year, day) / filename
 
     def copied_map(self, year: int, day: int) -> dict[Path, Path]:
         return {self.copied_source(year, day, file): self.path(file=file, year=year, day=day) for file in self.files}
 
-
-@dataclass
-class TestSled(YearSled):
-    subdirs: SledSubdirs = field(default_factory=lambda: [ESBConfig.tests_dir])
+    def working_dir(self, year: int, day: int) -> Path:
+        return self.day_dir(year, day)
```

### Comparing `esb-0.1.1/src/esb/blank/README.md` & `esb-0.1.2/src/esb/blank/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
-# Advent Of Code
+# Advent Of Code Solutions
+
 > In the heart of the North Pole, amidst the enchanting snow-covered landscape and the sparkling lights of Santa's Workshop, you, a devoted member of the [ElfScript Brigade](https://github.com/luxedo/esb?tab=readme-ov-file#esb---elfscript-brigade), step forward as the guiding star seeker. Fueled by an insatiable curiosity and a fervor for unraveling intricate coding puzzles, your resolve is unwavering. You believe wholeheartedly that every star collected is a step closer to weaving the magic of Christmas. As you conquer algorithms and elegantly craft lines of code, your vision extends beyond the monitor, picturing the joy and wonder these digital triumphs bring to children across the globe. In the tranquil hours of the Arctic night, armed with a keyboard and resolute determination, you persist in chasing those elusive stars. Each puzzle solved becomes a beacon of hope, a testament to your dedication, and a significant stride toward safeguarding Christmas for all.
 
-## Solutions
+<!-- Do not delete - Report start -->
+<!-- Do not delete - Report end -->
 
 ## Acknowledgment
+
 Part of the [ElfScript Brigade](https://github.com/luxedo/esb?tab=readme-ov-file#esb---elfscript-brigade) initiative, this project is integral to securing and enhancing the Christmas experience. Join us in ensuring a joyful and safe holiday season for all. Your skills can make a meaningful impact—become a part of the [ElfScript Brigade](https://github.com/luxedo/esb?tab=readme-ov-file#esb---elfscript-brigade), contributing to a brighter, safer Christmas.
```

### Comparing `esb-0.1.1/src/esb/commands/__init__.py` & `esb-0.1.2/src/esb/commands/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 Script your way to rescue Christmas as part of the ElfScript Brigade team.
 
 `esb` is a CLI tool to help us _elves_ to save christmas for the
 [Advent Of Code](https://adventofcode.com/) yearly events
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
+from esb.commands.dashboard import dashboard
 from esb.commands.fetch import fetch
 from esb.commands.new import new
 from esb.commands.run import run
 from esb.commands.show import show
 from esb.commands.start import start
 from esb.commands.status import status
 from esb.commands.test import test
 
-__all__ = ["fetch", "new", "run", "show", "start", "status", "test"]
+__all__ = ["dashboard", "fetch", "new", "run", "show", "start", "status", "test"]
```

### Comparing `esb-0.1.1/src/esb/commands/base.py` & `esb-0.1.2/src/esb/commands/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from functools import wraps
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from rich.console import Console
 from rich.theme import Theme
 
-from esb.paths import TestSled, find_esb_root, pad_day
+from esb.paths import CacheTestSled, find_esb_root, pad_day
 
 if TYPE_CHECKING:
     from esb.db import ECALanguage, ECAPuzzle, ElvenCrisisArchive
     from esb.langs import LangSpec
     from esb.protocol import fireplacev1_0 as fp1_0
 
 COLOR_INFO = "bold green"
@@ -70,15 +70,15 @@
     eprint_info(
         f"esb fetch --year {year} --day {day}",
     )
     return None
 
 
 def find_tests(repo_root: Path, year: int, day: int, part: fp1_0.FPPart) -> list[tuple[str, dict]]:
-    ts = TestSled(repo_root)
+    ts = CacheTestSled(repo_root)
     day_dir = ts.day_dir(year, day)
 
     test_files = [file for file in day_dir.iterdir() if file.suffix == ".toml"] if day_dir.is_dir() else []
 
     tests = [test for test_file in test_files for test in load_tests(test_file, part)]
 
     if len(tests) == 0:
```

### Comparing `esb-0.1.1/src/esb/commands/fetch.py` & `esb-0.1.2/src/esb/commands/fetch.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,22 @@
 `esb` is a CLI tool to help us _elves_ to save christmas for the
 [Advent Of Code](https://adventofcode.com/) yearly events
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
 from __future__ import annotations
 
+import sys
 from itertools import product
 from typing import TYPE_CHECKING
 
 from esb.commands.base import eprint_error, eprint_info, is_esb_repo
 from esb.db import ElvenCrisisArchive
 from esb.fetch import RudolphFetcher
-from esb.paths import CacheSled, pad_day
+from esb.paths import CacheInputSled, pad_day
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @is_esb_repo
 def fetch(repo_root: Path, years: list[int], days: list[int], *, force: bool = False):
@@ -32,19 +33,25 @@
 
 def fetch_day(repo_root: Path, db: ElvenCrisisArchive, year: int, day: int, *, force: bool = False):
     dp = db.ECAPuzzle.find_single({"year": year, "day": day})
     if not force and dp is not None and dp.pt2_answer is not None:
         eprint_error(f"Fetch for year {year} day {pad_day(day)} is already complete!")
         return
 
+    try:
+        RudolphFetcher.load_cookie(repo_root)
+    except ValueError:
+        eprint_error(f"Could not load {RudolphFetcher.sess_env} environment variable.")
+        sys.exit(2)
+
     rudolph = RudolphFetcher(repo_root)
 
     url, statement, pt1_answer, pt2_answer = rudolph.fetch_statement(year, day)
 
-    cache_sled = CacheSled(repo_root)
+    cache_sled = CacheInputSled(repo_root)
     st_file = cache_sled.path("statement", year, day)
     st_file.parent.mkdir(parents=True, exist_ok=True)
     st_file.write_text(statement)
 
     [_, title, *_] = statement.split("---")
     db.ECAPuzzle(year=year, day=day, title=title.strip(), url=url, pt1_answer=pt1_answer, pt2_answer=pt2_answer).insert(
         replace=True
```

### Comparing `esb-0.1.1/src/esb/commands/new.py` & `esb-0.1.2/src/esb/commands/new.py`

 * *Files identical despite different names*

### Comparing `esb-0.1.1/src/esb/commands/run.py` & `esb-0.1.2/src/esb/commands/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 `esb` is a CLI tool to help us _elves_ to save christmas for the
 [Advent Of Code](https://adventofcode.com/) yearly events
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
 from __future__ import annotations
 
+import sys
 from datetime import datetime
 from itertools import product
 from typing import TYPE_CHECKING
 
 from esb.commands.base import eprint_error, eprint_info, eprint_warn, find_puzzle, find_solution, is_esb_repo
 from esb.db import ElvenCrisisArchive
 from esb.fetch import RudolphFetcher, RudolphSubmitStatus
 from esb.langs import LangRunner, LangSpec
-from esb.paths import CacheSled, LangSled, pad_day
+from esb.paths import CacheInputSled, LangSled, pad_day
 from esb.protocol import fireplacev1_0 as fp1_0
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @is_esb_repo
@@ -53,21 +54,31 @@
 ):
     if (dl := find_solution(db, year, day, lang)) is None:
         return
 
     if (dp := find_puzzle(db, year, day)) is None:
         return
 
-    cache_sled = CacheSled(repo_root)
+    cache_sled = CacheInputSled(repo_root)
     lang_sled = LangSled.from_spec(repo_root, lang)
     runner = LangRunner(lang, lang_sled)
-    command = runner.build_command(year=year, day=day)
-    day_wd = runner.working_dir(year=year, day=day)
+
+    day_wd = lang_sled.working_dir(year=year, day=day)
+
+    if lang.build_command is not None:
+        runner = LangRunner(lang, lang_sled)
+        p = runner.exec_command(lang.build_command, year, day)
+        if p.returncode != 0:
+            eprint_error(f"Could not build program for: {lang.name}, year {year} day {pad_day(day)}")
+            sys.exit(2)
+
+    run_command = runner.prepare_run_command(year=year, day=day)
     day_input = cache_sled.path("input", year, day)
-    result = fp1_0.exec_protocol_from_file(command, part, day_wd, day_input)
+    args = None
+    result = fp1_0.exec_protocol_from_file(run_command, part, args, day_wd, day_input)
     match result.status:
         case fp1_0.FPStatus.Ok:
             pass
         case fp1_0.FPStatus.InputDoesNotExists:
             eprint_error(
                 f"\nCould not find input for year {year} day {pad_day(day)}. "
                 "Data seems corrupted. Please fetch again with --force"
```

### Comparing `esb-0.1.1/src/esb/commands/show.py` & `esb-0.1.2/src/esb/commands/show.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 
 from itertools import product
 from typing import TYPE_CHECKING
 
 from esb.commands.base import eprint_error, is_esb_repo, oprint_error, oprint_info, oprint_none
 from esb.config import ESBConfig
 from esb.db import ElvenCrisisArchive
-from esb.paths import CacheSled, pad_day
+from esb.paths import CacheInputSled, pad_day
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @is_esb_repo
 def show(repo_root: Path, years: list[int], days: list[int]):
     db = ElvenCrisisArchive(repo_root)
     for year, day in product(years, days):
         show_day(repo_root, db, year, day)
 
 
 def show_day(repo_root: Path, db: ElvenCrisisArchive, year: int, day: int):
     dp = db.ECAPuzzle.find_single({"year": year, "day": day})
-    cache_sled = CacheSled(repo_root)
+    cache_sled = CacheInputSled(repo_root)
     statement_file = cache_sled.path("statement", year, day)
     if dp is None:
         eprint_error(f"Solution for year {year} day {pad_day(day)} not cached. Please fetch first")
         return
 
     if not statement_file.is_file():
         eprint_error("Problem not fetched yet!")
```

### Comparing `esb-0.1.1/src/esb/commands/start.py` & `esb-0.1.2/src/esb/commands/start.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 `esb` is a CLI tool to help us _elves_ to save christmas for the
 [Advent Of Code](https://adventofcode.com/) yearly events
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
 from __future__ import annotations
 
+import sys
 from itertools import product
 from typing import TYPE_CHECKING
 
 from esb.boiler import CodeFurnace
-from esb.commands.base import eprint_error, eprint_info, is_esb_repo
+from esb.commands.base import eprint_error, eprint_info, eprint_warn, is_esb_repo
 from esb.commands.fetch import fetch_day
 from esb.db import ElvenCrisisArchive
+from esb.langs import LangRunner
 from esb.paths import LangSled, pad_day
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from esb.langs import LangSpec
 
@@ -37,27 +39,41 @@
     day_problem = db.ECAPuzzle.find_single({"year": year, "day": day})
     match (day_problem, force):
         case (_, True) | (None, _):
             fetch_day(repo_root, db, year, day, force=force)
             day_problem = db.ECAPuzzle.find_single({"year": year, "day": day})
 
     day_language = db.ECALanguage.find_single({"year": year, "day": day, "language": lang.name})
-    match day_language:
-        case db.ECALanguage(started=True):
+    match (day_language, force):
+        case (None, _):
+            pass
+        case (db.ECALanguage(), True):
+            eprint_warn(
+                f'Code for "{lang.name}" year {year} day {pad_day(day)} has already started. ' "Overwritting...",
+            )
+            day_language.delete()
+        case (db.ECALanguage(started=True), _):
             eprint_error(
                 f'Code for "{lang.name}" year {year} day {pad_day(day)} has already started. '
                 "If you wish to overwrite run the command with --force flag.",
             )
             return
         # @TODO: Handle started=False
 
     lang_sled = LangSled.from_spec(repo_root, lang)
     cf = CodeFurnace(lang, lang_sled)
     cf.start(year, day, day_problem.title, day_problem.url)
 
+    if lang.install is not None:
+        runner = LangRunner(lang, lang_sled)
+        p = runner.exec_command(lang.install, year, day)
+        if p.returncode != 0:
+            eprint_error(f"Could not install program for: {lang.name}, year {year} day {pad_day(day)}")
+            sys.exit(2)
+
     db.ECALanguage(
         year=year,
         day=day,
         language=lang.name,
         started=True,
         finished_pt1=False,
         finished_pt2=False,
```

### Comparing `esb-0.1.1/src/esb/commands/status.py` & `esb-0.1.2/src/esb/commands/dashboard.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,34 +9,26 @@
 (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from esb.commands.base import is_esb_repo, oprint_error, oprint_info, oprint_warn
-from esb.dash import CliDash
+from esb.commands.base import is_esb_repo, oprint_error, oprint_info
+from esb.dash import MdDash
 from esb.db import ElvenCrisisArchive
 from esb.langs import LangMap
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
 @is_esb_repo
-def status(repo_root: Path):
+def dashboard(repo_root: Path, *, reset: bool = False):
     db = ElvenCrisisArchive(repo_root)
     lmap = LangMap.load()
-    cli_dash = CliDash(db, lmap)
-
-    brigadista = cli_dash.brigadista()
-
-    oprint_error("ELFSCRIPT BRIGADE STATUS REPORT\n")
-    oprint_info(brigadista)
-    oprint_warn("\nSERVICE STARS")
-
-    ys = cli_dash.years_summary()
-
-    for year in sorted(ys.keys(), reverse=True):
-        summary = ys[year]
-        oprint_info(f"\n{year}")
-        oprint_warn(f"\n{summary}")
+    md_dash = MdDash(db, lmap, repo_root)
+    try:
+        md_dash.build_dash(reset=reset)
+        oprint_info("Dashboard rebuilt successfully!")
+    except ValueError:
+        oprint_error("Error building dashboard. Check if you have all the needed tags in the template")
```

### Comparing `esb-0.1.1/src/esb/commands/test.py` & `esb-0.1.2/src/esb/commands/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -55,19 +55,26 @@
         return
 
     if (tests := find_tests(repo_root, year, day, part)) == []:
         return
 
     lang_sled = LangSled.from_spec(repo_root, lang)
     runner = LangRunner(lang, lang_sled)
-    command = runner.build_command(year=year, day=day)
-    day_wd = runner.working_dir(year=year, day=day)
+
+    day_wd = lang_sled.working_dir(year=year, day=day)
+    if lang.build_command is not None:
+        runner.exec_command(lang.build_command, year, day)
+
+    run_command = runner.prepare_run_command(year=year, day=day)
     for name, test in tests:
         day_input_text = test["input"]
-        result = fp1_0.exec_protocol(command, part, day_wd, day_input_text)
-        match (result.status, result.answer == test["answer"]):
+        if "args" in test:
+            test["args"] = [str(arg) for arg in test["args"]]
+        args = test.get("args")
+        result = fp1_0.exec_protocol(run_command, part, args, day_wd, day_input_text)
+        match (result.status, result.answer == str(test["answer"])):
             case (fp1_0.FPStatus.Ok, True):
                 eprint_info(f"✔ Answer {name} pt{part}: {result.answer}")
             case (fp1_0.FPStatus.Ok, False):
                 eprint_error(f"✘ Answer {name} pt{part}: {result.answer}. Expected: {test['answer']}")
             case _:
                 eprint_error(f"✘ Could not run {name}")
```

### Comparing `esb-0.1.1/src/esb/protocol/fireplacev1_0.py` & `esb-0.1.2/src/esb/protocol/fireplacev1_0.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         type=int,
         help="Run solution part 1 or part 2",
     )
     parser.add_argument(
         "-a",
         "--args",
         nargs="*",
-        help="Run solution part 1 or part 2",
+        help="Additional arguments for running the solutions",
     )
     args = parser.parse_args()
     t0 = perf_counter_ns()
     ans = _run_solution(solve_pt1, solve_pt2, args.part, args.args)
     sys.stdout.write(f"{ans}\n")
     dt = perf_counter_ns() - t0
     sys.stdout.write(f"RT {dt} ns\n")
@@ -81,29 +81,29 @@
     status: FPStatus
     answer: str | None = None
     running_time: int | None = None
     unit: MetricPrefix | None = None
 
 
 # @TODO: type this
-async def _read_output(stream, threshold: int, print_stream):
+async def _read_output(stream, threshold: int, print_stream) -> str:
     ret = ""
     lines = 0
     while line := await stream.readline():
         line = line.decode("utf-8")
         ret += line
         if lines == threshold:
             print_stream.write(ret)
         elif lines > threshold:
             print_stream.write(line)
         lines += 1
-    return ret, lines
+    return ret
 
 
-async def _exec_protocol_command(cmd: list[str], cwd: Path, day_input_text: str) -> tuple[int, tuple[str, int]]:
+async def _exec_protocol_command(cmd: list[str], cwd: Path, day_input_text: str) -> tuple[int, str]:
     proc = await asyncio.create_subprocess_exec(
         *cmd,
         cwd=cwd,
         stdin=asyncio.subprocess.PIPE,
         stdout=asyncio.subprocess.PIPE,
     )
 
@@ -113,53 +113,58 @@
 
     proc.stdin.write(day_input_text.encode())
     proc.stdin.close()
 
     return await asyncio.gather(proc.wait(), _read_output(proc.stdout, threshold=2, print_stream=sys.stdout))
 
 
-def _parse_running_time(running_time_line: str) -> tuple[int, MetricPrefix]:
+def parse_running_time(running_time_line: str) -> tuple[int, MetricPrefix]:
     try:
         match running_time_line.split():
             case ["RT", running_time_str, unit_str]:
                 running_time = int(running_time_str)
                 unit = MetricPrefix.parse(unit_str, "second", "s")
                 return running_time, unit
-    except Exception as exc:  # noqa: BLE001
+    except Exception as exc:
         message = f"Could not parse running time for '{running_time_line}'"
         raise ValueError(message) from exc
     message = f"Could not parse running time for '{running_time_line}'"
     raise ValueError(message)
 
 
-def exec_protocol_from_file(command: list[str], part: FPPart, cwd: Path, day_input: Path) -> FPResult:
+def exec_protocol_from_file(
+    command: list[str], part: FPPart, args: list[str] | None, cwd: Path, day_input: Path
+) -> FPResult:
     if not day_input.is_file():
         return FPResult(status=FPStatus.InputDoesNotExists)
     day_input_text = day_input.read_text()
-    return exec_protocol(command, part, cwd, day_input_text)
+    return exec_protocol(command, part, args, cwd, day_input_text)
 
 
-def exec_protocol(command: list[str], part: FPPart, cwd: Path, day_input_text: str) -> FPResult:
+def exec_protocol(
+    command: list[str],
+    part: FPPart,
+    args: list[str] | None,
+    cwd: Path,
+    day_input_text: str,
+) -> FPResult:
     cmd = [*command, "--part", f"{part}"]
-    exitcode, (stdout, out_lines) = asyncio.run(_exec_protocol_command(cmd, cwd, day_input_text))
+    if args is not None:
+        cmd.extend(["--args", *args])
+    exitcode, stdout = asyncio.run(_exec_protocol_command(cmd, cwd, day_input_text))
 
     success_exit = 0
-    stdout_lines = [1, 2]
-    if exitcode != success_exit or out_lines not in stdout_lines:
+    if exitcode != success_exit or not stdout.endswith("\n"):
         return FPResult(status=FPStatus.ProtocolError)
 
-    answer = None
     running_time = None
     unit = None
-    match stdout.strip().split("\n"):
-        case [ans, running_time_line]:
-            answer = ans
-            try:
-                running_time, unit = _parse_running_time(running_time_line)
-            except ValueError:
-                return FPResult(status=FPStatus.ProtocolError)
-        case [ans]:
-            answer = ans
-        case _:
+    answer = stdout[:-1]
+    lines = answer.split("\n")
+    if lines[-1].startswith("RT "):
+        answer = "\n".join(lines[:-1])
+        try:
+            running_time, unit = parse_running_time(lines[-1])
+        except ValueError:
             return FPResult(status=FPStatus.ProtocolError)
 
     return FPResult(status=FPStatus.Ok, answer=answer, running_time=running_time, unit=unit)
```

### Comparing `esb-0.1.1/src/esb/protocol/metric_prefix.py` & `esb-0.1.2/src/esb/protocol/metric_prefix.py`

 * *Files identical despite different names*

### Comparing `esb-0.1.1/LICENSE.md` & `esb-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `esb-0.1.1/README.md` & `esb-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 > Script your way to rescue Christmas as part of the ElfScript Brigade team.
 >
 > This tool transforms Advent of Code into a CLI adventure
 
 <img src="doc/logo/png/logo-color-small.png" alt="ElfScript Brigade Logo"/>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/esb.svg)](https://pypi.org/project/esb)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/esb.svg)](https://pypi.org/project/esb)[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![PyPI - Version](https://img.shields.io/pypi/v/esb.svg)](https://pypi.org/project/esb) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/esb.svg)](https://pypi.org/project/esb) [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/luxedo/esb/publish.yml) ![Codecov](https://img.shields.io/codecov/c/github/luxedo/esb) ![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/luxedo/esb)
 
 ---
 
 In the bureaucratic workshop of Santa's IT department, where the spirit of Christmas and the magic of coding converge, a special group of coding elves emerged known as the **ElfScript Brigade**. These skilled and whimsical elves were bestowed with the mission of safeguarding the joyous essence of Christmas through the power of scripting and coding.
 
 `esb` is a CLI tool to help us _elves_ to save Christmas for the [Advent Of Code](https://adventofcode.com/) yearly events (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 
@@ -170,16 +170,14 @@
 
   > ## **No!**.
 
 - **But, why python 3.11? What about my Debian friends?**
 
   > Because the developer wanted to some of the newest features
 
-
-
 ## Rules of Automation
 
 ElfScript Brigade does follow the [automation guidelines](https://www.reddit.com/r/adventofcode/wiki/faqs/automation) on the [/r/adventofcode](https://www.reddit.com/r/adventofcode) community wiki
 Specifically:
 
 Once inputs are downloaded, they are cached locally in the `data` directory.
 If you suspect your input is corrupted, you can manually request a fresh copy using `esb fetch ... --force`
```

### Comparing `esb-0.1.1/pyproject.toml` & `esb-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -59,14 +59,18 @@
   "- coverage combine",
   "coverage report -m",
 ]
 cov = [
   "test-cov",
   "cov-report",
 ]
+cov-xml = [
+  "cov",
+  "coverage xml",
+]
 check = "mypy --install-types --non-interactive {args:src/esb tests}"
 
 [tool.mypy]
 exclude = ["esb/boilers"]
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.11", "3.12"]
@@ -89,16 +93,16 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.ruff]
 line-length = 120
-ignore = ["TRY", "ARG002"]
 include = ["pyproject.toml", "src/esb/*.py", "tests/**/*.py"]
 exclude = ["src/esb/boilers"]
 
 [tool.ruff.format]
 preview = true
 
 [tool.ruff.lint]
 preview = true
+ignore = ["TRY", "ARG002"]
```

### Comparing `esb-0.1.1/PKG-INFO` & `esb-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: esb
-Version: 0.1.1
+Version: 0.1.2
 Summary: Script your way to rescue Christmas as part of the ElfScript Brigade team.
 Project-URL: Documentation, https://github.com/luxedo/esb/README.md
 Project-URL: Repository, https://github.com/luxedo/esb.git
 Project-URL: Issues, https://github.com/luxedo/esb/issues
 Project-URL: Source, https://github.com/luxedo/esb
 Author-email: Luiz Eduardo Amaral <luizamaral306@gmail.com>
 Maintainer-email: Luiz Eduardo Amaral <luizamaral306@gmail.com>
@@ -706,15 +706,15 @@
 
 > Script your way to rescue Christmas as part of the ElfScript Brigade team.
 >
 > This tool transforms Advent of Code into a CLI adventure
 
 <img src="doc/logo/png/logo-color-small.png" alt="ElfScript Brigade Logo"/>
 
-[![PyPI - Version](https://img.shields.io/pypi/v/esb.svg)](https://pypi.org/project/esb)[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/esb.svg)](https://pypi.org/project/esb)[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![PyPI - Version](https://img.shields.io/pypi/v/esb.svg)](https://pypi.org/project/esb) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/esb.svg)](https://pypi.org/project/esb) [![License: GPL v3](https://img.shields.io/badge/License-GPL_v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0.en.html) ![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/luxedo/esb/publish.yml) ![Codecov](https://img.shields.io/codecov/c/github/luxedo/esb) ![CodeFactor Grade](https://img.shields.io/codefactor/grade/github/luxedo/esb)
 
 ---
 
 In the bureaucratic workshop of Santa's IT department, where the spirit of Christmas and the magic of coding converge, a special group of coding elves emerged known as the **ElfScript Brigade**. These skilled and whimsical elves were bestowed with the mission of safeguarding the joyous essence of Christmas through the power of scripting and coding.
 
 `esb` is a CLI tool to help us _elves_ to save Christmas for the [Advent Of Code](https://adventofcode.com/) yearly events (Thank you [Eric 😉!](https://twitter.com/ericwastl)).
 
@@ -872,16 +872,14 @@
 
   > ## **No!**.
 
 - **But, why python 3.11? What about my Debian friends?**
 
   > Because the developer wanted to some of the newest features
 
-
-
 ## Rules of Automation
 
 ElfScript Brigade does follow the [automation guidelines](https://www.reddit.com/r/adventofcode/wiki/faqs/automation) on the [/r/adventofcode](https://www.reddit.com/r/adventofcode) community wiki
 Specifically:
 
 Once inputs are downloaded, they are cached locally in the `data` directory.
 If you suspect your input is corrupted, you can manually request a fresh copy using `esb fetch ... --force`
```

