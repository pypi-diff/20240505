# Comparing `tmp/catframes-2024.3.1.tar.gz` & `tmp/catframes-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catframes-2024.3.1.tar", last modified: Wed Apr  3 00:23:10 2024, max compression
+gzip compressed data, was "catframes-2024.4.0.tar", last modified: Sun May  5 19:04:40 2024, max compression
```

## Comparing `catframes-2024.3.1.tar` & `catframes-2024.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.862280 catframes-2024.3.1/
--rw-r--r--   0 me        (1000) me        (1000)      875 2024-04-02 23:58:18.000000 catframes-2024.3.1/LICENSE.txt
--rw-r--r--   0 me        (1000) me        (1000)     6311 2024-04-03 00:23:10.862280 catframes-2024.3.1/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)     4808 2024-04-02 23:58:18.000000 catframes-2024.3.1/README.md
--rw-r--r--   0 me        (1000) me        (1000)      875 2024-04-03 00:00:14.000000 catframes-2024.3.1/pyproject.toml
--rw-r--r--   0 me        (1000) me        (1000)       38 2024-04-03 00:23:10.862280 catframes-2024.3.1/setup.cfg
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.812279 catframes-2024.3.1/src/
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.832279 catframes-2024.3.1/src/catframes/
--rw-r--r--   0 me        (1000) me        (1000)       18 2023-09-24 19:02:05.000000 catframes-2024.3.1/src/catframes/__init__.py
--rw-r--r--   0 me        (1000) me        (1000)   138208 2024-04-03 00:03:15.000000 catframes-2024.3.1/src/catframes/catframes.py
-drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-04-03 00:23:10.862280 catframes-2024.3.1/src/catframes.egg-info/
--rw-r--r--   0 me        (1000) me        (1000)     6311 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/PKG-INFO
--rw-r--r--   0 me        (1000) me        (1000)      313 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/SOURCES.txt
--rw-r--r--   0 me        (1000) me        (1000)        1 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/dependency_links.txt
--rw-r--r--   0 me        (1000) me        (1000)       55 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/entry_points.txt
--rw-r--r--   0 me        (1000) me        (1000)       14 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/requires.txt
--rw-r--r--   0 me        (1000) me        (1000)       10 2024-04-03 00:23:10.000000 catframes-2024.3.1/src/catframes.egg-info/top_level.txt
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-05-05 19:04:40.664498 catframes-2024.4.0/
+-rw-r--r--   0 me        (1000) me        (1000)      875 2024-05-03 21:36:30.000000 catframes-2024.4.0/LICENSE.txt
+-rw-r--r--   0 me        (1000) me        (1000)     6311 2024-05-05 19:04:40.644492 catframes-2024.4.0/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)     4808 2024-05-04 04:19:43.000000 catframes-2024.4.0/README.md
+-rw-r--r--   0 me        (1000) me        (1000)      875 2024-05-04 04:22:40.000000 catframes-2024.4.0/pyproject.toml
+-rw-r--r--   0 me        (1000) me        (1000)       38 2024-05-05 19:04:40.664498 catframes-2024.4.0/setup.cfg
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-05-05 19:04:40.584474 catframes-2024.4.0/src/
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-05-05 19:04:40.614483 catframes-2024.4.0/src/catframes/
+-rw-r--r--   0 me        (1000) me        (1000)       18 2023-09-24 19:02:05.000000 catframes-2024.4.0/src/catframes/__init__.py
+-rw-r--r--   0 me        (1000) me        (1000)   136869 2024-05-05 18:33:47.000000 catframes-2024.4.0/src/catframes/catframes.py
+drwxr-sr-x   0 me        (1000) me        (1000)        0 2024-05-05 19:04:40.644492 catframes-2024.4.0/src/catframes.egg-info/
+-rw-r--r--   0 me        (1000) me        (1000)     6311 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/PKG-INFO
+-rw-r--r--   0 me        (1000) me        (1000)      313 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/SOURCES.txt
+-rw-r--r--   0 me        (1000) me        (1000)        1 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/dependency_links.txt
+-rw-r--r--   0 me        (1000) me        (1000)       55 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/entry_points.txt
+-rw-r--r--   0 me        (1000) me        (1000)       14 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/requires.txt
+-rw-r--r--   0 me        (1000) me        (1000)       10 2024-05-05 19:04:40.000000 catframes-2024.4.0/src/catframes.egg-info/top_level.txt
```

### Comparing `catframes-2024.3.1/LICENSE.txt` & `catframes-2024.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `catframes-2024.3.1/PKG-INFO` & `catframes-2024.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catframes
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: A handy tool for combining images into videos via FFmpeg.
 Author-email: Georgy Ustinov <inbox@itustinov.ru>
 License: © Устинов Г.М., 2022–2024
         
         This software is provided 'as-is', without any express or implied
         warranty.  In no event will the authors be held liable for any damages
         arising from the use of this software.
```

