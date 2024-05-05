# Comparing `tmp/careamics-0.1.0rc3.tar.gz` & `tmp/careamics-0.1.0rc4.tar.gz`

## Comparing `careamics-0.1.0rc3.tar` & `careamics-0.1.0rc4.tar`

### file list

```diff
@@ -1,170 +1,173 @@
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/PR_TEMPLATE/pull_request.md
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2n/example_SEM_careamist.ipynb
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2n/n2n_2D_SEM.yml
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_careamist.ipynb
--rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_lightning.ipynb
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/example_SEM_lightning.ipynb
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/n2v/n2v_2D_BSD.yml
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/2D/pn2v/pN2V_Convallaria.yml
--rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/3D/example_flywing_3D.ipynb
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/examples/3D/n2v_flywing_3D.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/__init__.py
--rw-r--r--   0        0        0    28336 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/careamist.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/conftest.py
--rw-r--r--   0        0        0    28552 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_datamodule.py
--rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_module.py
--rw-r--r--   0        0        0    15053 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_prediction_datamodule.py
--rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/lightning_prediction_loop.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/py.typed
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/__init__.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/hyperparameters_callback.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/callbacks/progress_bar_callback.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/__init__.py
--rw-r--r--   0        0        0     5727 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/algorithm_model.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/callback_model.py
--rw-r--r--   0        0        0    14610 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/configuration_factory.py
--rw-r--r--   0        0        0    18730 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/configuration_model.py
--rw-r--r--   0        0        0    16806 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/data_model.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/inference_model.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/noise_models.py
--rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/optimizer_models.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/tile_information.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/training_model.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/architecture_model.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/custom_model.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/register_model.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/unet_model.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/architectures/vae_model.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/__init__.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/algorithm_descriptions.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/references/references.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/__init__.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_activations.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_algorithms.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_architectures.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_data.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_extraction_strategies.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_loggers.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_losses.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_optimizers.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_pixel_manipulations.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_struct_axis.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/support/supported_transforms.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/__init__.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/n2v_manipulate_model.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/nd_flip_model.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/normalize_model.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/transform_model.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/transformations/xy_random_rotate90_model.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/validators/__init__.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/config/validators/validator_utils.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/__init__.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/in_memory_dataset.py
--rw-r--r--   0        0        0    15030 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/iterable_dataset.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/zarr_dataset.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/__init__.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/dataset_utils.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/file_utils.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_tiff.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_utils.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_zarr.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/__init__.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/patch_transform.py
--rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/patching.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/random_patching.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/sequential_patching.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/tiled_patching.py
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/dataset/patching/validate_patch_dimension.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/__init__.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/loss_factory.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/losses.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/noise_model_factory.py
--rw-r--r--   0        0        0    17801 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/losses/noise_models.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/__init__.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bmz_io.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/model_io_utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/__init__.py
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/_readme_factory.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/bioimage_utils.py
--rw-r--r--   0        0        0     9204 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/model_io/bioimage/model_description.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/activation.py
--rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/layers.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/model_factory.py
--rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/models/unet.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/prediction/__init__.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/prediction/stitch_prediction.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/__init__.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/n2v_manipulate.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/nd_flip.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/normalize.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/pixel_manipulation.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/struct_mask_parameters.py
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/tta.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/transforms/xy_random_rotate90.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/__init__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/base_enum.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/context.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/logging.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/metrics.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/path_utils.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/ram.py
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/receptive_field.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/running_stats.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/src/careamics/utils/torch_utils.py
--rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/conftest.py
--rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_careamist.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_conftest.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_lightning_datamodule.py
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/test_lightning_module.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_algorithm_model.py
--rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_configuration_factory.py
--rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_configuration_model.py
--rw-r--r--   0        0        0    12298 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_data_model.py
--rw-r--r--   0        0        0     6234 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_inference_model.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_optimizers_model.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_tile_information.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/test_training_model.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_architecture_model.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_custom_model.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_register_model.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/architectures/test_unet_model.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/support/test_supported_data.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/support/test_supported_optimizers.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/transformations/test_n2v_manipulate_model.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/transformations/test_normalize_model.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/config/validators/test_validator_utils.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/test_in_memory_dataset.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/test_iterable_dataset.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/dataset_utils/test_list_files.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/dataset_utils/test_read_tiff.py
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_patching_utils.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_random_patching.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_sequential_patching.py
--rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/dataset/patching/test_tiled_patching.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/model_io/test_bmz_io.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/models/test_model_factory.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/models/test_unet.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/prediction/test_stitch_prediction.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_manipulate_n2v.py
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_nd_flip.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_normalize.py
--rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_pixel_manipulation.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_supported_transforms.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/transforms/test_xy_random_rotate90.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_base_enum.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_context.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_logging.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_metrics.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_torch_utils.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/tests/utils/test_wandb.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/.gitignore
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/LICENSE
--rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/README.md
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 careamics-0.1.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/PR_TEMPLATE/pull_request.md
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     5493 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2n/example_SEM_careamist.ipynb
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2n/n2n_2D_SEM.yml
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_careamist.ipynb
+-rw-r--r--   0        0        0     9737 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_lightning.ipynb
+-rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/example_SEM_lightning.ipynb
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/n2v/n2v_2D_BSD.yml
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/2D/pn2v/pN2V_Convallaria.yml
+-rw-r--r--   0        0        0     7882 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/3D/example_flywing_3D.ipynb
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/examples/3D/n2v_flywing_3D.yml
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/__init__.py
+-rw-r--r--   0        0        0    28409 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/careamist.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/conftest.py
+-rw-r--r--   0        0        0    31915 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_datamodule.py
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_module.py
+-rw-r--r--   0        0        0    15364 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_prediction_datamodule.py
+-rw-r--r--   0        0        0     4483 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/lightning_prediction_loop.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/py.typed
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/__init__.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/hyperparameters_callback.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/callbacks/progress_bar_callback.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/algorithm_model.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/callback_model.py
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_example.py
+-rw-r--r--   0        0        0    18793 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_factory.py
+-rw-r--r--   0        0        0    18754 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/configuration_model.py
+-rw-r--r--   0        0        0    16809 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/data_model.py
+-rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/inference_model.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/noise_models.py
+-rw-r--r--   0        0        0     5266 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/optimizer_models.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/tile_information.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/training_model.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/architecture_model.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/custom_model.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/register_model.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/unet_model.py
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/architectures/vae_model.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/__init__.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/algorithm_descriptions.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/references/references.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/__init__.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_activations.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_algorithms.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_architectures.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_data.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_extraction_strategies.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_loggers.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_losses.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_optimizers.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_pixel_manipulations.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_struct_axis.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/support/supported_transforms.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/__init__.py
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/n2v_manipulate_model.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/nd_flip_model.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/normalize_model.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/transform_model.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/transformations/xy_random_rotate90_model.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/validators/__init__.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/config/validators/validator_utils.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/__init__.py
+-rw-r--r--   0        0        0    12213 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/in_memory_dataset.py
+-rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/iterable_dataset.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/zarr_dataset.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/__init__.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/dataset_utils.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/file_utils.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_tiff.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_utils.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_zarr.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/__init__.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/patch_transform.py
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/patching.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/random_patching.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/sequential_patching.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/tiled_patching.py
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/dataset/patching/validate_patch_dimension.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/__init__.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/loss_factory.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/losses.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/noise_model_factory.py
+-rw-r--r--   0        0        0    17801 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/losses/noise_models.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/__init__.py
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bmz_io.py
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/model_io_utils.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/__init__.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/_readme_factory.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/bioimage_utils.py
+-rw-r--r--   0        0        0     9207 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/model_io/bioimage/model_description.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/activation.py
+-rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/layers.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/model_factory.py
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/models/unet.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/prediction/__init__.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/prediction/stitch_prediction.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/__init__.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/n2v_manipulate.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/nd_flip.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/normalize.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/pixel_manipulation.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/struct_mask_parameters.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/tta.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/transforms/xy_random_rotate90.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/__init__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/base_enum.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/context.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/logging.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/metrics.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/path_utils.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/ram.py
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/receptive_field.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/running_stats.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/src/careamics/utils/torch_utils.py
+-rw-r--r--   0        0        0     6602 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/conftest.py
+-rw-r--r--   0        0        0    22382 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_careamist.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_conftest.py
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_datamodule.py
+-rw-r--r--   0        0        0     7262 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_module.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/test_lightning_prediction_datamodule.py
+-rw-r--r--   0        0        0     3208 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_algorithm_model.py
+-rw-r--r--   0        0        0     6483 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_configuration_factory.py
+-rw-r--r--   0        0        0     6180 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_configuration_model.py
+-rw-r--r--   0        0        0    12328 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_data_model.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_full_config_example.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_inference_model.py
+-rw-r--r--   0        0        0     4267 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_optimizers_model.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_tile_information.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/test_training_model.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_architecture_model.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_custom_model.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_register_model.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/architectures/test_unet_model.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/support/test_supported_data.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/support/test_supported_optimizers.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/transformations/test_n2v_manipulate_model.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/transformations/test_normalize_model.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/config/validators/test_validator_utils.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/test_in_memory_dataset.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/test_iterable_dataset.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/dataset_utils/test_list_files.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/dataset_utils/test_read_tiff.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_patching_utils.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_random_patching.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_sequential_patching.py
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/dataset/patching/test_tiled_patching.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/model_io/test_bmz_io.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/models/test_model_factory.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/models/test_unet.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/prediction/test_stitch_prediction.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_manipulate_n2v.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_nd_flip.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_normalize.py
+-rw-r--r--   0        0        0     8954 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_pixel_manipulation.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_supported_transforms.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/transforms/test_xy_random_rotate90.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_base_enum.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_context.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_logging.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_metrics.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_torch_utils.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/tests/utils/test_wandb.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/.gitignore
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/LICENSE
+-rw-r--r--   0        0        0     3011 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/README.md
+-rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     4631 2020-02-02 00:00:00.000000 careamics-0.1.0rc4/PKG-INFO
```

### Comparing `careamics-0.1.0rc3/.pre-commit-config.yaml` & `careamics-0.1.0rc4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/bug_report.md` & `careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/.github/ISSUE_TEMPLATE/feature_request.md` & `careamics-0.1.0rc4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/.github/PR_TEMPLATE/pull_request.md` & `careamics-0.1.0rc4/.github/PR_TEMPLATE/pull_request.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/.github/workflows/ci.yml` & `careamics-0.1.0rc4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2n/example_SEM_careamist.ipynb` & `careamics-0.1.0rc4/examples/2D/n2n/example_SEM_careamist.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2n/n2n_2D_SEM.yml` & `careamics-0.1.0rc4/examples/2D/n2n/n2n_2D_SEM.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_careamist.ipynb` & `careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_careamist.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2v/example_BSD68_lightning.ipynb` & `careamics-0.1.0rc4/examples/2D/n2v/example_BSD68_lightning.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2v/example_SEM_lightning.ipynb` & `careamics-0.1.0rc4/examples/2D/n2v/example_SEM_lightning.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/n2v/n2v_2D_BSD.yml` & `careamics-0.1.0rc4/examples/2D/n2v/n2v_2D_BSD.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/2D/pn2v/pN2V_Convallaria.yml` & `careamics-0.1.0rc4/examples/2D/pn2v/pN2V_Convallaria.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/3D/example_flywing_3D.ipynb` & `careamics-0.1.0rc4/examples/3D/example_flywing_3D.ipynb`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/examples/3D/n2v_flywing_3D.yml` & `careamics-0.1.0rc4/examples/3D/n2v_flywing_3D.yml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/__init__.py` & `careamics-0.1.0rc4/src/careamics/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 try:
     __version__ = version("careamics")
 except PackageNotFoundError:
     __version__ = "uninstalled"
 
 __all__ = [
     "CAREamist",
-    "CAREamicsModule",
+    "CAREamicsModuleWrapper",
+    "CAREamicsPredictData",
+    "CAREamicsTrainData",
     "Configuration",
     "load_configuration",
     "save_configuration",
-    "CAREamicsTrainDataModule",
-    "CAREamicsPredictDataModule",
+    "TrainingDataWrapper",
+    "PredictDataWrapper",
 ]
 
 from .careamist import CAREamist
 from .config import Configuration, load_configuration, save_configuration
-from .lightning_datamodule import CAREamicsTrainDataModule
-from .lightning_module import CAREamicsModule
-from .lightning_prediction_datamodule import CAREamicsPredictDataModule
+from .lightning_datamodule import CAREamicsTrainData, TrainingDataWrapper
+from .lightning_module import CAREamicsModuleWrapper
+from .lightning_prediction_datamodule import CAREamicsPredictData, PredictDataWrapper
```

### Comparing `careamics-0.1.0rc3/src/careamics/careamist.py` & `careamics-0.1.0rc4/src/careamics/careamist.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from careamics.config import (
     Configuration,
     create_inference_configuration,
     load_configuration,
 )
 from careamics.config.inference_model import TRANSFORMS_UNION
 from careamics.config.support import SupportedAlgorithm, SupportedData, SupportedLogger
-from careamics.lightning_datamodule import CAREamicsWood
-from careamics.lightning_module import CAREamicsKiln
-from careamics.lightning_prediction_datamodule import CAREamicsClay
+from careamics.lightning_datamodule import CAREamicsTrainData
+from careamics.lightning_module import CAREamicsModule
+from careamics.lightning_prediction_datamodule import CAREamicsPredictData
 from careamics.lightning_prediction_loop import CAREamicsPredictionLoop
 from careamics.model_io import export_to_bmz, load_pretrained
 from careamics.utils import check_path_exists, get_logger
 
 from .callbacks import HyperParametersCallback
 
 logger = get_logger(__name__)
@@ -136,15 +136,15 @@
             self.work_dir = Path(work_dir)
 
         # configuration object
         if isinstance(source, Configuration):
             self.cfg = source
 
             # instantiate model
