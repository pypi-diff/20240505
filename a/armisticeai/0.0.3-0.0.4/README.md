# Comparing `tmp/armisticeai-0.0.3.tar.gz` & `tmp/armisticeai-0.0.4.tar.gz`

## Comparing `armisticeai-0.0.3.tar` & `armisticeai-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 armisticeai-0.0.3/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-03 01:19:45.000000 armisticeai-0.0.3/.gitignore
--rw-r--r--   0     1001      127      380 2024-05-03 01:19:45.000000 armisticeai-0.0.3/README.md
--rw-r--r--   0     1001      127      104 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/__init__.py
--rw-r--r--   0     1001      127       30 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/__main__.py
--rw-r--r--   0     1001      127     3654 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/_cli.py
--rw-r--r--   0     1001      127    11626 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/_client.py
--rw-r--r--   0     1001      127       44 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/_exceptions.py
--rw-r--r--   0     1001      127     4352 2024-05-03 01:19:45.000000 armisticeai-0.0.3/python/armisticeai/_utils.py
--rw-r--r--   0     1001      127      255 2024-05-03 01:19:45.000000 armisticeai-0.0.3/requirements.txt
--rw-r--r--   0     1001      127     5784 2024-05-03 01:19:45.000000 armisticeai-0.0.3/src/lib.rs
--rw-r--r--   0     1001      127    63223 2024-05-03 01:19:45.000000 armisticeai-0.0.3/Cargo.lock
--rw-r--r--   0     1001      127      563 2024-05-03 01:19:45.000000 armisticeai-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 armisticeai-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 armisticeai-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-05 18:23:03.000000 armisticeai-0.0.4/.gitignore
+-rw-r--r--   0     1001      127      380 2024-05-05 18:23:03.000000 armisticeai-0.0.4/README.md
+-rw-r--r--   0     1001      127      104 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/__init__.py
+-rw-r--r--   0     1001      127       30 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/__main__.py
+-rw-r--r--   0     1001      127     2478 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/_cli.py
+-rw-r--r--   0     1001      127    11966 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/_client.py
+-rw-r--r--   0     1001      127       44 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/_exceptions.py
+-rw-r--r--   0     1001      127     4352 2024-05-05 18:23:03.000000 armisticeai-0.0.4/python/armisticeai/_utils.py
+-rw-r--r--   0     1001      127      255 2024-05-05 18:23:03.000000 armisticeai-0.0.4/requirements.txt
+-rw-r--r--   0     1001      127     5784 2024-05-05 18:23:03.000000 armisticeai-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      127    63223 2024-05-05 18:23:03.000000 armisticeai-0.0.4/Cargo.lock
+-rw-r--r--   0     1001      127      563 2024-05-05 18:23:03.000000 armisticeai-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 armisticeai-0.0.4/PKG-INFO
```

### Comparing `armisticeai-0.0.3/Cargo.toml` & `armisticeai-0.0.4/Cargo.toml`

 * *Files identical despite different names*

### Comparing `armisticeai-0.0.3/.gitignore` & `armisticeai-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `armisticeai-0.0.3/python/armisticeai/_cli.py` & `armisticeai-0.0.4/python/armisticeai/_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,68 +21,27 @@
     parser.add_argument(
         "--dataset",
         type=str,
         default="ArmisticeAI/OCTDL2024",
         help="The dataset to train on. Default is 'ArmisticeAI/OCTDL2024'. Can be local directory or HuggingFace dataset.",
     )
     parser.add_argument(
-        "--checkpoint",
-        "-c",
-        type=str,
-        default="google/vit-base-patch16-224-in21k",
-        help="The model to start training from. Default is 'google/vit-base-patch16-224-in21k'.",
-    )
-    parser.add_argument(
         "--output-dir",
         "-o",
         type=str,
         default="retinal_classifier/",
         help="Output directory to store training checkpoints. Default is 'retinal_classifier'.",
     )
     parser.add_argument(
         "--batch-size",
         "-b",
         type=int,
         default=16,
         help="The local batch size to be used during training. Default is 16.",
     )
-    parser.add_argument(
-        "--training",
-        "-t",
-        type=str,
-        choices=["full", "lora_fp16", "lora_int8", "qlora_int4"],
-        default="full",
-        help="Training type. Default is 'full'.",
-    )
-    parser.add_argument(
-        "--rank",
-        "-r",
-        type=int,
-        default=64,
-        help="Rank of LoRA matrix. Default is 64.",
-    )
-    parser.add_argument(
-        "--alpha",
-        "-a",
-        type=int,
-        default=128,
-        help="Alpha of LoRA matrix. Default is 128 (alpha = 2*r is recommended).",
-    )
-    parser.add_argument(
-        "--dap",
-        action="store_true",
-        help="If set, use DAP to perform secure aggregation. Default is false.",
-    )
-    parser.add_argument(
-        "--dap-client-addr",
-        "-d",
-        type=str,
-        default="localhost:9000",
-        help="Address of DAP client to send parameters to. Default is 'localhost:9000'.",
-    )
     # Adding arguments for test partitioning as optional
     parser.add_argument(
         "--test-partition",
         action="store_true",
         help="Enables artificially splitting the dataset for testing. If set, requires --partition-percent and --partition-index.",
     )
     parser.add_argument(
```