### Comparing `catframes-2024.3.1/README.md` & `catframes-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `catframes-2024.3.1/pyproject.toml` & `catframes-2024.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "catframes"
-version = "2024.3.1"
+version = "2024.4.0"
 
 description = "A handy tool for combining images into videos via FFmpeg."
 
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
 requires-python = ">=3.7"
```

### Comparing `catframes-2024.3.1/src/catframes/catframes.py` & `catframes-2024.4.0/src/catframes/catframes.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 import http.client
 from time import sleep, monotonic
 from unittest import TestCase
 
 from PIL import Image, ImageColor, ImageDraw, ImageFont
 
 
-__version__ = '2024.3.1'
+__version__ = '2024.4.0'
 __license__ = 'Zlib'
 
 
 TITLE = f'Catframes {__version__}'
 
 DESCRIPTION = f"""{TITLE}
 
@@ -86,113 +86,115 @@
 
   This package source code: https://github.com/georgy7/catframes
   My collection of scripts: https://gitflic.ru/project/georgy7/cona
   Self-hosted Git bundle: http://itustinov.ru/cona/latest/cona.pack
 
 """
 
-WebApp = Callable[[dict, Callable], Iterable[bytes]]
-"""Первый аргумент — WSGI environment (включает всю информацию о запросе), второй — функция начала
-ответа, которая принимает статус HTTP-ответа и список HTTP-заголовков. В терминах MVC, это еще
-неразграниченные роутинг с контроллерами.
+HTTPService = Callable[[dict, Callable], Iterable[bytes]]
+"""A function that is similar to HttpServlet in Java.
 
-Подробнее читайте в официальной документации: :py:func:`wsgiref.simple_server.make_server`.
+The first argument is WSGI environment (includes all information about the request),
+the second is the response start function, which accepts the status of the HTTP response
+and a list of HTTP headers.
+
+Read more in the official documentation: :py:func:`wsgiref.simple_server.make_server`.
 """
 
-WebJob = Callable[[int], None]
-"""Функция, которая работает с локальным веб-приложением. Аргумент — номер порта."""
+HTTPClient = Callable[[int], None]
+"""A function that uses a local HTTP service. The argument is the port number."""
 
 
 @dataclass(frozen=True)
-class JobServerOptions:
+class TheChestParameterSet:
     min_http_port: int
     max_http_port: int
 
     def __post_init__(self):
         assert self.min_http_port > 0
         assert self.max_http_port > 0
         assert self.min_http_port <= self.max_http_port
 
 
-class JobServer:
-    """Механизм межпроцессного взаимодействия на основе HTTP. Открывает порт и обслуживает другие
-    программы, которые контролируются из этого же сервера.
-    Этот объект похож на два куска хлеба в сэндвиче, которые обнимают процесс-начинку.
-
-    Грубо говоря, эта штука позволяет делать что-то вроде динамической файловой системы, если
-    считать URL файлами: в тот момент, когда что-то запрашивается сторонней программой, оно
-    подготавливается на лету. Не тратится дисковое пространство, а если не использовать временные
-    файлы при обработке запросов, то и ресурс SSD.
-
-    В целях безопасности:
-
-    1. на компьютере следует использовать файрвол;
-    2. лучше не передавать списки URL по HTTP-каналу.
-
-    Номер порта выбирается случайно из диапазона, указанного в настройках.
-
-    :param app: Функция, которая обслуживает HTTP-запросы.
-    :param job: Запускается один раз. Сервер ждёт завершения. Выброшенные исключения приводят
-        к остановке сервера и вылетают из метода :meth:`run`.
-    :param options: Системные настройки.
+class TwoFromTheChest:
+    """Two from the chest, at my behest! Is that true, you'll do anything for me?
+
+    This is from the cartoon Vovka in the Far-Around Kingdom (1965).
+
+    It is an HTTP-based interprocess communication mechanism that works like a web server, providing data,
+    while simultaneously starting a data recipient and waiting for it to complete.
+    It is assumed that it is used to run an external process that can read data over the network.
+    FFmpeg can read images either from disk (as files) or over the network (as URLs).
+    If it is necessary to process the images before giving them to this program, it is faster to send them
+    over the network than to save them to disk. It also reduces disc wear.
+
+    For security reasons:
+
+    1. You should use a firewall on your computer.
+    2. It is better not to send URL lists over the HTTP channel.
+
+    :param giver: The function that responds to HTTP requests.
+    :param eater: The function that controls the source of HTTP requests. It runs synchronously and
+        only once. Exceptions thrown from here will be re-thrown from the method :meth:`start`.
+    :param options: System settings.
     """
