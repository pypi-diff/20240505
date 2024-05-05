# Comparing `tmp/sonatoki-0.1.2.tar.gz` & `tmp/sonatoki-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonatoki-0.1.2.tar", last modified: Sat May  4 19:13:30 2024, max compression
+gzip compressed data, was "sonatoki-0.1.3.tar", last modified: Sun May  5 21:18:08 2024, max compression
```

## Comparing `sonatoki-0.1.2.tar` & `sonatoki-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0    34523 2024-05-04 19:13:18.043206 sonatoki-0.1.2/LICENSE
--rw-r--r--   0        0        0     4560 2024-05-04 19:13:18.043206 sonatoki-0.1.2/README.md
--rw-r--r--   0        0        0     2013 2024-05-04 19:13:30.983266 sonatoki-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1160 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/Cleaners.py
--rw-r--r--   0        0        0     4093 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/Filters.py
--rw-r--r--   0        0        0     3499 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/Preprocessors.py
--rw-r--r--   0        0        0     4129 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/Scorers.py
--rw-r--r--   0        0        0     1741 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/Tokenizers.py
--rw-r--r--   0        0        0        0 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/__init__.py
--rw-r--r--   0        0        0       82 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/__main__.py
--rw-r--r--   0        0        0     1320 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/constants.py
--rw-r--r--   0        0        0     4278 2024-05-04 19:13:18.043206 sonatoki-0.1.2/src/sonatoki/ilo.py
--rw-r--r--   0        0        0   270928 2024-05-04 19:13:18.047206 sonatoki-0.1.2/src/sonatoki/linku.json
--rw-r--r--   0        0        0        0 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_cleaners.py
--rw-r--r--   0        0        0     2536 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_filters.py
--rw-r--r--   0        0        0     4872 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_ilo.py
--rw-r--r--   0        0        0     2808 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_preprocessors.py
--rw-r--r--   0        0        0      986 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_scorers.py
--rw-r--r--   0        0        0     2997 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_tokenize.py
--rw-r--r--   0        0        0      821 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/test_utils.py
--rw-r--r--   0        0        0      151 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/tokenize_cases/tokenize_sentences.yml
--rw-r--r--   0        0        0      743 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/tokenize_cases/tokenize_sentences_tok.yml
--rw-r--r--   0        0        0      440 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/tokenize_cases/tokenize_words.yml
--rw-r--r--   0        0        0     1522 2024-05-04 19:13:18.047206 sonatoki-0.1.2/tests/tokenize_cases/tokenize_words_tok.yml
--rw-r--r--   0        0        0     5020 1970-01-01 00:00:00.000000 sonatoki-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-05 21:17:54.139527 sonatoki-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4765 2024-05-05 21:17:54.139527 sonatoki-0.1.3/README.md
+-rw-r--r--   0        0        0     2013 2024-05-05 21:18:08.203592 sonatoki-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1160 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Cleaners.py
+-rw-r--r--   0        0        0     1939 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Configs.py
+-rw-r--r--   0        0        0     4194 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Filters.py
+-rw-r--r--   0        0        0     3347 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Preprocessors.py
+-rw-r--r--   0        0        0     4129 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Scorers.py
+-rw-r--r--   0        0        0     1942 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/Tokenizers.py
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/__main__.py
+-rw-r--r--   0        0        0     1647 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/constants.py
+-rw-r--r--   0        0        0     4343 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/ilo.py
+-rw-r--r--   0        0        0   271013 2024-05-05 21:17:54.139527 sonatoki-0.1.3/src/sonatoki/linku.json
+-rw-r--r--   0        0        0    77650 2024-05-05 21:17:54.143527 sonatoki-0.1.3/src/sonatoki/sandbox.json
+-rw-r--r--   0        0        0        0 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_cleaners.py
+-rw-r--r--   0        0        0     2536 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_filters.py
+-rw-r--r--   0        0        0     4063 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_ilo.py
+-rw-r--r--   0        0        0     2808 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_preprocessors.py
+-rw-r--r--   0        0        0      986 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_scorers.py
+-rw-r--r--   0        0        0     3039 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_tokenize.py
+-rw-r--r--   0        0        0      821 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/test_utils.py
+-rw-r--r--   0        0        0      151 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences.yml
+-rw-r--r--   0        0        0      743 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences_tok.yml
+-rw-r--r--   0        0        0      440 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_words.yml
+-rw-r--r--   0        0        0     1522 2024-05-05 21:17:54.143527 sonatoki-0.1.3/tests/tokenize_cases/tokenize_words_tok.yml
+-rw-r--r--   0        0        0     5225 1970-01-01 00:00:00.000000 sonatoki-0.1.3/PKG-INFO
```

### Comparing `sonatoki-0.1.2/LICENSE` & `sonatoki-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/README.md` & `sonatoki-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,67 @@
 
 ## What is **sona toki**?
 
 This library, "Language Knowledge," helps you identify whether a message is in Toki Pona. No grammar checking, yet, which means this more checks whether a given message has enough Toki Pona words.
 
 I wrote it with a variety of scraps and lessons learned from a prior project, [ilo pi toki pona taso, "toki-pona-only tool"](https://github.com/gregdan3/ilo-pi-toki-pona-taso). That tool will be rewritten to use this library shortly.
 
-If you've ever worked on a similar project, you know the question "is this message in [language]" is not a consistent one- the environment, time, preferences of the speaker, and much more, can all alter whether a given message is "in toki pona," and this applies to essentially any language.
+If you've ever worked on a similar project, you know the question "is this message in [language]" is not a consistent one- the environment, time, preferences of the speaker, and much more, can all alter whether a given message is "in" any specific language, and this question applies to Toki Pona too.
 
-This project "solves" that complex problem by offering a highly configurable and incredibly lazy parser
+This project "solves" that complex problem by offering a highly configurable parser, so you can tune it to your preferences and goals.
 
 ## Quick Start
 
 Install with your preferred Python package manager. Example:
 
 ```sh
 pdm init  # if your pyproject.toml doesn't exist yet
 pdm add sonatoki
 ```
 
 Then get started with a script along these lines:
 
 ```py
-from sonatoki.Filters import (
-    Numerics,
-    Syllabic,
-    NimiLinku,
-    Alphabetic,
-    ProperName,
-    Punctuations,
-)
-from sonatoki.Scorers import SoftScaling
-from sonatoki.Cleaners import ConsecutiveDuplicates
-from sonatoki.Tokenizers import word_tokenize_tok
-from sonatoki.Preprocessors import URLs, DiscordEmotes
+from sonatoki.ilo import Ilo
+from sonatoki.Configs import PrefConfig
 
 def main():
-    ilo = Ilo(
-        preprocessors=[URLs, DiscordEmotes],
-        ignoring_filters=[Numerics, Punctuations],
-        scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
-        cleaners=[ConsecutiveDuplicates],
-        scorer=SoftScaling,
-        tokenizer=word_tokenize_tok,
-    )
+    ilo = Ilo(**PrefConfig)
     ilo.is_toki_pona("imagine how is touch the sky")  # False
     ilo.is_toki_pona("o pilin insa e ni: sina pilin e sewi")  # True
     ilo.is_toki_pona("I Think I Can Evade Detection")  # False
 
 if __name__ == "__main__":
     main()
 ```
 
-`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I recommend using. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `word_tokenize_tok`.
+Or if you'd prefer to configure on your own:
+
+```py
+from copy import deepcopy
+from sonatoki.ilo import Ilo
+from sonatoki.Configs import BaseConfig
+from sonatoki.Filters import NimiPuAle, Phonotactic, ProperName
+from sonatoki.Scorers import SoftPassFail
+
+def main():
+    config = deepcopy(BaseConfig)
+    config["scoring_filters"].extend([NimiPuAle, Phonotactic, ProperName])
+    config["scorer"] = SoftPassFail
+
+    ilo = Ilo(**config)
+    ilo.is_toki_pona("mu mu!")  # True
+    ilo.is_toki_pona("mi namako e moku mi")  # True
+    ilo.is_toki_pona("ma wulin")  # False
+
+if __name__ == "__main__":
+    main()
+```
+
+`Ilo` is highly configurable by necessity, so I recommend looking through the premade configs in `Configs` as well as the individual `Preprocessors`, `Filters`, and `Scorers`. The `Cleaners` module only contains one cleaner, which I recommend always using. Similarly, the `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `WordTokenizerTok`.
 
 ## Development
 
 1. Install [pdm](https://github.com/pdm-project/pdm)
 1. `pdm install --dev`
 1. Open any file you like!
```

### Comparing `sonatoki-0.1.2/pyproject.toml` & `sonatoki-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sonatoki"
-version = "0.1.2"
+version = "0.1.3"
 description = "ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?"
 authors = [
     { name = "jan Kekan San (@gregdan3)", email = "gregory.danielson3@gmail.com" },
 ]
 dependencies = [
     "unidecode>=1.3.6",
     "regex>=2023.12.25",
```

### Comparing `sonatoki-0.1.2/src/sonatoki/Cleaners.py` & `sonatoki-0.1.3/src/sonatoki/Cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/src/sonatoki/Filters.py` & `sonatoki-0.1.3/src/sonatoki/Filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     CONSONANTS,
     NIMI_PU_SET,
     ALPHABET_SET,
     ALLOWABLES_SET,
     NIMI_LINKU_SET,
     NIMI_PU_ALE_SET,
     NIMI_LINKU_ALE_SET,
+    NIMI_LINKU_SANDBOX_SET,
 )
 
 re.DEFAULT_VERSION = re.VERSION1
 
 
 class Filter(ABC):
     @classmethod
@@ -83,14 +84,18 @@
     tokens = NIMI_LINKU_SET
 
 
 class NimiLinkuAle(SetFilter):
     tokens = NIMI_LINKU_ALE_SET
 
 
+class NimiLinkuSandbox(SetFilter):
+    tokens = NIMI_LINKU_SANDBOX_SET
+
+
 class Phonotactic(RegexFilter):
     """Determines if a given token is phonotactically valid Toki Pona (or `n`).
     Excludes both consecutive nasals and the illegal syllables:
     - "nm", "nn"
     - "wu", "wo", "ji", "ti"
 
     Note that if this validator is used after `Cleaners.ConsecutiveDuplicates`,
```

### Comparing `sonatoki-0.1.2/src/sonatoki/Preprocessors.py` & `sonatoki-0.1.3/src/sonatoki/Preprocessors.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,30 +9,28 @@
   - SingleQuotes
   - DoubleQuotes
   - Backticks
   - Spoilers
   - ArrowQuote
 
 Order does not generally matter, but if there were two overlapping containers such as in the string "|| spoiler ` monospace || `", order would matter.
-As such, each Preprocessor exposes a .precedence attribute which is optionally usable for ordering them. Lower precedence means it should be applied first.
+It is up to the user to order them appropriately.
 """
 
 # STL
 from abc import ABC, abstractmethod
 
 # PDM
 import regex as re
 from typing_extensions import override
 
 re.DEFAULT_VERSION = re.VERSION1
 
 
 class Preprocessor(ABC):
-    precedence: int = 0
-
     @classmethod  # order matters
     @abstractmethod
     def process(cls, msg: str) -> str:
         raise NotImplementedError
 
 
 class RegexPreprocessor(Preprocessor):
@@ -100,15 +98,14 @@
 class DoubleQuotes(RegexPreprocessor):
     pattern = re.compile(r'"[^"]+"', flags=re.S)
 
 
 class Backticks(RegexPreprocessor):
     """Remove paired backticks and their contents `like this`"""
 
-    precedence = -10
     pattern = re.compile(r"`[^`]+`", flags=re.S)
 
 
 class Spoilers(RegexPreprocessor):
     """Remove paired double bars and their contents `||like this||`"""
 
     pattern = re.compile(r"\|\|(?:(?!\|\|).)+\|\|", flags=re.S)
```

### Comparing `sonatoki-0.1.2/src/sonatoki/Scorers.py` & `sonatoki-0.1.3/src/sonatoki/Scorers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/src/sonatoki/constants.py` & `sonatoki-0.1.3/src/sonatoki/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # STL
 import json
 from typing import Dict, List
 from pathlib import Path
 
 LINKU = Path(__file__).resolve().parent / Path("linku.json")
+SANDBOX = Path(__file__).resolve().parent / Path("sandbox.json")
 
 VOWELS = "aeiou"
 CONSONANTS = "jklmnpstw"
 ALPHABET = VOWELS + CONSONANTS
 ALPHABET_SET = set(ALPHABET)
 
 """Commonly occurring strings which are some kind of valid Toki Pona or external token"""
@@ -25,18 +26,24 @@
     NIMI_PU: List[str] = [d["word"] for d in r.values() if d["book"] == "pu"]
     NIMI_PU_ALE: List[str] = NIMI_PU + ["namako", "kin", "oko"]
     NIMI_LINKU: List[str] = [
         d["word"] for d in r.values() if d["usage_category"] in ["core", "common"]
     ]
     NIMI_LINKU_ALE: List[str] = [d["word"] for d in r.values()]
 
+with open(SANDBOX) as f:
+    r: Dict[str, Dict[str, str]] = json.loads(f.read())
+    NIMI_LINKU_SANDBOX: List[str] = [d["word"] for d in r.values()]
+
+
 NIMI_PU_SET = set(NIMI_PU)
 NIMI_PU_ALE_SET = set(NIMI_PU_ALE)
 NIMI_LINKU_SET = set(NIMI_LINKU)
 NIMI_LINKU_ALE_SET = set(NIMI_LINKU_ALE)
+NIMI_LINKU_SANDBOX_SET = set(NIMI_LINKU_SANDBOX)
 ALLOWABLES_SET = set(ALLOWABLES)
 
 __all__ = [
     "VOWELS",
     #
     "CONSONANTS",
     #
@@ -50,8 +57,11 @@
     "NIMI_PU_ALE_SET",
     #
     "NIMI_LINKU",
     "NIMI_LINKU_SET",
     #
     "NIMI_LINKU_ALE",
     "NIMI_LINKU_ALE_SET",
+    #
+    "NIMI_LINKU_SANDBOX",
+    "NIMI_LINKU_SANDBOX_SET",
 ]
```

### Comparing `sonatoki-0.1.2/src/sonatoki/ilo.py` & `sonatoki-0.1.3/src/sonatoki/ilo.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,111 +10,111 @@
 from sonatoki.Preprocessors import Preprocessor
 
 LOG = logging.getLogger(__name__)
 
 
 class Ilo:
     __preprocessors: List[Type[Preprocessor]]
+    __word_tokenizer: Type[Tokenizer]
     __cleaners: List[Type[Cleaner]]
     __ignoring_filters: List[Type[Filter]]
     __scoring_filters: List[Type[Filter]]
     __scorer: Type[Scorer]
-    __tokenize: Tokenizer
     __passing_score: Number
-    logging_threshold: Number = 1.0
+    logging_threshold: Number = -1
 
     def __init__(
         self,
         preprocessors: List[Type[Preprocessor]],
         cleaners: List[Type[Cleaner]],
         ignoring_filters: List[Type[Filter]],
         scoring_filters: List[Type[Filter]],
         scorer: Type[Scorer],
-        tokenizer: Tokenizer,  # NOTE: no wrapper needed?
         passing_score: Number,
+        word_tokenizer: Type[Tokenizer],
     ):
         super().__init__()
         # avoid keeping a ref to user's list just in case
         self.__preprocessors = [*preprocessors]
+        self.__word_tokenizer = word_tokenizer
         self.__cleaners = [*cleaners]
         self.__ignoring_filters = [*ignoring_filters]
         self.__scoring_filters = [*scoring_filters]
         self.__scorer = scorer
-        self.__tokenize = tokenizer
         self.__passing_score = passing_score
 
-    def __preprocess(self, msg: str) -> str:
+    def preprocess(self, msg: str) -> str:
         for p in self.__preprocessors:
             msg = p.process(msg)
         return msg
 
-    def __clean_token(self, token: str) -> str:
+    def word_tokenize(self, msg: str) -> List[str]:
+        """It is *highly* recommended that you run `ilo.preprocess` first."""
+        return self.__word_tokenizer.tokenize(msg)
+
+    def clean_token(self, token: str) -> str:
         for c in self.__cleaners:
             token = c.clean(token)
         return token
 
-    def __clean_tokens(self, tokens: List[str]) -> List[str]:
-        # NOTE: tested, making a new list with a for loop *is* faster than
-        # - list comps
-        # - generator comps
-        # - in-place replacement/removal
-        # - in place replacement with result of generator comp
+    def clean_tokens(self, tokens: List[str]) -> List[str]:
+        # NOTE: tested, making a new list with a for loop *is* faster than:
+        # list comp, generator comp, in-place replacement
         cleaned_tokens: List[str] = list()
         for token in tokens:
-            cleaned_token = self.__clean_token(token)
+            cleaned_token = self.clean_token(token)
             if not cleaned_token:
                 # TODO: warn user?
                 continue
             cleaned_tokens.append(cleaned_token)
         return cleaned_tokens
 
-    def __filter_token(self, token: str) -> bool:
+    def _filter_token(self, token: str) -> bool:
         for f in self.__ignoring_filters:
             if f.filter(token):
                 return True
         return False
 
-    def __filter_tokens(self, tokens: List[str]) -> List[str]:
+    def filter_tokens(self, tokens: List[str]) -> List[str]:
         filtered_tokens: List[str] = []
         for token in tokens:
-            if self.__filter_token(token):
+            if self._filter_token(token):
                 continue
             # the ignoring filter is true if the token matches
             # the user wants to ignore these so keep non-matching tokens
             filtered_tokens.append(token)
         return filtered_tokens
 
-    def __score_tokens(self, tokens: List[str]) -> float:
+    def score_tokens(self, tokens: List[str]) -> float:
         return self.__scorer.score(tokens, self.__scoring_filters)
 
     def _is_toki_pona(
         self, message: str
     ) -> Tuple[str, List[str], List[str], List[str], Number, bool]:
         """Returns all components of the processing algorithm:
         - Preprocessed message (str)
         - Tokenized message (list[str])
         - Filtered message (list[str])
         - Cleaned message (list[str])
         - Score (float)
-        - Result (bool)
-        """
-        preprocessed = self.__preprocess(message)
-        tokenized = self.__tokenize(preprocessed)
-        filtered = self.__filter_tokens(tokenized)
-        cleaned = self.__clean_tokens(filtered)
-        score = self.__score_tokens(cleaned)
+        - Result (bool)"""
+        preprocessed = self.preprocess(message)
+        tokenized = self.word_tokenize(preprocessed)
+        filtered = self.filter_tokens(tokenized)
+        cleaned = self.clean_tokens(filtered)
+        score = self.score_tokens(cleaned)
         result = score >= self.__passing_score
 
-        # NOTE: this method may break if above funcs start sharing a list
         if score <= self.logging_threshold:
-            LOG.debug("Msg: %.2f  %s", score, repr(message))
-            LOG.debug("Preproc:   %s", repr(preprocessed))
-            LOG.debug("Tokenized: %s", tokenized)
-            LOG.debug("Filtered:  %s", filtered)
-            LOG.debug("Cleaned:   %s", cleaned)
+            LOG.debug("msg: %.2f  %s", score, repr(message))
+            LOG.debug("preproc:   %s", repr(preprocessed))
+            LOG.debug("tokenized: %s", tokenized)
+            LOG.debug("filtered:  %s", filtered)
+            LOG.debug("cleaned:   %s", cleaned)
         # TODO: Move to each function? Loses ability to control when logging occurs by threshold
 
         return preprocessed, tokenized, filtered, cleaned, score, result
 
     def is_toki_pona(self, message: str) -> bool:
+        """Determines whether a single statement is or is not Toki Pona."""
         *_, result = self._is_toki_pona(message)
         return result
```

### Comparing `sonatoki-0.1.2/src/sonatoki/linku.json` & `sonatoki-0.1.3/src/sonatoki/linku.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998861394932862%*

 * *Differences: {"'jonke'": "{'translations': {'eng': {'definition': 'hjönk, goose sound, goose'}}}",*

 * * "'konwe'": '{\'translations\': {\'eng\': {\'sp_etymology\': "pictogram of a glider in Conway\'s '*

 * *            'Game of Life, a machine which moves across the game board."}}}',*

 * * "'linluwi'": "{'translations': {'eng': {'definition': 'bonded things which are stronger through "*

 * *              "their bonds e.g. network, internet, connection; weave, braid, interlace'}}}",*

 * * "'misa'": "{'translations': {'eng': {'etymology': {0: {' […]*

```diff
@@ -2226,15 +2226,15 @@
             "mu",
             "nja"
         ],
         "source_language": "onomatopoeia",
         "translations": {
             "eng": {
                 "commentary": "Coined in reference to the Untitled Goose Game fandom.",
-                "definition": "goose, goose noise",
+                "definition": "hj\u00f6nk, goose sound, goose",
                 "etymology": [
                     {
                         "definition": "hj\u00f6nk",
                         "language": "onomatopoeia"
                     }
                 ],
                 "sp_etymology": ""
@@ -3637,15 +3637,15 @@
                         "language": "English"
                     },
                     {
                         "definition": "kon wile",
                         "language": "toki pona"
                     }
                 ],
-                "sp_etymology": ""
+                "sp_etymology": "pictogram of a glider in Conway's Game of Life, a machine which moves across the game board."
             }
         },
         "usage": {
             "2021-10": 25,
             "2022-08": 6,
             "2023-09": 7
         },
@@ -5109,15 +5109,15 @@
             "ilo",
             "wan"
         ],
         "source_language": "Welsh",
         "translations": {
             "eng": {
                 "commentary": "",
-                "definition": "network, internet, connection; weave, braid, interlace",
+                "definition": "bonded things which are stronger through their bonds e.g. network, internet, connection; weave, braid, interlace",
                 "etymology": [
                     {
                         "definition": "internet",
                         "language": "Welsh"
                     }
                 ],
                 "sp_etymology": ""
@@ -6676,15 +6676,15 @@
         "translations": {
             "eng": {
                 "commentary": "",
                 "definition": "Glires or Eulipotyphla; rat, mouse, squirrel, rabbit, rodent; {~ suli} capybara",
                 "etymology": [
                     {
                         "definition": "mouse (diminutive)",
-                        "language": "Ukranian"
+                        "language": "Ukrainian"
                     }
                 ],
                 "sp_etymology": ""
             }
         },
         "usage": {
             "2021-10": 35,
@@ -12337,15 +12337,14 @@
                         "language": "a priori"
                     }
                 ],
                 "sp_etymology": "pictogram of the front cover of The Wizard of Oz illustrated story book, depicting the yellow brick road from the story"
             }
         },
         "usage": {
-            "2020-04": 14,
             "2021-10": 28,
             "2022-08": 1,
             "2023-09": 0
         },
         "usage_category": "uncommon",
         "word": "su"
     },
@@ -12682,15 +12681,15 @@
         "audio": [
             {
                 "author": "kala Asi",
                 "link": "https://raw.githubusercontent.com/lipu-linku/ijo/main/kalama/kalaasi2023/sutopatikuna.mp3"
             }
         ],
         "author_verbatim": "Dear Sonja, That's a great idea, but if you do so, you need also to add a special word forthe Platypus (Ornithorhynchus anatinus). I would suggest the word \"sutopatikuna\"from the croatian word \u00c8udnovati kljuna\u00b9. Bonega ideo, sed se vi farus tion, vi devus ankaux aldoni apartan vorton porla Ornitorinko (Ornithorhynchus anatinus). Mi proponus la vorton \"sutopatikuna\"prenita de la kroatan vorton \u00c8udnovati kljuna\u00b9.:P",
-        "author_verbatim_source": "http://forums.tokipona.org/viewtopic.php?f=33&t=639&hilit=word+requests&sid=401a37e08cc5150e7a0738d068ea4a77&start=50#p2368",
+        "author_verbatim_source": "http://forums.tokipona.org/viewtopic.php?p=4927&hilit=sutopatikuna#p4927",
         "book": "ku lili",
         "coined_era": "pre-pu",
         "coined_year": "2009",
         "creator": [
             "Alexandre Baudry"
         ],
         "deprecated": false,
@@ -12801,15 +12800,15 @@
         "see_also": [
             "pona"
         ],
         "source_language": "Tok Pisin",
         "translations": {
             "eng": {
                 "commentary": "",
-                "definition": "sweet, fragrant; cute, innocent, adorable",
+                "definition": "sweet, fragrant; cute, adorable",
                 "etymology": [
                     {
                         "definition": "sweet",
                         "language": "Tok Pisin"
                     },
                     {
                         "definition": "sweet",
@@ -12872,15 +12871,15 @@
         "source_language": "Korean",
         "translations": {
             "eng": {
                 "commentary": "",
                 "definition": "sticky, magnetic; bond, attract, attach, clip",
                 "etymology": [
                     {
-                        "definition": "the sound of two magnets hitting each other (onomatopoiea)",
+                        "definition": "the sound of two magnets hitting each other (onomatopoeia)",
                         "language": "Korean"
                     }
                 ],
                 "sp_etymology": ""
             }
         },
         "usage": {
```

### Comparing `sonatoki-0.1.2/tests/test_cleaners.py` & `sonatoki-0.1.3/tests/test_cleaners.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/test_filters.py` & `sonatoki-0.1.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/test_ilo.py` & `sonatoki-0.1.3/tests/test_ilo.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 # PDM
 import pytest
 
 # LOCAL
 from sonatoki.ilo import Ilo
-from sonatoki.Filters import (
-    Numerics,
-    Syllabic,
-    NimiLinku,
-    Alphabetic,
-    ProperName,
-    Punctuations,
-)
-from sonatoki.Scorers import SoftScaling, SoftPassFail
-from sonatoki.Cleaners import ConsecutiveDuplicates
-from sonatoki.Tokenizers import word_tokenize_tok
-from sonatoki.Preprocessors import URLs
+from sonatoki.Configs import LazyConfig, PrefConfig
 
 
 @pytest.fixture
 def ilo():
-    ilo = Ilo(
-        preprocessors=[URLs],
-        ignoring_filters=[Numerics, Punctuations],
-        scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
-        cleaners=[ConsecutiveDuplicates],
-        scorer=SoftScaling,
-        tokenizer=word_tokenize_tok,
-        passing_score=0.8,
-    )
+    ilo = Ilo(**PrefConfig)
     # ilo.logging_threshold = 0.8
     return ilo
 
 
 @pytest.fixture()
 def lazy_ilo():
-    ilo = Ilo(
-        preprocessors=[URLs],
-        ignoring_filters=[Numerics, Punctuations],
-        scoring_filters=[Alphabetic, ProperName],
-        cleaners=[ConsecutiveDuplicates],
-        scorer=SoftPassFail,
-        tokenizer=word_tokenize_tok,
-        passing_score=0.8,
-    )
+    ilo = Ilo(**LazyConfig)
     # ilo.logging_threshold = 0.8
     return ilo
 
 
 ALL_VALID = [
     "mi unpa e mama sina",
     "mama sina li lon seme? mi wile toki tawa ona",
```

### Comparing `sonatoki-0.1.2/tests/test_preprocessors.py` & `sonatoki-0.1.3/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/test_scorers.py` & `sonatoki-0.1.3/tests/test_scorers.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/test_tokenize.py` & `sonatoki-0.1.3/tests/test_tokenize.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 
 # PDM
 import yaml
 import pytest
 
 # LOCAL
 from sonatoki.Tokenizers import (
-    sent_tokenize_re,
-    word_tokenize_re,
-    sent_tokenize_tok,
-    word_tokenize_tok,
+    SentTokenizerRe,
+    WordTokenizerRe,
+    SentTokenizerTok,
+    WordTokenizerTok,
 )
 
 try:
     # PDM
     import nltk
 
     # LOCAL
-    from sonatoki.Tokenizers import sent_tokenize_nltk, word_tokenize_nltk
+    from sonatoki.Tokenizers import SentTokenizerNLTK, WordTokenizerNLTK
 
 except ImportError as e:
     nltk = e
     # TODO: warn user
 
 
 class TokenizerTest(TypedDict):
@@ -60,52 +60,52 @@
 )
 def test_sentences_re(test: TokenizerTest):
     if isinstance(nltk, ImportError):
         pytest.skip("nltk not installed")
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_re = sent_tokenize_re(test["input"])
-    transformed_nltk = sent_tokenize_nltk(test["input"])
+    transformed_re = SentTokenizerRe.tokenize(test["input"])
+    transformed_nltk = SentTokenizerNLTK.tokenize(test["input"])
     assert (transformed_re == transformed_nltk) == test["should_be_equal"], test["name"]
 
 
 @pytest.mark.parametrize(
     "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words.yml")
 )
 def test_word_tokenize_re(test: TokenizerTest):
     if isinstance(nltk, ImportError):
         pytest.skip("nltk not installed")
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_re = word_tokenize_re(test["input"])
-    transformed_nltk = word_tokenize_nltk(test["input"])
+    transformed_re = WordTokenizerRe.tokenize(test["input"])
+    transformed_nltk = WordTokenizerNLTK.tokenize(test["input"])
     assert (transformed_re == transformed_nltk) == test["should_be_equal"], test["name"]
 
 
 @pytest.mark.parametrize(
     "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_sentences_tok.yml")
 )
 def test_sentences_tok(test: TokenizerTest):
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_tok = sent_tokenize_tok(test["input"])
+    transformed_tok = SentTokenizerTok.tokenize(test["input"])
     if test["should_be_equal"]:
         assert transformed_tok == test["output"], test["name"]
     else:
         assert transformed_tok != test["output"], test["name"]
 
 
 @pytest.mark.parametrize(
     "test", load_tokenizer_tests("tests/tokenize_cases/tokenize_words_tok.yml")
 )
 def test_word_tokenize_tok(test: TokenizerTest):
     if test["xfail"]:
         pytest.xfail()
 
-    transformed_tok = word_tokenize_tok(test["input"])
+    transformed_tok = WordTokenizerTok.tokenize(test["input"])
     if test["should_be_equal"]:
         assert transformed_tok == test["output"], test["name"]
     else:
         assert transformed_tok != test["output"], test["name"]
```

### Comparing `sonatoki-0.1.2/tests/test_utils.py` & `sonatoki-0.1.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/tokenize_cases/tokenize_sentences_tok.yml` & `sonatoki-0.1.3/tests/tokenize_cases/tokenize_sentences_tok.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/tests/tokenize_cases/tokenize_words_tok.yml` & `sonatoki-0.1.3/tests/tokenize_cases/tokenize_words_tok.yml`

 * *Files identical despite different names*

### Comparing `sonatoki-0.1.2/PKG-INFO` & `sonatoki-0.1.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonatoki
-Version: 0.1.2
+Version: 0.1.3
 Summary: ilo li moku e toki li pana e sona ni: ni li toki ala toki pona?
 Author-Email: "jan Kekan San (@gregdan3)" <gregory.danielson3@gmail.com>
 License: AGPL-3.0-or-later
 Requires-Python: >=3.8
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: regex>=2023.12.25
 Requires-Dist: typing-extensions>=4.11.0
@@ -16,61 +16,67 @@
 
 ## What is **sona toki**?
 
 This library, "Language Knowledge," helps you identify whether a message is in Toki Pona. No grammar checking, yet, which means this more checks whether a given message has enough Toki Pona words.
 
 I wrote it with a variety of scraps and lessons learned from a prior project, [ilo pi toki pona taso, "toki-pona-only tool"](https://github.com/gregdan3/ilo-pi-toki-pona-taso). That tool will be rewritten to use this library shortly.
 
-If you've ever worked on a similar project, you know the question "is this message in [language]" is not a consistent one- the environment, time, preferences of the speaker, and much more, can all alter whether a given message is "in toki pona," and this applies to essentially any language.
+If you've ever worked on a similar project, you know the question "is this message in [language]" is not a consistent one- the environment, time, preferences of the speaker, and much more, can all alter whether a given message is "in" any specific language, and this question applies to Toki Pona too.
 
-This project "solves" that complex problem by offering a highly configurable and incredibly lazy parser
+This project "solves" that complex problem by offering a highly configurable parser, so you can tune it to your preferences and goals.
 
 ## Quick Start
 
 Install with your preferred Python package manager. Example:
 
 ```sh
 pdm init  # if your pyproject.toml doesn't exist yet
 pdm add sonatoki
 ```
 
 Then get started with a script along these lines:
 
 ```py
-from sonatoki.Filters import (
-    Numerics,
-    Syllabic,
-    NimiLinku,
-    Alphabetic,
-    ProperName,
-    Punctuations,
-)
-from sonatoki.Scorers import SoftScaling
-from sonatoki.Cleaners import ConsecutiveDuplicates
-from sonatoki.Tokenizers import word_tokenize_tok
-from sonatoki.Preprocessors import URLs, DiscordEmotes
+from sonatoki.ilo import Ilo
+from sonatoki.Configs import PrefConfig
 
 def main():
-    ilo = Ilo(
-        preprocessors=[URLs, DiscordEmotes],
-        ignoring_filters=[Numerics, Punctuations],
-        scoring_filters=[NimiLinku, Syllabic, ProperName, Alphabetic],
-        cleaners=[ConsecutiveDuplicates],
-        scorer=SoftScaling,
-        tokenizer=word_tokenize_tok,
-    )
+    ilo = Ilo(**PrefConfig)
     ilo.is_toki_pona("imagine how is touch the sky")  # False
     ilo.is_toki_pona("o pilin insa e ni: sina pilin e sewi")  # True
     ilo.is_toki_pona("I Think I Can Evade Detection")  # False
 
 if __name__ == "__main__":
     main()
 ```
 
-`Ilo` is highly configurable by design, so I recommend exploring the `Preprocessors`, `Filters`, and `Scorers` modules. The `Cleaners` module only contains one cleaner, which I recommend using. The `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `word_tokenize_tok`.
+Or if you'd prefer to configure on your own:
+
+```py
+from copy import deepcopy
+from sonatoki.ilo import Ilo
+from sonatoki.Configs import BaseConfig
+from sonatoki.Filters import NimiPuAle, Phonotactic, ProperName
+from sonatoki.Scorers import SoftPassFail
+
+def main():
+    config = deepcopy(BaseConfig)
+    config["scoring_filters"].extend([NimiPuAle, Phonotactic, ProperName])
+    config["scorer"] = SoftPassFail
+
+    ilo = Ilo(**config)
+    ilo.is_toki_pona("mu mu!")  # True
+    ilo.is_toki_pona("mi namako e moku mi")  # True
+    ilo.is_toki_pona("ma wulin")  # False
+
+if __name__ == "__main__":
+    main()
+```
+
+`Ilo` is highly configurable by necessity, so I recommend looking through the premade configs in `Configs` as well as the individual `Preprocessors`, `Filters`, and `Scorers`. The `Cleaners` module only contains one cleaner, which I recommend always using. Similarly, the `Tokenizers` module contains several other word tokenizers, but their performance will be worse than the dedicated Toki Pona tokenizer `WordTokenizerTok`.
 
 ## Development
 
 1. Install [pdm](https://github.com/pdm-project/pdm)
 1. `pdm install --dev`
 1. Open any file you like!
```