-            self.model = CAREamicsKiln(
+            self.model = CAREamicsModule(
                 algorithm_config=self.cfg.algorithm_config,
             )
 
         # path to configuration file or model
         else:
             source = check_path_exists(source)
 
@@ -152,15 +152,15 @@
             if source.is_file() and (
                 source.suffix == ".yaml" or source.suffix == ".yml"
             ):
                 # load configuration
                 self.cfg = load_configuration(source)
 
                 # instantiate model
-                self.model = CAREamicsKiln(
+                self.model = CAREamicsModule(
                     algorithm_config=self.cfg.algorithm_config,
                 )
 
             # attempt loading a pre-trained model
             else:
                 self.model, self.cfg = load_pretrained(source)
 
@@ -189,16 +189,16 @@
             logger=self.experiment_logger,
         )
 
         # change the prediction loop, necessary for tiled prediction
         self.trainer.predict_loop = CAREamicsPredictionLoop(self.trainer)
 
         # place holder for the datamodules
-        self.train_datamodule: Optional[CAREamicsWood] = None
-        self.pred_datamodule: Optional[CAREamicsClay] = None
+        self.train_datamodule: Optional[CAREamicsTrainData] = None
+        self.pred_datamodule: Optional[CAREamicsPredictData] = None
 
     def _define_callbacks(self) -> List[Callback]:
         """
         Define the callbacks for the training loop.
 
         Returns
         -------
@@ -223,15 +223,15 @@
             )
 
         return self.callbacks
 
     def train(
         self,
         *,
-        datamodule: Optional[CAREamicsWood] = None,
+        datamodule: Optional[CAREamicsTrainData] = None,
         train_source: Optional[Union[Path, str, np.ndarray]] = None,
         val_source: Optional[Union[Path, str, np.ndarray]] = None,
         train_target: Optional[Union[Path, str, np.ndarray]] = None,
         val_target: Optional[Union[Path, str, np.ndarray]] = None,
         use_in_memory: bool = True,
         val_percentage: float = 0.1,
         val_minimum_split: int = 1,
@@ -356,15 +356,15 @@
 
             else:
                 raise ValueError(
                     f"Invalid input, expected a str, Path, array or CAREamicsWood "
                     f"instance (got {type(train_source)})."
                 )
 
-    def _train_on_datamodule(self, datamodule: CAREamicsWood) -> None:
+    def _train_on_datamodule(self, datamodule: CAREamicsTrainData) -> None:
         """
         Train the model on the provided datamodule.
 
         Parameters
         ----------
         datamodule : CAREamicsWood
             Datamodule to train on.
@@ -398,15 +398,15 @@
             Validation target data, by default None.
         val_percentage : float, optional
             Percentage of patches to use for validation, by default 0.1.
         val_minimum_split : int, optional
             Minimum number of patches to use for validation, by default 5.
         """
         # create datamodule
-        datamodule = CAREamicsWood(
+        datamodule = CAREamicsTrainData(
             data_config=self.cfg.data_config,
             train_data=train_data,
             val_data=val_data,
             train_data_target=train_target,
             val_data_target=val_target,
             val_percentage=val_percentage,
             val_minimum_split=val_minimum_split,
@@ -454,15 +454,15 @@
         if path_to_train_target is not None:
             path_to_train_target = check_path_exists(path_to_train_target)
 
         if path_to_val_target is not None:
             path_to_val_target = check_path_exists(path_to_val_target)
 
         # create datamodule
-        datamodule = CAREamicsWood(
+        datamodule = CAREamicsTrainData(
             data_config=self.cfg.data_config,
             train_data=path_to_train_data,
             val_data=path_to_val_data,
             train_data_target=path_to_train_target,
             val_data_target=path_to_val_target,
             use_in_memory=use_in_memory,
             val_percentage=val_percentage,
@@ -471,15 +471,15 @@
 
         # train
         self.train(datamodule=datamodule)
 
     @overload
     def predict(  # numpydoc ignore=GL08
         self,
-        source: CAREamicsClay,
+        source: CAREamicsPredictData,
         *,
         checkpoint: Optional[Literal["best", "last"]] = None,
     ) -> Union[list, np.ndarray]:
         ...
 
     @overload
     def predict(  # numpydoc ignore=GL08
@@ -515,15 +515,15 @@
         dataloader_params: Optional[Dict] = None,
         checkpoint: Optional[Literal["best", "last"]] = None,
     ) -> Union[list, np.ndarray]:
         ...
 
     def predict(
         self,
-        source: Union[CAREamicsClay, Path, str, np.ndarray],
+        source: Union[CAREamicsPredictData, Path, str, np.ndarray],
         *,
         batch_size: int = 1,
         tile_size: Optional[Tuple[int, ...]] = None,
         tile_overlap: Tuple[int, ...] = (48, 48),
         axes: Optional[str] = None,
         data_type: Optional[Literal["array", "tiff", "custom"]] = None,
         transforms: Optional[List[TRANSFORMS_UNION]] = None,
@@ -583,15 +583,15 @@
             Predictions made by the model.
 
         Raises
         ------
         ValueError
             If the input is not a CAREamicsClay instance, a path or a numpy array.
         """
-        if isinstance(source, CAREamicsClay):
+        if isinstance(source, CAREamicsPredictData):
             # record datamodule
             self.pred_datamodule = source
 
             return self.trainer.predict(
                 model=self.model, datamodule=source, ckpt_path=checkpoint
             )
         else:
@@ -619,16 +619,16 @@
                 del dataloader_params["batch_size"]
 
             if isinstance(source, Path) or isinstance(source, str):
                 # Check the source
                 source_path = check_path_exists(source)
 
                 # create datamodule
-                datamodule = CAREamicsClay(
-                    prediction_config=prediction_config,
+                datamodule = CAREamicsPredictData(
+                    pred_config=prediction_config,
                     pred_data=source_path,
                     read_source_func=read_source_func,
                     extension_filter=extension_filter,
                     dataloader_params=dataloader_params,
                 )
 
                 # record datamodule
@@ -636,16 +636,16 @@
 
                 return self.trainer.predict(
                     model=self.model, datamodule=datamodule, ckpt_path=checkpoint
                 )
 
             elif isinstance(source, np.ndarray):
                 # create datamodule
-                datamodule = CAREamicsClay(
-                    prediction_config=prediction_config,
+                datamodule = CAREamicsPredictData(
+                    pred_config=prediction_config,
                     pred_data=source,
                     dataloader_params=dataloader_params,
                 )
 
                 # record datamodule
                 self.pred_datamodule = datamodule
```

### Comparing `careamics-0.1.0rc3/src/careamics/conftest.py` & `careamics-0.1.0rc4/src/careamics/conftest.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/lightning_datamodule.py` & `careamics-0.1.0rc4/src/careamics/lightning_datamodule.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+"""Training and validation Lightning data modules."""
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 import numpy as np
 import pytorch_lightning as L
 from albumentations import Compose
 from torch.utils.data import DataLoader
 
-from careamics.config import DataModel
+from careamics.config import DataConfig
 from careamics.config.data_model import TRANSFORMS_UNION
 from careamics.config.support import SupportedData
 from careamics.dataset.dataset_utils import (
     get_files_size,
     get_read_func,
     list_files,
     validate_source_target_files,
@@ -24,17 +25,17 @@
 from careamics.utils import get_logger, get_ram_size
 
 DatasetType = Union[InMemoryDataset, PathIterableDataset]
 
 logger = get_logger(__name__)
 
 
-class CAREamicsWood(L.LightningDataModule):
+class CAREamicsTrainData(L.LightningDataModule):
     """
-    LightningDataModule for training and validation datasets.
+    CAREamics Ligthning training and validation data module.
 
     The data module can be used with Path, str or numpy arrays. In the case of
     numpy arrays, it loads and computes all the patches in memory. For Path and str
     inputs, it calculates the total file size and estimate whether it can fit in
     memory. If it does not, it iterates through the files. This behaviour can be
     deactivated by setting `use_in_memory` to False, in which case it will
     always use the iterating dataset to train on a Path or str.
@@ -49,19 +50,78 @@
     To read custom data types, you can set `data_type` to `custom` in `data_config`
     and provide a function that returns a numpy array from a path as
     `read_source_func` parameter. The function will receive a Path object and
     an axies string as arguments, the axes being derived from the `data_config`.
 
     You can also provide a `fnmatch` and `Path.rglob` compatible expression (e.g.
     "*.czi") to filter the files extension using `extension_filter`.
+
+    Parameters
+    ----------
+    data_config : DataModel
+        Pydantic model for CAREamics data configuration.
+    train_data : Union[Path, str, np.ndarray]
+        Training data, can be a path to a folder, a file or a numpy array.
+    val_data : Optional[Union[Path, str, np.ndarray]], optional
+        Validation data, can be a path to a folder, a file or a numpy array, by
+        default None.
+    train_data_target : Optional[Union[Path, str, np.ndarray]], optional
+        Training target data, can be a path to a folder, a file or a numpy array, by
+        default None.
+    val_data_target : Optional[Union[Path, str, np.ndarray]], optional
+        Validation target data, can be a path to a folder, a file or a numpy array,
+        by default None.
+    read_source_func : Optional[Callable], optional
+        Function to read the source data, by default None. Only used for `custom`
+        data type (see DataModel).
+    extension_filter : str, optional
+        Filter for file extensions, by default "". Only used for `custom` data types
+        (see DataModel).
+    val_percentage : float, optional
+        Percentage of the training data to use for validation, by default 0.1. Only
+        used if `val_data` is None.
+    val_minimum_split : int, optional
+        Minimum number of patches or files to split from the training data for
+        validation, by default 5. Only used if `val_data` is None.
+    use_in_memory : bool, optional
+        Use in memory dataset if possible, by default True.
+
+    Attributes
+    ----------
+    data_config : DataModel
+        CAREamics data configuration.
+    data_type : SupportedData
+        Expected data type, one of "tiff", "array" or "custom".
+    batch_size : int
+        Batch size.
+    use_in_memory : bool
+        Whether to use in memory dataset if possible.
+    train_data : Union[Path, str, np.ndarray]
+        Training data.
+    val_data : Optional[Union[Path, str, np.ndarray]]
+        Validation data.
+    train_data_target : Optional[Union[Path, str, np.ndarray]]
+        Training target data.
+    val_data_target : Optional[Union[Path, str, np.ndarray]]
+        Validation target data.
+    val_percentage : float
+        Percentage of the training data to use for validation, if no validation data is
+        provided.
+    val_minimum_split : int
+        Minimum number of patches or files to split from the training data for
+        validation, if no validation data is provided.
+    read_source_func : Optional[Callable]
+        Function to read the source data, used if `data_type` is `custom`.
+    extension_filter : str
+        Filter for file extensions, used if `data_type` is `custom`.
     """
 
     def __init__(
         self,
-        data_config: DataModel,
+        data_config: DataConfig,
         train_data: Union[Path, str, np.ndarray],
         val_data: Optional[Union[Path, str, np.ndarray]] = None,
         train_data_target: Optional[Union[Path, str, np.ndarray]] = None,
         val_data_target: Optional[Union[Path, str, np.ndarray]] = None,
         read_source_func: Optional[Callable] = None,
         extension_filter: str = "",
         val_percentage: float = 0.1,
@@ -94,14 +154,16 @@
             (see DataModel).
         val_percentage : float, optional
             Percentage of the training data to use for validation, by default 0.1. Only
             used if `val_data` is None.
         val_minimum_split : int, optional
             Minimum number of patches or files to split from the training data for
             validation, by default 5. Only used if `val_data` is None.
+        use_in_memory : bool, optional
+            Use in memory dataset if possible, by default True.
 
         Raises
         ------
         NotImplementedError
             Raised if target data is provided.
         ValueError
             If the input types are mixed (e.g. Path and np.ndarray).
@@ -124,33 +186,38 @@
                 f"{types_set}."
             )
 
         # check that a read source function is provided for custom types
         if data_config.data_type == SupportedData.CUSTOM and read_source_func is None:
             raise ValueError(
                 f"Data type {SupportedData.CUSTOM} is not allowed without "
-                f"specifying a `read_source_func`."
+                f"specifying a `read_source_func` and an `extension_filer`."
             )
 
-        # and that arrays are passed, if array type specified
-        elif data_config.data_type == SupportedData.ARRAY and not isinstance(
-            train_data, np.ndarray
+        # check correct input type
+        if (
+            isinstance(train_data, np.ndarray)
+            and data_config.data_type != SupportedData.ARRAY
         ):
             raise ValueError(
-                f"Expected array input (see configuration.data.data_type), but got "
-                f"{type(train_data)} instead."
+                f"Received a numpy array as input, but the data type was set to "
+                f"{data_config.data_type}. Set the data type in the configuration "
+                f"to {SupportedData.ARRAY} to train on numpy arrays."
             )
 
         # and that Path or str are passed, if tiff file type specified
-        elif data_config.data_type == SupportedData.TIFF and (
-            not isinstance(train_data, Path) and not isinstance(train_data, str)
+        elif (isinstance(train_data, Path) or isinstance(train_data, str)) and (
+            data_config.data_type != SupportedData.TIFF
+            and data_config.data_type != SupportedData.CUSTOM
         ):
             raise ValueError(
-                f"Expected Path or str input (see configuration.data.data_type), "
-                f"but got {type(train_data)} instead."
+                f"Received a path as input, but the data type was neither set to "
+                f"{SupportedData.TIFF} nor {SupportedData.CUSTOM}. Set the data type "
+                f"in the configuration to {SupportedData.TIFF} or "
+                f"{SupportedData.CUSTOM} to train on files."
             )
 
         # configuration
         self.data_config = data_config
         self.data_type = data_config.data_type
         self.batch_size = data_config.batch_size
         self.use_in_memory = use_in_memory
@@ -227,15 +294,23 @@
                     self.val_data_target, self.data_type, self.extension_filter
                 )
 
                 # verify that they match the validation data
                 validate_source_target_files(self.val_files, self.val_target_files)
 
     def setup(self, *args: Any, **kwargs: Any) -> None:
-        """Hook called at the beginning of fit, validate, or predict."""
+        """Hook called at the beginning of fit, validate, or predict.
+
+        Parameters
+        ----------
+        *args : Any
+            Unused.
+        **kwargs : Any
+            Unused.
+        """
         # if numpy array
         if self.data_type == SupportedData.ARRAY:
             # train dataset
             self.train_dataset: DatasetType = InMemoryDataset(
                 data_config=self.data_config,
                 inputs=self.train_data,
                 data_target=self.train_data_target,
@@ -349,17 +424,20 @@
         """
         return DataLoader(
             self.val_dataset,
             batch_size=self.batch_size,
         )
 
 
-class CAREamicsTrainDataModule(CAREamicsWood):
+class TrainingDataWrapper(CAREamicsTrainData):
     """
-    LightningDataModule wrapper for training and validation datasets.
+    Wrapper around the CAREamics Lightning training data module.
+
+    This class is used to explicitely pass the parameters usually contained in a
+    `data_model` configuration.
 
     Since the lightning datamodule has no access to the model, make sure that the
     parameters passed to the datamodule are consistent with the model's requirements and
     are coherent.
 
     The data module can be used with Path, str or numpy arrays. In the case of
     numpy arrays, it loads and computes all the patches in memory. For Path and str
@@ -438,61 +516,61 @@
         Axis for the structN2V mask, only applied if `struct_n2v_axis` is `none`, by
         default "none".
     struct_n2v_span : int, optional
         Span for the structN2V mask, by default 5.
 
     Examples
     --------
-    Create a CAREamicsTrainDataModule with default transforms with a numpy array:
+    Create a TrainingDataWrapper with default transforms with a numpy array:
     >>> import numpy as np
-    >>> from careamics import CAREamicsTrainDataModule
+    >>> from careamics import TrainingDataWrapper
     >>> my_array = np.arange(256).reshape(16, 16)
-    >>> data_module = CAREamicsTrainDataModule(
+    >>> data_module = TrainingDataWrapper(
     ...     train_data=my_array,
     ...     data_type="array",
     ...     patch_size=(8, 8),
     ...     axes='YX',
     ...     batch_size=2,
     ... )
 
     For custom data types (those not supported by CAREamics), then one can pass a read
     function and a filter for the files extension:
     >>> import numpy as np
-    >>> from careamics import CAREamicsTrainDataModule
+    >>> from careamics import TrainingDataWrapper
     >>>
     >>> def read_npy(path):
     ...     return np.load(path)
     >>>
-    >>> data_module = CAREamicsTrainDataModule(
+    >>> data_module = TrainingDataWrapper(
     ...     train_data="path/to/data",
     ...     data_type="custom",
     ...     patch_size=(8, 8),
     ...     axes='YX',
     ...     batch_size=2,
     ...     read_source_func=read_npy,
     ...     extension_filter="*.npy",
     ... )
 
     If you want to use a different set of transformations, you can pass a list of
     transforms:
     >>> import numpy as np
-    >>> from careamics import CAREamicsTrainDataModule
+    >>> from careamics import TrainingDataWrapper
     >>> from careamics.config.support import SupportedTransform
     >>> my_array = np.arange(256).reshape(16, 16)
     >>> my_transforms = [
     ...     {
     ...         "name": SupportedTransform.NORMALIZE.value,
     ...         "mean": 0,
     ...         "std": 1,
     ...     },
     ...     {
     ...         "name": SupportedTransform.N2V_MANIPULATE.value,
     ...     }
     ... ]
-    >>> data_module = CAREamicsTrainDataModule(
+    >>> data_module = TrainingDataWrapper(
     ...     train_data=my_array,
     ...     data_type="array",
     ...     patch_size=(8, 8),
     ...     axes='YX',
     ...     batch_size=2,
     ...     transforms=my_transforms,
     ... )
@@ -624,15 +702,15 @@
         }
 
         # if transforms are passed (otherwise it will use the default ones)
         if transforms is not None:
             data_dict["transforms"] = transforms
 
         # validate configuration
-        self.data_config = DataModel(**data_dict)
+        self.data_config = DataConfig(**data_dict)
 
         # N2V specific checks, N2V, structN2V, and transforms
         if (
             self.data_config.has_transform_list()
             and self.data_config.has_n2v_manipulate()
         ):
             # there is not target, n2v2 and structN2V can be changed
```

### Comparing `careamics-0.1.0rc3/src/careamics/lightning_module.py` & `careamics-0.1.0rc4/src/careamics/lightning_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, Optional, Union
 
 import pytorch_lightning as L
 from torch import Tensor, nn
 
-from careamics.config import AlgorithmModel
+from careamics.config import AlgorithmConfig
 from careamics.config.support import (
     SupportedAlgorithm,
     SupportedArchitecture,
     SupportedLoss,
     SupportedOptimizer,
     SupportedScheduler,
 )
 from careamics.losses import loss_factory
 from careamics.models.model_factory import model_factory
 from careamics.transforms import Denormalize, ImageRestorationTTA
 from careamics.utils.torch_utils import get_optimizer, get_scheduler
 
 
-class CAREamicsKiln(L.LightningModule):
+class CAREamicsModule(L.LightningModule):
     """
     CAREamics Lightning module.
 
     This class encapsulates the a PyTorch model along with the training, validation,
     and testing logic. It is configured using an `AlgorithmModel` Pydantic class.
 
     Attributes
@@ -34,30 +34,30 @@
         Optimizer name.
     optimizer_params : dict
         Optimizer parameters.
     lr_scheduler_name : str
         Learning rate scheduler name.
     """
 
-    def __init__(self, algorithm_config: Union[AlgorithmModel, dict]) -> None:
+    def __init__(self, algorithm_config: Union[AlgorithmConfig, dict]) -> None:
         """
         CAREamics Lightning module.
 
         This class encapsulates the a PyTorch model along with the training, validation,
         and testing logic. It is configured using an `AlgorithmModel` Pydantic class.
 
         Parameters
         ----------
         algorithm_config : Union[AlgorithmModel, dict]
             Algorithm configuration.
         """
         super().__init__()
         # if loading from a checkpoint, AlgorithmModel needs to be instantiated
         if isinstance(algorithm_config, dict):
-            algorithm_config = AlgorithmModel(**algorithm_config)
+            algorithm_config = AlgorithmConfig(**algorithm_config)
 
         # create model and loss function
         self.model: nn.Module = model_factory(algorithm_config.model)
         self.loss_func = loss_factory(algorithm_config.loss)
 
         # save optimizer and lr_scheduler names and parameters
         self.optimizer_name = algorithm_config.optimizer.name
@@ -188,15 +188,15 @@
         return {
             "optimizer": optimizer,
             "lr_scheduler": scheduler,
             "monitor": "val_loss",  # otherwise triggers MisconfigurationException
         }
 
 
-class CAREamicsModule(CAREamicsKiln):
+class CAREamicsModuleWrapper(CAREamicsModule):
     """Class defining the API for CAREamics Lightning layer.
 
     This class exposes parameters used to create an AlgorithmModel instance, triggering
     parameters validation.
 
     Parameters
     ----------
@@ -283,10 +283,10 @@
         model_configuration = {"architecture": architecture}
         model_configuration.update(model_parameters)
 
         # add model parameters to algorithm configuration
         algorithm_configuration["model"] = model_configuration
 
         # call the parent init using an AlgorithmModel instance
-        super().__init__(AlgorithmModel(**algorithm_configuration))
+        super().__init__(AlgorithmConfig(**algorithm_configuration))
 
         # TODO add load_from_checkpoint wrapper
```

### Comparing `careamics-0.1.0rc3/src/careamics/lightning_prediction_datamodule.py` & `careamics-0.1.0rc4/src/careamics/lightning_prediction_datamodule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+"""Prediction Lightning data modules."""
 from pathlib import Path
 from typing import Any, Callable, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pytorch_lightning as L
 from albumentations import Compose
 from torch.utils.data import DataLoader
 from torch.utils.data.dataloader import default_collate
 
-from careamics.config import InferenceModel
+from careamics.config import InferenceConfig
 from careamics.config.support import SupportedData
 from careamics.config.tile_information import TileInformation
 from careamics.dataset.dataset_utils import (
     get_read_func,
     list_files,
 )
 from careamics.dataset.in_memory_dataset import (
@@ -58,46 +59,46 @@
             (tile, t.last_tile, t.array_shape, t.overlap_crop_coords, t.stitch_coords)
             for tile, t in batch
         ]
 
         return default_collate(new_batch)
 
 
-class CAREamicsClay(L.LightningDataModule):
+class CAREamicsPredictData(L.LightningDataModule):
     """
-    LightningDataModule for prediction dataset.
+    CAREamics Lightning prediction data module.
 
     The data module can be used with Path, str or numpy arrays. The data can be either
     a folder containing images or a single file.
 
     To read custom data types, you can set `data_type` to `custom` in `data_config`
     and provide a function that returns a numpy array from a path as
     `read_source_func` parameter. The function will receive a Path object and
     an axies string as arguments, the axes being derived from the `data_config`.
 
     You can also provide a `fnmatch` and `Path.rglob` compatible expression (e.g.
     "*.czi") to filter the files extension using `extension_filter`.
 
     Parameters
     ----------
-    prediction_config : InferenceModel
+    pred_config : InferenceModel
         Pydantic model for CAREamics prediction configuration.
     pred_data : Union[Path, str, np.ndarray]
         Prediction data, can be a path to a folder, a file or a numpy array.
     read_source_func : Optional[Callable], optional
         Function to read custom types, by default None.
     extension_filter : str, optional
         Filter to filter file extensions for custom types, by default "".
     dataloader_params : dict, optional
         Dataloader parameters, by default {}.
     """
 
     def __init__(
         self,
-        prediction_config: InferenceModel,
+        pred_config: InferenceConfig,
         pred_data: Union[Path, str, np.ndarray],
         read_source_func: Optional[Callable] = None,
         extension_filter: str = "",
         dataloader_params: Optional[dict] = None,
     ) -> None:
         """
         Constructor.
@@ -111,15 +112,15 @@
         an axies string as arguments, the axes being derived from the `data_config`.
 
         You can also provide a `fnmatch` and `Path.rglob` compatible expression (e.g.
         "*.czi") to filter the files extension using `extension_filter`.
 
         Parameters
         ----------
-        prediction_config : InferenceModel
+        pred_config : InferenceModel
             Pydantic model for CAREamics prediction configuration.
         pred_data : Union[Path, str, np.ndarray]
             Prediction data, can be a path to a folder, a file or a numpy array.
         read_source_func : Optional[Callable], optional
             Function to read custom types, by default None.
         extension_filter : str, optional
             Filter to filter file extensions for custom types, by default "".
@@ -138,59 +139,61 @@
         if dataloader_params is None:
             dataloader_params = {}
         if dataloader_params is None:
             dataloader_params = {}
         super().__init__()
 
         # check that a read source function is provided for custom types
-        if (
-            prediction_config.data_type == SupportedData.CUSTOM
-            and read_source_func is None
-        ):
+        if pred_config.data_type == SupportedData.CUSTOM and read_source_func is None:
             raise ValueError(
                 f"Data type {SupportedData.CUSTOM} is not allowed without "
-                f"specifying a `read_source_func`."
+                f"specifying a `read_source_func` and an `extension_filer`."
             )
 
-        # and that arrays are passed, if array type specified
-        elif prediction_config.data_type == SupportedData.ARRAY and not isinstance(
-            pred_data, np.ndarray
+        # check correct input type
+        if (
+            isinstance(pred_data, np.ndarray)
+            and pred_config.data_type != SupportedData.ARRAY
         ):
             raise ValueError(
-                f"Expected array input (see configuration.data.data_type), but got "
-                f"{type(pred_data)} instead."
+                f"Received a numpy array as input, but the data type was set to "
+                f"{pred_config.data_type}. Set the data type "
+                f"to {SupportedData.ARRAY} to predict on numpy arrays."
             )
 
         # and that Path or str are passed, if tiff file type specified
-        elif prediction_config.data_type == SupportedData.TIFF and not (
-            isinstance(pred_data, Path) or isinstance(pred_data, str)
+        elif (isinstance(pred_data, Path) or isinstance(pred_config, str)) and (
+            pred_config.data_type != SupportedData.TIFF
+            and pred_config.data_type != SupportedData.CUSTOM
         ):
             raise ValueError(
-                f"Expected Path or str input (see configuration.data.data_type), "
-                f"but got {type(pred_data)} instead."
+                f"Received a path as input, but the data type was neither set to "
+                f"{SupportedData.TIFF} nor {SupportedData.CUSTOM}. Set the data type "
+                f" to {SupportedData.TIFF} or "
+                f"{SupportedData.CUSTOM} to predict on files."
             )
 
         # configuration data
-        self.prediction_config = prediction_config
-        self.data_type = prediction_config.data_type
-        self.batch_size = prediction_config.batch_size
+        self.prediction_config = pred_config
+        self.data_type = pred_config.data_type
+        self.batch_size = pred_config.batch_size
         self.dataloader_params = dataloader_params
 
         self.pred_data = pred_data
-        self.tile_size = prediction_config.tile_size
-        self.tile_overlap = prediction_config.tile_overlap
+        self.tile_size = pred_config.tile_size
+        self.tile_overlap = pred_config.tile_overlap
 
         # read source function
-        if prediction_config.data_type == SupportedData.CUSTOM:
+        if pred_config.data_type == SupportedData.CUSTOM:
             # mypy check
             assert read_source_func is not None
 
             self.read_source_func: Callable = read_source_func
-        elif prediction_config.data_type != SupportedData.ARRAY:
-            self.read_source_func = get_read_func(prediction_config.data_type)
+        elif pred_config.data_type != SupportedData.ARRAY:
+            self.read_source_func = get_read_func(pred_config.data_type)
 
         self.extension_filter = extension_filter
 
     def prepare_data(self) -> None:
         """Hook used to prepare the data before calling `setup`."""
         # if the data is a Path or a str
         if not isinstance(self.pred_data, np.ndarray):
@@ -234,17 +237,20 @@
             self.predict_dataset,
             batch_size=self.batch_size,
             collate_fn=_collate_tiles,
             **self.dataloader_params,
         )  # TODO check workers are used
 
 
-class CAREamicsPredictDataModule(CAREamicsClay):
+class PredictDataWrapper(CAREamicsPredictData):
     """
-    LightningDataModule wrapper of an inference dataset.
+    Wrapper around the CAREamics inference Lightning data module.
+
+    This class is used to explicitely pass the parameters usually contained in a
+    `inference_model` configuration.
 
     Since the lightning datamodule has no access to the model, make sure that the
     parameters passed to the datamodule are consistent with the model's requirements
     and are coherent.
 
     The data module can be used with Path, str or numpy arrays. To use array data, set
     `data_type` to `array` and pass a numpy array to `train_data`.
@@ -325,30 +331,30 @@
 
         Parameters
         ----------
         pred_data : Union[str, Path, np.ndarray]
             Prediction data.
         data_type : Union[Literal["array", "tiff", "custom"], SupportedData]
             Data type, see `SupportedData` for available options.
+        mean : float
+            Mean value for normalization, only used if Normalization is defined in the
+            transforms.
+        std : float
+            Standard deviation value for normalization, only used if Normalization is
+            defined in the transform.
         tile_size : List[int]
             Tile size, 2D or 3D tile size.
         tile_overlap : List[int]
             Tile overlap, 2D or 3D tile overlap.
         axes : str
             Axes of the data, choosen amongst SCZYX.
         batch_size : int
             Batch size.
         tta_transforms : bool, optional
             Use test time augmentation, by default True.
-        mean : Optional[float], optional
-            Mean value for normalization, only used if Normalization is defined, by
-            default None.
-        std : Optional[float], optional
-            Standard deviation value for normalization, only used if Normalization is
-            defined, by default None.
         transforms : Optional[Union[List[TRANSFORMS_UNION], Compose]], optional
             List of transforms to apply to prediction patches. If None, default
             transforms are applied.
         read_source_func : Optional[Callable], optional
             Function to read the source data, used if `data_type` is `custom`, by
             default None.
         extension_filter : str, optional
@@ -370,21 +376,21 @@
         }
 
         # if transforms are passed (otherwise it will use the default ones)
         if transforms is not None:
             prediction_dict["transforms"] = transforms
 
         # validate configuration
-        self.prediction_config = InferenceModel(**prediction_dict)
+        self.prediction_config = InferenceConfig(**prediction_dict)
 
         # sanity check on the dataloader parameters
         if "batch_size" in dataloader_params:
             # remove it
             del dataloader_params["batch_size"]
 
         super().__init__(
-            prediction_config=self.prediction_config,
+            pred_config=self.prediction_config,
             pred_data=pred_data,
             read_source_func=read_source_func,
             extension_filter=extension_filter,
             dataloader_params=dataloader_params,
         )
```

### Comparing `careamics-0.1.0rc3/src/careamics/lightning_prediction_loop.py` & `careamics-0.1.0rc4/src/careamics/lightning_prediction_loop.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/callbacks/hyperparameters_callback.py` & `careamics-0.1.0rc4/src/careamics/callbacks/hyperparameters_callback.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/callbacks/progress_bar_callback.py` & `careamics-0.1.0rc4/src/careamics/callbacks/progress_bar_callback.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/__init__.py` & `careamics-0.1.0rc4/src/careamics/config/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """Configuration module."""
 
 
 __all__ = [
-    "AlgorithmModel",
-    "DataModel",
+    "AlgorithmConfig",
+    "DataConfig",
     "Configuration",
     "CheckpointModel",
-    "InferenceModel",
+    "InferenceConfig",
     "load_configuration",
     "save_configuration",
-    "TrainingModel",
+    "TrainingConfig",
     "create_n2v_configuration",
+    "create_n2n_configuration",
+    "create_care_configuration",
     "register_model",
     "CustomModel",
     "create_inference_configuration",
     "clear_custom_models",
     "ConfigurationInformation",
 ]
 
-from .algorithm_model import AlgorithmModel
+from .algorithm_model import AlgorithmConfig
 from .architectures import CustomModel, clear_custom_models, register_model
 from .callback_model import CheckpointModel
 from .configuration_factory import (
+    create_care_configuration,
     create_inference_configuration,
+    create_n2n_configuration,
     create_n2v_configuration,
 )
 from .configuration_model import (
     Configuration,
     load_configuration,
     save_configuration,
 )
-from .data_model import DataModel
-from .inference_model import InferenceModel
-from .training_model import TrainingModel
+from .data_model import DataConfig
+from .inference_model import InferenceConfig
+from .training_model import TrainingConfig
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/algorithm_model.py` & `careamics-0.1.0rc4/src/careamics/config/algorithm_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 from typing_extensions import Self
 
 from .architectures import CustomModel, UNetModel, VAEModel
 from .optimizer_models import LrSchedulerModel, OptimizerModel
 
 
-class AlgorithmModel(BaseModel):
+class AlgorithmConfig(BaseModel):
     """Algorithm configuration.
 
     This Pydantic model validates the parameters governing the components of the
     training algorithm: which algorithm, loss function, model architecture, optimizer,
     and learning rate scheduler to use.
 
     Currently, we only support N2V and custom algorithms. The `n2v` algorithm is only
@@ -41,27 +41,27 @@
         Algorithm parameter type validation errors.
     ValueError
         If the algorithm, loss and model are not compatible.
 
     Examples
     --------
     Minimum example:
-    >>> from careamics.config import AlgorithmModel
+    >>> from careamics.config import AlgorithmConfig
     >>> config_dict = {
     ...     "algorithm": "n2v",
     ...     "loss": "n2v",
     ...     "model": {
     ...         "architecture": "UNet",
     ...     }
     ... }
-    >>> config = AlgorithmModel(**config_dict)
+    >>> config = AlgorithmConfig(**config_dict)
 
     Using a custom model:
     >>> from torch import nn, ones
-    >>> from careamics.config import AlgorithmModel, register_model
+    >>> from careamics.config import AlgorithmConfig, register_model
     ...
     >>> @register_model(name="linear_model")
     ... class LinearModel(nn.Module):
     ...    def __init__(self, in_features, out_features, *args, **kwargs):
     ...        super().__init__()
     ...        self.in_features = in_features
     ...        self.out_features = out_features
@@ -76,15 +76,15 @@
     ...     "model": {
     ...         "architecture": "Custom",
     ...         "name": "linear_model",
     ...         "in_features": 10,
     ...         "out_features": 5,
     ...     }
     ... }
-    >>> config = AlgorithmModel(**config_dict)
+    >>> config = AlgorithmConfig(**config_dict)
     """
 
     # Pydantic class configuration
     model_config = ConfigDict(
         protected_namespaces=(),  # allows to use model_* as a field name
         validate_assignment=True,
     )
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/callback_model.py` & `careamics-0.1.0rc4/src/careamics/config/callback_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/configuration_factory.py` & `careamics-0.1.0rc4/src/careamics/config/configuration_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,111 +1,105 @@
 """Convenience functions to create configurations for training and inference."""
 
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 from albumentations import Compose
 
-from .algorithm_model import AlgorithmModel
+from .algorithm_model import AlgorithmConfig
 from .architectures import UNetModel
 from .configuration_model import Configuration
-from .data_model import DataModel
-from .inference_model import InferenceModel
+from .data_model import DataConfig
+from .inference_model import InferenceConfig
 from .support import (
     SupportedAlgorithm,
     SupportedArchitecture,
     SupportedLoss,
     SupportedPixelManipulation,
     SupportedTransform,
 )
-from .training_model import TrainingModel
+from .training_model import TrainingConfig
 
 
-def create_n2n_configuration(
+def _create_supervised_configuration(
+    algorithm: Literal["care", "n2n"],
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
-    use_n2v2: bool = False,
-    n_channels: int = 1,
+    loss: Literal["mae", "mse"] = "mae",
+    n_channels: int = -1,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
     model_kwargs: Optional[dict] = None,
 ) -> Configuration:
     """
-    Create a configuration for training N2V.
-
-    If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
-    2.
-
-    By setting `use_augmentations` to False, the only transformation applied will be
-    normalization and N2V manipulation.
-
-    The parameter `use_n2v2` overrides the corresponding `n2v2` that can be passed
-    in `model_kwargs`.
-
-    If you pass "horizontal" or "vertical" to `struct_n2v_axis`, then structN2V mask
-    will be applied to each manipulated pixel.
+    Create a configuration for training CARE or Noise2Noise.
 
     Parameters
     ----------
+    algorithm : Literal["care", "n2n"]
+        Algorithm to use.
     experiment_name : str
         Name of the experiment.
     data_type : Literal["array", "tiff", "custom"]
         Type of the data.
     axes : str
         Axes of the data (e.g. SYX).
     patch_size : List[int]
         Size of the patches along the spatial dimensions (e.g. [64, 64]).
     batch_size : int
         Batch size.
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
-    use_n2v2 : bool, optional
-        Whether to use N2V2, by default False.
+    loss : Literal["mae", "mse"], optional
+        Loss function to use, by default "mae".
     n_channels : int, optional
-        Number of channels (in and out), by default 1.
-    roi_size : int, optional
-        N2V pixel manipulation area, by default 11.
-    masked_pixel_percentage : float, optional
-        Percentage of pixels masked in each patch, by default 0.2.
-    struct_n2v_axis : Literal["horizontal", "vertical", "none"], optional
-        Axis along which to apply structN2V mask, by default "none".
-    struct_n2v_span : int, optional
-        Span of the structN2V mask, by default 5.
+        Number of channels (in and out), by default -1.
     logger : Literal["wandb", "tensorboard", "none"], optional
         Logger to use, by default "none".
     model_kwargs : dict, optional
         UNetModel parameters, by default {}.
 
     Returns
     -------
     Configuration
-        Configuration for training N2V.
+        Configuration for training CARE or Noise2Noise.
     """
+    # if there are channels, we need to specify their number
+    if "C" in axes and n_channels == 1:
+        raise ValueError(
+            f"Number of channels must be specified when using channels "
+            f"(got {n_channels} channel)."
+        )
+    elif "C" not in axes and n_channels > 1:
+        raise ValueError(
+            f"C is not present in the axes, but number of channels is specified "
+            f"(got {n_channels} channel)."
+        )
+
     # model
     if model_kwargs is None:
         model_kwargs = {}
-    model_kwargs["n2v2"] = use_n2v2
     model_kwargs["conv_dims"] = 3 if "Z" in axes else 2
     model_kwargs["in_channels"] = n_channels
     model_kwargs["num_classes"] = n_channels
 
     unet_model = UNetModel(
         architecture=SupportedArchitecture.UNET.value,
         **model_kwargs,
     )
 
     # algorithm model
-    algorithm = AlgorithmModel(
-        algorithm=SupportedAlgorithm.N2V.value,
-        loss=SupportedLoss.N2V.value,
+    algorithm = AlgorithmConfig(
+        algorithm=algorithm,
+        loss=loss,
         model=unet_model,
     )
 
     # augmentations
     if use_augmentations:
         transforms: List[Dict[str, Any]] = [
             {
@@ -122,24 +116,24 @@
         transforms = [
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
         ]
 
     # data model
-    data = DataModel(
+    data = DataConfig(
         data_type=data_type,
         axes=axes,
         patch_size=patch_size,
         batch_size=batch_size,
         transforms=transforms,
     )
 
     # training model
-    training = TrainingModel(
+    training = TrainingConfig(
         num_epochs=num_epochs,
         batch_size=batch_size,
         logger=None if logger == "none" else logger,
     )
 
     # create configuration
     configuration = Configuration(
@@ -148,33 +142,178 @@
         data_config=data,
         training_config=training,
     )
 
     return configuration
 
 
+def create_care_configuration(
+    experiment_name: str,
+    data_type: Literal["array", "tiff", "custom"],
+    axes: str,
+    patch_size: List[int],
+    batch_size: int,
+    num_epochs: int,
+    use_augmentations: bool = True,
+    loss: Literal["mae", "mse"] = "mae",
+    n_channels: int = 1,
+    logger: Literal["wandb", "tensorboard", "none"] = "none",
+    model_kwargs: Optional[dict] = None,
+) -> Configuration:
+    """
+    Create a configuration for training CARE.
+
+    If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
+    2.
+
+    If "C" is present in `axes`, then you need to set `n_channels` to the number of
+    channels. Likewise, if you set the number of channels, then "C" must be present in
+    `axes`.
+
+    By setting `use_augmentations` to False, the only transformation applied will be
+    normalization.
+
+    Parameters
+    ----------
+    experiment_name : str
+        Name of the experiment.
+    data_type : Literal["array", "tiff", "custom"]
+        Type of the data.
+    axes : str
+        Axes of the data (e.g. SYX).
+    patch_size : List[int]
+        Size of the patches along the spatial dimensions (e.g. [64, 64]).
+    batch_size : int
+        Batch size.
+    num_epochs : int
+        Number of epochs.
+    use_augmentations : bool, optional
+        Whether to use augmentations, by default True.
+    loss : Literal["mae", "mse"], optional
+        Loss function to use, by default "mae".
+    n_channels : int, optional
+        Number of channels (in and out), by default 1.
+    logger : Literal["wandb", "tensorboard", "none"], optional
+        Logger to use, by default "none".
+    model_kwargs : dict, optional
+        UNetModel parameters, by default {}.
+
+    Returns
+    -------
+    Configuration
+        Configuration for training CARE.
+    """
+    return _create_supervised_configuration(
+        algorithm="care",
+        experiment_name=experiment_name,
+        data_type=data_type,
+        axes=axes,
+        patch_size=patch_size,
+        batch_size=batch_size,
+        num_epochs=num_epochs,
+        use_augmentations=use_augmentations,
+        loss=loss,
+        # TODO in the future we might support different in and out channels for CARE
+        n_channels=n_channels,
+        logger=logger,
+        model_kwargs=model_kwargs,
+    )
+
+
+def create_n2n_configuration(
+    experiment_name: str,
+    data_type: Literal["array", "tiff", "custom"],
+    axes: str,
+    patch_size: List[int],
+    batch_size: int,
+    num_epochs: int,
+    use_augmentations: bool = True,
+    loss: Literal["mae", "mse"] = "mae",
+    n_channels: int = 1,
+    logger: Literal["wandb", "tensorboard", "none"] = "none",
+    model_kwargs: Optional[dict] = None,
+) -> Configuration:
+    """
+    Create a configuration for training Noise2Noise.
+
+    If "Z" is present in `axes`, then `path_size` must be a list of length 3, otherwise
+    2.
+
+    If "C" is present in `axes`, then you need to set `n_channels` to the number of
+    channels. Likewise, if you set the number of channels, then "C" must be present in
+    `axes`.
+
+    By setting `use_augmentations` to False, the only transformation applied will be
+    normalization.
+
+    Parameters
+    ----------
+    experiment_name : str
+        Name of the experiment.
+    data_type : Literal["array", "tiff", "custom"]
+        Type of the data.
+    axes : str
+        Axes of the data (e.g. SYX).
+    patch_size : List[int]
+        Size of the patches along the spatial dimensions (e.g. [64, 64]).
+    batch_size : int
+        Batch size.
+    num_epochs : int
+        Number of epochs.
+    use_augmentations : bool, optional
+        Whether to use augmentations, by default True.
+    loss : Literal["mae", "mse"], optional
+        Loss function to use, by default "mae".
+    n_channels : int, optional
+        Number of channels (in and out), by default 1.
+    logger : Literal["wandb", "tensorboard", "none"], optional
+        Logger to use, by default "none".
+    model_kwargs : dict, optional
+        UNetModel parameters, by default {}.
+
+    Returns
+    -------
+    Configuration
+        Configuration for training Noise2Noise.
+    """
+    return _create_supervised_configuration(
+        algorithm="n2n",
+        experiment_name=experiment_name,
+        data_type=data_type,
+        axes=axes,
+        patch_size=patch_size,
+        batch_size=batch_size,
+        num_epochs=num_epochs,
+        use_augmentations=use_augmentations,
+        loss=loss,
+        n_channels=n_channels,
+        logger=logger,
+        model_kwargs=model_kwargs,
+    )
+
+
 def create_n2v_configuration(
     experiment_name: str,
     data_type: Literal["array", "tiff", "custom"],
     axes: str,
     patch_size: List[int],
     batch_size: int,
     num_epochs: int,
     use_augmentations: bool = True,
     use_n2v2: bool = False,
-    n_channels: int = -1,
+    n_channels: int = 1,
     roi_size: int = 11,
     masked_pixel_percentage: float = 0.2,
     struct_n2v_axis: Literal["horizontal", "vertical", "none"] = "none",
     struct_n2v_span: int = 5,
     logger: Literal["wandb", "tensorboard", "none"] = "none",
     model_kwargs: Optional[dict] = None,
 ) -> Configuration:
     """
-    Create a configuration for training N2V.
+    Create a configuration for training Noise2Void.
 
     N2V uses a UNet model to denoise images in a self-supervised manner. To use its
     variants structN2V and N2V2, set the `struct_n2v_axis` and `struct_n2v_span`
     (structN2V) parameters, or set `use_n2v2` to True (N2V2).
 
     N2V2 modifies the UNet architecture by adding blur pool layers and removes the skip
     connections, thus removing checkboard artefacts. StructN2V is used when vertical
@@ -216,15 +355,15 @@
     num_epochs : int
         Number of epochs.
     use_augmentations : bool, optional
         Whether to use augmentations, by default True.
     use_n2v2 : bool, optional
         Whether to use N2V2, by default False.
     n_channels : int, optional
-        Number of channels (in and out), by default -1.
+        Number of channels (in and out), by default 1.
     roi_size : int, optional
         N2V pixel manipulation area, by default 11.
     masked_pixel_percentage : float, optional
         Percentage of pixels masked in each patch, by default 0.2.
     struct_n2v_axis : Literal["horizontal", "vertical", "none"], optional
         Axis along which to apply structN2V mask, by default "none".
     struct_n2v_span : int, optional
@@ -296,26 +435,24 @@
     ...     patch_size=[64, 64],
     ...     batch_size=32,
     ...     num_epochs=100,
     ...     use_augmentations=False
     ... )
     """
     # if there are channels, we need to specify their number
-    if "C" in axes and n_channels == -1:
+    if "C" in axes and n_channels == 1:
         raise ValueError(
             f"Number of channels must be specified when using channels "
             f"(got {n_channels} channel)."
         )
-    elif "C" not in axes and n_channels != -1:
+    elif "C" not in axes and n_channels > 1:
         raise ValueError(
             f"C is not present in the axes, but number of channels is specified "
             f"(got {n_channels} channel)."
         )
-    elif n_channels == -1:
-        n_channels = 1
 
     # model
     if model_kwargs is None:
         model_kwargs = {}
     model_kwargs["n2v2"] = use_n2v2
     model_kwargs["conv_dims"] = 3 if "Z" in axes else 2
     model_kwargs["in_channels"] = n_channels
@@ -323,15 +460,15 @@
 
     unet_model = UNetModel(
         architecture=SupportedArchitecture.UNET.value,
         **model_kwargs,
     )
 
     # algorithm model
-    algorithm = AlgorithmModel(
+    algorithm = AlgorithmConfig(
         algorithm=SupportedAlgorithm.N2V.value,
         loss=SupportedLoss.N2V.value,
         model=unet_model,
     )
 
     # augmentations
     if use_augmentations:
@@ -363,24 +500,24 @@
         "masked_pixel_percentage": masked_pixel_percentage,
         "struct_mask_axis": struct_n2v_axis,
         "struct_mask_span": struct_n2v_span,
     }
     transforms.append(nv2_transform)
 
     # data model
-    data = DataModel(
+    data = DataConfig(
         data_type=data_type,
         axes=axes,
         patch_size=patch_size,
         batch_size=batch_size,
         transforms=transforms,
     )
 
     # training model
-    training = TrainingModel(
+    training = TrainingConfig(
         num_epochs=num_epochs,
         batch_size=batch_size,
         logger=None if logger == "none" else logger,
     )
 
     # create configuration
     configuration = Configuration(
@@ -399,15 +536,15 @@
     tile_size: Optional[Tuple[int, ...]] = None,
     tile_overlap: Optional[Tuple[int, ...]] = None,
     data_type: Optional[Literal["array", "tiff", "custom"]] = None,
     axes: Optional[str] = None,
     transforms: Optional[Union[List[Dict[str, Any]], Compose]] = None,
     tta_transforms: bool = True,
     batch_size: Optional[int] = 1,
-) -> InferenceModel:
+) -> InferenceConfig:
     """
     Create a configuration for inference with N2V.
 
     If not provided, `data_type` and `axes` are taken from the training
     configuration. If `transforms` are not provided, only normalization is applied.
 
     Parameters
@@ -443,15 +580,15 @@
     if transforms is None:
         transforms = [
             {
                 "name": SupportedTransform.NORMALIZE.value,
             },
         ]
 
-    return InferenceModel(
+    return InferenceConfig(
         data_type=data_type or training_configuration.data_config.data_type,
         tile_size=tile_size,
         tile_overlap=tile_overlap,
         axes=axes or training_configuration.data_config.axes,
         mean=training_configuration.data_config.mean,
         std=training_configuration.data_config.std,
         transforms=transforms,
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/configuration_model.py` & `careamics-0.1.0rc4/src/careamics/config/configuration_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import Dict, List, Literal, Union
 
 import yaml
 from bioimageio.spec.generic.v0_3 import CiteEntry
 from pydantic import BaseModel, ConfigDict, Field, field_validator, model_validator
 from typing_extensions import Self
 
-from .algorithm_model import AlgorithmModel
-from .data_model import DataModel
+from .algorithm_model import AlgorithmConfig
+from .data_model import DataConfig
 from .references import (
     CARE,
     CUSTOM,
     N2N,
     N2V,
     N2V2,
     STRUCT_N2V,
@@ -30,15 +30,15 @@
     N2VDescription,
     N2VRef,
     StructN2V2Description,
     StructN2VDescription,
     StructN2VRef,
 )
 from .support import SupportedAlgorithm, SupportedPixelManipulation, SupportedTransform
-from .training_model import TrainingModel
+from .training_model import TrainingConfig
 from .transformations.n2v_manipulate_model import (
     N2VManipulateModel,
 )
 
 
 class Configuration(BaseModel):
     """
@@ -152,17 +152,18 @@
 
     # required parameters
     experiment_name: str = Field(
         ..., description="Name of the experiment, used to name logs and checkpoints."
     )
 
     # Sub-configurations
-    algorithm_config: AlgorithmModel
-    data_config: DataModel
-    training_config: TrainingModel
+    algorithm_config: AlgorithmConfig
+
+    data_config: DataConfig
+    training_config: TrainingConfig
 
     @field_validator("experiment_name")
     @classmethod
     def no_symbol(cls, name: str) -> str:
         """
         Validate experiment name.
 
@@ -587,10 +588,10 @@
             raise ValueError(
                 f"Path must be a directory or .yml or .yaml file (got {config_path})."
             )
 
     # save configuration as dictionary to yaml
     with open(config_path, "w") as f:
         # dump configuration
-        yaml.dump(config.model_dump(), f, default_flow_style=False)
+        yaml.dump(config.model_dump(), f, default_flow_style=False, sort_keys=False)
 
     return config_path
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/data_model.py` & `careamics-0.1.0rc4/src/careamics/config/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,40 +29,40 @@
         NormalizeModel,
         N2VManipulateModel,
     ],
     Discriminator("name"),  # used to tell the different transform models apart
 ]
 
 
-class DataModel(BaseModel):
+class DataConfig(BaseModel):
     """
     Data configuration.
 
     If std is specified, mean must be specified as well. Note that setting the std first
     and then the mean (if they were both `None` before) will raise a validation error.
     Prefer instead `set_mean_and_std` to set both at once.
 
     Examples
     --------
     Minimum example:
 
-    >>> data = DataModel(
+    >>> data = DataConfig(
     ...     data_type="array", # defined in SupportedData
     ...     patch_size=[128, 128],
     ...     batch_size=4,
     ...     axes="YX"
     ... )
 
     To change the mean and std of the data:
     >>> data.set_mean_and_std(mean=214.3, std=84.5)
 
     One can pass also a list of transformations, by keyword, using the
     SupportedTransform or the name of an Albumentation transform:
     >>> from careamics.config.support import SupportedTransform
-    >>> data = DataModel(
+    >>> data = DataConfig(
     ...     data_type="tiff",
     ...     patch_size=[128, 128],
     ...     batch_size=4,
     ...     axes="YX",
     ...     transforms=[
     ...         {
     ...             "name": SupportedTransform.NORMALIZE.value,
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/inference_model.py` & `careamics-0.1.0rc4/src/careamics/config/inference_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .support import SupportedTransform
 from .transformations.normalize_model import NormalizeModel
 from .validators import check_axes_validity, patch_size_ge_than_8_power_of_2
 
 TRANSFORMS_UNION = Union[NormalizeModel]
 
 
-class InferenceModel(BaseModel):
+class InferenceConfig(BaseModel):
     """Configuration class for the prediction model."""
 
     model_config = ConfigDict(validate_assignment=True, arbitrary_types_allowed=True)
 
     # Mandatory fields
     data_type: Literal["array", "tiff", "custom"]  # As defined in SupportedData
     tile_size: Optional[Union[List[int]]] = Field(
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/noise_models.py` & `careamics-0.1.0rc4/src/careamics/config/noise_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/optimizer_models.py` & `careamics-0.1.0rc4/src/careamics/config/optimizer_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/tile_information.py` & `careamics-0.1.0rc4/src/careamics/config/tile_information.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/training_model.py` & `careamics-0.1.0rc4/src/careamics/config/training_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     ConfigDict,
     Field,
 )
 
 from .callback_model import CheckpointModel, EarlyStoppingModel
 
 
-class TrainingModel(BaseModel):
+class TrainingConfig(BaseModel):
     """
     Parameters related to the training.
 
     Mandatory parameters are:
         - num_epochs: number of epochs, greater than 0.
         - batch_size: batch size, greater than 0.
         - augmentation: whether to use data augmentation or not (True or False).
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/architectures/architecture_model.py` & `careamics-0.1.0rc4/src/careamics/config/architectures/architecture_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/architectures/custom_model.py` & `careamics-0.1.0rc4/src/careamics/config/architectures/custom_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/architectures/register_model.py` & `careamics-0.1.0rc4/src/careamics/config/architectures/register_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/architectures/unet_model.py` & `careamics-0.1.0rc4/src/careamics/config/architectures/unet_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/architectures/vae_model.py` & `careamics-0.1.0rc4/src/careamics/config/architectures/vae_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/references/__init__.py` & `careamics-0.1.0rc4/src/careamics/config/references/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/references/algorithm_descriptions.py` & `careamics-0.1.0rc4/src/careamics/config/references/algorithm_descriptions.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/references/references.py` & `careamics-0.1.0rc4/src/careamics/config/references/references.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/support/__init__.py` & `careamics-0.1.0rc4/src/careamics/config/support/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/support/supported_data.py` & `careamics-0.1.0rc4/src/careamics/config/support/supported_data.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/support/supported_extraction_strategies.py` & `careamics-0.1.0rc4/src/careamics/config/support/supported_extraction_strategies.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/support/supported_optimizers.py` & `careamics-0.1.0rc4/src/careamics/config/support/supported_optimizers.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     SGD : str
         Stochastic Gradient Descent optimizer.
     """
 
     # ASGD = "ASGD"
     # Adadelta = "Adadelta"
     # Adagrad = "Adagrad"
-    Adam = "Adam"
+    ADAM = "Adam"
     # AdamW = "AdamW"
     # Adamax = "Adamax"
     # LBFGS = "LBFGS"
     # NAdam = "NAdam"
     # RAdam = "RAdam"
     # RMSprop = "RMSprop"
     # Rprop = "Rprop"
@@ -46,10 +46,10 @@
     # ExponentialLR = "ExponentialLR"
     # LambdaLR = "LambdaLR"
     # LinearLR = "LinearLR"
     # MultiStepLR = "MultiStepLR"
     # MultiplicativeLR = "MultiplicativeLR"
     # OneCycleLR = "OneCycleLR"
     # PolynomialLR = "PolynomialLR"
-    ReduceLROnPlateau = "ReduceLROnPlateau"
+    REDUCE_LR_ON_PLATEAU = "ReduceLROnPlateau"
     # SequentialLR = "SequentialLR"
-    StepLR = "StepLR"
+    STEP_LR = "StepLR"
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/support/supported_transforms.py` & `careamics-0.1.0rc4/src/careamics/config/support/supported_transforms.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/transformations/n2v_manipulate_model.py` & `careamics-0.1.0rc4/src/careamics/config/transformations/n2v_manipulate_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         Span of the structN2V mask, by default 5.
     """
 
     model_config = ConfigDict(
         validate_assignment=True,
     )
 
-    name: Literal["N2VManipulate"]
+    name: Literal["N2VManipulate"] = "N2VManipulate"
     roi_size: int = Field(default=11, ge=3, le=21)
     masked_pixel_percentage: float = Field(default=0.2, ge=0.05, le=1.0)
     strategy: Literal["uniform", "median"] = Field(default="uniform")
     struct_mask_axis: Literal["horizontal", "vertical", "none"] = Field(default="none")
     struct_mask_span: int = Field(default=5, ge=3, le=15)
 
     @field_validator("roi_size", "struct_mask_span")
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/transformations/nd_flip_model.py` & `careamics-0.1.0rc4/src/careamics/config/transformations/nd_flip_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,11 +22,11 @@
         Whether to flip the z axis, by default True.
     """
 
     model_config = ConfigDict(
         validate_assignment=True,
     )
 
-    name: Literal["NDFlip"]
+    name: Literal["NDFlip"] = "NDFlip"
     p: float = Field(default=0.5, ge=0.0, le=1.0)
     is_3D: bool = Field(default=False)
     flip_z: bool = Field(default=True)
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/transformations/normalize_model.py` & `careamics-0.1.0rc4/src/careamics/config/transformations/normalize_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,10 +22,10 @@
         Standard deviation value for normalization.
     """
 
     model_config = ConfigDict(
         validate_assignment=True,
     )
 
-    name: Literal["Normalize"]
+    name: Literal["Normalize"] = "Normalize"
     mean: float = Field(default=0.485)  # albumentations defaults
     std: float = Field(default=0.229)
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/transformations/transform_model.py` & `careamics-0.1.0rc4/src/careamics/config/transformations/transform_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/config/transformations/xy_random_rotate90_model.py` & `careamics-0.1.0rc4/src/careamics/config/transformations/xy_random_rotate90_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,10 +20,10 @@
         Whether the transformation should be applied in 3D, by default False.
     """
 
     model_config = ConfigDict(
         validate_assignment=True,
     )
 
-    name: Literal["XYRandomRotate90"]
+    name: Literal["XYRandomRotate90"] = "XYRandomRotate90"
     p: float = Field(default=0.5, ge=0.0, le=1.0)
     is_3D: bool = Field(default=False)
```

### Comparing `careamics-0.1.0rc3/src/careamics/config/validators/validator_utils.py` & `careamics-0.1.0rc4/src/careamics/config/validators/validator_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/in_memory_dataset.py` & `careamics-0.1.0rc4/src/careamics/dataset/in_memory_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import copy
 from pathlib import Path
 from typing import Any, Callable, List, Optional, Tuple, Union
 
 import numpy as np
 from torch.utils.data import Dataset
 
-from ..config import DataModel, InferenceModel
+from ..config import DataConfig, InferenceConfig
 from ..config.tile_information import TileInformation
 from ..utils.logging import get_logger
 from .dataset_utils import read_tiff, reshape_array
 from .patching.patch_transform import get_patch_transform
 from .patching.patching import (
     prepare_patches_supervised,
     prepare_patches_supervised_array,
@@ -25,15 +25,15 @@
 
 
 class InMemoryDataset(Dataset):
     """Dataset storing data in memory and allowing generating patches from it."""
 
     def __init__(
         self,
-        data_config: DataModel,
+        data_config: DataConfig,
         inputs: Union[np.ndarray, List[Path]],
         data_target: Optional[Union[np.ndarray, List[Path]]] = None,
         read_source_func: Callable = read_tiff,
         **kwargs: Any,
     ) -> None:
         """
         Constructor.
@@ -275,15 +275,15 @@
     Dataset storing data in memory and allowing generating patches from it.
 
     # TODO
     """
 
     def __init__(
         self,
-        prediction_config: InferenceModel,
+        prediction_config: InferenceConfig,
         inputs: np.ndarray,
         data_target: Optional[np.ndarray] = None,
         read_source_func: Optional[Callable] = read_tiff,
     ) -> None:
         """Constructor.
 
         Parameters
```

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/iterable_dataset.py` & `careamics-0.1.0rc4/src/careamics/dataset/iterable_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import copy
 from pathlib import Path
 from typing import Any, Callable, Generator, List, Optional, Tuple, Union
 
 import numpy as np
 from torch.utils.data import IterableDataset, get_worker_info
 
-from ..config import DataModel, InferenceModel
+from ..config import DataConfig, InferenceConfig
 from ..config.tile_information import TileInformation
 from ..utils.logging import get_logger
 from .dataset_utils import read_tiff, reshape_array
 from .patching import (
     get_patch_transform,
 )
 from .patching.random_patching import extract_patches_random
@@ -42,15 +42,15 @@
         Expected standard deviation of the dataset, by default None.
     patch_transform : Optional[Callable], optional
         Patch transform callable, by default None.
     """
 
     def __init__(
         self,
-        data_config: Union[DataModel, InferenceModel],
+        data_config: Union[DataConfig, InferenceConfig],
         src_files: List[Path],
         target_files: Optional[List[Path]] = None,
         read_source_func: Callable = read_tiff,
     ) -> None:
         self.data_config = data_config
         self.data_files = src_files
         self.target_files = target_files
@@ -342,15 +342,15 @@
         Expected standard deviation of the dataset, by default None.
     patch_transform : Optional[Callable], optional
         Patch transform callable, by default None.
     """
 
     def __init__(
         self,
-        prediction_config: InferenceModel,
+        prediction_config: InferenceConfig,
         src_files: List[Path],
         read_source_func: Callable = read_tiff,
         **kwargs: Any,
     ) -> None:
         super().__init__(
             data_config=prediction_config,
             src_files=src_files,
```

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/zarr_dataset.py` & `careamics-0.1.0rc4/src/careamics/dataset/zarr_dataset.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/dataset_utils.py` & `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/file_utils.py` & `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_tiff.py` & `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_tiff.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_utils.py` & `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/dataset_utils/read_zarr.py` & `careamics-0.1.0rc4/src/careamics/dataset/dataset_utils/read_zarr.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/patch_transform.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/patch_transform.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/patching.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/random_patching.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/random_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/sequential_patching.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/sequential_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/tiled_patching.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/tiled_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/dataset/patching/validate_patch_dimension.py` & `careamics-0.1.0rc4/src/careamics/dataset/patching/validate_patch_dimension.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/losses/loss_factory.py` & `careamics-0.1.0rc4/src/careamics/losses/loss_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/losses/losses.py` & `careamics-0.1.0rc4/src/careamics/losses/losses.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/losses/noise_model_factory.py` & `careamics-0.1.0rc4/src/careamics/losses/noise_model_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/losses/noise_models.py` & `careamics-0.1.0rc4/src/careamics/losses/noise_models.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/model_io/bmz_io.py` & `careamics-0.1.0rc4/src/careamics/model_io/bmz_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 import pkg_resources
 from bioimageio.core import load_description, test_model
 from bioimageio.spec import ValidationSummary, save_bioimageio_package
 from torch import __version__, load, save
 
 from careamics.config import Configuration, load_configuration, save_configuration
 from careamics.config.support import SupportedArchitecture
-from careamics.lightning_module import CAREamicsKiln
+from careamics.lightning_module import CAREamicsModule
 
 from .bioimage import (
     create_env_text,
     create_model_description,
     extract_model_path,
     get_unzip_path,
 )
 
 
-def _export_state_dict(model: CAREamicsKiln, path: Union[Path, str]) -> Path:
+def _export_state_dict(model: CAREamicsModule, path: Union[Path, str]) -> Path:
     """
     Export the model state dictionary to a file.
 
     Parameters
     ----------
     model : CAREamicsKiln
         CAREamics model to export.
@@ -47,15 +47,15 @@
     # we save through the torch model itself to avoid the initial "model." in the
     # layers naming, which is incompatible with the way the BMZ load torch state dicts
     save(model.model.state_dict(), path)
 
     return path
 
 
-def _load_state_dict(model: CAREamicsKiln, path: Union[Path, str]) -> None:
+def _load_state_dict(model: CAREamicsModule, path: Union[Path, str]) -> None:
     """
     Load a model from a state dictionary.
 
     Parameters
     ----------
     model : CAREamicsKiln
         CAREamics model to be updated with the weights.
@@ -69,15 +69,15 @@
     # witht bioimageio.core expectations for a torch state dict
     state_dict = load(path)
     model.model.load_state_dict(state_dict)
 
 
 # TODO break down in subfunctions
 def export_to_bmz(
-    model: CAREamicsKiln,
+    model: CAREamicsModule,
     config: Configuration,
     path: Union[Path, str],
     name: str,
     general_description: str,
     authors: List[dict],
     input_array: np.ndarray,
     output_array: np.ndarray,
@@ -181,15 +181,15 @@
         if summary.status == "failed":
             raise ValueError(f"Model description test failed: {summary}")
 
         # save bmz model
         save_bioimageio_package(model_description, output_path=path)
 
 
-def load_from_bmz(path: Union[Path, str]) -> Tuple[CAREamicsKiln, Configuration]:
+def load_from_bmz(path: Union[Path, str]) -> Tuple[CAREamicsModule, Configuration]:
     """Load a model from a BioImage Model Zoo archive.
 
     Parameters
     ----------
     path : Union[Path, str]
         Path to the BioImage Model Zoo archive.
 
@@ -219,13 +219,13 @@
     weights_path = unzip_path / weights_path
     config_path = unzip_path / config_path
 
     # load configuration
     config = load_configuration(config_path)
 
     # create careamics lightning module
-    model = CAREamicsKiln(algorithm_config=config.algorithm_config)
+    model = CAREamicsModule(algorithm_config=config.algorithm_config)
 
     # load model state dictionary
     _load_state_dict(model, weights_path)
 
     return model, config
```

### Comparing `careamics-0.1.0rc3/src/careamics/model_io/model_io_utils.py` & `careamics-0.1.0rc4/src/careamics/model_io/model_io_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from pathlib import Path
 from typing import Tuple, Union
 
 from torch import load
 
 from careamics.config import Configuration
-from careamics.lightning_module import CAREamicsKiln
+from careamics.lightning_module import CAREamicsModule
 from careamics.model_io.bmz_io import load_from_bmz
 from careamics.utils import check_path_exists
 
 
-def load_pretrained(path: Union[Path, str]) -> Tuple[CAREamicsKiln, Configuration]:
+def load_pretrained(path: Union[Path, str]) -> Tuple[CAREamicsModule, Configuration]:
     """
     Load a pretrained model from a checkpoint or a BioImage Model Zoo model.
 
     Expected formats are .ckpt or .zip files.
 
     Parameters
     ----------
@@ -40,15 +40,15 @@
         return load_from_bmz(path)
     else:
         raise ValueError(
             f"Invalid model format. Expected .ckpt or .zip, got {path.suffix}."
         )
 
 
-def _load_checkpoint(path: Union[Path, str]) -> Tuple[CAREamicsKiln, Configuration]:
+def _load_checkpoint(path: Union[Path, str]) -> Tuple[CAREamicsModule, Configuration]:
     """
     Load a model from a checkpoint and return both model and configuration.
 
     Parameters
     ----------
     path : Union[Path, str]
         Path to the checkpoint.
@@ -71,10 +71,10 @@
         cfg_dict = checkpoint["hyper_parameters"]
     except KeyError as e:
         raise ValueError(
             f"Invalid checkpoint file. No `hyper_parameters` found in the "
             f"checkpoint: {checkpoint.keys()}"
         ) from e
 
-    model = CAREamicsKiln.load_from_checkpoint(path)
+    model = CAREamicsModule.load_from_checkpoint(path)
 
     return model, Configuration(**cfg_dict)
```

### Comparing `careamics-0.1.0rc3/src/careamics/model_io/bioimage/_readme_factory.py` & `careamics-0.1.0rc4/src/careamics/model_io/bioimage/_readme_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/model_io/bioimage/bioimage_utils.py` & `careamics-0.1.0rc4/src/careamics/model_io/bioimage/bioimage_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/model_io/bioimage/model_description.py` & `careamics-0.1.0rc4/src/careamics/model_io/bioimage/model_description.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,22 @@
     SpaceInputAxis,
     SpaceOutputAxis,
     TensorId,
     Version,
     WeightsDescr,
 )
 
-from careamics.config import Configuration, DataModel
+from careamics.config import Configuration, DataConfig
 
 from ._readme_factory import readme_factory
 
 
 def _create_axes(
     array: np.ndarray,
-    data_config: DataModel,
+    data_config: DataConfig,
     channel_names: Optional[List[str]] = None,
     is_input: bool = True,
 ) -> List[AxisBase]:
     """Create axes description.
 
     Array shape is expected to be SC(Z)YX.
 
@@ -96,15 +96,15 @@
 
     return axes_model
 
 
 def _create_inputs_ouputs(
     input_array: np.ndarray,
     output_array: np.ndarray,
-    data_config: DataModel,
+    data_config: DataConfig,
     input_path: Union[Path, str],
     output_path: Union[Path, str],
     channel_names: Optional[List[str]] = None,
 ) -> Tuple[InputTensorDescr, OutputTensorDescr]:
     """Create input and output tensor description.
 
     Input and output paths must point to a `.npy` file.
```

### Comparing `careamics-0.1.0rc3/src/careamics/models/activation.py` & `careamics-0.1.0rc4/src/careamics/models/activation.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/models/layers.py` & `careamics-0.1.0rc4/src/careamics/models/layers.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/models/model_factory.py` & `careamics-0.1.0rc4/src/careamics/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/models/unet.py` & `careamics-0.1.0rc4/src/careamics/models/unet.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/prediction/stitch_prediction.py` & `careamics-0.1.0rc4/src/careamics/prediction/stitch_prediction.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/__init__.py` & `careamics-0.1.0rc4/src/careamics/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/n2v_manipulate.py` & `careamics-0.1.0rc4/src/careamics/transforms/n2v_manipulate.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/nd_flip.py` & `careamics-0.1.0rc4/src/careamics/transforms/nd_flip.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/normalize.py` & `careamics-0.1.0rc4/src/careamics/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/pixel_manipulation.py` & `careamics-0.1.0rc4/src/careamics/transforms/pixel_manipulation.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/tta.py` & `careamics-0.1.0rc4/src/careamics/transforms/tta.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/transforms/xy_random_rotate90.py` & `careamics-0.1.0rc4/src/careamics/transforms/xy_random_rotate90.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/base_enum.py` & `careamics-0.1.0rc4/src/careamics/utils/base_enum.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/context.py` & `careamics-0.1.0rc4/src/careamics/utils/context.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/logging.py` & `careamics-0.1.0rc4/src/careamics/utils/logging.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/metrics.py` & `careamics-0.1.0rc4/src/careamics/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/path_utils.py` & `careamics-0.1.0rc4/src/careamics/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/receptive_field.py` & `careamics-0.1.0rc4/src/careamics/utils/receptive_field.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/running_stats.py` & `careamics-0.1.0rc4/src/careamics/utils/running_stats.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/src/careamics/utils/torch_utils.py` & `careamics-0.1.0rc4/src/careamics/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/conftest.py` & `careamics-0.1.0rc4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/test_careamist.py` & `careamics-0.1.0rc4/tests/test_careamist.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/test_lightning_datamodule.py` & `careamics-0.1.0rc4/tests/test_lightning_datamodule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,78 @@
 import pytest
 
-from careamics import CAREamicsPredictDataModule, CAREamicsTrainDataModule
-from careamics.config.support import SupportedPixelManipulation, SupportedStructAxis
+from careamics import CAREamicsTrainData, TrainingDataWrapper
+from careamics.config import DataConfig
+from careamics.config.support import (
+    SupportedData,
+    SupportedPixelManipulation,
+    SupportedStructAxis,
+)
 
 
 @pytest.fixture
 def simple_array(ordered_array):
     return ordered_array((10, 10))
 
 
-def test_lightning_train_datamodule_wrong_type(simple_array):
+def test_mismatching_types_array(simple_array, minimum_data):
+    """Test that an error is raised if the data type does not match the passed data."""
+    minimum_data["data_type"] = SupportedData.TIFF.value
+    with pytest.raises(ValueError):
+        CAREamicsTrainData(
+            data_config=DataConfig(**minimum_data), train_data=simple_array
+        )
+
+    minimum_data["data_type"] = SupportedData.CUSTOM.value
+    with pytest.raises(ValueError):
+        CAREamicsTrainData(
+            data_config=DataConfig(**minimum_data), train_data=simple_array
+        )
+
+    minimum_data["data_type"] = SupportedData.ARRAY.value
+    with pytest.raises(ValueError):
+        CAREamicsTrainData(
+            data_config=DataConfig(**minimum_data), train_data="path/to/data"
+        )
+
+
+def test_wrapper_unknown_type(simple_array):
     """Test that an error is raised if the data type is not supported."""
     with pytest.raises(ValueError):
-        CAREamicsTrainDataModule(
+        TrainingDataWrapper(
             train_data=simple_array,
             data_type="wrong_type",
             patch_size=(10, 10),
             axes="YX",
             batch_size=2,
         )
 
 
-def test_lightning_train_datamodule_array(simple_array):
+def test_wrapper_train_array(simple_array):
     """Test that the data module is created correctly with an array."""
     # create data module
-    data_module = CAREamicsTrainDataModule(
+    data_module = TrainingDataWrapper(
         train_data=simple_array,
         data_type="array",
         patch_size=(8, 8),
         axes="YX",
         batch_size=2,
         val_minimum_patches=2,
     )
     data_module.prepare_data()
     data_module.setup()
 
     assert len(list(data_module.train_dataloader())) > 0
 
 
-def test_lightning_train_datamodule_supervised_n2v_throws_error(simple_array):
+def test_wrapper_supervised_n2v_throws_error(simple_array):
     """Test that an error is raised if target data is passed but the transformations
     (default ones) contain N2V manipulate."""
     with pytest.raises(ValueError):
-        CAREamicsTrainDataModule(
+        TrainingDataWrapper(
             train_data=simple_array,
             data_type="array",
             patch_size=(10, 10),
             axes="YX",
             batch_size=2,
             train_target_data=simple_array,
             val_minimum_patches=2,
@@ -56,85 +82,36 @@
 @pytest.mark.parametrize(
     "use_n2v2, strategy",
     [
         (True, SupportedPixelManipulation.MEDIAN),
         (False, SupportedPixelManipulation.UNIFORM),
     ],
 )
-def test_lightning_train_datamodule_n2v2(simple_array, use_n2v2, strategy):
+def test_wrapper_n2v2(simple_array, use_n2v2, strategy):
     """Test that n2v2 parameter is correctly passed."""
-    data_module = CAREamicsTrainDataModule(
+    data_module = TrainingDataWrapper(
         train_data=simple_array,
         data_type="array",
         patch_size=(16, 16),
         axes="YX",
         batch_size=2,
         use_n2v2=use_n2v2,
     )
     assert data_module.data_config.transforms[-1].strategy == strategy
 
 
-def test_lightning_train_datamodule_structn2v(simple_array):
+def test_wrapper_structn2v(simple_array):
     """Test that structn2v parameter is correctly passed."""
     struct_axis = SupportedStructAxis.HORIZONTAL.value
     struct_span = 11
 
-    data_module = CAREamicsTrainDataModule(
+    data_module = TrainingDataWrapper(
         train_data=simple_array,
         data_type="array",
         patch_size=(16, 16),
         axes="YX",
         batch_size=2,
         struct_n2v_axis=struct_axis,
         struct_n2v_span=struct_span,
     )
     assert data_module.data_config.transforms[-1].struct_mask_axis == struct_axis
     assert data_module.data_config.transforms[-1].struct_mask_span == struct_span
-
-
-def test_lightning_predict_datamodule_wrong_type(simple_array):
-    """Test that an error is raised if the data type is not supported."""
-    with pytest.raises(ValueError):
-        CAREamicsPredictDataModule(
-            pred_data=simple_array,
-            data_type="wrong_type",
-            mean=0.5,
-            std=0.1,
-            axes="YX",
-            batch_size=2,
-        )
-
-
-def test_lightning_pred_datamodule_tiling(simple_array):
-    """Test that the data module is created correctly with an array."""
-    # create data module
-    data_module = CAREamicsPredictDataModule(
-        pred_data=simple_array,
-        data_type="array",
-        mean=0.5,
-        std=0.1,
-        axes="YX",
-        batch_size=2,
-        tile_overlap=[2, 2],
-        tile_size=[8, 8],
-    )
-
-    data_module.prepare_data()
-    data_module.setup()
-    assert len(list(data_module.predict_dataloader())) == 2
-
-
-def test_lightning_pred_datamodule_no_tiling(simple_array):
-    """Test that the data module is created correctly with an array."""
-    # create data module
-    data_module = CAREamicsPredictDataModule(
-        pred_data=simple_array,
-        data_type="array",
-        mean=0.5,
-        std=0.1,
-        axes="YX",
-        batch_size=2,
-    )
-
-    data_module.prepare_data()
-    data_module.setup()
-    assert len(list(data_module.predict_dataloader())) == 1
```

### Comparing `careamics-0.1.0rc3/tests/test_lightning_module.py` & `careamics-0.1.0rc4/tests/test_lightning_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import pytest
 import torch
 
-from careamics.config import AlgorithmModel
-from careamics.lightning_module import CAREamicsKiln, CAREamicsModule
+from careamics.config import AlgorithmConfig
+from careamics.lightning_module import CAREamicsModule, CAREamicsModuleWrapper
 
 
 def test_careamics_module(minimum_algorithm_n2v):
     """Test that the minimum algorithm allows instantiating a the Lightning API
     intermediate layer."""
-    algo_config = AlgorithmModel(**minimum_algorithm_n2v)
+    algo_config = AlgorithmConfig(**minimum_algorithm_n2v)
 
     # extract model parameters
     model_parameters = algo_config.model.model_dump(exclude_none=True)
 
     # instantiate CAREamicsModule
-    CAREamicsModule(
+    CAREamicsModuleWrapper(
         algorithm=algo_config.algorithm,
         loss=algo_config.loss,
         architecture=algo_config.model.architecture,
         model_parameters=model_parameters,
         optimizer=algo_config.optimizer.name,
         optimizer_parameters=algo_config.optimizer.parameters,
         lr_scheduler=algo_config.lr_scheduler.name,
         lr_scheduler_parameters=algo_config.lr_scheduler.parameters,
     )
 
 
 def test_careamics_kiln(minimum_algorithm_n2v):
     """Test that the minimum algorithm allows instantiating a CAREamicsKiln."""
-    algo_config = AlgorithmModel(**minimum_algorithm_n2v)
+    algo_config = AlgorithmConfig(**minimum_algorithm_n2v)
 
     # instantiate CAREamicsKiln
-    CAREamicsKiln(algo_config)
+    CAREamicsModule(algo_config)
 
 
 @pytest.mark.parametrize(
     "shape",
     [
         (8, 8),
         (16, 16),
@@ -50,18 +50,18 @@
             "conv_dims": 2,
             "in_channels": 1,
             "num_classes": 1,
             "depth": 2,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, 1, *shape))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -85,18 +85,18 @@
             "conv_dims": 2,
             "in_channels": 1,
             "num_classes": 1,
             "depth": 3,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, 1, *shape))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -118,18 +118,18 @@
             "conv_dims": 3,
             "in_channels": 1,
             "num_classes": 1,
             "depth": 2,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, 1, *shape))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -151,18 +151,18 @@
             "conv_dims": 3,
             "in_channels": 1,
             "num_classes": 1,
             "depth": 3,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, 1, *shape))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -176,18 +176,18 @@
             "conv_dims": 2,
             "in_channels": n_channels,
             "num_classes": n_channels,
             "depth": 2,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, n_channels, 32, 32))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -201,18 +201,18 @@
             "conv_dims": 2,
             "in_channels": n_channels,
             "num_classes": n_channels,
             "depth": 3,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, n_channels, 64, 64))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -226,18 +226,18 @@
             "conv_dims": 3,
             "in_channels": n_channels,
             "num_classes": n_channels,
             "depth": 2,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((2, n_channels, 16, 32, 32))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
 
@@ -251,17 +251,17 @@
             "conv_dims": 3,
             "in_channels": n_channels,
             "num_classes": n_channels,
             "depth": 3,
         },
         "loss": "mae",
     }
-    algo_config = AlgorithmModel(**algo_dict)
+    algo_config = AlgorithmConfig(**algo_dict)
 
     # instantiate CAREamicsKiln
-    model = CAREamicsKiln(algo_config)
+    model = CAREamicsModule(algo_config)
     # set model to evaluation mode to avoid batch dimension error
     model.model.eval()
     # test forward pass
     x = torch.rand((1, n_channels, 16, 64, 64))
     y: torch.Tensor = model.forward(x)
     assert y.shape == x.shape
```

### Comparing `careamics-0.1.0rc3/tests/config/test_algorithm_model.py` & `careamics-0.1.0rc4/tests/config/test_algorithm_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import pytest
 
-from careamics.config.algorithm_model import AlgorithmModel
+from careamics.config.algorithm_model import AlgorithmConfig
 from careamics.config.support import (
     SupportedAlgorithm,
     SupportedArchitecture,
     SupportedLoss,
 )
 
 
 def test_all_algorithms_are_supported():
     """Test that all algorithms defined in the Literal are supported."""
     # list of supported algorithms
     algorithms = list(SupportedAlgorithm)
 
     # Algorithm json schema to extract the literal value
-    schema = AlgorithmModel.model_json_schema()
+    schema = AlgorithmConfig.model_json_schema()
 
     # check that all algorithms are supported
     for algo in schema["properties"]["algorithm"]["enum"]:
         assert algo in algorithms
 
 
 def test_supported_losses(minimum_algorithm_custom):
     """Test that all supported losses are accepted by the AlgorithmModel."""
     for loss in SupportedLoss:
         minimum_algorithm_custom["loss"] = loss.value
-        AlgorithmModel(**minimum_algorithm_custom)
+        AlgorithmConfig(**minimum_algorithm_custom)
 
 
 def test_all_losses_are_supported():
     """Test that all losses defined in the Literal are supported."""
     # list of supported losses
     losses = list(SupportedLoss)
 
     # Algorithm json schema
-    schema = AlgorithmModel.model_json_schema()
+    schema = AlgorithmConfig.model_json_schema()
 
     # check that all losses are supported
     for loss in schema["properties"]["loss"]["enum"]:
         assert loss in losses
 
 
 def test_model_discriminator(minimum_algorithm_n2v):
     """Test that discriminator permits correct assignment."""
     for model_name in SupportedArchitecture:
         # TODO change once VAE are implemented
         if model_name.value == "UNet":
             minimum_algorithm_n2v["model"]["architecture"] = model_name.value
 
-            algo = AlgorithmModel(**minimum_algorithm_n2v)
+            algo = AlgorithmConfig(**minimum_algorithm_n2v)
             assert algo.model.architecture == model_name.value
 
 
 @pytest.mark.parametrize(
     "algorithm, loss, model",
     [
         ("n2v", "n2v", {"architecture": "UNet", "n2v2": False}),
         ("custom", "mae", {"architecture": "UNet", "n2v2": True}),
     ],
 )
 def test_algorithm_constraints(algorithm: str, loss: str, model: dict):
     """Test that constraints are passed for each algorithm."""
-    AlgorithmModel(algorithm=algorithm, loss=loss, model=model)
+    AlgorithmConfig(algorithm=algorithm, loss=loss, model=model)
 
 
 @pytest.mark.parametrize("algorithm", ["n2v", "n2n"])
 def test_n_channels_n2v_and_n2n(algorithm):
     """Check that an error is raised if n2v and n2n have different number of channels in
     input and output."""
     model = {
@@ -73,15 +73,15 @@
         "in_channels": 1,
         "num_classes": 2,
         "n2v2": False,
     }
     loss = "mae" if algorithm == "n2n" else "n2v"
 
     with pytest.raises(ValueError):
-        AlgorithmModel(algorithm=algorithm, loss=loss, model=model)
+        AlgorithmConfig(algorithm=algorithm, loss=loss, model=model)
 
 
 @pytest.mark.parametrize(
     "algorithm, n_in, n_out",
     [
         ("n2v", 2, 2),
         ("n2n", 3, 3),
@@ -95,8 +95,8 @@
         "architecture": "UNet",
         "in_channels": n_in,
         "num_classes": n_out,
         "n2v2": False,
     }
     loss = "n2v" if algorithm == "n2v" else "mae"
 
-    AlgorithmModel(algorithm=algorithm, loss=loss, model=model)
+    AlgorithmConfig(algorithm=algorithm, loss=loss, model=model)
```

### Comparing `careamics-0.1.0rc3/tests/config/test_configuration_factory.py` & `careamics-0.1.0rc4/tests/config/test_configuration_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/test_configuration_model.py` & `careamics-0.1.0rc4/tests/config/test_configuration_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/test_data_model.py` & `careamics-0.1.0rc4/tests/config/test_data_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from albumentations import Compose
 
-from careamics.config.data_model import DataModel
+from careamics.config.data_model import DataConfig
 from careamics.config.support import (
     SupportedPixelManipulation,
     SupportedStructAxis,
     SupportedTransform,
 )
 from careamics.config.transformations import (
     N2VManipulateModel,
@@ -19,123 +19,123 @@
 @pytest.mark.parametrize("ext", ["nd2", "jpg", "png ", "zarr", "npy"])
 def test_wrong_extensions(minimum_data: dict, ext: str):
     """Test that supported model raises ValueError for unsupported extensions."""
     minimum_data["data_type"] = ext
 
     # instantiate DataModel model
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
 
 @pytest.mark.parametrize("mean, std", [(0, 124.5), (12.6, 0.1)])
 def test_mean_std_non_negative(minimum_data: dict, mean, std):
     """Test that non negative mean and std are accepted."""
     minimum_data["mean"] = mean
     minimum_data["std"] = std
 
-    data_model = DataModel(**minimum_data)
+    data_model = DataConfig(**minimum_data)
     assert data_model.mean == mean
     assert data_model.std == std
 
 
 def test_mean_std_both_specified_or_none(minimum_data: dict):
     """Test an error is raised if std is specified but mean is None."""
     # No error if both are None
-    DataModel(**minimum_data)
+    DataConfig(**minimum_data)
 
     # Error if only mean is defined
     minimum_data["mean"] = 10.4
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
     # Error if only std is defined
     minimum_data.pop("mean")
     minimum_data["std"] = 10.4
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
     # No error if both are specified
     minimum_data["mean"] = 10.4
     minimum_data["std"] = 10.4
-    DataModel(**minimum_data)
+    DataConfig(**minimum_data)
 
 
 def test_set_mean_and_std(minimum_data: dict):
     """Test that mean and std can be set after initialization."""
     # they can be set both, when they None
     mean = 4.07
     std = 14.07
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     data.set_mean_and_std(mean, std)
     assert data.mean == mean
     assert data.std == std
 
     # and if they are already set
     minimum_data["mean"] = 10.4
     minimum_data["std"] = 3.2
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     data.set_mean_and_std(mean, std)
     assert data.mean == mean
     assert data.std == std
 
 
 def test_mean_and_std_in_normalize(minimum_data: dict):
     """Test that mean and std are added to the Normalize transform."""
     minimum_data["mean"] = 10.4
     minimum_data["std"] = 3.2
     minimum_data["transforms"] = [
         {"name": SupportedTransform.NORMALIZE.value},
     ]
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     assert data.transforms[0].mean == 10.4
     assert data.transforms[0].std == 3.2
 
 
 def test_patch_size(minimum_data: dict):
     """Test that non-zero even patch size are accepted."""
     # 2D
-    data_model = DataModel(**minimum_data)
+    data_model = DataConfig(**minimum_data)
 
     # 3D
     minimum_data["patch_size"] = [16, 8, 8]
     minimum_data["axes"] = "ZYX"
 
-    data_model = DataModel(**minimum_data)
+    data_model = DataConfig(**minimum_data)
     assert data_model.patch_size == minimum_data["patch_size"]
 
 
 @pytest.mark.parametrize(
     "patch_size", [[12], [0, 12, 12], [12, 12, 13], [16, 10, 16], [12, 12, 12, 12]]
 )
 def test_wrong_patch_size(minimum_data: dict, patch_size):
     """Test that wrong patch sizes are not accepted (zero or odd, dims 1 or > 3)."""
     minimum_data["axes"] = "ZYX" if len(patch_size) == 3 else "YX"
     minimum_data["patch_size"] = patch_size
 
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
 
 def test_set_3d(minimum_data: dict):
     """Test that 3D can be set."""
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     assert "Z" not in data.axes
     assert len(data.patch_size) == 2
 
     # error if changing Z manually
     with pytest.raises(ValueError):
         data.axes = "ZYX"
 
     # or patch size
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     with pytest.raises(ValueError):
         data.patch_size = [64, 64, 64]
 
     # set 3D
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     data.set_3D("ZYX", [64, 64, 64])
     assert "Z" in data.axes
     assert len(data.patch_size) == 3
 
 
 @pytest.mark.parametrize(
     "transforms",
@@ -154,15 +154,15 @@
             {"name": SupportedTransform.N2V_MANIPULATE.value},
         ],
     ],
 )
 def test_passing_supported_transforms(minimum_data: dict, transforms):
     """Test that list of supported transforms can be passed."""
     minimum_data["transforms"] = transforms
-    model = DataModel(**minimum_data)
+    model = DataConfig(**minimum_data)
 
     supported = {
         "NDFlip": NDFlipModel,
         "XYRandomRotate90": XYRandomRotate90Model,
         "Normalize": NormalizeModel,
         "N2VManipulate": N2VManipulateModel,
     }
@@ -189,46 +189,46 @@
             {"name": SupportedTransform.XY_RANDOM_ROTATE90.value},
         ],
     ],
 )
 def test_n2vmanipulate_last_transform(minimum_data: dict, transforms):
     """Test that N2V Manipulate is moved to the last position if it is not."""
     minimum_data["transforms"] = transforms
-    model = DataModel(**minimum_data)
+    model = DataConfig(**minimum_data)
     assert model.transforms[-1].name == SupportedTransform.N2V_MANIPULATE.value
 
 
 def test_multiple_n2v_manipulate(minimum_data: dict):
     """Test that passing multiple n2v manipulate raises an error."""
     minimum_data["transforms"] = [
         {"name": SupportedTransform.N2V_MANIPULATE.value},
         {"name": SupportedTransform.N2V_MANIPULATE.value},
     ]
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
 
 def test_remove_n2v_manipulate(minimum_data: dict):
     """Test that N2V Manipulate can be removed."""
     minimum_data["transforms"] = [
         {"name": SupportedTransform.NDFLIP.value},
         {"name": SupportedTransform.N2V_MANIPULATE.value},
     ]
-    model = DataModel(**minimum_data)
+    model = DataConfig(**minimum_data)
     model.remove_n2v_manipulate()
     assert len(model.transforms) == 1
     assert model.transforms[-1].name == SupportedTransform.NDFLIP.value
 
 
 def test_add_n2v_manipulate(minimum_data: dict):
     """Test that N2V Manipulate can be added."""
     minimum_data["transforms"] = [
         {"name": SupportedTransform.NDFLIP.value},
     ]
-    model = DataModel(**minimum_data)
+    model = DataConfig(**minimum_data)
     model.add_n2v_manipulate()
     assert len(model.transforms) == 2
     assert model.transforms[-1].name == SupportedTransform.N2V_MANIPULATE.value
 
     # test that adding twice doesn't change anything
     model.add_n2v_manipulate()
     assert len(model.transforms) == 2
@@ -243,15 +243,15 @@
     """
     minimum_data["transforms"] = [
         {"name": SupportedTransform.NORMALIZE.value},
         {"name": SupportedTransform.NDFLIP.value},
         {"name": SupportedTransform.XY_RANDOM_ROTATE90.value},
         {"name": SupportedTransform.N2V_MANIPULATE.value},
     ]
-    model = DataModel(**minimum_data)
+    model = DataConfig(**minimum_data)
 
     # Normalize
     params = model.transforms[0].model_dump()
     assert "mean" in params
     assert "std" in params
 
     # NDFlip
@@ -274,36 +274,36 @@
     assert "struct_mask_axis" in params
     assert "struct_mask_span" in params
 
 
 def test_passing_empty_transforms(minimum_data: dict):
     """Test that empty list of transforms can be passed."""
     minimum_data["transforms"] = []
-    DataModel(**minimum_data)
+    DataConfig(**minimum_data)
 
 
 def test_passing_incorrect_element(minimum_data: dict):
     """Test that incorrect element in the list of transforms raises an error (
     e.g. passing un object rather than a string)."""
     minimum_data["transforms"] = [
         {"name": get_all_transforms()[SupportedTransform.NDFLIP.value]()},
     ]
     with pytest.raises(ValueError):
-        DataModel(**minimum_data)
+        DataConfig(**minimum_data)
 
 
 def test_passing_compose_transform(minimum_data: dict):
     """Test that Compose transform can be passed."""
     minimum_data["transforms"] = Compose(
         [
             get_all_transforms()[SupportedTransform.NDFLIP](),
             get_all_transforms()[SupportedTransform.N2V_MANIPULATE](),
         ]
     )
-    DataModel(**minimum_data)
+    DataConfig(**minimum_data)
 
 
 def test_3D_and_transforms(minimum_data: dict):
     """Test that NDFlip is corrected if the data is 3D."""
     minimum_data["transforms"] = [
         {
             "name": SupportedTransform.NDFLIP.value,
@@ -311,54 +311,54 @@
             "flip_z": True,
         },
         {
             "name": SupportedTransform.XY_RANDOM_ROTATE90.value,
             "is_3D": True,
         },
     ]
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     assert data.transforms[0].is_3D is False
     assert data.transforms[1].is_3D is False
 
     # change to 3D
     data.set_3D("ZYX", [64, 64, 64])
     data.transforms[0].is_3D = True
     data.transforms[1].is_3D = True
 
 
 def test_set_n2v_strategy(minimum_data: dict):
     """Test that the N2V strategy can be set."""
     uniform = SupportedPixelManipulation.UNIFORM.value
     median = SupportedPixelManipulation.MEDIAN.value
 
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     assert data.transforms[-1].name == SupportedTransform.N2V_MANIPULATE.value
     assert data.transforms[-1].strategy == uniform
 
     data.set_N2V2_strategy(median)
     assert data.transforms[-1].strategy == median
 
     data.set_N2V2_strategy(uniform)
     assert data.transforms[-1].strategy == uniform
 
 
 def test_set_n2v_strategy_wrong_value(minimum_data: dict):
     """Test that passing a wrong strategy raises an error."""
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     with pytest.raises(ValueError):
         data.set_N2V2_strategy("wrong_value")
 
 
 def test_set_struct_mask(minimum_data: dict):
     """Test that the struct mask can be set."""
     none = SupportedStructAxis.NONE.value
     vertical = SupportedStructAxis.VERTICAL.value
     horizontal = SupportedStructAxis.HORIZONTAL.value
 
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     assert data.transforms[-1].name == SupportedTransform.N2V_MANIPULATE.value
     assert data.transforms[-1].struct_mask_axis == none
     assert data.transforms[-1].struct_mask_span == 5
 
     data.set_structN2V_mask(vertical, 3)
     assert data.transforms[-1].struct_mask_axis == vertical
     assert data.transforms[-1].struct_mask_span == 3
@@ -370,13 +370,13 @@
     data.set_structN2V_mask(none, 11)
     assert data.transforms[-1].struct_mask_axis == none
     assert data.transforms[-1].struct_mask_span == 11
 
 
 def test_set_struct_mask_wrong_value(minimum_data: dict):
     """Test that passing a wrong struct mask axis raises an error."""
-    data = DataModel(**minimum_data)
+    data = DataConfig(**minimum_data)
     with pytest.raises(ValueError):
         data.set_structN2V_mask("wrong_value", 3)
 
     with pytest.raises(ValueError):
         data.set_structN2V_mask(SupportedStructAxis.VERTICAL.value, 1)
```

### Comparing `careamics-0.1.0rc3/tests/config/test_inference_model.py` & `careamics-0.1.0rc4/tests/config/test_inference_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,125 +1,125 @@
 import pytest
 from albumentations import Compose
 
-from careamics.config.inference_model import InferenceModel
+from careamics.config.inference_model import InferenceConfig
 from careamics.config.support import (
     SupportedTransform,
 )
 from careamics.transforms import get_all_transforms
 
 
 @pytest.mark.parametrize("ext", ["nd2", "jpg", "png ", "zarr", "npy"])
 def test_wrong_extensions(minimum_inference: dict, ext: str):
     """Test that supported model raises ValueError for unsupported extensions."""
     minimum_inference["data_type"] = ext
 
     # instantiate InferenceModel model
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
 
 def test_mean_std_both_specified_or_none(minimum_inference: dict):
     """Test error raising when setting mean and std."""
     # Errors if both are None
     minimum_inference["mean"] = None
     minimum_inference["std"] = None
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
     # Error if only mean is defined
     minimum_inference["mean"] = 10.4
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
     # Error if only std is defined
     minimum_inference.pop("mean")
     minimum_inference["std"] = 10.4
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
     # No error if both are specified
     minimum_inference["mean"] = 10.4
     minimum_inference["std"] = 10.4
-    InferenceModel(**minimum_inference)
+    InferenceConfig(**minimum_inference)
 
 
 def test_tile_size(minimum_inference: dict):
     """Test that non-zero even patch size are accepted."""
     # no tiling
-    prediction_model = InferenceModel(**minimum_inference)
+    prediction_model = InferenceConfig(**minimum_inference)
 
     # 2D
     minimum_inference["tile_size"] = [16, 8]
     minimum_inference["tile_overlap"] = [2, 2]
     minimum_inference["axes"] = "YX"
 
-    prediction_model = InferenceModel(**minimum_inference)
+    prediction_model = InferenceConfig(**minimum_inference)
     assert prediction_model.tile_size == minimum_inference["tile_size"]
     assert prediction_model.tile_overlap == minimum_inference["tile_overlap"]
 
     # 3D
     minimum_inference["tile_size"] = [16, 8, 32]
     minimum_inference["tile_overlap"] = [2, 2, 2]
     minimum_inference["axes"] = "ZYX"
 
-    prediction_model = InferenceModel(**minimum_inference)
+    prediction_model = InferenceConfig(**minimum_inference)
     assert prediction_model.tile_size == minimum_inference["tile_size"]
     assert prediction_model.tile_overlap == minimum_inference["tile_overlap"]
 
 
 @pytest.mark.parametrize(
     "tile_size", [[12], [0, 12, 12], [12, 12, 13], [12, 12, 12, 12]]
 )
 def test_wrong_tile_size(minimum_inference: dict, tile_size):
     """Test that wrong patch sizes are not accepted (zero or odd, dims 1 or > 3)."""
     minimum_inference["axes"] = "ZYX" if len(tile_size) == 3 else "YX"
     minimum_inference["tile_size"] = tile_size
 
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
 
 @pytest.mark.parametrize(
     "tile_size, tile_overlap", [([12, 12], [2, 2, 2]), ([12, 12, 12], [14, 2, 2])]
 )
 def test_wrong_tile_overlap(minimum_inference: dict, tile_size, tile_overlap):
     """Test that wrong patch sizes are not accepted (zero or odd, dims 1 or > 3)."""
     minimum_inference["axes"] = "ZYX" if len(tile_size) == 3 else "YX"
     minimum_inference["tile_size"] = tile_size
     minimum_inference["tile_overlap"] = tile_overlap
 
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
 
 def test_set_3d(minimum_inference: dict):
     """Test that 3D can be set."""
     minimum_inference["tile_size"] = [64, 64]
     minimum_inference["tile_overlap"] = [32, 32]
 
-    pred = InferenceModel(**minimum_inference)
+    pred = InferenceConfig(**minimum_inference)
     assert "Z" not in pred.axes
     assert len(pred.tile_size) == 2
     assert len(pred.tile_overlap) == 2
 
     # error if changing Z manually
     with pytest.raises(ValueError):
         pred.axes = "ZYX"
 
     # or patch size
-    pred = InferenceModel(**minimum_inference)
+    pred = InferenceConfig(**minimum_inference)
     with pytest.raises(ValueError):
         pred.tile_size = [64, 64, 64]
 
     with pytest.raises(ValueError):
         pred.tile_overlap = [64, 64, 64]
 
     # set 3D
-    pred = InferenceModel(**minimum_inference)
+    pred = InferenceConfig(**minimum_inference)
     pred.set_3D("ZYX", [64, 64, 64], [32, 32, 32])
     assert "Z" in pred.axes
     assert len(pred.tile_size) == 3
     assert len(pred.tile_overlap) == 3
 
 
 @pytest.mark.parametrize(
@@ -129,57 +129,57 @@
             {"name": SupportedTransform.NORMALIZE.value},
         ],
     ],
 )
 def test_passing_supported_transforms(minimum_inference: dict, transforms):
     """Test that list of supported transforms can be passed."""
     minimum_inference["transforms"] = transforms
-    InferenceModel(**minimum_inference)
+    InferenceConfig(**minimum_inference)
 
 
 def test_cannot_pass_n2v_manipulate(minimum_inference: dict):
     """Test that passing N2V pixel manipulate transform raises an error."""
     minimum_inference["transforms"] = [
         {"name": SupportedTransform.N2V_MANIPULATE.value},
     ]
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
 
 def test_passing_empty_transforms(minimum_inference: dict):
     """Test that empty list of transforms can be passed."""
     minimum_inference["transforms"] = []
-    InferenceModel(**minimum_inference)
+    InferenceConfig(**minimum_inference)
 
 
 def test_passing_incorrect_element(minimum_inference: dict):
     """Test that incorrect element in the list of transforms raises an error (
     e.g. passing un object rather than a string)."""
     minimum_inference["transforms"] = [
         {"name": get_all_transforms()[SupportedTransform.NDFLIP.value]()},
     ]
     with pytest.raises(ValueError):
-        InferenceModel(**minimum_inference)
+        InferenceConfig(**minimum_inference)
 
 
 def test_passing_compose_transform(minimum_inference: dict):
     """Test that Compose transform can be passed."""
     minimum_inference["transforms"] = Compose(
         [
             get_all_transforms()[SupportedTransform.NORMALIZE](mean=10.4, std=3.2),
             get_all_transforms()[SupportedTransform.NDFLIP](),
         ]
     )
-    InferenceModel(**minimum_inference)
+    InferenceConfig(**minimum_inference)
 
 
 def test_mean_and_std_in_normalize(minimum_inference: dict):
     """Test that mean and std are added to the Normalize transform."""
     minimum_inference["mean"] = 10.4
     minimum_inference["std"] = 3.2
     minimum_inference["transforms"] = [
         {"name": SupportedTransform.NORMALIZE.value},
     ]
 
-    data = InferenceModel(**minimum_inference)
+    data = InferenceConfig(**minimum_inference)
     assert data.transforms[0].mean == 10.4
     assert data.transforms[0].std == 3.2
```

### Comparing `careamics-0.1.0rc3/tests/config/test_optimizers_model.py` & `careamics-0.1.0rc4/tests/config/test_optimizers_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 
 
 @pytest.mark.parametrize(
     "optimizer_name, parameters",
     [
         (
-            SupportedOptimizer.Adam.value,
+            SupportedOptimizer.ADAM.value,
             {
                 "lr": 0.08,
                 "betas": (0.1, 0.11),
                 "eps": 6e-08,
                 "weight_decay": 0.2,
                 "amsgrad": True,
             },
@@ -61,15 +61,15 @@
     )
     assert optimizer.parameters == {"lr": 0.1}
 
 
 def test_optimizer_wrong_values_by_assignments():
     """Test that wrong values cause an error during assignment."""
     optimizer = OptimizerModel(
-        name=SupportedOptimizer.Adam.value, parameters={"lr": 0.08}
+        name=SupportedOptimizer.ADAM.value, parameters={"lr": 0.08}
     )
 
     # name
     optimizer.name = SupportedOptimizer.SGD.value
     with pytest.raises(ValueError):
         optimizer.name = "MyOptim"
 
@@ -93,28 +93,28 @@
     assert optim_minimum == config
 
 
 @pytest.mark.parametrize(
     "lr_scheduler_name, parameters",
     [
         (
-            SupportedScheduler.ReduceLROnPlateau.value,
+            SupportedScheduler.REDUCE_LR_ON_PLATEAU.value,
             {
                 "mode": "max",
                 "factor": 0.3,
                 "patience": 5,
                 "threshold": 0.003,
                 "threshold_mode": "abs",
                 "cooldown": 3,
                 "min_lr": 0.1,
                 "eps": 5e-08,
             },
         ),
         (
-            SupportedScheduler.StepLR.value,
+            SupportedScheduler.STEP_LR.value,
             {
                 "step_size": 2,
                 "gamma": 0.3,
                 "last_epoch": -5,
             },
         ),
     ],
@@ -133,14 +133,14 @@
     lr_scheduler = LrSchedulerModel(name=lr_scheduler_name, parameters=new_parameters)
     assert lr_scheduler.parameters == parameters
 
 
 def test_scheduler_missing_parameter():
     """Test that StepLR scheduler fails if `step_size` is not provided"""
     with pytest.raises(ValueError):
-        LrSchedulerModel(name=SupportedScheduler.StepLR.value, parameters={})
+        LrSchedulerModel(name=SupportedScheduler.STEP_LR.value, parameters={})
 
     # test that it works if lr is provided
     lr_scheduler = LrSchedulerModel(
-        name=SupportedScheduler.StepLR.value, parameters={"step_size": "5"}
+        name=SupportedScheduler.STEP_LR.value, parameters={"step_size": "5"}
     )
     assert lr_scheduler.parameters == {"step_size": "5"}
```

### Comparing `careamics-0.1.0rc3/tests/config/test_tile_information.py` & `careamics-0.1.0rc4/tests/config/test_tile_information.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/architectures/test_custom_model.py` & `careamics-0.1.0rc4/tests/config/architectures/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/architectures/test_register_model.py` & `careamics-0.1.0rc4/tests/config/architectures/test_register_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/architectures/test_unet_model.py` & `careamics-0.1.0rc4/tests/config/architectures/test_unet_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/support/test_supported_data.py` & `careamics-0.1.0rc4/tests/config/support/test_supported_data.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/support/test_supported_optimizers.py` & `careamics-0.1.0rc4/tests/config/support/test_supported_optimizers.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/transformations/test_n2v_manipulate_model.py` & `careamics-0.1.0rc4/tests/config/transformations/test_n2v_manipulate_model.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/config/validators/test_validator_utils.py` & `careamics-0.1.0rc4/tests/config/validators/test_validator_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/test_in_memory_dataset.py` & `careamics-0.1.0rc4/tests/dataset/test_in_memory_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 import tifffile
 
-from careamics.config import DataModel
+from careamics.config import DataConfig
 from careamics.config.support import SupportedData
 from careamics.dataset import InMemoryDataset
 
 
 def test_number_of_patches(ordered_array):
     """Test the number of patches extracted from InMemoryDataset."""
     # create array
@@ -14,15 +14,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.ARRAY.value,
         "patch_size": [8, 8],
         "axes": "YX",
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = InMemoryDataset(
         data_config=config,
         inputs=array,
     )
 
@@ -44,15 +44,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.ARRAY.value,
         "patch_size": [8, 8],
         "axes": "YX",
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = InMemoryDataset(
         data_config=config,
         inputs=array,
     )
 
@@ -84,15 +84,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.ARRAY.value,
         "patch_size": [8, 8],
         "axes": "YX",
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = InMemoryDataset(
         data_config=config,
         inputs=[file_path],
     )
```

### Comparing `careamics-0.1.0rc3/tests/dataset/test_iterable_dataset.py` & `careamics-0.1.0rc4/tests/dataset/test_iterable_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 import tifffile
 
-from careamics.config import DataModel
+from careamics.config import DataConfig
 from careamics.config.support import SupportedData
 from careamics.dataset import PathIterableDataset
 from careamics.dataset.dataset_utils import read_tiff
 
 
 @pytest.mark.parametrize(
     "shape",
@@ -37,15 +37,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.TIFF.value,
         "patch_size": patch_sizes,
         "axes": axes,
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = PathIterableDataset(
         data_config=config, src_files=files, read_source_func=read_tiff
     )
 
     # check number of files
@@ -80,15 +80,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.CUSTOM.value,
         "patch_size": patch_sizes,
         "axes": "YX",
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = PathIterableDataset(
         data_config=config,
         src_files=files,
         read_source_func=read_npy,
     )
@@ -114,15 +114,15 @@
 
     # create config
     config_dict = {
         "data_type": SupportedData.TIFF.value,
         "patch_size": [8, 8],
         "axes": "YX",
     }
-    config = DataModel(**config_dict)
+    config = DataConfig(**config_dict)
 
     # create dataset
     dataset = PathIterableDataset(
         data_config=config, src_files=files, read_source_func=read_tiff
     )
 
     # compute number of patches
```

### Comparing `careamics-0.1.0rc3/tests/dataset/dataset_utils/test_list_files.py` & `careamics-0.1.0rc4/tests/dataset/dataset_utils/test_list_files.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/dataset_utils/test_read_tiff.py` & `careamics-0.1.0rc4/tests/dataset/dataset_utils/test_read_tiff.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/patching/test_patching_utils.py` & `careamics-0.1.0rc4/tests/dataset/patching/test_patching_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/patching/test_random_patching.py` & `careamics-0.1.0rc4/tests/dataset/patching/test_random_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/patching/test_sequential_patching.py` & `careamics-0.1.0rc4/tests/dataset/patching/test_sequential_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/dataset/patching/test_tiled_patching.py` & `careamics-0.1.0rc4/tests/dataset/patching/test_tiled_patching.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/model_io/test_bmz_io.py` & `careamics-0.1.0rc4/tests/model_io/test_bmz_io.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/models/test_model_factory.py` & `careamics-0.1.0rc4/tests/models/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/models/test_unet.py` & `careamics-0.1.0rc4/tests/models/test_unet.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/prediction/test_stitch_prediction.py` & `careamics-0.1.0rc4/tests/prediction/test_stitch_prediction.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/transforms/test_manipulate_n2v.py` & `careamics-0.1.0rc4/tests/transforms/test_manipulate_n2v.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/transforms/test_nd_flip.py` & `careamics-0.1.0rc4/tests/transforms/test_nd_flip.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/transforms/test_normalize.py` & `careamics-0.1.0rc4/tests/transforms/test_normalize.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/transforms/test_pixel_manipulation.py` & `careamics-0.1.0rc4/tests/transforms/test_pixel_manipulation.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/transforms/test_xy_random_rotate90.py` & `careamics-0.1.0rc4/tests/transforms/test_xy_random_rotate90.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/utils/test_context.py` & `careamics-0.1.0rc4/tests/utils/test_context.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/utils/test_logging.py` & `careamics-0.1.0rc4/tests/utils/test_logging.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/utils/test_metrics.py` & `careamics-0.1.0rc4/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/utils/test_torch_utils.py` & `careamics-0.1.0rc4/tests/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/tests/utils/test_wandb.py` & `careamics-0.1.0rc4/tests/utils/test_wandb.py`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/LICENSE` & `careamics-0.1.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/README.md` & `careamics-0.1.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/pyproject.toml` & `careamics-0.1.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `careamics-0.1.0rc3/PKG-INFO` & `careamics-0.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: careamics
-Version: 0.1.0rc3
+Version: 0.1.0rc4
 Summary: Toolbox for running N2V and friends.
 Project-URL: homepage, https://careamics.github.io/
 Project-URL: repository, https://github.com/CAREamics/careamics
 Author-email: Igor Zubarev <igor.zubarev@fht.org>, Joran Deschamps <joran.deschamps@fht.org>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: careamics Version: 0.1.0rc3 Summary: Toolbox for
+Metadata-Version: 2.3 Name: careamics Version: 0.1.0rc4 Summary: Toolbox for
 running N2V and friends. Project-URL: homepage, https://careamics.github.io/
 Project-URL: repository, https://github.com/CAREamics/careamics Author-email:
 Igor Zubarev
 fht.org>, Joran Deschamps
 fht.org> License: BSD-3-Clause License-File: LICENSE Classifier: Development
 Status :: 3 - Alpha Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