### Comparing `armisticeai-0.0.3/python/armisticeai/_client.py` & `armisticeai-0.0.4/python/armisticeai/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,24 +46,20 @@
 
 
 # Flower client
 class ArmisticeAI(fl.client.NumPyClient):
     def __init__(
         self,
         *,
-        api_key: str | None = None,
+        api_key: str | None = None,  # client_uuid
         organization: str | None = None,
         project: str | None = None,
-        checkpoint: str | None = "google/vit-base-patch16-224-in21k",
-        training_type: str = "lora_fp16",
         dataset: str,
         output_dir: str,
         batch_size: int = 16,
-        r: int = 16,
-        dap: bool = True,
         test_partition: bool = False,
         partition_percent: List | None = None,
         partition_index: int | None = None,
         wandb: bool | None = None,
         server_address: str | None = "127.0.0.1:8080",
     ) -> None:
         """Construct a new armisticeai client instance.
@@ -85,89 +81,98 @@
             organization = os.environ.get("ARMISTICEAI_ORG_ID")
         self.organization = organization
 
         if project is None:
             project = os.environ.get("ARMISTICEAI_PROJECT_ID")
         self.project = project
 
-        trainset, testset = load_dataset(dataset)
+        self.trainset, self.testset = load_dataset(dataset)
         if test_partition:
-            trainset = split_dataset(trainset, partition_percent)[partition_index]
-            testset = split_dataset(testset, partition_percent)[partition_index]
-
-        self.image_processor = AutoImageProcessor.from_pretrained(
-            checkpoint, device_map="auto"
-        )
-        self.trainset, self.testset = preprocess(
-            self.image_processor, trainset, testset
-        )
-
-        self.training_type = TrainingType[training_type.upper()]
-
-        self.client_id = uuid.uuid4()
+            self.trainset = split_dataset(self.trainset, partition_percent)[
+                partition_index
+            ]
+            self.testset = split_dataset(self.testset, partition_percent)[
+                partition_index
+            ]
 
-        labels = load_labels(trainset)
-        label2id, id2label = load_label_id_map(labels)
+        self.labels = load_labels(self.trainset)
+        self.label2id, self.id2label = load_label_id_map(self.labels)
 
-        load_in_8bit = False
-        load_in_4bit = False
-        if self.training_type == TrainingType.LORA_INT8:
-            load_in_8bit = True
+        self.dap = True
 
         # NOTE: Using LoftQ for now
         # if training_type == TrainingType.QLORA_INT4:
         #     load_in_4bit = True
-        print(f"labels: {labels}, load_in_8_bit: {load_in_8bit}")
-        self.model = load_model(
-            checkpoint, labels, label2id, id2label, load_in_8bit, load_in_4bit
-        )
-        self.dap = dap
-        if r is not None:
-            alpha = 2 * r
-        if (
-            self.training_type == TrainingType.LORA_FP16
-            or self.training_type == TrainingType.LORA_INT8
-        ):
-            lora_config = LoraConfig(
-                r=r,
-                lora_alpha=alpha,
-                target_modules=["query", "value"],
-                lora_dropout=0.1,
-                bias="none",
-                modules_to_save=["classifier"],
-            )
-            if self.training_type == TrainingType.LORA_INT8:
-                self.model = prepare_model_for_kbit_training(self.model)
-            self.model = get_peft_model(self.model, lora_config)
-        elif self.training_type == TrainingType.QLORA_INT4:
-            loftq_config = LoftQConfig(loftq_bits=4)
-            lora_config = LoraConfig(
-                init_lora_weights="loftq",
-                loftq_config=loftq_config,
-                r=r,
-                lora_alpha=alpha,
-                target_modules=["query", "value"],
-                lora_dropout=0.1,
-                bias="none",
-                modules_to_save=["classifier"],
-            )
-            self.model = get_peft_model(self.model, lora_config)
-
-        if self.training_type != TrainingType.FULL:
-            print(f"Init model: {self.get_parameters({})[2][0][:10]}")
-        else:
-            print(f"Init model: {self.get_parameters({})[1][0][0][:10]}")
 
         self.data_collator = DefaultDataCollator()
         self.accuracy = evaluate.load("accuracy")
-        self.output_dir = output_dir + "/client_" + str(self.client_id)
+        self.output_dir = output_dir + "/client_" + str(self.api_key)
         self.batch_size = batch_size
         self.server_address = server_address
 
     def get_parameters(self, config: Dict[str, Scalar]) -> NDArrays:
+        if "init" in config:
+            # During first round of training, we configure every piece
+            checkpoint = config["checkpoint"]
+            self.image_processor = AutoImageProcessor.from_pretrained(
+                checkpoint, device_map="auto"
+            )
+            self.trainset, self.testset = preprocess(
+                self.image_processor, self.trainset, self.testset
+            )
+            self.training_type = TrainingType[config["training_type"].upper()]
+
+            load_in_8bit = False
+            load_in_4bit = False
+            if self.training_type == TrainingType.LORA_INT8:
+                load_in_8bit = True
+
+            self.model = load_model(
+                config["checkpoint"],
+                self.labels,
+                self.label2id,
+                self.id2label,
+                load_in_8bit,
+                load_in_4bit,
+            )
+            r = config["rank"]
+            if (
+                self.training_type == TrainingType.LORA_FP16
+                or self.training_type == TrainingType.LORA_INT8
+            ):
+                lora_config = LoraConfig(
+                    r=r,
+                    lora_alpha=2 * r,
+                    target_modules=["query", "value"],
+                    lora_dropout=0.1,
+                    bias="none",
+                    modules_to_save=["classifier"],
+                )
+                if self.training_type == TrainingType.LORA_INT8:
+                    self.model = prepare_model_for_kbit_training(self.model)
+                self.model = get_peft_model(self.model, lora_config)
+            elif self.training_type == TrainingType.QLORA_INT4:
+                loftq_config = LoftQConfig(loftq_bits=4)
+                lora_config = LoraConfig(
+                    init_lora_weights="loftq",
+                    loftq_config=loftq_config,
+                    r=r,
+                    lora_alpha=2 * r,
+                    target_modules=["query", "value"],
+                    lora_dropout=0.1,
+                    bias="none",
+                    modules_to_save=["classifier"],
+                )
+                self.model = get_peft_model(self.model, lora_config)
+
+            if self.training_type != TrainingType.FULL:
+                print(f"Init model: {self.get_parameters({})[2][0][:10]}")
+            else:
+                print(f"Init model: {self.get_parameters({})[1][0][0][:10]}")
+
         if self.training_type == TrainingType.FULL:
             state_dict = self.model.state_dict()
         else:
             state_dict = get_peft_model_state_dict(self.model)
         return [val.cpu().numpy() for _, val in state_dict.items()]
 
     def set_parameters(self, parameters):
@@ -259,14 +264,15 @@
                 raise KeyError(f"Missing keys: {', '.join(missing_keys)}")
             print(f"[DAP]: task_id_encoded inside fit: {config['task_id']}")
 
         train_results = trainer.train()
         eval_results = trainer.evaluate()
 
         out = {
+            "client_id": self.api_key,
             "train_loss": train_results.training_loss,
             "eval_loss": eval_results["eval_loss"],
             "accuracy": eval_results["eval_accuracy"],
         }
         train_accuracy = eval_results["eval_accuracy"]
         params = self.get_parameters(config)
         if self.training_type != TrainingType.FULL:
```

### Comparing `armisticeai-0.0.3/python/armisticeai/_utils.py` & `armisticeai-0.0.4/python/armisticeai/_utils.py`

 * *Files identical despite different names*

### Comparing `armisticeai-0.0.3/src/lib.rs` & `armisticeai-0.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `armisticeai-0.0.3/Cargo.lock` & `armisticeai-0.0.4/Cargo.lock`

 * *Files identical despite different names*

### Comparing `armisticeai-0.0.3/pyproject.toml` & `armisticeai-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
 module-name = "armisticeai.armisticeai"
 
 [project]
 name = "armisticeai"
-version = "0.0.3"
+version = "0.0.4"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{ name = 'ArmisticeAI', email = 'tanya@armistice.ai' }]
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
```

### Comparing `armisticeai-0.0.3/PKG-INFO` & `armisticeai-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: armisticeai
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Author-email: ArmisticeAI <tanya@armistice.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