-    def __init__(self, app: WebApp, job: WebJob, options: JobServerOptions):
-        self._app: WebApp = app
-        self._job: WebJob = job
+    def __init__(self, giver: HTTPService, eater: HTTPClient, options: TheChestParameterSet):
+        self._giver: HTTPService = giver
+        self._eater: HTTPClient = eater
         self._options = options
-        self._job_error: Union[Exception, None] = None
+        self._eater_error: Union[Exception, None] = None
 
-    def run(self):
-        """Запускает сервер, ждёт завершения работ, останавливает сервер.
+    def start(self):
+        """It waits until the eater is full.
 
-        :raises Exception: если исключение вылетело из джобы.
+        :raises Exception: thrown by the eater.
         """
         while not self._was_running():
             print('Trying different port...')
-        if self._job_error:
-            raise self._job_error
+        if self._eater_error:
+            raise self._eater_error
 
-    def _do_the_job(self, port):
+    def _eat(self, http_port):
         try:
-            self._job(port)
+            self._eater(http_port)
         except Exception as exc:
-            # Ловля общего исключения обоснована:
-            # нужно остановить сервер, а потом можно перевыбросить.
-            self._job_error = exc
+            # Catching a general exception is justified:
+            # I stop the server and then re-throw this exception.
+            self._eater_error = exc
 
     def _was_running(self) -> bool:
-        port = random.randint(
+        http_port = random.randint(
             self._options.min_http_port,
             self._options.max_http_port
         )
-        print(f"\nPort: {port}\n")
+        print(f"\nPort: {http_port}\n")
         try:
 
-            httpd = make_server(host='', port=port, app=self._app)
+            httpd = make_server(host='', port=http_port, app=self._giver)
             try:
                 web_thread = threading.Thread(target = httpd.serve_forever)
                 web_thread.daemon = True
                 web_thread.start()
-                self._do_the_job(port)
+                self._eat(http_port)
             finally:
                 httpd.shutdown()        # Exit loop.
                 httpd.server_close()    # Clean up the server.
 
             return True
         except OSError:
             return False
 
 
-class _JobServerTest(TestCase):
+class _TwoFromTheChestTest(TestCase):
     def test_get(self):
         """Сервер должен ждать завершения работ. Здесь используются GET-запросы и ASCII-пути."""
 
         content = 'Hello World'.encode("utf-8")
 
-        def webapp(environ, start_response):
+        def service(environ, start_response):
             method: str = environ['REQUEST_METHOD']
             pathname: str = environ['PATH_INFO']
 
             if method == 'GET' and pathname == '/abc.txt':
                 status = '200 OK'
                 headers = [('Content-type', 'text/plain; charset=utf-8')]
                 start_response(status, headers)
@@ -205,15 +207,15 @@
                 return [pathname.encode("utf-8")]
 
             status = '404 Not Found'
             headers = [('Content-type', 'text/plain; charset=utf-8')]
             start_response(status, headers)
             return ['Not found.'.encode("utf-8")]
 
-        def webjob(port):
+        def client(port):
             base_url = f'localhost:{port}'
 
             def read(pathname):
                 conn = http.client.HTTPConnection(base_url)
                 conn.request('GET', pathname)
                 response = conn.getresponse()
                 return (response.status, response.read())
@@ -223,24 +225,24 @@
             sleep(1)
             self.assertEqual(read('/abc.txt'), (200, content))
 
             self.assertEqual(
                 read('/Item/123'),
                 (200, '/Item/123'.encode("utf-8")))
 
-        server = JobServer(webapp, webjob, JobServerOptions(10240, 65535))
-        server.run()
+        these_guys = TwoFromTheChest(service, client, TheChestParameterSet(10240, 65535))
+        these_guys.start()
 
 
 class FileUtils:
-    """Модуль вспомогательных функций, связанных с файловой системой."""
+    """A module of auxiliary functions related to the file system."""
 
     @staticmethod
     def get_checksum(path: Union[Path, None]) -> Optional[str]:
-        """Функция не выбрасывает исключения."""
+        """This function does not throw exceptions."""
         if not path:
             return None
         hashsum = hashlib.sha1()
         try:
             with path.expanduser().open(mode = 'rb') as binary:
                 chunk = binary.read(4096)
                 while chunk:
@@ -248,38 +250,38 @@
                     chunk = binary.read(4096)
             return hashsum.hexdigest()
         except OSError:
             return None
 
     @staticmethod
     def get_mtime(path: Union[Path, None]) -> Optional[datetime]:
-        """Функция не выбрасывает исключения."""
+        """This function does not throw exceptions."""
         if not path:
             return None
         try:
             return datetime.fromtimestamp(os.path.getmtime(path.expanduser()))
         except OSError:
             return None
 
     @staticmethod
     def get_file_size(path: Union[Path, None]) -> Optional[int]:
-        """Функция не выбрасывает исключения."""
+        """This function does not throw exceptions."""
         if not path:
             return None
         try:
             normal_path = path.expanduser()
             if normal_path.is_file():
                 return os.path.getsize(normal_path)
             return None
         except OSError:
             return None
 
     @staticmethod
     def is_symlink(path: Union[Path, None]) -> bool:
-        """Функция не выбрасывает исключения."""
+        """This function does not throw exceptions."""
         if not path:
             return False
         return path.expanduser().is_symlink()
 
     @staticmethod
     def list_images(path: Path) -> List[Path]:
         """Набор файлов JPEG и PNG в порядке, предоставляемом pathlib (не определён в документации
@@ -597,32 +599,32 @@
 
         FileUtils.sort_natural(items)
         self.assertSequenceEqual(expected, items)
 
 
 @dataclass(frozen=True)
 class Resolution:
-    """Ненулевое разрешение в пикселях."""
+    """Non-zero size in pixels."""
 
     width: int
     height: int
 
     def __post_init__(self):
         assert self.width > 0
         assert self.height > 0
 
     def __str__(self):
-        """Возвращает строку вида ``ШxВ``. Икс в качестве разделителя выбран из соображений
-        совместимости с максимальным числом шрифтов оверлеев и кодировок терминалов.
+        """Returns a string of the form `WxH". The letter X was chosen as the separator
+        for compatibility reasons with most fonts and encodings.
         """
         return f'{self.width}x{self.height}'
 
     @property
     def ratio(self) -> float:
-        """Соотношение сторон. Всегда больше нуля."""
+        """Aspect ratio. Always more than zero."""
         return self.width / self.height
 
 
 class Frame:
     """Кадр на диске. Сырьё для :class:`FrameView`. Конструктор создаёт объект, даже если путь
     ведёт в никуда. Не иммутабельная сущность, некоторые поля могут обновляться.
 
@@ -905,23 +907,23 @@
 
         result = Resolution(
                 ResolutionUtils.round(raw_result.width),
                 ResolutionUtils.round(raw_result.height))
 
         alternatives = []
 
-        if result.height < ResolutionUtils.round(find_other_axis(raw_result.width, width, height, count)):
+        if result.height < ResolutionUtils.round(find_other_axis(raw_result.width, width, height, list(count))):
             alternatives.append(Resolution(
                 result.width,
-                ResolutionUtils.round(find_other_axis(result.width, width, height, count))
+                ResolutionUtils.round(find_other_axis(result.width, width, height, list(count)))
             ))
 
-        if result.width < ResolutionUtils.round(find_other_axis(raw_result.height, height, width, count)):
+        if result.width < ResolutionUtils.round(find_other_axis(raw_result.height, height, width, list(count))):
             alternatives.append(Resolution(
-                ResolutionUtils.round(find_other_axis(result.height, height, width, count)),
+                ResolutionUtils.round(find_other_axis(result.height, height, width, list(count))),
                 result.height
             ))
 
         if len(alternatives) == 1:
             return alternatives[0]
         elif len(alternatives) > 1:
             alternatives.sort(key=lambda x: x.width*x.height, reverse=True)
@@ -1581,16 +1583,16 @@
 
     def limit_frames(self, frames: Sequence[Frame]):
         if self.limit_seconds:
             frames = frames[:(self.limit_seconds*self.frame_rate)]
         return frames
 
     def make(self, frames: Sequence[Frame], \
-            frame_processor: FrameProcessor, \
-            server_options: JobServerOptions):
+             frame_processor: FrameProcessor, \
+             server_options: TheChestParameterSet):
 
         # На случай отсутствия файрвола, адреса не должны быть предсказуемыми. При таком смещении,
         # шанс угадать URL одного кадра 24-часового видео с 60 fps — 1:2e12 на 64-битной машине.
         offset: int = random.randint(0, max(0, sys.maxsize - len(frames)))
 
         render_results = deque()
         max_results = 10
@@ -1628,15 +1630,15 @@
                             result = x[1]
 
             while len(render_results) > max_results:
                 render_results.popleft()
 
             return result
 
-        def app(environ, start_response):
+        def service(environ, start_response):
             method: str = environ['REQUEST_METHOD']
             pathname: str = environ['PATH_INFO']
 
             http_get = (method == 'GET')
             img_page = re.fullmatch(r'/img/(\d+)', pathname)
 
             if http_get and img_page:
@@ -1649,15 +1651,15 @@
                     return [render_result.data]
 
             status = '404 Not Found'
             headers = [('Content-type', 'text/plain; charset=utf-8')]
             start_response(status, headers)
             return ['Not found.'.encode("utf-8")]
 
-        def job(port: int):
+        def client(port: int):
             base_url = f'http://localhost:{port}/img/'
 
             with tempfile.TemporaryDirectory() as folder_path_string:
                 folder_path = Path(folder_path_string)
                 list_path = folder_path / 'list.txt'
 
                 duration = 1 / self.frame_rate
@@ -1687,16 +1689,16 @@
                     '-r', str(self.frame_rate),
                     ('-y' if self.overwrite else '-n'),
                     str(self.destination.expanduser())
                 ])
 
                 subprocess.check_call(ffmpeg_options)
 
-        server = JobServer(app, job, server_options)
-        server.run()
+        these_guys = TwoFromTheChest(service, client, server_options)
+        these_guys.start()
 
 
 class PillowFrameView(FrameView):
     """Каркас для гарантированно однопоточного рендеринга библиотекой Pillow. Синхронизация
     позволяет использовать один и тот же холст многократно, не нагружая кучу и сборщик мусора.
     """
     def __init__(self, resolution: Resolution):
@@ -2980,16 +2982,16 @@
         return OutputOptions(
             destination=destination,
             overwrite=bool(self._args.force),
             limit_seconds=self._args.limit,
             quality=quality,
             frame_rate=self._args.frame_rate)
 
-    def get_server_options(self) -> JobServerOptions:
-        return JobServerOptions(
+    def get_server_options(self) -> TheChestParameterSet:
+        return TheChestParameterSet(
             self._args.port_range[0],
             self._args.port_range[1]
         )
 
     @property
     def statistics_only(self) -> bool:
         """Пользователь не хочет пока делать видео, только посмотреть логику выбора разрешения."""
```

### Comparing `catframes-2024.3.1/src/catframes.egg-info/PKG-INFO` & `catframes-2024.4.0/src/catframes.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catframes
-Version: 2024.3.1
+Version: 2024.4.0
 Summary: A handy tool for combining images into videos via FFmpeg.
 Author-email: Georgy Ustinov <inbox@itustinov.ru>
 License: © Устинов Г.М., 2022–2024
         
         This software is provided 'as-is', without any express or implied
         warranty.  In no event will the authors be held liable for any damages
         arising from the use of this software.
```

