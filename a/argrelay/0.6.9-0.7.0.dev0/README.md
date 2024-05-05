# Comparing `tmp/argrelay-0.6.9.tar.gz` & `tmp/argrelay-0.7.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argrelay-0.6.9.tar", last modified: Sat Mar 16 19:19:34 2024, max compression
+gzip compressed data, was "argrelay-0.7.0.dev0.tar", last modified: Sun May  5 09:58:43 2024, max compression
```

## Comparing `argrelay-0.6.9.tar` & `argrelay-0.7.0.dev0.tar`

### file list

```diff
@@ -1,396 +1,414 @@
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.630345 argrelay-0.6.9/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.6.9/LICENSE
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1127 2024-03-16 19:19:34.630345 argrelay-0.6.9/PKG-INFO
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.595345 argrelay-0.6.9/docs/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.596345 argrelay-0.6.9/docs/dev_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5523 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.1.project_creation.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/brief_history.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/code_style.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/dev_notes/completion_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/completion_perf_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/gui_tests_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/how_search_works.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/library_vs_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/mongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/next_steps_tutorial.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/origin_story.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_10_x_more_data_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_cache_vs_no_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_mongomock_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/dev_notes/query_perf_pymongo_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/dev_notes/release_procedure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/screencast_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/scripts_summary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/semver_notes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5694 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/term_dictionary.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11130 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/top_todos.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/dev_notes/version_format.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.602345 argrelay-0.6.9/docs/feature_stories/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_01_89_09_24.interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_14_59_14_06.pending_requests.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      886 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_15_79_76_85.line_processor.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1470 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      956 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_20_88_05_60.named_args.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_26_43_73_72.func_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_29_54_67_86.dir_structure.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_31_70_49_15.search_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      628 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_33_76_82_84.global_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1135 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_36_17_84_44.check_script.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_39_58_01_91.query_cache.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_46_96_59_05.init_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1280 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_47_63_35_61.env_vars.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.6.9/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1557 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_55_57_45_04.enum_selector.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1756 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_58_61_77_69.dev_shell.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_62_25_92_06.assigned_context.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_63_63_14_08.generated_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_66_17_43_42.test_infra.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_67_16_61_97.git_plugin.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_71_87_33_52.help_hint.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_72_40_53_00.fill_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_78_91_27_22.interp_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4506 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1729 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_91_88_07_23.jump_tree.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.6.9/docs/feature_stories/FS_94_30_49_28.help_doc.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_98_55_40_77.invoke_control.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/feature_stories/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.604345 argrelay-0.6.9/docs/release_notes/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev0.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev27.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev28.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.dev42.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.0.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.1.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.2.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.2.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.3.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.4.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.5.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.0.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.1.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.2.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.3.final.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/release_notes/v0.6.4.final.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.606345 argrelay-0.6.9/docs/task_refs/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      420 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2977 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_unconsumed_arg_vals.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      648 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2669 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-13 15:11:16.000000 argrelay-0.6.9/docs/task_refs/readme.md
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/docs/test_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.6.9/docs/test_data/TD_38_03_48_51.large_data_set.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10511 2024-03-13 15:12:40.000000 argrelay-0.6.9/docs/test_data/TD_63_37_05_36.demo_services_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.6.9/docs/test_data/TD_70_69_38_46.no_data.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-16 19:14:19.000000 argrelay-0.6.9/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.6.9/docs/test_data/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.6.9/pyproject.toml
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14598 2024-03-13 15:12:40.000000 argrelay-0.6.9/readme.md
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-03-16 19:19:34.630345 argrelay-0.6.9/setup.cfg
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4177 2024-03-16 19:14:19.000000 argrelay-0.6.9/setup.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.593345 argrelay-0.6.9/src/
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/src/argrelay/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_command_local/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/AbstractLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/client_command_local/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_command_remote/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3936 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/client_command_remote/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.608345 argrelay-0.6.9/src/argrelay/client_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3749 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_spec/ShellContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/client_spec/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.610345 argrelay-0.6.9/src/argrelay/custom_integ/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8495 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2326 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3640 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3511 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1597 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/FuncConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8391 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1849 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12645 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1605 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      830 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    16189 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    65313 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/custom_integ/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/git_utils.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      371 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/custom_integ/value_constants.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.611345 argrelay-0.6.9/src/argrelay/custom_integ_res/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7005 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_common_lib.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8106 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_rc.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    32228 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3392 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/dev_shell.bash
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3672 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/init_shell_env.bash
--rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2644 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/custom_integ_res/upgrade_all_packages.bash
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.612345 argrelay-0.6.9/src/argrelay/enum_desc/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ArgSource.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CallConv.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CompScope.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/CompType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/enum_desc/DistinctValuesQuery.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/InterpStep.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/PluginType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ReservedArgType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ReservedEnvelopeClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/RunMode.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/ServerAction.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      105 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/SpecialChar.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/SpecialFunc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2905 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/TermColor.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/enum_desc/TokenType.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/enum_desc/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.612345 argrelay-0.6.9/src/argrelay/handler_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/AbstractServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1535 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/handler_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/handler_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/AbstractClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9137 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/handler_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/misc_helper_common/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/ElapsedTime.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/TypeDesc.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1550 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_common/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.613345 argrelay-0.6.9/src/argrelay/misc_helper_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/misc_helper_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.614345 argrelay-0.6.9/src/argrelay/mongo_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoClientWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/mongo_data/MongoServerWrapper.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/mongo_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.614345 argrelay-0.6.9/src/argrelay/plugin_config/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/AbstractConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfigurator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_config/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.615345 argrelay-0.6.9/src/argrelay/plugin_delegator/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3147 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2418 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/EchoDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1847 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5882 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/HelpDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5639 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/InterceptDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1201 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/NoopDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/QueryEnumDelegator.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.6.9/src/argrelay/plugin_delegator/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.616345 argrelay-0.6.9/src/argrelay/plugin_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3680 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4862 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    15370 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11293 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1449 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7437 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5262 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2805 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterpFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7555 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_interp/TreeWalker.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/plugin_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.617345 argrelay-0.6.9/src/argrelay/plugin_loader/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/plugin_loader/AbstractLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.6.9/src/argrelay/plugin_loader/NoopLoader.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/plugin_loader/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.618345 argrelay-0.6.9/src/argrelay/relay_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      967 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClientCommand.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/AbstractClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.6.9/src/argrelay/relay_client/RemoteClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/RemoteClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.6.9/src/argrelay/relay_client/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4629 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/__main__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3702 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/proc_parent.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2102 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_client/proc_split.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-16 18:22:38.000000 argrelay-0.6.9/src/argrelay/relay_server/CustomFlaskApp.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/GuiBannerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/HelpHintCache.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/LocalServer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryCacheConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryEngine.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/QueryResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.6.9/src/argrelay/relay_server/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/relay_server/__main__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/gui_static/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_client.js
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-03-13 15:12:40.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_style.css
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_static/external_link.svg
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.619345 argrelay-0.6.9/src/argrelay/relay_server/gui_templates/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/gui_templates/argrelay_main.html
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4948 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/route_api.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/relay_server/route_gui.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.620345 argrelay-0.6.9/src/argrelay/runtime_context/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2841 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/AbstractPlugin.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4186 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/runtime_context/EnvelopeContainer.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_context/InitControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14498 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/runtime_context/InterpContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5861 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/ParsedContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_context/SearchControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/runtime_context/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/runtime_data/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_data/AssignedValue.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      376 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ClientConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-01-17 14:42:50.000000 argrelay-0.6.9/src/argrelay/runtime_data/ConnectionConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/EnvelopeCollection.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/PluginEntry.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ServerConfig.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/ServerPluginControl.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/runtime_data/StaticData.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.6.9/src/argrelay/runtime_data/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/sample_conf/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/sample_conf/argrelay.client.json
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31479 2024-03-16 14:33:33.000000 argrelay-0.6.9/src/argrelay/sample_conf/argrelay.server.yaml
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.621345 argrelay-0.6.9/src/argrelay/schema_config_core_client/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2690 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/ClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1094 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_core_client/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.622345 argrelay-0.6.9/src/argrelay/schema_config_core_server/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3001 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      890 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1104 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2226 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1279 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1301 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6951 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerConfigSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1630 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1249 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/StaticDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_core_server/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_config_interp/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1073 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/InitControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3158 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/SearchControlSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_interp/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_config_plugin/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2284 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_config_plugin/PluginEntrySchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_config_plugin/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.623345 argrelay-0.6.9/src/argrelay/schema_request/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3285 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_request/CallContextSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_request/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.624345 argrelay-0.6.9/src/argrelay/schema_response/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/ArgValues.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1625 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/ArgValuesSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1417 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/AssignedValueSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3087 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/EnvelopeContainerSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1311 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InterpResult.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2371 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InterpResultSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      950 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InvocationInput.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1732 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/schema_response/InvocationInputSchema.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.6.9/src/argrelay/schema_response/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.624345 argrelay-0.6.9/src/argrelay/server_spec/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/CallContext.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/DescribeLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/ProposeArgValuesSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/RelayLineArgsSpec.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.6.9/src/argrelay/server_spec/__init__.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/const_int.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/server_spec/server_data_schema.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.626345 argrelay-0.6.9/src/argrelay/test_infra/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/BaseTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/ClientServerTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/CustomTestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/CustomVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/End2EndTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37631 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/EnvMockBuilder.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11214 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/InOutTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/JsonTestOutputVerifier.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalClient.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalClientCommandFactory.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4818 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/LocalTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/OpenFileMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3419 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/PopenMock.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4365 2024-03-16 19:14:19.000000 argrelay-0.6.9/src/argrelay/test_infra/RemoteTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/ServerOnlyTestClass.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/TestCase.py
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-13 15:11:16.000000 argrelay-0.6.9/src/argrelay/test_infra/__init__.py
-drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-03-16 19:19:34.607345 argrelay-0.6.9/src/argrelay.egg-info/
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1127 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/PKG-INFO
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    30872 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/SOURCES.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/dependency_links.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      171 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/requires.txt
--rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-03-16 19:19:34.000000 argrelay-0.6.9/src/argrelay.egg-info/top_level.txt
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.435866 argrelay-0.7.0.dev0/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11346 2022-12-27 20:38:16.000000 argrelay-0.7.0.dev0/LICENSE
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-05 09:58:43.435866 argrelay-0.7.0.dev0/PKG-INFO
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.405867 argrelay-0.7.0.dev0/docs/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.407867 argrelay-0.7.0.dev0/docs/dev_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5523 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.1.project_creation.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2509 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1924 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1243 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/brief_history.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2781 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/code_style.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      734 2024-01-17 14:42:50.000000 argrelay-0.7.0.dev0/docs/dev_notes/completion_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6986 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/completion_perf_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/dev_notes/gui_tests_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5196 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/how_search_works.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2495 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/library_vs_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/mongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1469 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/next_steps_tutorial.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3776 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/origin_story.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7809 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/query_perf_10_x_more_data_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7149 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/query_perf_cache_vs_no_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4285 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/query_perf_mongomock_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8388 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/query_perf_pymongo_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1736 2024-01-17 14:42:50.000000 argrelay-0.7.0.dev0/docs/dev_notes/release_procedure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      769 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/screencast_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      787 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/scripts_summary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/semver_notes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5697 2024-04-30 17:59:55.000000 argrelay-0.7.0.dev0/docs/dev_notes/term_dictionary.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11129 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/dev_notes/top_todos.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3241 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/dev_notes/version_format.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.411867 argrelay-0.7.0.dev0/docs/feature_stories/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3725 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_00_13_77_97.plugin_framework.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_01_89_09_24.interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      778 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2912 2024-04-21 14:23:13.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_06_99_43_60.list_arg_value.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      228 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_07_10_10_74.relay_to_another_server.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1839 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      994 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      770 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_14_59_14_06.pending_requests.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      886 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_15_79_76_85.line_processor.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1470 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1028 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      761 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_20_88_05_60.named_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1914 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      917 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_26_43_73_72.func_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1321 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_27_16_67_19.line_syntax.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3596 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_29_54_67_86.dir_structure.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1029 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_31_70_49_15.search_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      393 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      649 2024-04-30 17:59:55.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_33_76_82_84.composite_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1230 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_36_17_84_44.check_script.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1764 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      849 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_39_58_01_91.query_cache.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1739 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1450 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      296 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_43_50_57_71.echo_args_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      792 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      424 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_46_96_59_05.init_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1280 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_47_63_35_61.env_vars.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1348 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      379 2023-07-22 05:41:07.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_53_81_66_18.types_and_classes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1556 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_55_57_45_04.enum_selector.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2481 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1756 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      758 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_58_61_77_69.dev_shell.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      751 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1457 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_62_25_92_06.assigned_context.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1211 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_63_63_14_08.generated_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1889 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_66_17_43_42.test_infra.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2246 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_67_16_61_97.git_plugin.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1507 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_71_87_33_52.help_hint.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1916 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_72_40_53_00.fill_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_72_53_55_13.show_non_default_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_74_69_61_79.get_set_data_envelope.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1370 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      155 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_78_91_27_22.interp_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1306 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_80_45_89_81.integrated_functions.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2391 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2089 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4506 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      493 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1841 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1735 2024-04-30 17:59:55.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_91_88_07_23.jump_tree.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3287 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_92_75_93_01.clean_command_line.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      504 2024-01-17 14:42:50.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_94_30_49_28.help_doc.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1653 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_97_64_39_94.arg_buckets.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      189 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_98_55_40_77.invoke_control.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      505 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      454 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/feature_stories/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      637 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.412867 argrelay-0.7.0.dev0/docs/release_notes/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1240 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      165 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.dev0.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1368 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.dev27.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.dev28.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      133 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.dev42.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      269 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       37 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.1.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       98 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.2.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       75 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.2.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      124 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.3.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      273 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.4.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      328 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.5.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      136 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.5.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      245 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.5.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      403 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.6.0.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      411 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.6.1.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      110 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.6.2.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       62 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.6.3.final.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      143 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/release_notes/v0.6.4.final.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.414867 argrelay-0.7.0.dev0/docs/task_refs/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      573 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      336 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_04_84_79_11.reorganize_tests_for_CI.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      689 2024-04-30 17:59:55.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      277 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      420 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2979 2024-04-30 17:59:55.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      343 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      206 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      459 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      388 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      352 2024-05-05 04:41:56.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      221 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      349 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      560 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       85 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      703 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      497 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      640 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      224 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      439 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      422 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      304 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      170 2024-04-30 18:02:47.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      187 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      456 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      648 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2669 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      256 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/docs/task_refs/readme.md
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.415867 argrelay-0.7.0.dev0/docs/test_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      695 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      395 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/docs/test_data/TD_38_03_48_51.large_data_set.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      387 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/test_data/TD_43_24_76_58.single_value_multiple_envelopes.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11158 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/test_data/TD_63_37_05_36.demo_services_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      531 2023-07-22 05:41:07.000000 argrelay-0.7.0.dev0/docs/test_data/TD_70_69_38_46.no_data.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      550 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      960 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       78 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/docs/test_data/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       87 2022-12-27 20:32:06.000000 argrelay-0.7.0.dev0/pyproject.toml
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    14879 2024-05-05 09:51:09.000000 argrelay-0.7.0.dev0/readme.md
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       38 2024-05-05 09:58:43.435866 argrelay-0.7.0.dev0/setup.cfg
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4217 2024-05-05 09:52:34.000000 argrelay-0.7.0.dev0/setup.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.404867 argrelay-0.7.0.dev0/src/
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.415867 argrelay-0.7.0.dev0/src/argrelay/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.415867 argrelay-0.7.0.dev0/src/argrelay/client_command_local/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1714 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_local/AbstractLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1018 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      997 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_local/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.416867 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2304 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      857 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3936 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      854 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/client_command_remote/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.416867 argrelay-0.7.0.dev0/src/argrelay/client_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3749 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/client_spec/ShellContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/client_spec/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.417867 argrelay-0.7.0.dev0/src/argrelay/composite_tree/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      344 2024-05-05 03:55:12.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeForest.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1138 2024-05-05 05:18:34.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeForestSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2071 2024-05-05 08:20:35.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeInfoType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1144 2024-05-05 09:20:09.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeNode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-05-05 09:22:20.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeNodeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      657 2024-05-05 09:25:26.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeNodeType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13830 2024-05-05 08:17:20.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/CompositeTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    10886 2024-05-04 18:24:05.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/DictTreeWalker.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/composite_tree/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.418866 argrelay-0.7.0.dev0/src/argrelay/custom_integ/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8164 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/BaseConfigDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      996 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2325 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3643 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3533 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1598 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1737 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/FuncConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1492 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8075 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1869 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12644 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1615 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      853 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    18325 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      217 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    69098 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      842 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2512 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/git_utils.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      413 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ/value_constants.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.419867 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7005 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/argrelay_common_lib.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     8106 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/argrelay_rc.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)    32319 2024-05-05 02:41:54.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/bootstrap_dev_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     3392 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/dev_shell.bash
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3672 2024-04-22 16:25:03.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/init_shell_env.bash
+-rwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)     2644 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/upgrade_all_packages.bash
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.420867 argrelay-0.7.0.dev0/src/argrelay/enum_desc/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1313 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/ArgSource.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1011 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/CallConv.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1498 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/CompScope.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2952 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/CompType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4670 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/DistinctValuesQuery.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      414 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/InterpStep.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      470 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/PluginType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      547 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/ReservedArgType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      190 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/ReservedEnvelopeClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1707 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/RunMode.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      468 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/ServerAction.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      390 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/SpecialChar.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      511 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/SpecialFunc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3091 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/TermColor.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1259 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/TokenType.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/enum_desc/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.420867 argrelay-0.7.0.dev0/src/argrelay/handler_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/handler_request/AbstractServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1156 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      986 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3103 2024-04-22 16:25:28.000000 argrelay-0.7.0.dev0/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/handler_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.421867 argrelay-0.7.0.dev0/src/argrelay/handler_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      200 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/handler_response/AbstractClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     9401 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1122 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1023 2024-04-13 16:33:00.000000 argrelay-0.7.0.dev0/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/handler_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.421867 argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1954 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/ElapsedTime.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      741 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/ObjectSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/TypeDesc.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1269 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.421867 argrelay-0.7.0.dev0/src/argrelay/misc_helper_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      521 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/misc_helper_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.421867 argrelay-0.7.0.dev0/src/argrelay/mongo_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      198 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3649 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoClientWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      616 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      347 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2086 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoServerWrapper.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.0.dev0/src/argrelay/mongo_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.422866 argrelay-0.7.0.dev0/src/argrelay/plugin_config/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4367 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_config/AbstractConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4265 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfigurator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1555 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_config/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.423867 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5958 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/AbstractDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4075 2024-05-05 05:58:59.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1697 2024-05-05 05:12:16.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2087 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/EchoDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1516 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/ErrorDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      814 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5791 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/HelpDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5308 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/InterceptDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      870 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/NoopDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1813 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/QueryEnumDelegator.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-08-06 08:09:50.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.424867 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3681 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/AbstractInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2278 2024-04-22 16:25:28.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/AbstractInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      701 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5365 2024-05-05 08:19:11.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1349 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17429 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12627 2024-05-05 06:51:51.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1684 2024-05-05 05:00:26.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7762 2024-05-05 09:35:06.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     5952 2024-05-05 08:18:33.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2925 2024-05-05 05:00:26.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      384 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/NoopInterp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1389 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/NoopInterpFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.424867 argrelay-0.7.0.dev0/src/argrelay/plugin_loader/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      426 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_loader/AbstractLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      281 2023-12-14 14:18:48.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_loader/NoopLoader.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/plugin_loader/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.424867 argrelay-0.7.0.dev0/src/argrelay/relay_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      967 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/AbstractClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      366 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/AbstractClientCommand.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      266 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/AbstractClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      636 2023-10-21 04:19:27.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/RemoteClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1861 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/RemoteClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      118 2022-12-27 20:32:06.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4703 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/__main__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3702 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/proc_parent.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2102 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_client/proc_split.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.425866 argrelay-0.7.0.dev0/src/argrelay/relay_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    11191 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/CustomFlaskApp.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      139 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/GuiBannerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1500 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/HelpHintCache.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7312 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/LocalServer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      251 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/QueryCacheConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    13331 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/QueryEngine.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1147 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/QueryResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      123 2022-12-27 20:32:06.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      163 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/__main__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.425866 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31127 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/argrelay_client.js
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      318 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/argrelay_favicon.ico
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4987 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/argrelay_style.css
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      265 2024-01-17 14:42:50.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/external_link.svg
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.426867 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_templates/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7812 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_templates/argrelay_main.html
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4947 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/route_api.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1894 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/relay_server/route_gui.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.426867 argrelay-0.7.0.dev0/src/argrelay/runtime_context/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3180 2024-05-05 06:01:48.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/AbstractPlugin.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4398 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/EnvelopeContainer.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      225 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/InitControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    17397 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/InterpContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6354 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/ParsedContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2343 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/SearchControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      440 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_context/arg_buckets_utils.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.427867 argrelay-0.7.0.dev0/src/argrelay/runtime_data/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      192 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/AssignedValue.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      407 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/ClientConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      167 2024-03-18 13:46:05.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/ConnectionConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      549 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/EnvelopeCollection.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      313 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/PluginEntry.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3457 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/ServerConfig.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      455 2024-05-05 02:54:47.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/ServerPluginControl.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      556 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/StaticData.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-03-06 12:58:57.000000 argrelay-0.7.0.dev0/src/argrelay/runtime_data/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.427867 argrelay-0.7.0.dev0/src/argrelay/sample_conf/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      207 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/sample_conf/argrelay.client.json
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    35309 2024-05-05 08:13:45.000000 argrelay-0.7.0.dev0/src/argrelay/sample_conf/argrelay.server.yaml
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.427867 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2370 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/ClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1005 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.428866 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2839 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      736 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/GuiBannerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      976 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1767 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1068 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1054 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     6371 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/ServerConfigSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1822 2024-05-05 02:54:47.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1148 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/StaticDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        0 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.428866 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4775 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/DataEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1968 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1544 2024-04-22 16:25:28.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      953 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/InitControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2943 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/SearchControlSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.428866 argrelay-0.7.0.dev0/src/argrelay/schema_config_plugin/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1465 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_plugin/PluginEntrySchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_config_plugin/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.428866 argrelay-0.7.0.dev0/src/argrelay/schema_request/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2310 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_request/CallContextSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_request/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.429866 argrelay-0.7.0.dev0/src/argrelay/schema_response/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      272 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/ArgValues.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1221 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/ArgValuesSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      897 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/AssignedValueSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2763 2024-04-30 17:59:54.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/EnvelopeContainerSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2433 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/InterpResult.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2217 2024-04-30 17:59:50.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/InterpResultSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1802 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/InvocationInput.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1355 2024-04-30 17:59:50.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/InvocationInputSchema.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-15 14:33:40.000000 argrelay-0.7.0.dev0/src/argrelay/schema_response/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.429866 argrelay-0.7.0.dev0/src/argrelay/server_spec/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1066 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/CallContext.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1752 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/DescribeLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1356 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/ProposeArgValuesSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1410 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/RelayLineArgsSpec.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        8 2023-01-03 11:36:47.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/__init__.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      612 2024-03-18 13:48:29.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/const_int.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3140 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/server_spec/server_data_schema.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.431867 argrelay-0.7.0.dev0/src/argrelay/test_infra/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      804 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/BaseTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2886 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/ClientServerTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1435 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/CustomTestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2039 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/CustomVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     7157 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/End2EndTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    37737 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/EnvMockBuilder.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    12616 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/InOutTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1425 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/JsonTestOutputVerifier.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1374 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalClient.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2785 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalClientCommandFactory.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4990 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      822 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/OpenFileMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     3449 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/PopenMock.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     4519 2024-04-23 14:23:44.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/RemoteTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2353 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/ServerOnlyTestClass.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1375 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/TestCase.py
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     2104 2024-03-18 13:51:36.000000 argrelay-0.7.0.dev0/src/argrelay/test_infra/__init__.py
+drwxr-xr-x   0 uvsmtid   (1001) uvsmtid   (1001)        0 2024-05-05 09:58:43.415867 argrelay-0.7.0.dev0/src/argrelay.egg-info/
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)     1132 2024-05-05 09:58:43.000000 argrelay-0.7.0.dev0/src/argrelay.egg-info/PKG-INFO
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)    31835 2024-05-05 09:58:43.000000 argrelay-0.7.0.dev0/src/argrelay.egg-info/SOURCES.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)        1 2024-05-05 09:58:43.000000 argrelay-0.7.0.dev0/src/argrelay.egg-info/dependency_links.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)      195 2024-05-05 09:58:43.000000 argrelay-0.7.0.dev0/src/argrelay.egg-info/requires.txt
+-rw-r--r--   0 uvsmtid   (1001) uvsmtid   (1001)       23 2024-05-05 09:58:43.000000 argrelay-0.7.0.dev0/src/argrelay.egg-info/top_level.txt
```

### Comparing `argrelay-0.6.9/LICENSE` & `argrelay-0.7.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/PKG-INFO` & `argrelay-0.7.0.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.6.9
+Version: 0.7.0.dev0
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.1.project_creation.md` & `argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.1.project_creation.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md` & `argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.2.initial_deployment.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md` & `argrelay-0.7.0.dev0/docs/dev_notes/bootstrap_procedure.3.argrelay_upgrade.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/brief_history.md` & `argrelay-0.7.0.dev0/docs/dev_notes/brief_history.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/code_style.md` & `argrelay-0.7.0.dev0/docs/dev_notes/code_style.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/completion_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/completion_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/completion_perf_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/completion_perf_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/gui_tests_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/gui_tests_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/how_search_works.md` & `argrelay-0.7.0.dev0/docs/dev_notes/how_search_works.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/library_vs_framework.md` & `argrelay-0.7.0.dev0/docs/dev_notes/library_vs_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/mongo_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/mongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/next_steps_tutorial.md` & `argrelay-0.7.0.dev0/docs/dev_notes/next_steps_tutorial.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/origin_story.md` & `argrelay-0.7.0.dev0/docs/dev_notes/origin_story.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/query_perf_10_x_more_data_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/query_perf_10_x_more_data_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/query_perf_cache_vs_no_cache.md` & `argrelay-0.7.0.dev0/docs/dev_notes/query_perf_cache_vs_no_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/query_perf_mongomock_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/query_perf_mongomock_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/query_perf_pymongo_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/query_perf_pymongo_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/release_procedure.md` & `argrelay-0.7.0.dev0/docs/dev_notes/release_procedure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/screencast_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/screencast_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/scripts_summary.md` & `argrelay-0.7.0.dev0/docs/dev_notes/scripts_summary.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/semver_notes.md` & `argrelay-0.7.0.dev0/docs/dev_notes/semver_notes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/dev_notes/term_dictionary.md` & `argrelay-0.7.0.dev0/docs/dev_notes/term_dictionary.md`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 See also FS_00_13_77_97 plugin framework.
 
 # T
 
 ### `tree_path`
 
 Tree (direct acyclic graphs with one parent per child) are often used in config - see:
-*   FS_33_76_82_84 global tree
+*   FS_33_76_82_84 composite tree
 *   FS_01_89_09_24 interp tree
 *   FS_26_43_73_72 func tree
 *   FS_91_88_07_23 jump tree
 
 For example, a tree can be expressed in YAML as:
 
 ```yaml
```

### Comparing `argrelay-0.6.9/docs/dev_notes/top_todos.md` & `argrelay-0.7.0.dev0/docs/dev_notes/top_todos.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     See also: FS_80_45_89_81 / list_envelope
     REGISTER
 
 *   Clean `#`-comments from command line arguments by parser.
     Tracked via FS_92_75_93_01.clean_command_line.md
     CLOSED
 
-*   Consumed and unconsumed tokens:
+*   Consumed and remaining tokens:
     *   Send them to invocation (e.g. to decide to run or not to run function and how they can be used).
     *   Verify them in tests.
     FINALIZE
 
 *   Meta function: list all objects of specified query.
     See also: FS_80_45_89_81 / list_envelope
     REGISTER
```

### Comparing `argrelay-0.6.9/docs/dev_notes/version_format.md` & `argrelay-0.7.0.dev0/docs/dev_notes/version_format.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_00_13_77_97.plugin_framework.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_00_13_77_97.plugin_framework.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_01_89_09_24.interp_tree.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_01_89_09_24.interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_02_25_41_81.query_enum_items_func.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_06_99_43_60.list_arg_value.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_06_99_43_60.list_arg_value.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_11_87_76_73.highlight_tangent_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_13_51_07_97.singled_out_implicit_values.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_14_59_14_06.pending_requests.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_14_59_14_06.pending_requests.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_15_79_76_85.line_processor.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_15_79_76_85.line_processor.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 
 The feature is similar to function varargs (in programming languages) -
 here, instead of arbitrary number of trailing function arguments,
 the search result for the trailing `envelop_container` may contain number of `data_envelope`-s.
 
 # Possible future
 
+TODO_75_52_01_67: `arg_bucket`-s to support multiple var args:
 Note that it is logically possible to allow any `envelope_container` search for arbitrary `data_envelope`-s,
-but this requires some (non-trivial) rules how to decide:
+but this requires some rules how to decide (using `arg_bucket`-s):
 *   where interrogation for args of curr `envelope_container` ends
 *   where interrogation for args of next `envelope_container` starts
```

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_20_88_05_60.named_args.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_20_88_05_60.named_args.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_26_43_73_72.func_tree.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_26_43_73_72.func_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_29_54_67_86.dir_structure.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_29_54_67_86.dir_structure.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_31_70_49_15.search_control.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_31_70_49_15.search_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_36_17_84_44.check_script.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_36_17_84_44.check_script.md`

 * *Files 19% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 *   server availability
 *   server version and compatibility
 *   prints server instance id and whatever we can query to verify its state
 *   print plugin list (serialized DAG) with types and activation status
 *   any useful `readline` settings set or not
 *   FS_57_36_37_48 (multiple clients) show all registered clients
 *   show all registered commands (FS_57_36_37_48 per client)
+*   print the same line info what `@/exe/dev_shell.bash` prints about version, conf, URL, etc.
 
 What else?
```

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_39_58_01_91.query_cache.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_39_58_01_91.query_cache.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_47_63_35_61.env_vars.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_47_63_35_61.env_vars.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_49_96_50_77.config_only_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_51_67_38_37.impossible_arg_combinations.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_55_57_45_04.enum_selector.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_55_57_45_04.enum_selector.md`

 * *Files 3% similar despite different names*

```diff
@@ -30,8 +30,8 @@
 These types are:
 *   discrete (limited set of values) and
 *   non-orthogonal (possible values of one type may affect/depend on already given values for another type).
 
 The arg type for the value is determined in several attempts:
 *   In case of named args, the arg type is known by its mapping from key to type.
 *   If it is positional arg, next unspecified arg type is assumed, and typed value set is checked for that value.
-*   if value is not in the arg type value set, then the value is unconsumed.
+*   if value is not in the arg type value set, then the value is remaining.
```

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_56_43_05_79.search_diff_collection.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_57_36_37_48.multiple_clients_coexistence.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_58_61_77_69.dev_shell.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_58_61_77_69.dev_shell.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_61_67_08_53.non_searchable_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_62_25_92_06.assigned_context.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_62_25_92_06.assigned_context.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_63_63_14_08.generated_config.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_63_63_14_08.generated_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_65_22_23_82.redirect_per_command.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_66_17_43_42.test_infra.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_66_17_43_42.test_infra.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_67_16_61_97.git_plugin.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_67_16_61_97.git_plugin.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_71_87_33_52.help_hint.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_71_87_33_52.help_hint.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_72_40_53_00.fill_control.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_72_40_53_00.fill_control.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_76_29_13_28.arg_consumption_priorities.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_80_45_89_81.integrated_functions.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_80_45_89_81.integrated_functions.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_80_82_13_35.option_list_on_describe_with_prefix.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_82_35_57_62.envelope_relationship_data_design.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_91_88_07_23.jump_tree.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_91_88_07_23.jump_tree.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ---
 feature_story: FS_91_88_07_23
 feature_title: jump tree
 feature_status: TEST
 ---
 
 TODO: The plan is to obsolete this feature.
-      A separate tree can be avoided - simply add configuration in FS_33_76_82_84 global tree nodes.
+      A separate tree can be avoided - simply add configuration in FS_33_76_82_84 composite tree nodes.
 
 TODO: All this feature does is to return curr tree path to tha last interp used within that path
       (the first interp from the tail of the path).
       Do we really want to have excessive flexibility to jump anywhere when we only jump in well-defined place?
 
-      `jump_tree` is already "global" (suitable to FS_33_76_82_84 to merge into global tree).
+      `jump_tree` is already "global" (suitable to FS_33_76_82_84 to merge into composite tree).
 
       It navigates (jumps) back to another interpreter when function is selected (to select next func).
       `FuncTreeInterpFactory` uses `select_next_interp_tree_abs_path` func which is where the jump is performed
       based on current `interp_ctx.interp_tree_abs_path`.
       What `run_interp_control` for `FuncTreeInterpFactory` does is to ask e.g. `HelpDelegator` what is the next
       `plugin_id` (interp) to use.
```

### Comparing `argrelay-0.6.9/docs/feature_stories/FS_92_75_93_01.clean_command_line.md` & `argrelay-0.7.0.dev0/docs/feature_stories/FS_92_75_93_01.clean_command_line.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/readme.md` & `argrelay-0.7.0.dev0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/release_notes/readme.md` & `argrelay-0.7.0.dev0/docs/release_notes/readme.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/release_notes/v0.0.0.dev27.md` & `argrelay-0.7.0.dev0/docs/release_notes/v0.0.0.dev27.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_00_79_72_55.remove_static_data_from_server_config.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_10_72_28_05.help_for_multiple_commands.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,13 +2,13 @@
 TODO_10_72_28_05: Support `help` for any number of commands.
 
 It also applies to `intercept` and `query_enum`.
 
 The issue is temporarily fixed via `tree_abs_path_to_interp_id` config.
 But this fix is cumbersome.
 
-The proper fix should be addressed via FS_33_76_82_84 global tree (g-tree).
+The proper fix should be addressed via FS_33_76_82_84 composite tree.
 The change is to use single config place where all interps, delegators, functions are referenced.
 Instead of configuring parts of the tree (sub-trees) under different plugins.
 It should be made convenient to see the whole picture in single place
 (and that tree is used as a config for the plugins).
 Think how to encode the tree via YAML for both func ids and interp ids (it seems it should contain both).
```

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 This task is to think and see if FS_26_43_73_72 func tree interp (FT-interp) and delegator can
 converge into a single building block.
 
 Just to emphasise - the interp below is actually not any interp
 (like FS_42_76_93_51 first/zero-ipos arg or FS_01_89_09_24 interp tree),
 but FS_26_43_73_72 func tree interp (FT-interp).
-In other words (in terms of upcoming FS_33_76_82_84 `global_tree`):
+In other words (in terms of upcoming FS_33_76_82_84 `composite_tree`):
 *   irrelevant: `node_type: zero_arg_node`
 *   irrelevant: `node_type: interp_tree_node` with `InterpTreeInterpFactory`
 *   relevant: `node_type: interp_tree_node` with `FuncTreeInterpFactory` vs `node_type: func_tree_node` (delegator)
 
 # Why do we need single-func `FuncTreeInterpFactory` interp instances?
 
 All funcs are searched within the tree in a standard way:
 *   args to the path within a tree can be specified out of order
-*   all unconsumed args are eaten eagerly if possible (without re-querying)
+*   all remaining args are eaten eagerly if possible (without re-querying)
 
 For example, if `relay_demo intercept goto` is specified, and there are some paths with the 2nd step `goto`,
 this would select (based on how `intercept` is normally configured) no function - the user interrogation will stop.
 This happens because there is no funcs with 1st step `intercept` and 2nd step `goto`.
 
 By using FS_01_89_09_24 interp tree instead of FS_26_43_73_72 func tree,
 `intercept` becomes terminal (single) function under interp tree with 1st step `intercept`,
```

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md` & `argrelay-0.7.0.dev0/docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md` & `argrelay-0.7.0.dev0/docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/test_data/TD_63_37_05_36.demo_services_data.md` & `argrelay-0.7.0.dev0/docs/test_data/TD_63_37_05_36.demo_services_data.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 ---
 test_data: TD_63_37_05_36
 test_title: demo service data
 ---
 
 This data is what `ServiceLoader` uses for `relay_demo` client from root `readme.md`:
 
-| `code_maturity` | `geo_region` | `flow_stage`  | `cluster_name`          | `data_center` | `host_name`   | `service_name` | `ip_address`      | `group_label`         | is_populated     | comment                           |
-|----------------|-------------|--------------|------------------------|--------------|--------------|---------------|------------------|----------------------|------------------|-----------------------------------|
-| -------------- | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- | `dev` is everywhere but limited   |
-| `dev`          | `apac`      | `upstream`   | `dev-apac-upstream`    | `dc.01`      | `zxcv-du`    | `s_a`         | `ip.192.168.1.1` | `aaa,sss`            | Y                |                                   |
-| `dev`          | `apac`      | `upstream`   | `dev-apac-upstream`    | `dc.01`      | `zxcv-du`    | `s_b`         | `ip.192.168.1.1` | `bbb,sss`            | Y                |                                   |
-| `dev`          | `apac`      | `upstream`   | `dev-apac-upstream`    | `dc.01`      | `zxcv-du`    | `s_c`         | `ip.192.168.1.1` | `ccc,sss`            | Y                |                                   |
-|                |             | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `dev`          | `apac`      | `downstream` | `dev-apac-downstream`  | `dc.11`      | `zxcv-dd`    | `tt`          | `ip.172.16.1.2`  | `rrr`                | Y                |                                   |
-| `dev`          | `apac`      | `downstream` | `dev-apac-downstream`  | `dc.01`      | `poiu-dd`    | `xx`          | `ip.192.168.1.3` | `rrr,hhh`            | Y                |                                   |
-|                | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- | `emea` has no `s_c`               |
-| `dev`          | `emea`      | `upstream`   | `dev-emea-upstream`    | `dc.22`      | `asdf-du`    | `s_a`         | `ip.172.16.2.1`  | `aaa,sss`            | Y                |                                   |
-| `dev`          | `emea`      | `upstream`   | `dev-emea-upstream`    | `dc.22`      | `asdf-du`    | `s_b`         | `ip.172.16.2.1`  | `bbb,sss`            | Y                |                                   |
-|                |             | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `dev`          | `emea`      | `downstream` | `dev-emea-downstream`  | `dc.02`      | `xcvb-dd`    | `xx`          | `ip.192.168.2.2` | `rrr,hhh`            | Y                |                                   |
-| `dev`          | `emea`      | `downstream` | `dev-emea-downstream`  | `dc.02`      | `xcvb-dd`    | `zz`          | `ip.192.168.2.2` | `rrr,hhh,odd`        | Y                |                                   |
-|                | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- | `amer` has only `dev` `upstream`  |
-| `dev`          | `amer`      | `upstream`   | `dev-amer-upstream`    | `dc.03`      | `qwer-du`    | `s_a`         | `ip.192.168.3.1` | `aaa,sss`            | Y                | `amer` has only `s_a` service     |
-| -------------- | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `qa`           | `apac`      | `upstream`   | `qa-apac-upstream`     | `dc.04`      | `hjkl-qu`    | `s_a`         | `ip.192.168.4.1` | `aaa,sss`            | Y                |                                   |
-| `qa`           | `apac`      | `upstream`   | `qa-apac-upstream`     | `dc.04`      | `hjkl-qu`    | `s_b`         | `ip.192.168.4.1` | `bbb,sss`            | Y                |                                   |
-| `qa`           | `apac`      | `upstream`   | `qa-apac-upstream`     | `dc.44`      | `poiu-qu`    | `s_c`         | `ip.172.16.4.2`  | `ccc,sss`            | Y                |                                   |
-|                | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `qa`           | `emea`      | `downstream` | `qa-emea-downstream`   | `dc.05`      |              |               |                  |                      | Y                | no `qa` in `emea` (empty cluster) |
-|                | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `qa`           | `amer`      | `upstream`   | `qa-amer-upstream`     | `dc.06`      | `rtyu-qu`    | `s_a`         | `ip.192.168.6.1` | `aaa,sss`            | Y                |                                   |
-| `qa`           | `amer`      | `upstream`   | `qa-amer-upstream`     | `dc.06`      | `rt-qu`      |               | `ip.192.168.6.2` |                      | Y                | host `rt-du` has no services      |
-|                |             | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `qa`           | `amer`      | `downstream` | `qa-amer-downstream`   | `dc.06`      | `sdfgh-qd`   | `tt1`         | `ip.192.168.6.3` | `rrr`                | Y                |                                   |
-| `qa`           | `amer`      | `downstream` | `qa-amer-downstream`   | `dc.06`      | `sdfgb-qd`   | `xx`          | `ip.192.168.6.4` | `rrr,hhh`            | Y                |                                   |
-| `qa`           | `amer`      | `downstream` | `qa-amer-downstream`   | `dc.66`      | `sdfg-qd`    |               | `ip.172.16.6.5`  |                      | Y                | host `sdfg-qd` has no services    |
-| -------------- | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- | `prod` is only in `apac`          |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.07`      | `qwer-pd-1`  | `s_a`         | `ip.192.168.7.1` | `aaa,sss`            | Y                |                                   |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.07`      | `qwer-pd-1`  | `s_b`         | `ip.192.168.7.1` | `bbb,sss`            | Y                |                                   |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.07`      | `qwer-pd-3`  | `s_c`         | `ip.192.168.7.2` | `ccc,sss`            | Y                |                                   |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.77`      | `qwer-pd-2`  | `s_a`         | `ip.172.16.7.2`  | `aaa,sss`            | Y                |                                   |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.77`      | `qwer-pd-2`  | `s_b`         | `ip.172.16.7.2`  | `bbb,xxx`            | Y                | diff `group_label` for `s_b`       |
-| `prod`         | `apac`      | `upstream`   | `prod-apac-upstream`   | `dc.77`      | `qwer-pd-2`  | `s_c`         | `ip.172.16.7.2`  | `ccc,sss`            | Y                |                                   |
-|                | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- |                                   |
-| `prod`         | `apac`      | `downstream` | `prod-apac-downstream` | `dc.07`      | `wert-pd-1`  | `tt1`         | `ip.192.168.7.3` | `rrr`                | Y                |                                   |
-| `prod`         | `apac`      | `downstream` | `prod-apac-downstream` | `dc.07`      | `wert-pd-2`  | `tt2`         | `ip.192.168.7.4` | `rrr`                | Y                |                                   |
-| `prod`         | `apac`      | `downstream` | `prod-apac-downstream` | `dc.07`      | `wert-pd-2`  | `xx`          | `ip.192.168.7.4` | `rrr,hhh`            | Y                |                                   |
-| -------------- | ----------- | ------------ | ---------------------- | ------------ | ------------ | ------------- | ---------------- | -------------------- | ---------------- | ------------------------------    |
-|                |             |              |                        |              |              |               |                  |                      |                  |                                   |
+| `code_maturity` | `geo_region` | `flow_stage` | `cluster_name`         | `data_center` | `host_name` | `service_name` | `run_mode` | `ip_address`     | `group_label` | is_populated | comment                           |
+|-----------------|--------------|--------------|------------------------|---------------|-------------|----------------|------------|------------------|---------------|--------------|-----------------------------------|
+| --------------- | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ | `dev` is everywhere but limited   |
+| `dev`           | `apac`       | `upstream`   | `dev-apac-upstream`    | `dc.01`       | `zxcv-du`   | `s_a`          | `active`   | `ip.192.168.1.1` | `aaa,sss`     | Y            |                                   |
+| `dev`           | `apac`       | `upstream`   | `dev-apac-upstream`    | `dc.01`       | `zxcv-du`   | `s_b`          | `active`   | `ip.192.168.1.1` | `bbb,sss`     | Y            |                                   |
+| `dev`           | `apac`       | `upstream`   | `dev-apac-upstream`    | `dc.01`       | `zxcv-du`   | `s_c`          | `active`   | `ip.192.168.1.1` | `ccc,sss`     | Y            |                                   |
+|                 |              | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `dev`           | `apac`       | `downstream` | `dev-apac-downstream`  | `dc.11`       | `zxcv-dd`   | `tt`           | `active`   | `ip.172.16.1.2`  | `rrr`         | Y            |                                   |
+| `dev`           | `apac`       | `downstream` | `dev-apac-downstream`  | `dc.01`       | `poiu-dd`   | `xx`           | `active`   | `ip.192.168.1.3` | `rrr,hhh`     | Y            |                                   |
+|                 | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ | `emea` has no `s_c`               |
+| `dev`           | `emea`       | `upstream`   | `dev-emea-upstream`    | `dc.22`       | `asdf-du`   | `s_a`          | `active`   | `ip.172.16.2.1`  | `aaa,sss`     | Y            |                                   |
+| `dev`           | `emea`       | `upstream`   | `dev-emea-upstream`    | `dc.22`       | `asdf-du`   | `s_b`          | `active`   | `ip.172.16.2.1`  | `bbb,sss`     | Y            |                                   |
+|                 |              | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `dev`           | `emea`       | `downstream` | `dev-emea-downstream`  | `dc.02`       | `xcvb-dd`   | `xx`           | `active`   | `ip.192.168.2.2` | `rrr,hhh`     | Y            |                                   |
+| `dev`           | `emea`       | `downstream` | `dev-emea-downstream`  | `dc.02`       | `xcvb-dd`   | `zz`           | `active`   | `ip.192.168.2.2` | `rrr,hhh,odd` | Y            |                                   |
+|                 | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ | `amer` has only `dev` `upstream`  |
+| `dev`           | `amer`       | `upstream`   | `dev-amer-upstream`    | `dc.03`       | `qwer-du`   | `s_a`          | `active`   | `ip.192.168.3.1` | `aaa,sss`     | Y            | `amer` has only `s_a` service     |
+| --------------- | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `qa`            | `apac`       | `upstream`   | `qa-apac-upstream`     | `dc.04`       | `hjkl-qu`   | `s_a`          | `active`   | `ip.192.168.4.1` | `aaa,sss`     | Y            |                                   |
+| `qa`            | `apac`       | `upstream`   | `qa-apac-upstream`     | `dc.04`       | `hjkl-qu`   | `s_b`          | `active`   | `ip.192.168.4.1` | `bbb,sss`     | Y            |                                   |
+| `qa`            | `apac`       | `upstream`   | `qa-apac-upstream`     | `dc.44`       | `poiu-qu`   | `s_c`          | `active`   | `ip.172.16.4.2`  | `ccc,sss`     | Y            |                                   |
+|                 | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `qa`            | `emea`       | `downstream` | `qa-emea-downstream`   | `dc.05`       |             |                |            |                  |               | Y            | no `qa` in `emea` (empty cluster) |
+|                 | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `qa`            | `amer`       | `upstream`   | `qa-amer-upstream`     | `dc.06`       | `rtyu-qu`   | `s_a`          | `active`   | `ip.192.168.6.1` | `aaa,sss`     | Y            |                                   |
+| `qa`            | `amer`       | `upstream`   | `qa-amer-upstream`     | `dc.06`       | `rt-qu`     |                |            | `ip.192.168.6.2` |               | Y            | host `rt-du` has no services      |
+|                 |              | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `qa`            | `amer`       | `downstream` | `qa-amer-downstream`   | `dc.06`       | `sdfgh-qd`  | `tt1`          | `active`   | `ip.192.168.6.3` | `rrr`         | Y            |                                   |
+| `qa`            | `amer`       | `downstream` | `qa-amer-downstream`   | `dc.06`       | `sdfgb-qd`  | `xx`           | `active`   | `ip.192.168.6.4` | `rrr,hhh`     | Y            |                                   |
+| `qa`            | `amer`       | `downstream` | `qa-amer-downstream`   | `dc.66`       | `sdfg-qd`   |                |            | `ip.172.16.6.5`  |               | Y            | host `sdfg-qd` has no services    |
+| --------------- | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ | `prod` is only in `apac`          |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.07`       | `qwer-pd-1` | `s_a`          | `active`   | `ip.192.168.7.1` | `aaa,sss`     | Y            |                                   |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.07`       | `qwer-pd-1` | `s_b`          | `active`   | `ip.192.168.7.1` | `bbb,sss`     | Y            |                                   |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.07`       | `qwer-pd-3` | `s_c`          | `active`   | `ip.192.168.7.2` | `ccc,sss`     | Y            |                                   |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.77`       | `qwer-pd-2` | `s_a`          | `active`   | `ip.172.16.7.2`  | `aaa,sss`     | Y            |                                   |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.77`       | `qwer-pd-2` | `s_b`          | `active`   | `ip.172.16.7.2`  | `bbb,xxx`     | Y            | diff `group_label` for `s_b`      |
+| `prod`          | `apac`       | `upstream`   | `prod-apac-upstream`   | `dc.77`       | `qwer-pd-2` | `s_c`          | `active`   | `ip.172.16.7.2`  | `ccc,sss`     | Y            |                                   |
+|                 | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ |                                   |
+| `prod`          | `apac`       | `downstream` | `prod-apac-downstream` | `dc.07`       | `wert-pd-1` | `tt1`          | `active`   | `ip.192.168.7.3` | `rrr`         | Y            |                                   |
+| `prod`          | `apac`       | `downstream` | `prod-apac-downstream` | `dc.07`       | `wert-pd-1` | `tt2`          | `passive`  | `ip.192.168.7.3` | `rrr`         | Y            |                                   |
+| `prod`          | `apac`       | `downstream` | `prod-apac-downstream` | `dc.07`       | `wert-pd-2` | `tt1`          | `passive`  | `ip.192.168.7.4` | `rrr`         | Y            |                                   |
+| `prod`          | `apac`       | `downstream` | `prod-apac-downstream` | `dc.07`       | `wert-pd-2` | `tt2`          | `active`   | `ip.192.168.7.4` | `rrr`         | Y            |                                   |
+| `prod`          | `apac`       | `downstream` | `prod-apac-downstream` | `dc.07`       | `wert-pd-2` | `xx`           | `active`   | `ip.192.168.7.4` | `rrr,hhh`     | Y            |                                   |
+| --------------- | ------------ | ------------ | ---------------------- | ------------- | ----------- | -------------- | ---------- | ---------------- | ------------- | ------------ | ------------------------------    |
+|                 |              |              |                        |               |             |                |            |                  |               |              |                                   |
 
 There is no purpose to cover all special cases (other `test_data` is supposed to cover that) -
 the intention is to provide enough data to play with (without overwhelming manual maintenance).
 
 It permutes arg values for arg types defined in `ServiceArgType`:
 
 *   `code_maturity`:
```

### Comparing `argrelay-0.6.9/docs/test_data/TD_70_69_38_46.no_data.md` & `argrelay-0.7.0.dev0/docs/test_data/TD_70_69_38_46.no_data.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.0.dev0/docs/test_data/TD_76_09_29_31.overlapped_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md` & `argrelay-0.7.0.dev0/docs/test_data/TD_99_99_88_75.mutually_exclusive_arg_vals_from_diff_arg_types.md`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/readme.md` & `argrelay-0.7.0.dev0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 <!--
 See: docs/dev_notes/screencast_notes.md
 -->
 
 <a name="argrelay-about"></a>
 # What's this?
 
-A method to "ergonomically" select **custom data** input for command line interface (CLI) tools.
+A framework to "ergonomically" select **custom data** input for command line interface (CLI) tools.
 
-The aim is to enrich two-way &#10231; interaction by **"pre-pared"** data:
-*   &#10230; You input args you **remember** (via `Tab`-auto-completion) in **relaxed order**.
-*   &#10229; It reports (via `Alt+Shift+Q` query):
-    *   What args it **matched**.
-    *   What **else** it needs.
+The aim is to enrich two-way &#10231; interaction by **prepared** reference data:
+*   &#10230; Human inputs args you **remember** (via `Tab`-auto-completion) in **relaxed order**.
+*   &#10229; Machine feeds back (via `Alt+Shift+Q` query):
+    *   What args it **matched** to server data within command schema.
+    *   What **else** it needs to populate remaining command args.
 
 This broadens applicability of CLI input as a slim alternative to graphical user interface (GUI)
-competing in **convenience** for apps especially for developers.
+competing in **convenience** for apps especially for developers = "doing more with less".
 
-*   When your data is (luckily) instantly and directly queryable, use [`argcomplete`][argcomplete_github].
-*   When your data is sizeable, user needs performance (indexing), relaxed syntax, keyword-based search, use `argrelay`.
+*   When your data is instantly and directly queryable, try [`argcomplete`][argcomplete_github].
+*   When your data is sizeable, user needs performance (indexing), relaxed syntax, keyword-based search, try `argrelay`.
 
 <a name="argrelay-overview"></a>
 # Interaction overview
 
 User is interrogated based on:
 *  command **input schema**
 *  data matching already given input
@@ -52,26 +52,27 @@
 
 | GUI                                                                           | CLI                                                       |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------|
 | :heavy_plus_sign: diagrams, images, video                                     | :heavy_multiplication_x: only via integration with GUI    |
 | :heavy_minus_sign: might be time-consuming for an ad-hoc functionality        | :heavy_plus_sign: always quick dev option (low ceremony)  |
 | :heavy_minus_sign: may not exist early in feature development                 | :heavy_plus_sign: likely available early in development   |
 | :heavy_minus_sign: no simple way to store and share GUI output                | :heavy_plus_sign: store and share results as **text**     |
+| :heavy_minus_sign: repeat steps 500 times? give up!                           | :heavy_plus_sign: repeat steps 500 time? loop!            |
 | :heavy_minus_sign: no universal way to reproduce (composite) GUI actions      | :heavy_plus_sign: paste and "replay" commands as **text** |
 | :heavy_minus_sign: no universal way to search stored GUI output               | :heavy_plus_sign: `grep`-search results as **text**       |
 | :heavy_minus_sign: no universal way to compare GUI output                     | :heavy_plus_sign: `diff`-compare results as **text**      |
 | :heavy_minus_sign: no universal way to auto-trigger GUI actions on events     | :heavy_plus_sign: hook commands anyhow (e.g. schedule)    |
 | :heavy_minus_sign: a separate stack (skill set) from backend to contribute to | :heavy_plus_sign: familiarly dominates backend tools      |
 | :heavy_minus_sign: uses APIs but hardly exposes API to integrate itself       | :heavy_plus_sign: inherent script-ability                 |
 | :heavy_minus_sign: limits system access (a layer behind a narrow API)         | :heavy_plus_sign: ultimate control                        |
 | :heavy_plus_sign: keyword captions                                            | :heavy_minus_sign: hardly remembered cryptic `-o` options |
-| :heavy_plus_sign: point-click actions                                         | :heavy_minus_sign: typing:exclamation:                    |
-| :heavy_plus_sign: intuitive data-driven interface                             | :heavy_minus_sign: interface:question:                    |
+| :heavy_plus_sign: point-click actions                                         | :heavy_minus_sign: increased typing:exclamation:          |
+| :heavy_plus_sign: intuitive data-driven interface                             | :heavy_minus_sign: interface:question: more like API      |
 
-While retaining advantages of a CLI tool, `argrelay` tries to provide:
+While retaining advantages of a CLI tool, `argrelay` tries to provide those last :heavy_plus_sign:-s:
 *   intuitive data-driven interface
 *   reduced typing (args auto-reduction)
 *   keyword options (args auto-completion)
 
 As opposed to GUI-demanding approaches like [Warp][Warp_site] or [IDEA terminal][IDEA_terminal],<br/>
 `argrelay` survives in basic text modes.
```

### Comparing `argrelay-0.6.9/setup.py` & `argrelay-0.7.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     # All paths start with `top_dir_path`:
     return file_paths
 
 
 setuptools.setup(
     name = "argrelay",
     # See `docs/dev_notes/version_format.md`:
-    version = "0.6.9",
+    version = "0.7.0.dev0",
     author = "uvsmtid",
     author_email = "uvsmtid@gmail.com",
     description = "Tab-completion & data search server = total recall for Bash shell",
     long_description = """
 See: https://github.com/argrelay/argrelay
     """,
     long_description_content_type = "text/markdown",
@@ -124,14 +124,15 @@
     install_requires = [
         "Flask",
         "Werkzeug",
         "PyYaml",
         "jsonschema",
         "flasgger",
         "marshmallow",
+        "marshmallow-oneofschema",
         "apispec",
         "pymongo",
         "GitPython",
         # Use `mongomock` as replacement for Mongo DB in simple prod cases:
         "mongomock",
         "requests",
         "cachetools",
```

### Comparing `argrelay-0.6.9/src/argrelay/client_command_local/AbstractLocalClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_local/AbstractLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_local/DescribeLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_local/ProposeArgValuesLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_local/RelayLineArgsLocalClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_remote/AbstractRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py` & `argrelay-0.7.0.dev0/src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/client_spec/ShellContext.py` & `argrelay-0.7.0.dev0/src/argrelay/client_spec/ShellContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/BaseConfigDelegator.py`

 * *Files 4% similar despite different names*

```diff
@@ -183,21 +183,16 @@
         # The first envelope (`DataEnvelopeSchema`) is assumed to be of
         # `ReservedEnvelopeClass.ClassFunction` with `FunctionEnvelopeInstanceDataSchema` for its `instance_data`:
         function_container = interp_ctx.envelope_containers[function_container_ipos_]
         delegator_plugin_instance_id = (
             function_container.data_envelopes[0][instance_data_]
             [delegator_plugin_instance_id_]
         )
-        invocation_input = InvocationInput(
-            arg_values = interp_ctx.comp_suggestions,
-            all_tokens = interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = interp_ctx.consumed_tokens,
-            envelope_containers = interp_ctx.envelope_containers,
-            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+        invocation_input = InvocationInput.with_interp_context(
+            interp_ctx,
             delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyDelegator.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
             config_only_delegator_config_desc,
         )
 
     @staticmethod
     def invoke_action(
         invocation_input: InvocationInput,
     ):
-
         # TODO_74_73_60_93: Support expected envelope count in config-only delegator:
         # Use common static functions in `BaseConfigDelegator`.
 
         # Keep this as it is supposed to be referenced in the `command_template`
         envelope_containers = invocation_input.envelope_containers
 
         # There is no way to check on client side if this function belongs to this plugin
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from argrelay.schema_config_interp.FuncEnvelopeSchema import (
     func_id_some_func_,
 )
 
 command_template_ = "command_template"
 echo_command_on_stderr_ = "echo_command_on_stderr"
 
+
 class ConfigOnlyDelegatorConfigSchema(BaseConfigDelegatorConfigSchema):
     """
     Part of FS_49_96_50_77 config_only_delegator implementation.
     """
 
     class Meta:
         unknown = RAISE
@@ -52,36 +53,38 @@
         `FuncConfigSchema.func_envelope` of `FuncEnvelopeSchema` which allows arbitrary dict in `envelope_payload`.
 
         `ConfigOnlyDelegatorConfigSchema` expects them to be of `ConfigOnlyDelegatorEnvelopePayloadSchema`.
         """
         for func_config in input_dict[func_configs_].values():
             config_only_delegator_envelope_payload_desc.validate_dict(func_config[func_envelope_][envelope_payload_])
 
+
 class ConfigOnlyDelegatorEnvelopePayloadSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     command_template = fields.String(
         required = True,
     )
 
     echo_command_on_stderr = fields.Boolean(
-        load_default = False,
         required = False,
+        load_default = False,
     )
 
     # TODO_54_68_18_12: Support defaults for config-only delegator:
     # Add a schema for this config but likely into _new_ `BaseConfigDelegatorEnvelopePayloadSchema`
     # as it can be used with other configurable plugins even if they do not use
     # `command_template` (as this `ConfigOnlyDelegatorEnvelopePayloadSchema` class does).
 
     # TODO_74_73_60_93: Support expected envelope count in config-only delegator:
     # Similar to TODO_54_68_18_12 (above), it should be part of _new_ `BaseConfigDelegatorEnvelopePayloadSchema`.
 
+
 _config_only_func_config_dict_example = deepcopy(func_config_desc.dict_example)
 _config_only_func_config_dict_example[func_envelope_][envelope_payload_].update({
     command_template_: "echo",
 })
 
 config_only_delegator_envelope_payload_desc = TypeDesc(
     dict_schema = ConfigOnlyDelegatorEnvelopePayloadSchema(),
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoader.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     ) -> StaticData:
 
         # Config for FS_56_43_05_79 different collections:
         class_to_collection_map: dict = self.server_config.class_to_collection_map
 
         # FS_49_96_50_77 config_only_loader plugin:
         # *   `collection_name_to_index_fields_map`:
-        collection_name_to_index_fields_map: dict[str, list[str]] = self.plugin_config_dict[collection_name_to_index_fields_map_]
+        collection_name_to_index_fields_map: dict[str, list[str]] = self.plugin_config_dict[
+            collection_name_to_index_fields_map_
+        ]
         # *   list of `data_envelope`-s (actual data):
         data_envelopes = [
             convert_envelope_fields_to_string(data_envelope)
             for data_envelope in deepcopy(self.plugin_config_dict[data_envelopes_])
         ]
 
         class_names: list[str] = [
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     sample_field_type_B_,
     sample_field_type_C_,
 )
 from argrelay.schema_response.EnvelopeContainerSchema import data_envelopes_
 
 collection_name_to_index_fields_map_ = "collection_name_to_index_fields_map"
 
+
 class ConfigOnlyLoaderConfigSchema(Schema):
     """
     Part of FS_49_96_50_77 config_only_loader implementation.
     """
 
     class Meta:
         unknown = RAISE
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/FuncConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/FuncConfigSchema.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from argrelay.schema_config_interp.FuncEnvelopeSchema import (
     func_envelope_desc,
 )
 
 func_envelope_ = "func_envelope"
 fill_control_list_ = "fill_control_list"
 
+
 class FuncConfigSchema(Schema):
     """
     Part of FS_49_96_50_77 config_only_plugins implementation.
     """
 
     class Meta:
         unknown = RAISE
@@ -33,14 +34,15 @@
     Each `dict` controls setting default values (based on already found `data_envelope`-s):
     *   Each key is a prop name to set default value for.
     *   Each value is an expression for prop value which may refer to already prev `envelope_container`-s.
     """
 
     func_envelope = fields.Nested(func_envelope_desc.dict_schema)
 
+
 func_config_desc = TypeDesc(
     dict_schema = FuncConfigSchema(),
     ref_name = FuncConfigSchema.__name__,
     dict_example = {
         fill_control_list_: [
             {
             },
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoArgType.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoDelegator.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 func_id_: goto_git_repo_func_,
                 delegator_plugin_instance_id_: self.plugin_instance_id,
                 search_control_list_: [
                     repo_search_control,
                 ],
             },
             ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
-            ReservedArgType.HelpHint.name: "Describe Git repository",
+            ReservedArgType.HelpHint.name: "Goto Git repository (`cd` to its path)",
             ReservedArgType.FuncId.name: goto_git_repo_func_,
         }
         func_envelopes.append(given_function_envelope)
 
         given_function_envelope = {
             instance_data_: {
                 func_id_: desc_git_tag_func_,
@@ -162,21 +162,16 @@
         # The first envelope (`DataEnvelopeSchema`) is assumed to be of
         # `ReservedEnvelopeClass.ClassFunction` with `FunctionEnvelopeInstanceDataSchema` for its `instance_data`:
         function_container = interp_ctx.envelope_containers[function_container_ipos_]
         delegator_plugin_instance_id = (
             function_container.data_envelopes[0][instance_data_]
             [delegator_plugin_instance_id_]
         )
-        invocation_input = InvocationInput(
-            arg_values = interp_ctx.comp_suggestions,
-            all_tokens = interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = interp_ctx.consumed_tokens,
-            envelope_containers = interp_ctx.envelope_containers,
-            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+        invocation_input = InvocationInput.with_interp_context(
+            interp_ctx,
             delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoEntryConfigSchema.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,36 +20,36 @@
         strict = True
 
     repo_rel_path = fields.String(
         required = True,
     )
 
     load_repo_tags = fields.Boolean(
-        default = False,
         required = False,
+        load_default = False,
     )
 
     load_repo_commits = fields.Boolean(
-        default = False,
         required = False,
+        load_default = False,
     )
 
     load_tags_last_days = fields.Integer(
-        default = 300,
         required = False,
+        load_default = 300,
     )
 
     load_commits_max_count = fields.Integer(
-        default = 100,
         required = False,
+        load_default = 100,
     )
 
     is_repo_enabled = fields.Boolean(
-        load_default = True,
         required = False,
+        load_default = True,
     )
 
     # These key-values are copied into `data_envelope`:
     envelope_properties = fields.Dict(
         keys = fields.String(),
         values = fields.String(),
         required = True,
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoader.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
                     ########################################################################################################
                     # commits
 
                     load_commits_max_count = repo_entry[load_commits_max_count_]
 
                     git_repo = Repo(repo_root_abs_path)
                     for git_commit in git_repo.iter_commits(max_count = load_commits_max_count):
-
                         (
                             commit_timestamp_utc,
                             commit_date_utc,
                             commit_time_utc,
                         ) = self.get_commit_date_and_time(git_commit)
 
                         commit_envelope: dict = copy.deepcopy(repo_entry[envelope_properties_])
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/GitRepoLoaderConfigSchema.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 class GitRepoLoaderConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     load_git_tags_default = fields.Boolean(
-        default = False,
         required = False,
+        load_default = False,
     )
 
     load_git_commits_default = fields.Boolean(
-        default = False,
         required = False,
+        load_default = False,
     )
 
     # Maps `repo_base_path` to list of repo entries.
     # *   If `repo_base_path` starts with `/` (absolute), it is used verbatim.
     # *   If `repo_base_path` does not start with `/` (relative),
     #     it is converted to absolute assuming it is relative to `argrelay_dir` (`@/`).
     repo_entries = fields.Dict(
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ServiceArgType.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceArgType.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     ip_address = auto()
 
     # FS_06_99_43_60: example of using non-scalar value (array|list):
     group_label = auto()
 
     service_name = auto()
 
+    run_mode = auto()
+
     # ---
 
     access_type = auto()
 
     # ---
 
     live_status = auto()
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ServiceDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceDelegator.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from argrelay.custom_integ.ServiceArgType import ServiceArgType
 from argrelay.custom_integ.ServiceEnvelopeClass import ServiceEnvelopeClass
 from argrelay.custom_integ.value_constants import (
     goto_host_func_,
     goto_service_func_,
     list_host_func_,
     list_service_func_,
+    diff_service_func_,
     desc_host_func_,
     desc_service_func_,
 )
 from argrelay.enum_desc.ArgSource import ArgSource
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.plugin_delegator.AbstractDelegator import (
@@ -45,14 +46,17 @@
 )
 from argrelay.schema_response.InvocationInput import InvocationInput
 
 host_container_ipos_ = 1
 service_container_ipos_ = 1
 access_container_ipos_ = 2
 
+diff_service_container_left_ipos_ = 1
+diff_service_container_right_ipos_ = 2
+
 
 def set_default_to(arg_type, arg_val, envelope_container) -> bool:
     if arg_type in envelope_container.search_control.types_to_keys_dict:
         if arg_type not in envelope_container.assigned_types_to_values:
             if arg_type in envelope_container.remaining_types_to_values:
                 if arg_val in envelope_container.remaining_types_to_values[arg_type]:
                     del envelope_container.remaining_types_to_values[arg_type]
@@ -89,21 +93,16 @@
     # TODO: Do not hardcode plugin id (instance of `ErrorDelegator`):
     delegator_plugin_instance_id = f"{ErrorDelegator.__name__}.default"
     custom_plugin_data = {
         error_message_: error_message,
         error_code_: error_code,
     }
     error_delegator_custom_data_desc.validate_dict(custom_plugin_data)
-    invocation_input = InvocationInput(
-        arg_values = interp_ctx.comp_suggestions,
-        all_tokens = interp_ctx.parsed_ctx.all_tokens,
-        consumed_tokens = interp_ctx.consumed_tokens,
-        envelope_containers = interp_ctx.envelope_containers,
-        tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-        tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+    invocation_input = InvocationInput.with_interp_context(
+        interp_ctx,
         delegator_plugin_entry = server_config.plugin_instance_entries[delegator_plugin_instance_id],
         custom_plugin_data = custom_plugin_data,
     )
     return invocation_input
 
 
 class ServiceDelegator(AbstractDelegator):
@@ -161,14 +160,15 @@
                 {"code": ServiceArgType.code_maturity.name},
                 {"stage": ServiceArgType.flow_stage.name},
                 {"region": ServiceArgType.geo_region.name},
                 {"cluster": ServiceArgType.cluster_name.name},
                 # ClassService:
                 {"group": ServiceArgType.group_label.name},
                 {"service": ServiceArgType.service_name.name},
+                {"mode": ServiceArgType.run_mode.name},
                 # ClassHost:
                 {"host": ServiceArgType.host_name.name},
                 # ---
                 {"status": ServiceArgType.live_status.name},
                 {"dc": ServiceArgType.data_center.name},
                 {"ip": ServiceArgType.ip_address.name},
             ],
@@ -255,35 +255,58 @@
                         service_search_control,
                     ],
                 },
                 ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
                 ReservedArgType.HelpHint.name: "List service instances matching search query",
                 ReservedArgType.FuncId.name: list_service_func_,
             },
+            {
+                instance_data_: {
+                    func_id_: diff_service_func_,
+                    delegator_plugin_instance_id_: self.plugin_instance_id,
+                    search_control_list_: [
+                        # This function was created to demo FS_97_64_39_94 `arg_bucket`-s:
+                        # it intentionally uses two services as to specify in its args:
+                        service_search_control,
+                        service_search_control,
+                    ],
+                },
+                ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
+                ReservedArgType.HelpHint.name: "Diff two service instances",
+                ReservedArgType.FuncId.name: diff_service_func_,
+            },
         ]
         return func_envelopes
 
     def has_fill_control(
         self,
     ) -> bool:
         return True
 
     def run_fill_control(
         self,
         interp_ctx: "InterpContext",
     ) -> bool:
         func_id = get_func_id_from_interp_ctx(interp_ctx)
         any_assignment = False
+
         if func_id in [
             goto_host_func_,
             goto_service_func_,
         ]:
             assert host_container_ipos_ == service_container_ipos_
             object_container_ipos = host_container_ipos_
 
+            if func_id == goto_service_func_:
+                any_assignment = self._fill_service_container(
+                    any_assignment,
+                    interp_ctx,
+                    object_container_ipos,
+                )
+
             # If we need to specify `access_type` `data_envelope`:
             if interp_ctx.curr_container_ipos == interp_ctx.curr_interp.base_container_ipos + access_container_ipos_:
                 # Take object found so far:
                 data_envelope = interp_ctx.envelope_containers[(
                     interp_ctx.curr_interp.base_container_ipos + object_container_ipos
                 )].data_envelopes[0]
 
@@ -303,25 +326,56 @@
                         )
                     else:
                         any_assignment = (
                             set_default_to(ServiceArgType.access_type.name, "rw", access_container)
                             or
                             any_assignment
                         )
-
+        elif func_id in [
+            diff_service_func_,
+        ]:
+            any_assignment = self._fill_service_container(
+                any_assignment,
+                interp_ctx,
+                diff_service_container_left_ipos_,
+            )
+            any_assignment = self._fill_service_container(
+                any_assignment,
+                interp_ctx,
+                diff_service_container_right_ipos_,
+            )
         elif func_id in [
             list_host_func_,
             list_service_func_,
         ]:
             pass
         else:
             raise RuntimeError
 
         return any_assignment
 
+    def _fill_service_container(
+        self,
+        any_assignment,
+        interp_ctx,
+        object_container_ipos,
+    ):
+        if (
+            interp_ctx.curr_container_ipos == interp_ctx.curr_interp.base_container_ipos + object_container_ipos
+        ):
+            service_container = interp_ctx.envelope_containers[(
+                interp_ctx.curr_interp.base_container_ipos + object_container_ipos
+            )]
+            any_assignment = (
+                set_default_to(ServiceArgType.run_mode.name, "active", service_container)
+                or
+                any_assignment
+            )
+        return any_assignment
+
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
 
@@ -346,14 +400,27 @@
             return redirect_to_error(
                 interp_ctx,
                 local_server.server_config,
                 error_delegator_stub_custom_data_example[error_message_],
                 error_delegator_stub_custom_data_example[error_code_],
             )
         elif func_id in [
+            diff_service_func_,
+        ]:
+            # TODO_75_52_01_67: `arg_bucket`-s to support multiple var args:
+            #                   query both service lists and compare them.
+
+            # Actual implementation is not defined for demo:
+            return redirect_to_error(
+                interp_ctx,
+                local_server.server_config,
+                error_delegator_stub_custom_data_example[error_message_],
+                error_delegator_stub_custom_data_example[error_code_],
+            )
+        elif func_id in [
             list_host_func_,
             list_service_func_,
         ]:
             # Verify that func is selected and all what is left to do is to query 0...N objects:
             if interp_ctx.curr_container_ipos >= vararg_container_ipos:
                 # Search `data_envelope`-s based on existing args on command line:
                 vararg_container = interp_ctx.envelope_containers[vararg_container_ipos]
@@ -362,21 +429,16 @@
                     .get_query_engine()
                     .query_data_envelopes_for(vararg_container)
                 )
 
                 # Plugin to invoke on client side:
                 delegator_plugin_instance_id = self.plugin_instance_id
                 # Package into `InvocationInput` payload object:
-                invocation_input = InvocationInput(
-                    arg_values = interp_ctx.comp_suggestions,
-                    all_tokens = interp_ctx.parsed_ctx.all_tokens,
-                    consumed_tokens = interp_ctx.consumed_tokens,
-                    envelope_containers = interp_ctx.envelope_containers,
-                    tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-                    tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+                invocation_input = InvocationInput.with_interp_context(
+                    interp_ctx,
                     delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
                         delegator_plugin_instance_id
                     ],
                     custom_plugin_data = {},
                 )
                 return invocation_input
             else:
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoader.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceLoader.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,16 @@
                 if data_envelope[ReservedArgType.EnvelopeClass.name] == ServiceEnvelopeClass.ClassService.name:
                     data_envelope[envelope_id_] = (
                         data_envelope[ServiceArgType.cluster_name.name]
                         + "." +
                         data_envelope[ServiceArgType.host_name.name]
                         + "." +
                         data_envelope[ServiceArgType.service_name.name]
+                        + "." +
+                        data_envelope[ServiceArgType.run_mode.name]
                     )
 
     @staticmethod
     def generate_help_hints(
         class_to_collection_map: dict,
         static_data: StaticData,
     ):
@@ -628,14 +630,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-apac-upstream",
                 ServiceArgType.data_center.name: "dc.01",
                 ServiceArgType.host_name.name: "zxcv-du",
                 ServiceArgType.ip_address.name: "ip.192.168.1.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -646,14 +649,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-apac-upstream",
                 ServiceArgType.data_center.name: "dc.01",
                 ServiceArgType.host_name.name: "zxcv-du",
                 ServiceArgType.ip_address.name: "ip.192.168.1.1",
                 ServiceArgType.service_name.name: "s_b",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "bbb",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -664,14 +668,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-apac-upstream",
                 ServiceArgType.data_center.name: "dc.01",
                 ServiceArgType.host_name.name: "zxcv-du",
                 ServiceArgType.ip_address.name: "ip.192.168.1.1",
                 ServiceArgType.service_name.name: "s_c",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "ccc",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -682,14 +687,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-apac-downstream",
                 ServiceArgType.data_center.name: "dc.11",
                 ServiceArgType.host_name.name: "zxcv-dd",
                 ServiceArgType.ip_address.name: "ip.172.16.1.2",
                 ServiceArgType.service_name.name: "tt",
+                ServiceArgType.run_mode.name: "active",
                 # FS_06_99_43_60 providing scalar value for list/array field is also possible:
                 ServiceArgType.group_label.name: "rrr",
             },
             {
                 envelope_payload_: {
                 },
                 test_data_: "TD_63_37_05_36",  # demo
@@ -698,14 +704,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-apac-downstream",
                 ServiceArgType.data_center.name: "dc.01",
                 ServiceArgType.host_name.name: "poiu-dd",
                 ServiceArgType.ip_address.name: "ip.192.168.1.3",
                 ServiceArgType.service_name.name: "xx",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "rrr",
                     "hhh",
                 ],
             },
             {
                 envelope_payload_: {
@@ -716,14 +723,15 @@
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-emea-upstream",
                 ServiceArgType.data_center.name: "dc.22",
                 ServiceArgType.host_name.name: "asdf-du",
                 ServiceArgType.ip_address.name: "ip.172.16.2.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -734,14 +742,15 @@
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-emea-upstream",
                 ServiceArgType.data_center.name: "dc.22",
                 ServiceArgType.host_name.name: "asdf-du",
                 ServiceArgType.ip_address.name: "ip.172.16.2.1",
                 ServiceArgType.service_name.name: "s_b",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "bbb",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -752,14 +761,15 @@
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-emea-downstream",
                 ServiceArgType.data_center.name: "dc.02",
                 ServiceArgType.host_name.name: "xcvb-dd",
                 ServiceArgType.ip_address.name: "ip.192.168.2.2",
                 ServiceArgType.service_name.name: "xx",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "rrr",
                     "hhh",
                 ],
             },
             {
                 envelope_payload_: {
@@ -770,14 +780,15 @@
                 ServiceArgType.geo_region.name: "emea",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "dev-emea-downstream",
                 ServiceArgType.data_center.name: "dc.02",
                 ServiceArgType.host_name.name: "xcvb-dd",
                 ServiceArgType.ip_address.name: "ip.192.168.2.2",
                 ServiceArgType.service_name.name: "zz",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "rrr",
                     "hhh",
                     "odd",
                 ],
             },
             {
@@ -789,14 +800,15 @@
                 ServiceArgType.geo_region.name: "amer",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "dev-amer-upstream",
                 ServiceArgType.data_center.name: "dc.03",
                 ServiceArgType.host_name.name: "qwer-du",
                 ServiceArgType.ip_address.name: "ip.192.168.3.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -807,14 +819,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "qa-apac-upstream",
                 ServiceArgType.data_center.name: "dc.04",
                 ServiceArgType.host_name.name: "hjkl-qu",
                 ServiceArgType.ip_address.name: "ip.192.168.4.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -825,14 +838,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "qa-apac-upstream",
                 ServiceArgType.data_center.name: "dc.04",
                 ServiceArgType.host_name.name: "hjkl-qu",
                 ServiceArgType.ip_address.name: "ip.192.168.4.1",
                 ServiceArgType.service_name.name: "s_b",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "bbb",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -843,14 +857,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "qa-apac-upstream",
                 ServiceArgType.data_center.name: "dc.44",
                 ServiceArgType.host_name.name: "poiu-qu",
                 ServiceArgType.ip_address.name: "ip.172.16.4.2",
                 ServiceArgType.service_name.name: "s_c",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "ccc",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -861,14 +876,15 @@
                 ServiceArgType.geo_region.name: "amer",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "qa-amer-upstream",
                 ServiceArgType.data_center.name: "dc.06",
                 ServiceArgType.host_name.name: "rtyu-qu",
                 ServiceArgType.ip_address.name: "ip.192.168.6.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -879,14 +895,15 @@
                 ServiceArgType.geo_region.name: "amer",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "qa-amer-downstream",
                 ServiceArgType.data_center.name: "dc.06",
                 ServiceArgType.host_name.name: "sdfgh-qd",
                 ServiceArgType.ip_address.name: "ip.192.168.6.3",
                 ServiceArgType.service_name.name: "tt1",
+                ServiceArgType.run_mode.name: "active",
                 # FS_06_99_43_60 providing scalar value for list/array field is also possible:
                 ServiceArgType.group_label.name: "rrr",
             },
             {
                 envelope_payload_: {
                 },
                 test_data_: "TD_63_37_05_36",  # demo
@@ -895,14 +912,15 @@
                 ServiceArgType.geo_region.name: "amer",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "qa-amer-downstream",
                 ServiceArgType.data_center.name: "dc.06",
                 ServiceArgType.host_name.name: "sdfgb-qd",
                 ServiceArgType.ip_address.name: "ip.192.168.6.4",
                 ServiceArgType.service_name.name: "xx",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "rrr",
                     "hhh",
                 ],
             },
             {
                 envelope_payload_: {
@@ -913,14 +931,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "qwer-pd-1",
                 ServiceArgType.ip_address.name: "ip.192.168.7.1",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -931,14 +950,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "qwer-pd-1",
                 ServiceArgType.ip_address.name: "ip.192.168.7.1",
                 ServiceArgType.service_name.name: "s_b",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "bbb",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -949,14 +969,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "qwer-pd-3",
                 ServiceArgType.ip_address.name: "ip.192.168.7.2",
                 ServiceArgType.service_name.name: "s_c",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "ccc",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -967,14 +988,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.77",
                 ServiceArgType.host_name.name: "qwer-pd-2",
                 ServiceArgType.ip_address.name: "ip.172.16.7.2",
                 ServiceArgType.service_name.name: "s_a",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "aaa",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -985,14 +1007,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.77",
                 ServiceArgType.host_name.name: "qwer-pd-2",
                 ServiceArgType.ip_address.name: "ip.172.16.7.2",
                 ServiceArgType.service_name.name: "s_b",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "bbb",
                     "xxx",
                 ],
             },
             {
                 envelope_payload_: {
@@ -1003,14 +1026,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "upstream",
                 ServiceArgType.cluster_name.name: "prod-apac-upstream",
                 ServiceArgType.data_center.name: "dc.77",
                 ServiceArgType.host_name.name: "qwer-pd-2",
                 ServiceArgType.ip_address.name: "ip.172.16.7.2",
                 ServiceArgType.service_name.name: "s_c",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "ccc",
                     "sss",
                 ],
             },
             {
                 envelope_payload_: {
@@ -1021,14 +1045,49 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "prod-apac-downstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "wert-pd-1",
                 ServiceArgType.ip_address.name: "ip.192.168.7.3",
                 ServiceArgType.service_name.name: "tt1",
+                ServiceArgType.run_mode.name: "active",
+                # FS_06_99_43_60 providing scalar value for list/array field is also possible:
+                ServiceArgType.group_label.name: "rrr",
+            },
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_63_37_05_36",  # demo
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassService.name,
+                ServiceArgType.code_maturity.name: "prod",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "prod-apac-downstream",
+                ServiceArgType.data_center.name: "dc.07",
+                ServiceArgType.host_name.name: "wert-pd-1",
+                ServiceArgType.ip_address.name: "ip.192.168.7.3",
+                ServiceArgType.service_name.name: "tt2",
+                ServiceArgType.run_mode.name: "passive",
+                # FS_06_99_43_60 providing scalar value for list/array field is also possible:
+                ServiceArgType.group_label.name: "rrr",
+            },
+            {
+                envelope_payload_: {
+                },
+                test_data_: "TD_63_37_05_36",  # demo
+                ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassService.name,
+                ServiceArgType.code_maturity.name: "prod",
+                ServiceArgType.geo_region.name: "apac",
+                ServiceArgType.flow_stage.name: "downstream",
+                ServiceArgType.cluster_name.name: "prod-apac-downstream",
+                ServiceArgType.data_center.name: "dc.07",
+                ServiceArgType.host_name.name: "wert-pd-2",
+                ServiceArgType.ip_address.name: "ip.192.168.7.4",
+                ServiceArgType.service_name.name: "tt1",
+                ServiceArgType.run_mode.name: "passive",
                 # FS_06_99_43_60 providing scalar value for list/array field is also possible:
                 ServiceArgType.group_label.name: "rrr",
             },
             {
                 envelope_payload_: {
                 },
                 test_data_: "TD_63_37_05_36",  # demo
@@ -1037,14 +1096,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "prod-apac-downstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "wert-pd-2",
                 ServiceArgType.ip_address.name: "ip.192.168.7.4",
                 ServiceArgType.service_name.name: "tt2",
+                ServiceArgType.run_mode.name: "active",
                 # FS_06_99_43_60 providing scalar value for list/array field is also possible:
                 ServiceArgType.group_label.name: "rrr",
             },
             {
                 envelope_payload_: {
                 },
                 test_data_: "TD_63_37_05_36",  # demo
@@ -1053,14 +1113,15 @@
                 ServiceArgType.geo_region.name: "apac",
                 ServiceArgType.flow_stage.name: "downstream",
                 ServiceArgType.cluster_name.name: "prod-apac-downstream",
                 ServiceArgType.data_center.name: "dc.07",
                 ServiceArgType.host_name.name: "wert-pd-2",
                 ServiceArgType.ip_address.name: "ip.192.168.7.4",
                 ServiceArgType.service_name.name: "xx",
+                ServiceArgType.run_mode.name: "active",
                 ServiceArgType.group_label.name: [
                     "rrr",
                     "hhh",
                 ],
             },
         ])
 
@@ -1327,14 +1388,15 @@
                             ServiceArgType.flow_stage.name: flow_stage,
                             ServiceArgType.cluster_name.name: cluster_name,
                             ServiceArgType.host_name.name: host_name,
                         }
 
                         host_envelopes.append(generated_host)
 
+                        run_mode = "active"
                         for service_name in ["sn{:02d}".format(snn) for snn in range(0, self.object_multiplier)]:
                             ############################################################################################################
                             # services
 
                             generated_service = {
                                 envelope_payload_: {
                                 },
@@ -1342,16 +1404,24 @@
                                 ReservedArgType.EnvelopeClass.name: ServiceEnvelopeClass.ClassService.name,
                                 ServiceArgType.code_maturity.name: code_maturity,
                                 ServiceArgType.geo_region.name: geo_region,
                                 ServiceArgType.flow_stage.name: flow_stage,
                                 ServiceArgType.cluster_name.name: cluster_name,
                                 ServiceArgType.host_name.name: host_name,
                                 ServiceArgType.service_name.name: service_name,
+                                ServiceArgType.run_mode.name: run_mode,
                             }
 
+                            # Even (0, 2, ...) => active
+                            # Odd (1, 3, ...) => passive
+                            if run_mode == "active":
+                                run_mode = "passive"
+                            else:
+                                run_mode = "active"
+
                             service_envelopes.append(generated_service)
 
     def populate_TD_43_24_76_58_single(
         self,
         cluster_envelopes: list[dict],
         host_envelopes: list[dict],
         service_envelopes: list[dict],
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/ServiceLoaderConfigSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ/git_utils.py` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ/git_utils.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_common_lib.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/argrelay_common_lib.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/argrelay_rc.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/argrelay_rc.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/bootstrap_dev_env.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/bootstrap_dev_env.bash`

 * *Files 1% similar despite different names*

```diff
@@ -227,18 +227,21 @@
 source "${argrelay_dir}/conf/python_conf.bash"
 
 # Cut out Python version number chars (from first digit until first space):
 # shellcheck disable=SC2154
 curr_python_version="$( "${path_to_pythonX}" --version 2>&1 | sed 's/^[^[:digit:]]*\([^[:space:]]*\).*$/\1/g' )"
 # Ensure Python version is not old:
 min_required_version="3.7"
-if ( echo "${curr_python_version}"; echo "${min_required_version}"; ) | sort --version-sort --check 2> /dev/null
+if [[ "${curr_python_version}" != "${min_required_version}" ]]
 then
-    # versions sorted = curr Python version is older:
-    "${ret_command}" 1
+    if ( echo "${curr_python_version}"; echo "${min_required_version}"; ) | sort --version-sort --check 2> /dev/null
+    then
+        # versions sorted = curr Python version is older:
+        "${ret_command}" 1
+    fi
 fi
 
 if [ ! -e "${path_to_venvX}" ]
 then
     pythonX_basename="$(basename "${path_to_pythonX}")"
     pythonX_dirname="$(dirname "${path_to_pythonX}")"
```

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/dev_shell.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/dev_shell.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/init_shell_env.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/init_shell_env.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/custom_integ_res/upgrade_all_packages.bash` & `argrelay-0.7.0.dev0/src/argrelay/custom_integ_res/upgrade_all_packages.bash`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/ArgSource.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/ArgSource.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/CallConv.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/CallConv.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/CompScope.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/CompScope.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/CompType.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/CompType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/DistinctValuesQuery.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/DistinctValuesQuery.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,27 @@
         ================================
         use_mongomock: True
         use_single_collection: True
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.011     0.035     0.122     0.461     1.650     5.945    27.836
-                         native_distinct     0.062     0.192     0.576     1.455     2.993     6.287    10.603
-                        native_aggregate     0.084     0.212     0.909     3.650    15.173    58.340   326.188
+                  original_find_and_loop     0.012     0.044     0.134     0.459     1.715     6.159    28.553
+                         native_distinct     0.077     0.209     0.581     1.538     3.186     6.295    11.231
+                        native_aggregate     0.077     0.227     0.913     3.717    15.944    63.955   375.196
         ================================
         use_mongomock: True
         use_single_collection: False
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.007     0.028     0.096     0.439     1.672     5.939    27.561
-                         native_distinct     0.048     0.159     0.465     1.224     2.725     5.539     9.572
-                        native_aggregate     0.031     0.109     0.398     1.758     7.802    28.463   126.566
+                  original_find_and_loop     0.011     0.031     0.102     0.431     1.750     6.061    35.473
+                         native_distinct     0.057     0.172     0.468     1.247     2.938     5.556    10.528
+                        native_aggregate     0.037     0.116     0.401     1.725     7.852    27.517   169.423
         ```
 
         *   The fastest on small collections is `original_find_and_loop`.
         *   The fastest on large collections is `native_distinct`.
 
     *   `pymongo`:
 
@@ -45,27 +45,27 @@
         ================================
         use_mongomock: False
         use_single_collection: True
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.022     0.031     0.065     0.115     0.222     0.505     0.748
-                         native_distinct     0.063     0.102     0.195     0.435     0.857     1.493     2.591
-                        native_aggregate     0.022     0.038     0.064     0.109     0.165     0.324     0.469
+                  original_find_and_loop     0.028     0.034     0.070     0.147     0.255     0.493     1.040
+                         native_distinct     0.070     0.137     0.264     0.550     0.976     1.896     3.452
+                        native_aggregate     0.028     0.046     0.070     0.115     0.207     0.354     0.550
         ================================
         use_mongomock: False
         use_single_collection: False
 
                        object_multiplier         3         4         5         6         7         8         9
                             object_count       243      1024      3125      7776     16807     32768     59049
         --------------------------------
-                  original_find_and_loop     0.020     0.025     0.048     0.144     0.175     0.383     0.590
-                         native_distinct     0.048     0.067     0.123     0.228     0.365     0.594     0.991
-                        native_aggregate     0.022     0.027     0.040     0.067     0.109     0.176     0.271
+                  original_find_and_loop     0.033     0.027     0.055     0.141     0.197     0.342     0.744
+                         native_distinct     0.047     0.088     0.158     0.285     0.479     0.821     1.389
+                        native_aggregate     0.023     0.030     0.054     0.073     0.120     0.191     0.326
         ```
 
         The fastest is `native_aggregate`.
     """
 
     original_find_and_loop = auto()
     """
```

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/ReservedArgType.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/ReservedArgType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/RunMode.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/RunMode.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/TermColor.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/TermColor.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,25 +22,26 @@
     back_bright_red = "\033[101m"
     back_bright_green = "\033[102m"
     back_bright_yellow = "\033[103m"
 
     fore_dark_red = "\033[31m"
     fore_dark_green = "\033[32m"
     fore_dark_yellow = "\033[33m"
-    fore_dark_cyan = "\033[36m"
+    fore_dark_blue = "\033[34m"
     fore_dark_magenta = "\033[35m"
+    fore_dark_cyan = "\033[36m"
     fore_dark_gray = "\033[90m"
 
     fore_bright_gray = "\033[90m"
     fore_bright_red = "\033[91m"
     fore_bright_green = "\033[92m"
     fore_bright_yellow = "\033[93m"
     fore_bright_blue = "\033[94m"
-    fore_bright_cyan = "\033[96m"
     fore_bright_magenta = "\033[95m"
+    fore_bright_cyan = "\033[96m"
     fore_bright_white = "\033[97m"
 
     fore_bold_dark_red = "\033[1;31m"
 
     ###################################################################################################################
     # Semantic colors:
 
@@ -74,33 +75,40 @@
     """
 
     remaining_value = fore_bright_yellow
     """
     See `EnvelopeContainer.remaining_types_to_values`.
     """
 
+    excluded_token = fore_dark_blue
+    """
+    See:
+    *   `InterpContext.excluded_tokens`
+    *   `InterpResult.excluded_tokens`
+    """
+
     consumed_token = fore_bright_blue
     """
     See:
-    *   `InterpContext.consumed_tokens`
-    *   `BaseResponse.consumed_tokens`
+    *   `InterpContext.consumed_arg_buckets`
+    *   `InterpResult.consumed_arg_buckets`
     """
 
-    unconsumed_token = fore_dark_magenta
+    remaining_token = fore_bright_magenta
     """
     See:
-    *   `InterpContext.unconsumed_tokens`
+    *   `InterpContext.remaining_arg_buckets`
     """
 
     no_option_to_suggest = fore_dark_gray
     """
     When none of the relevant `data_envelope`-s has values for the given prop.
     """
 
-    caption_hidden_by_default = fore_bright_magenta
+    caption_hidden_by_default = fore_dark_magenta
     """
     FS_72_53_55_13: Caption for values hidden by default.
     """
 
     value_hidden_by_default = fore_dark_yellow
     """
     FS_72_53_55_13: Option hidden by default.
```

### Comparing `argrelay-0.6.9/src/argrelay/enum_desc/TokenType.py` & `argrelay-0.7.0.dev0/src/argrelay/enum_desc/TokenType.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/handler_request/AbstractServerRequestHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_request/AbstractServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_request/DescribeLineArgsServerRequestHandler.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,18 +24,11 @@
         call_ctx: CallContext,
     ) -> dict:
         assert call_ctx.server_action is ServerAction.DescribeLineArgs
 
         self.interpret_command(self.local_server, call_ctx)
         ElapsedTime.measure("after_interpret_command")
 
-        input_object = InterpResult(
-            arg_values = self.interp_ctx.comp_suggestions,
-            all_tokens = self.interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = self.interp_ctx.consumed_tokens,
-            envelope_containers = self.interp_ctx.envelope_containers,
-            tan_token_ipos = self.interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = self.interp_ctx.parsed_ctx.tan_token_l_part,
-        )
+        input_object = InterpResult.from_interp_context(self.interp_ctx)
         response_dict = interp_result_desc.dict_schema.dump(input_object)
 
         return response_dict
```

### Comparing `argrelay-0.6.9/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_request/ProposeArgValuesServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_request/RelayLineArgsServerRequestHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from argrelay.schema_response.InterpResult import InterpResult
 from argrelay.schema_response.InterpResultSchema import interp_result_desc
 
 indent_size = 2
 
 
 class DescribeLineArgsClientResponseHandler(AbstractClientResponseHandler):
-
     default_overrides_caption: str = "overrides"
     """
     FS_72_53_55_13: Caption for options hidden by defaults.
     """
 
     def __init__(
         self,
@@ -44,22 +43,27 @@
 
         print()
 
         # Print command line:
         for i in range(len(interp_result.all_tokens)):
             if i == interp_result.tan_token_ipos:
                 DescribeLineArgsClientResponseHandler.render_tangent_token(interp_result, interp_result.all_tokens[i])
-            elif i in interp_result.consumed_tokens:
+            elif i in interp_result.consumed_token_ipos_list():
                 print(
                     f"{TermColor.consumed_token.value}{interp_result.all_tokens[i]}{TermColor.reset_style.value}",
                     end = " ",
                 )
+            elif i in interp_result.excluded_tokens:
+                print(
+                    f"{TermColor.excluded_token.value}{interp_result.all_tokens[i]}{TermColor.reset_style.value}",
+                    end = " ",
+                )
             else:
                 print(
-                    f"{TermColor.unconsumed_token.value}{interp_result.all_tokens[i]}{TermColor.reset_style.value}",
+                    f"{TermColor.remaining_token.value}{interp_result.all_tokens[i]}{TermColor.reset_style.value}",
                     end = " ",
                 )
 
         DescribeLineArgsClientResponseHandler.render_envelope_containers(
             interp_result.envelope_containers,
             interp_result.tan_token_l_part,
         )
@@ -128,21 +132,20 @@
                         f"[{envelope_container.assigned_types_to_values[arg_type].arg_source.name}]",
                         end = ""
                     )
                     print(TermColor.reset_style.value, end = "")
 
                     # FS_72_53_55_13: Renders options hidden by default:
                     if len(envelope_container.filled_types_to_values_hidden_by_defaults) != 0:
-
-                        print(" ", end = "")
-                        print(TermColor.caption_hidden_by_default.value, end = "")
-                        print(f"{DescribeLineArgsClientResponseHandler.default_overrides_caption}:", end = "")
-                        print(TermColor.reset_style.value, end = " ")
-
                         if arg_type in envelope_container.filled_types_to_values_hidden_by_defaults:
+                            print(" ", end = "")
+                            print(TermColor.caption_hidden_by_default.value, end = "")
+                            print(f"{DescribeLineArgsClientResponseHandler.default_overrides_caption}:", end = "")
+                            print(TermColor.reset_style.value, end = " ")
+
                             values_hidden_by_defaults = envelope_container.filled_types_to_values_hidden_by_defaults[
                                 arg_type
                             ]
                             DescribeLineArgsClientResponseHandler.highlight_prefix(
                                 values_hidden_by_defaults,
                                 value_prefix,
                                 TermColor.value_hidden_by_default,
```

### Comparing `argrelay-0.6.9/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py` & `argrelay-0.7.0.dev0/src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/misc_helper_common/ElapsedTime.py` & `argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/ElapsedTime.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/misc_helper_common/TypeDesc.py` & `argrelay-0.7.0.dev0/src/argrelay/misc_helper_common/TypeDesc.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/misc_helper_server/__init__.py` & `argrelay-0.7.0.dev0/src/argrelay/misc_helper_server/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/mongo_data/MongoClientWrapper.py` & `argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoClientWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/mongo_data/MongoConfig.py` & `argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/mongo_data/MongoServerWrapper.py` & `argrelay-0.7.0.dev0/src/argrelay/mongo_data/MongoServerWrapper.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_config/AbstractConfigurator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_config/AbstractConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfigurator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfigurator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfig.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.plugin_config.DefaultConfiguratorConfig import DefaultConfiguratorConfig
 
 """
 Schema for :class:`DefaultConfiguratorConfig`
 """
 
@@ -12,48 +13,41 @@
 project_page_url_ = "project_page_url"
 
 git_files_by_commit_id_url_prefix_ = "git_files_by_commit_id_url_prefix"
 
 commit_id_url_prefix_ = "commit_id_url_prefix"
 
 
-class DefaultConfiguratorConfigSchema(Schema):
+class DefaultConfiguratorConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         ordered = True
 
+    model_class = DefaultConfiguratorConfig
+
     project_title = fields.String(
         required = False,
+        load_default = None,
     )
 
     project_page_url = fields.String(
         required = False,
+        load_default = None,
     )
 
     git_files_by_commit_id_url_prefix = fields.String(
         required = False,
+        load_default = None,
     )
 
     commit_id_url_prefix = fields.String(
         required = False,
+        load_default = None,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return DefaultConfiguratorConfig(
-            project_title = input_dict.get(project_title_, None),
-            project_page_url = input_dict.get(project_page_url_, None),
-            git_files_by_commit_id_url_prefix = input_dict.get(git_files_by_commit_id_url_prefix_, None),
-            commit_id_url_prefix = input_dict.get(commit_id_url_prefix_, None),
-        )
-
 
 default_configurator_config_desc = TypeDesc(
     dict_schema = DefaultConfiguratorConfigSchema(),
     ref_name = DefaultConfiguratorConfigSchema.__name__,
     dict_example = {
         project_title_: "relay_demo",
         project_page_url_: "https://argrelay.org",
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/AbstractDelegator.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/AbstractJumpDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/AbstractJumpDelegator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 from typing import Union
 
+from argrelay.composite_tree.CompositeForestSchema import composite_forest_desc
+from argrelay.composite_tree.CompositeInfoType import CompositeInfoType
+from argrelay.composite_tree.CompositeTreeWalker import extract_tree_abs_path_to_interp_id
+from argrelay.composite_tree.DictTreeWalker import DictTreeWalker
 from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator
+from argrelay.plugin_delegator.AbstractJumpDelegatorConfigSchema import (
+    tree_abs_path_to_interp_id_,
+    abstract_jump_delegator_config_desc, single_func_id_,
+)
 from argrelay.plugin_interp.AbstractInterp import AbstractInterp
-from argrelay.plugin_interp.TreeWalker import TreeWalker
 from argrelay.runtime_data.ServerConfig import ServerConfig
 
-# TODO: TODO_10_72_28_05: Consider config schema for both `InterceptDelegator` and `HelpDelegator` (however, this should be removed with FS_33_76_82_84 gtree):
-tree_abs_path_to_interp_id_ = "tree_abs_path_to_interp_id"
-
 
 class AbstractJumpDelegator(AbstractDelegator):
 
     def __init__(
         self,
         server_config: ServerConfig,
         plugin_instance_id: str,
@@ -21,27 +25,46 @@
     ):
         super().__init__(
             server_config,
             plugin_instance_id,
             plugin_config_dict,
         )
 
-        func_tree_walker = TreeWalker(
-            tree_abs_path_to_interp_id_,
+        self._compare_config_with_composite_tree()
+
+        dict_tree_walker = DictTreeWalker(
+            CompositeInfoType.tree_abs_path_to_interp_id,
             self.plugin_config_dict[tree_abs_path_to_interp_id_],
         )
         # Temporary (reversed) map which contains path per id (instead of id per path):
-        temporary_id_to_paths: dict[str, list[list[str]]] = func_tree_walker.build_str_leaves_paths()
+        temporary_id_to_paths: dict[str, list[list[str]]] = dict_tree_walker.build_str_leaves_paths()
 
         # Reverse temporary path per id map into id per path map:
         self.tree_path_to_next_interp_plugin_instance_id: dict[tuple[str, ...], str] = {}
         for interp_plugin_id, tree_abs_paths in temporary_id_to_paths.items():
             for tree_abs_path in tree_abs_paths:
                 self.tree_path_to_next_interp_plugin_instance_id[tuple(tree_abs_path)] = interp_plugin_id
 
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree(
+        self,
+    ):
+        expected_dict = self.plugin_config_dict[tree_abs_path_to_interp_id_]
+        actual_dict = extract_tree_abs_path_to_interp_id(
+            self.server_config.server_plugin_control.composite_forest,
+            self.plugin_config_dict[single_func_id_],
+        )
+        assert expected_dict == actual_dict
+
+    def load_config(
+        self,
+        plugin_config_dict,
+    ) -> dict:
+        return abstract_jump_delegator_config_desc.dict_from_input_dict(plugin_config_dict)
+
     def run_interp_control(
         self,
         curr_interp: AbstractInterp,
     ) -> Union[None, str]:
         # TODO_10_72_28_05: support special funcs for all commands:
         #                   Delegator must select next `interp_factory_id` based on `interp_tree_abs_path` via `tree_abs_path_to_interp_id` (not based on single plugin id specified)
         #                   because delegator can be accessible through multiple tree paths.
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/EchoDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/QueryEnumDelegator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,43 @@
 from __future__ import annotations
 
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.enum_desc.SpecialFunc import SpecialFunc
-from argrelay.plugin_delegator.AbstractDelegator import AbstractDelegator
-from argrelay.relay_server.LocalServer import LocalServer
-from argrelay.runtime_context.InterpContext import InterpContext
+from argrelay.handler_response.DescribeLineArgsClientResponseHandler import DescribeLineArgsClientResponseHandler
+from argrelay.plugin_delegator.AbstractJumpDelegator import AbstractJumpDelegator
+from argrelay.runtime_context.InterpContext import function_container_ipos_
 from argrelay.schema_config_interp.DataEnvelopeSchema import instance_data_
 from argrelay.schema_config_interp.FunctionEnvelopeInstanceDataSchema import (
-    func_id_,
     delegator_plugin_instance_id_,
     search_control_list_,
+    func_id_,
 )
 from argrelay.schema_response.InvocationInput import InvocationInput
 
+subsequent_function_container_ipos_ = function_container_ipos_ + 1
+
 
-class EchoDelegator(AbstractDelegator):
+class QueryEnumDelegator(AbstractJumpDelegator):
     """
-    Implements FS_43_50_57_71 `echo_args` func.
+    FS_02_25_41_81: Implements `query_enum_items_func`.
     """
 
     def get_supported_func_envelopes(
         self,
     ) -> list[dict]:
         func_envelopes = [{
             instance_data_: {
-                func_id_: SpecialFunc.echo_args_func.name,
+                func_id_: SpecialFunc.query_enum_items_func.name,
                 delegator_plugin_instance_id_: self.plugin_instance_id,
                 search_control_list_: [
                 ],
             },
             ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
-            ReservedArgType.HelpHint.name: (
-                f"Print command line args `{InvocationInput.__name__}`"
-            ),
-            ReservedArgType.FuncId.name: SpecialFunc.echo_args_func.name,
+            ReservedArgType.HelpHint.name: "Enumerate available arg options (based on existing arg values)",
+            ReservedArgType.FuncId.name: SpecialFunc.query_enum_items_func.name,
         }]
         return func_envelopes
 
-    def run_invoke_control(
-        self,
-        interp_ctx: InterpContext,
-        local_server: LocalServer,
-    ) -> InvocationInput:
-        invocation_input = InvocationInput(
-            arg_values = interp_ctx.comp_suggestions,
-            all_tokens = interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = interp_ctx.consumed_tokens,
-            envelope_containers = interp_ctx.envelope_containers,
-            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
-            delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
-                self.plugin_instance_id
-            ],
-            custom_plugin_data = {},
-        )
-        return invocation_input
-
     @staticmethod
     def invoke_action(invocation_input: InvocationInput):
-        print(" ".join(invocation_input.all_tokens))
+        DescribeLineArgsClientResponseHandler.render_result(invocation_input)
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/ErrorDelegator.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,21 +14,16 @@
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
             self.plugin_instance_id
         ]
-        invocation_input = InvocationInput(
-            arg_values = interp_ctx.comp_suggestions,
-            all_tokens = interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = interp_ctx.consumed_tokens,
-            envelope_containers = interp_ctx.envelope_containers,
-            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+        invocation_input = InvocationInput.with_interp_context(
+            interp_ctx,
             delegator_plugin_entry = delegator_plugin_entry,
             custom_plugin_data = {},
         )
         return invocation_input
 
     @staticmethod
     def invoke_action(invocation_input: InvocationInput):
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/HelpDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/HelpDelegator.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from argrelay.custom_integ.ServiceDelegator import redirect_to_no_func_error
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.enum_desc.SpecialFunc import SpecialFunc
 from argrelay.enum_desc.TermColor import TermColor
 from argrelay.plugin_delegator.AbstractDelegator import get_func_id_from_invocation_input
 from argrelay.plugin_delegator.AbstractJumpDelegator import AbstractJumpDelegator
-from argrelay.plugin_delegator.InterceptDelegator import InterceptDelegator
 from argrelay.plugin_interp.FuncTreeInterpFactory import tree_path_selector_prefix_
 from argrelay.relay_server.LocalServer import LocalServer
 from argrelay.runtime_context.InterpContext import function_container_ipos_, InterpContext
 from argrelay.schema_config_interp.DataEnvelopeSchema import instance_data_
 from argrelay.schema_config_interp.FunctionEnvelopeInstanceDataSchema import (
     delegator_plugin_instance_id_,
     search_control_list_,
@@ -37,15 +36,14 @@
             },
             ReservedArgType.EnvelopeClass.name: ReservedEnvelopeClass.ClassFunction.name,
             ReservedArgType.HelpHint.name: "List defined function matching search criteria with their help hints",
             ReservedArgType.FuncId.name: SpecialFunc.help_hint_func.name,
         }]
         return func_envelopes
 
-
     def run_invoke_control(
         self,
         interp_ctx: InterpContext,
         local_server: LocalServer,
     ) -> InvocationInput:
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
 
@@ -59,21 +57,16 @@
                 .query_data_envelopes_for(subsequent_function_container)
             )
 
             delegator_plugin_instance_id = self.plugin_instance_id
 
             custom_plugin_data = search_control_desc.dict_schema.dump(subsequent_function_container.search_control)
 
-            invocation_input = InvocationInput(
-                arg_values = interp_ctx.comp_suggestions,
-                all_tokens = interp_ctx.parsed_ctx.all_tokens,
-                consumed_tokens = interp_ctx.consumed_tokens,
-                envelope_containers = interp_ctx.envelope_containers,
-                tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-                tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+            invocation_input = InvocationInput.with_interp_context(
+                interp_ctx,
                 delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
                     delegator_plugin_instance_id
                 ],
                 custom_plugin_data = custom_plugin_data,
             )
             return invocation_input
         else:
@@ -90,18 +83,22 @@
                     .envelope_containers[subsequent_function_container_ipos_]
                     .data_envelopes
             ):
 
                 # Dynamic `search_control` does not contain full paths to funcs all the time -
                 # it is based on curr path within FS_01_89_09_24 interp tree and FS_26_43_73_72 func tree.
                 # Recognize props with the prefix instead (which are set on loading and remain static):
+                tree_path_selector_prop_names = []
                 for prop_name in data_envelope:
-                    if not prop_name.startswith(tree_path_selector_prefix_):
-                        continue
-                    print(f"{data_envelope[prop_name]}", end = " ")
+                    if prop_name.startswith(tree_path_selector_prefix_):
+                        tree_path_selector_prop_names.append(prop_name)
+                # Iterate through sorted prop names - `tree_path_selector_prefix_` is numbered:
+                tree_path_selector_prop_names.sort()
+                for tree_path_selector_prop_name in tree_path_selector_prop_names:
+                    print(f"{data_envelope[tree_path_selector_prop_name]}", end = " ")
 
                 # TODO: FS_02_25_41_81 (query_enum_items_func): perform color control only if the output is a terminal:
 
                 print(TermColor.known_envelope_id.value, end = "")
                 print("#", end = " ")
                 print(TermColor.reset_style.value, end = "")
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_delegator/InterceptDelegator.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_delegator/InterceptDelegator.py`

 * *Files 14% similar despite different names*

```diff
@@ -103,21 +103,16 @@
         local_server: LocalServer,
     ) -> InvocationInput:
         assert interp_ctx.is_func_found(), "the (first) function envelope must be found"
 
         # TODO: Fail (send to ErrorDelegator) if next function is not specified -
         #       showing the payload in this case is misleading.
         delegator_plugin_instance_id = self.plugin_instance_id
-        invocation_input = InvocationInput(
-            arg_values = interp_ctx.comp_suggestions,
-            all_tokens = interp_ctx.parsed_ctx.all_tokens,
-            consumed_tokens = interp_ctx.consumed_tokens,
-            envelope_containers = interp_ctx.envelope_containers,
-            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
-            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+        invocation_input = InvocationInput.with_interp_context(
+            interp_ctx,
             delegator_plugin_entry = local_server.server_config.plugin_instance_entries[
                 delegator_plugin_instance_id
             ],
             custom_plugin_data = {},
         )
         return invocation_input
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterp.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/AbstractInterp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from argrelay.enum_desc.InterpStep import InterpStep
 from argrelay.enum_desc.TokenType import get_token_type, TokenType
 
 from argrelay.runtime_context.InterpContext import InterpContext
 
+
 # `AbstractInterp` is NOT a plugin `AbstractInterpFactory` is:
 class AbstractInterp:
     """
     Interpreter processes command line sharing current state via :class:`InterpContext`.
 
     New instance of interpreter is created by (a plugin implementing) `AbstractInterpFactory` for each request.
     """
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/AbstractInterpFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/AbstractInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterp.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterpFactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from argrelay.composite_tree.CompositeTreeWalker import extract_zero_arg_interp_tree
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.plugin_interp.FirstArgInterp import FirstArgInterp
 from argrelay.plugin_interp.FirstArgInterpFactoryConfigSchema import (
     first_arg_interp_factory_config_desc,
     first_arg_vals_to_next_interp_factory_ids_,
     ignored_func_ids_list_,
 )
@@ -31,14 +32,24 @@
         converted_config = convert_FirstArgInterpConfig_to_InterpTreeInterpFactoryConfig(plugin_config_dict)
         super().__init__(
             server_config,
             plugin_instance_id,
             converted_config,
         )
 
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree(
+        self,
+    ):
+        expected_dict = self.plugin_config_dict[interp_selector_tree_]
+        actual_dict = extract_zero_arg_interp_tree(
+            self.server_config.server_plugin_control.composite_forest,
+        )
+        assert expected_dict == actual_dict
+
     def activate_plugin(
         self,
     ) -> None:
         """
         # NOTE: FS_42_76_93_51 first interp special case:
         TODO: Think of anther way because `FirstArgInterp` is obsolete - this role here only extends its agony.
         `FirstArgInterp` is used as the root and single instance which
@@ -72,15 +83,14 @@
                     raise RuntimeError(
                         f"plugin_instance_id='{self.plugin_instance_id}': func_id='{func_id}' is neither mapped anywhere nor is in `{ignored_func_ids_list_}`"
                     )
                 else:
                     # Func is ignored - skip:
                     continue
 
-
     def create_interp(
         self,
         interp_ctx: InterpContext,
     ) -> FirstArgInterp:
         return FirstArgInterp(
             self.plugin_instance_id,
             # FS_42_76_93_51 first interp special case:
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FirstArgInterpFactoryConfigSchema.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.plugin_interp.InterpTreeInterpFactory import InterpTreeInterpFactory
 from argrelay.plugin_interp.InterpTreeInterpFactoryConfigSchema import ignored_func_ids_list_
 
 first_arg_vals_to_next_interp_factory_ids_ = "first_arg_vals_to_next_interp_factory_ids"
 
+
 class FirstArgInterpFactoryConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     first_arg_vals_to_next_interp_factory_ids = fields.Dict(
         keys = fields.String(),
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterp.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterp.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,67 +94,105 @@
         # Function `search_control` is populated based on
         # tree path (FS_01_89_09_24 interp tree + FS_26_43_73_72 func tree)
         # and plugin config (rather than data found in `data_envelope`):
         self.interp_ctx.curr_container.search_control = search_control_desc.dict_schema.load(
             self.interp_tree_node_config_dict[func_search_control_]
         )
 
-
     def consume_pos_args(self) -> bool:
         """
-        Scans through `unconsumed_tokens` and tries to match its value against values of each type.
+        Scans through `remaining_arg_buckets` and tries to match its value against values of each type.
 
         Implements:
-        *   FS_76_29_13_28 arg consumption priorities
-        *   FS_44_36_84_88 consume args one by one
-            This func consumes all until the first unconsumed non-singled out arg.
+        *   FS_76_29_13_28 arg consumption priorities.
+        *   FS_44_36_84_88 consume args one by one:
+            This func consumes all until the first remaining non-singled out arg.
+        *   FS_97_64_39_94 `arg_bucket`-s: consumption is limited to single bucket per `envelope_container`.
         """
 
         consumed_token_ipos_list = []
         any_consumed = False
         # Related to FS_13_51_07_97 singled out implicit values:
-        # Whether we can consume more than one (without creating FS_51_67_38_37 impossible arg combinations)
-        # depends on whether first set of consumed args are already singled out.
-        # If arg is singled out but still matches unconsumed arg, it must be assigned as `ArgSource.ExplicitPosArg`
-        # rather than be left unconsumed and (later) be assigned as `ArgSource.ImplicitValue`.
-        can_consume_more = True
-        for unconsumed_token_ipos in self.interp_ctx.unconsumed_tokens:
-            unconsumed_token = self.interp_ctx.parsed_ctx.all_tokens[unconsumed_token_ipos]
+        # We can keep consuming args (without creating FS_51_67_38_37 impossible arg combinations)
+        # as long as they are singled out - we cannot consume two ambiguous args at once, but
+        # we can consume as many singled out as possible (plus one ambiguous).
+        # If arg is singled out but still matches remaining arg, it must be assigned as `ArgSource.ExplicitPosArg`
+        # rather than be left remaining and (later) be assigned as `ArgSource.ImplicitValue`.
+        consumed_ambiguous_value = False
+        if self.interp_ctx.curr_container.used_arg_bucket is not None:
+            # If `envelope_container` has one `used_arg_bucket`, loop through it only:
+            any_consumed = self.consume_pos_args_from_arg_bucket(
+                bucket_index = self.interp_ctx.curr_container.used_arg_bucket,
+                bucket_list = self.interp_ctx.remaining_arg_buckets[self.interp_ctx.curr_container.used_arg_bucket],
+                consumed_ambiguous_value = consumed_ambiguous_value,
+                consumed_token_ipos_list = consumed_token_ipos_list,
+            )
+        else:
+            # Otherwise, loop through all buckets until the single `used_arg_bucket` is chosen:
+            for bucket_index, bucket_list in enumerate(self.interp_ctx.remaining_arg_buckets):
+                any_consumed = self.consume_pos_args_from_arg_bucket(
+                    bucket_index = bucket_index,
+                    bucket_list = bucket_list,
+                    consumed_ambiguous_value = consumed_ambiguous_value,
+                    consumed_token_ipos_list = consumed_token_ipos_list,
+                )
+                if any_consumed:
+                    # Consume from single `arg_bucket` only:
+                    break
+
+        # perform list modifications out of the prev loop:
+        for consumed_token_ipos in consumed_token_ipos_list:
+            bucket_index = self.interp_ctx.token_ipos_to_arg_bucket_map[consumed_token_ipos]
+            self.interp_ctx.remaining_arg_buckets[bucket_index].remove(consumed_token_ipos)
+
+        return any_consumed
+
+    def consume_pos_args_from_arg_bucket(
+        self,
+        bucket_index,
+        bucket_list,
+        consumed_ambiguous_value,
+        consumed_token_ipos_list,
+    ) -> bool:
+        any_consumed = False
+        for remaining_token_ipos in bucket_list:
+
+            remaining_token = self.interp_ctx.parsed_ctx.all_tokens[remaining_token_ipos]
 
             # TODO: FS_76_29_13_28 Why not define the order based on FS_31_70_49_15 `search_control`
             #       (instead of whatever internal order `remaining_types_to_values` has)?
             #       It could already be the case that `remaining_types_to_values` are ordered as `search_control`.
             #       Why not make it explicit?
 
             # See if token matches any type by value:
             for arg_type, arg_values in self.interp_ctx.curr_container.remaining_types_to_values.items():
-                if unconsumed_token in arg_values:
-                    self.interp_ctx.curr_container.assigned_types_to_values[arg_type] = AssignedValue(
-                        unconsumed_token,
-                        ArgSource.ExplicitPosArg,
-                    )
-                    if len(arg_values) != 1:
-                        # This was not singled out arg:
-                        # stop consuming to avoid FS_51_67_38_37 impossible arg combinations.
-                        can_consume_more = False
-                    any_consumed = True
-                    consumed_token_ipos_list.append(unconsumed_token_ipos)
-                    self.interp_ctx.consumed_tokens.append(unconsumed_token_ipos)
-                    # TD_76_09_29_31: overlapped
-                    # Assign matching unconsumed arg value to the first type it matches (only once):
-                    del self.interp_ctx.curr_container.remaining_types_to_values[arg_type]
-                    break
-
-            if not can_consume_more:
-                break
-
-        # perform list modifications out of the prev loop:
-        for consumed_token_ipos in consumed_token_ipos_list:
-            self.interp_ctx.unconsumed_tokens.remove(consumed_token_ipos)
-
+                if remaining_token in arg_values:
+                    if (
+                        len(arg_values) == 1
+                        or
+                        not consumed_ambiguous_value
+                    ):
+                        self.interp_ctx.curr_container.assigned_types_to_values[arg_type] = AssignedValue(
+                            remaining_token,
+                            ArgSource.ExplicitPosArg,
+                        )
+                        self.interp_ctx.curr_container.used_arg_bucket = bucket_index
+                        if len(arg_values) > 1:
+                            # This was not singled out arg:
+                            # allow only one ambiguous consumption to avoid FS_51_67_38_37 impossible arg combinations.
+                            consumed_ambiguous_value = True
+                        any_consumed = True
+                        consumed_token_ipos_list.append(remaining_token_ipos)
+
+                        self.interp_ctx.consumed_arg_buckets[bucket_index].append(remaining_token_ipos)
+
+                        # TD_76_09_29_31: overlapped
+                        # Assign matching remaining arg value to the first type it matches (only once):
+                        del self.interp_ctx.curr_container.remaining_types_to_values[arg_type]
+                        break
         return any_consumed
 
     def try_iterate(self) -> InterpStep:
         """
         Try to consume more args if possible.
 
         *   If function was found, start with search for its first envelope class.
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from __future__ import annotations
 
 from copy import deepcopy
 
+from argrelay.composite_tree.CompositeInfoType import CompositeInfoType
+from argrelay.composite_tree.CompositeTreeWalker import extract_jump_tree, extract_func_tree
+from argrelay.composite_tree.DictTreeWalker import DictTreeWalker, normalize_tree
 from argrelay.enum_desc.ReservedArgType import ReservedArgType
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
 from argrelay.plugin_interp.AbstractInterp import AbstractInterp
 from argrelay.plugin_interp.AbstractInterpFactory import AbstractInterpFactory
 from argrelay.plugin_interp.FuncTreeInterp import FuncTreeInterp, func_init_control_, func_search_control_
 from argrelay.plugin_interp.FuncTreeInterpFactoryConfigSchema import (
     func_selector_tree_,
     func_tree_interp_config_desc,
     jump_tree_,
 )
-from argrelay.plugin_interp.TreeWalker import TreeWalker
 from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_core_server.EnvelopeCollectionSchema import init_envelop_collections
 from argrelay.schema_config_interp.InitControlSchema import init_types_to_values_
 from argrelay.schema_config_interp.SearchControlSchema import (
     keys_to_types_list_,
     populate_search_control,
@@ -40,32 +42,58 @@
         plugin_config_dict: dict,
     ):
         super().__init__(
             server_config,
             plugin_instance_id,
             plugin_config_dict,
         )
+
+        self._compare_config_with_composite_tree()
+
         # FS_26_43_73_72 func tree: func id to list of its relative paths populated by `load_func_envelopes`.
         # These func tree paths are relative to the interp node within FS_01_89_09_24 interp tree
         # (as fully qualified func path is composed of interp tree path where this plugin instance is attached to).
         # Each func id can be attached to more than one leaf (hence, there is a list of paths to that func id).
         self.func_ids_to_func_rel_paths: dict[str, list[list[str]]] = {}
 
         # FS_91_88_07_23 jump tree
         self.plugin_config_dict.setdefault(jump_tree_, {})
-        tree_walker: TreeWalker = TreeWalker(
-            "jump_tree",
+        dict_tree_walker: DictTreeWalker = DictTreeWalker(
+            CompositeInfoType.jump_tree,
             self.plugin_config_dict[jump_tree_],
         )
-        self.paths_to_jump: dict[tuple[str, ...], tuple[str, ...]] = tree_walker.build_paths_to_paths()
+        self.paths_to_jump: dict[tuple[str, ...], tuple[str, ...]] = dict_tree_walker.build_paths_to_paths()
         """
         Implements FS_91_88_07_23 jump tree:
         for given `interp_tree_abs_path` (FS_01_89_09_24) selects next `interp_tree_abs_path`.
         """
 
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree(
+        self,
+    ):
+        expected_dict = self.plugin_config_dict[jump_tree_]
+        actual_dict = extract_jump_tree(
+            self.server_config.server_plugin_control.composite_forest,
+        )
+        assert expected_dict == actual_dict
+
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree_func_tree(
+        self,
+        expected_func_selector_tree_dict: dict,
+    ):
+        expected_dict = normalize_tree(expected_func_selector_tree_dict)
+        actual_dict = extract_func_tree(
+            self.server_config.server_plugin_control.composite_forest,
+            self.plugin_instance_id,
+        )
+
+        assert expected_dict == actual_dict
+
     def load_config(
         self,
         plugin_config_dict,
     ) -> dict:
         return func_tree_interp_config_desc.dict_from_input_dict(plugin_config_dict)
 
     def load_func_envelopes(
@@ -82,19 +110,23 @@
 
         mapped_func_ids: list[str] = super().load_func_envelopes(
             interp_tree_abs_path,
             func_ids_to_func_envelopes,
         )
         interp_tree_node_config_dict = self.interp_tree_abs_paths_to_node_configs[interp_tree_abs_path]
 
-        func_tree_walker = TreeWalker(
-            "func_tree",
+        self._compare_config_with_composite_tree_func_tree(
+            interp_tree_node_config_dict[func_selector_tree_],
+        )
+
+        dict_tree_walker = DictTreeWalker(
+            CompositeInfoType.func_tree,
             interp_tree_node_config_dict[func_selector_tree_],
         )
-        self.func_ids_to_func_rel_paths: dict[str, list[list[str]]] = func_tree_walker.build_str_leaves_paths()
+        self.func_ids_to_func_rel_paths: dict[str, list[list[str]]] = dict_tree_walker.build_str_leaves_paths()
 
         # Loop through func `data_envelope`-s from all delegators:
         func_envelopes_index: dict[str, dict[tuple[str, ...], dict]] = {}
         for func_id, func_envelope in func_ids_to_func_envelopes.items():
             if func_id not in self.func_ids_to_func_rel_paths:
                 # Not used here:
                 continue
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 
 func_selector_tree_ = "func_selector_tree"
 
 jump_tree_ = "jump_tree"
 
 
+# TODO_40_10_18_32: add custom base to all schemas:
 class FuncTreeInterpFactoryConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    # TODO_79_67_28_83: Express recursive dict schema:
     # This is a tree (`dict`) of arbitrary depth with `str` leaves.
     # Ideally, this should be defined as nested `dict`,
     # but it is unknown how to do it in marshmallow.
     # Implements FS_26_43_73_72 func tree.
     func_selector_tree = fields.Raw(
         required = True,
     )
 
+    # TODO_79_67_28_83: Express recursive dict schema:
     # This is a tree (`dict`) of arbitrary depth with `list[str]` leaves.
     # Ideally, this should be defined as nested `dict`,
     # but it is unknown how to do it in marshmallow.
     # Implements FS_91_88_07_23 jump tree.
     jump_tree = fields.Raw(
         required = False,
     )
@@ -31,14 +34,17 @@
 
 func_tree_interp_config_example = {
     func_selector_tree_: {
         "list": {
             "repo": "list_repo_func",
             "service": "list_service_func",
         },
+        "diff": {
+            "service": "diff_service_func",
+        },
         "goto": {
             "repo": "goto_git_repo_func",
             "service": "goto_service_func",
         },
     },
     jump_tree_: [
         "relay_demo",
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterp.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterp.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Union
 
 from argrelay.enum_desc.InterpStep import InterpStep
 from argrelay.misc_helper_server import insert_unique_to_sorted_list
 from argrelay.plugin_interp.AbstractInterp import AbstractInterp
 from argrelay.plugin_interp.InterpTreeInterpFactoryConfigSchema import interp_selector_tree_
 from argrelay.plugin_interp.NoopInterpFactory import NoopInterpFactory
-from argrelay.plugin_interp.TreeWalker import default_tree_leaf_
+from argrelay.composite_tree.DictTreeWalker import surrogate_node_id_
 from argrelay.runtime_context.InterpContext import InterpContext
 
 
 def fetch_tree_node(
     tree_dict: dict,
     node_path: list[str],
 ):
@@ -53,62 +53,70 @@
         self.base_token_ipos: int = 1
 
     def consumes_args_at_once(self) -> bool:
         return True
 
     def consume_pos_args(self) -> bool:
         """
-        Consumes heading args in `unconsumed_tokens` according to the `interp_selector_tree`.
+        Consumes heading args in `remaining_arg_buckets` according to the `interp_selector_tree`.
 
-        Unlike normal guideline to consume one arg at time (FS_44_36_84_88), this func consumes all possible
+        Unlike normal guideline to consume one arg at time (FS_44_36_84_88),
+        this func consumes all possible args
         because args are selected according to the `interp_selector_tree` (not via query)
         and do not become incompatible by consuming all (causing FS_51_67_38_37 impossible arg combinations).
+
+        Also, FS_01_89_09_24 interp tree does not observe FS_97_64_39_94 `arg_bucket` boundaries
+        and consumes all necessary args sequentially.
         """
 
         curr_sub_tree = self.interp_selector_tree
         any_consumed = False
         while True:
             if isinstance(curr_sub_tree, str):
                 # Tree leaf is reached - use it:
                 self.next_interp_factory_id = curr_sub_tree
                 return any_consumed
 
-            if not self.interp_ctx.unconsumed_tokens:
+            # Always consume next remaining token:
+            # TODO: Is this assumption valid/safe that next remaining `ipos` is in the order it appears on command line?
+            #       Apparently, it is fine as we keep deleting head of `remaining_arg_buckets` below:
+            curr_token_ipos = self.interp_ctx.next_remaining_token_ipos()
+
+            if curr_token_ipos is None:
                 self.set_default_factory_id(curr_sub_tree)
                 return any_consumed
 
-            # Always consume next unconsumed token:
-            # TODO: Is this assumption valid/safe that next unconsumed `ipos` is in the order it appears on command line?
-            #       Apparently, it is fine as we keep deleting head of `unconsumed_tokens` below:
-            curr_token_ipos = self.interp_ctx.unconsumed_tokens[0]
             curr_token_value = self.interp_ctx.parsed_ctx.all_tokens[curr_token_ipos]
             assert self.is_pos_arg(curr_token_ipos)
 
             if isinstance(curr_sub_tree, dict):
                 if curr_token_value in curr_sub_tree:
                     # Consume one more arg into path:
                     self.interp_tree_rel_path.append(curr_token_value)
-                    self.interp_ctx.consumed_tokens.append(curr_token_ipos)
-                    del self.interp_ctx.unconsumed_tokens[0]
+
+                    bucket_index = self.interp_ctx.token_ipos_to_arg_bucket_map[curr_token_ipos]
+                    self.interp_ctx.consumed_arg_buckets[bucket_index].append(curr_token_ipos)
+                    del self.interp_ctx.remaining_arg_buckets[bucket_index][0]
+
                     curr_sub_tree = curr_sub_tree[curr_token_value]
                     any_consumed = True
                     continue
                 else:
                     self.set_default_factory_id(curr_sub_tree)
                     return any_consumed
             else:
                 raise LookupError()
 
     def set_default_factory_id(
         self,
         curr_sub_tree,
     ):
         # Impossible to consume more arg - use default of the current sub-tree:
-        if default_tree_leaf_ in curr_sub_tree:
-            self.next_interp_factory_id = curr_sub_tree[default_tree_leaf_]
+        if surrogate_node_id_ in curr_sub_tree:
+            self.next_interp_factory_id = curr_sub_tree[surrogate_node_id_]
         else:
             # TODO: Do not hardcode plugin id (instance of `NoopInterpFactory`):
             self.next_interp_factory_id = f"{NoopInterpFactory.__name__}.default"
 
     def try_iterate(self) -> InterpStep:
         return InterpStep.NextInterp
 
@@ -135,38 +143,38 @@
         )
         if isinstance(curr_sub_tree, dict):
             for proposed_value in [
                 x for x in curr_sub_tree
                 if (
                     isinstance(x, str)
                     and
-                    x != default_tree_leaf_
+                    x != surrogate_node_id_
                     and
                     # FS_32_05_46_00: using `startswith`:
                     x.startswith(self.interp_ctx.parsed_ctx.tan_token_l_part)
                 )
             ]:
                 insert_unique_to_sorted_list(self.interp_ctx.comp_suggestions, proposed_value)
 
     def is_eligible_for_suggestion(self):
         """
         Suggesting anything is possible only if there is no other tokens
         (after those recorded in `interp_tree_rel_path`) available for consumption by subsequent interpreters.
         """
 
-        if len(self.interp_ctx.unconsumed_tokens) == 0:
+        if self.interp_ctx.next_remaining_token_ipos() is None:
             return True
         else:
             return False
 
         # TODO: Clean up code below or take into account tangent token (ipos cursor position).
         #       Note that there is no ipos cursor position at the moment.
         #       It has to be computed with help of FS_23_62_89_43 tangent token
-        #       (which might be a surrogate one if cursor does nto touch non-whitespace chars).
-        remaining_consumed_tokens = deepcopy(self.interp_ctx.consumed_tokens)
+        #       (which might be a surrogate one if cursor does not touch non-whitespace chars).
+        remaining_consumed_tokens = deepcopy(self.interp_ctx.consumed_token_ipos_list())
 
         # Remove everything until `base_token_ipos`:
         for token_ipos in range(0, self.base_token_ipos):
             assert token_ipos in remaining_consumed_tokens
             remaining_consumed_tokens.remove(token_ipos)
 
         # Remove everything eaten into `interp_tree_rel_path`:
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 import contextlib
 
+from argrelay.composite_tree.CompositeInfoType import CompositeInfoType
+from argrelay.composite_tree.CompositeTreeWalker import extract_interp_tree
+from argrelay.composite_tree.DictTreeWalker import DictTreeWalker
 from argrelay.enum_desc.PluginType import PluginType
 from argrelay.plugin_interp.AbstractInterpFactory import AbstractInterpFactory
 from argrelay.plugin_interp.InterpTreeInterp import InterpTreeInterp
 from argrelay.plugin_interp.InterpTreeInterpFactoryConfigSchema import (
     tree_path_interp_factory_config_desc,
     interp_selector_tree_,
 )
-from argrelay.plugin_interp.TreeWalker import TreeWalker
 from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_data.ServerConfig import ServerConfig, assert_plugin_instance_id
 
 
 class InterpTreeInterpFactory(AbstractInterpFactory):
     """
     Implements FS_01_89_09_24 interp tree.
@@ -28,14 +30,27 @@
         super().__init__(
             server_config,
             plugin_instance_id,
             plugin_config_dict,
         )
         self.is_recursive_func_load = False
 
+        self._compare_config_with_composite_tree()
+
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree(
+        self,
+    ):
+        expected_dict = self.plugin_config_dict[interp_selector_tree_]
+        actual_dict = extract_interp_tree(
+            self.server_config.server_plugin_control.composite_forest,
+            self.plugin_instance_id,
+        )
+        assert expected_dict == actual_dict
+
     def load_config(
         self,
         plugin_config_dict,
     ) -> dict:
         return tree_path_interp_factory_config_desc.dict_from_input_dict(plugin_config_dict)
 
     def load_func_envelopes(
@@ -71,20 +86,20 @@
         interp_tree_abs_path: tuple[str, ...],
         func_ids_to_func_envelopes: dict[str, dict],
     ) -> list[str]:
         mapped_func_ids: list[str] = super().load_func_envelopes(
             interp_tree_abs_path,
             func_ids_to_func_envelopes,
         )
-        tree_walker: TreeWalker = TreeWalker(
-            "interp_tree",
+        dict_tree_walker: DictTreeWalker = DictTreeWalker(
+            CompositeInfoType.interp_tree,
             self.plugin_config_dict[interp_selector_tree_],
         )
         # Walk configured interp tree and call `load_func_envelopes` with `interp_tree_abs_path` for each interp.
-        interp_rel_paths: dict[str, list[list[str]]] = tree_walker.build_str_leaves_paths()
+        interp_rel_paths: dict[str, list[list[str]]] = dict_tree_walker.build_str_leaves_paths()
         for interp_plugin_id in interp_rel_paths:
             for interp_rel_path in interp_rel_paths[interp_plugin_id]:
                 assert_plugin_instance_id(
                     self.server_config,
                     interp_plugin_id,
                     PluginType.InterpFactoryPlugin,
                 )
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from marshmallow import Schema, RAISE, fields, validates_schema, ValidationError
 
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.plugin_interp.FuncTreeInterpFactory import FuncTreeInterpFactory
-from argrelay.plugin_interp.TreeWalker import default_tree_leaf_
+from argrelay.composite_tree.DictTreeWalker import surrogate_node_id_
 
 interp_selector_tree_ = "interp_selector_tree"
 
 ignored_func_ids_list_ = "ignored_func_ids_list"
 
+
 def validate_tree_node(interp_selector_sub_tree: dict):
     if isinstance(interp_selector_sub_tree, str):
         return
     elif isinstance(interp_selector_sub_tree, dict):
         for sub_tree_node in interp_selector_sub_tree.values():
             validate_tree_node(sub_tree_node)
     else:
         raise ValidationError(f"neither a str nor a dict: {interp_selector_sub_tree}")
 
 
+# TODO_40_10_18_32: add custom base to all schemas:
 class InterpTreeInterpFactoryConfigSchema(Schema):
     class Meta:
         unknown = RAISE
         strict = True
 
     interp_selector_tree = fields.Dict(
         keys = fields.String(),
+        # TODO_79_67_28_83: Express recursive dict schema:
         # This is a tree (`dict`) of arbitrary depth with `str` leaves.
         # Ideally, this should be defined as nested `dict`,
         # but it is unknown how to do it in marshmallow.
         values = fields.Raw(),
         required = True,
     )
 
     # TODO: FS_42_76_93_51: Decide already whether first zero arg interp deserves its future life.
     #                       This `ignored_func_ids_list` field is propagated down from
-    #                       the first zero arg interp (needed for its logic as root plugin instance in the global tree)
+    #                       the first zero arg interp (needed for its logic as root plugin instance in the composite tree)
     #                       and it also needs to pass validation of this schema (which it converts its config to):
     # It is an error if `func_id` is published by enabled delegator but missing in `func_selector_tree`.
     # To avoid the error, list such func id in `ignored_func_ids_list`.
     ignored_func_ids_list = fields.List(
         fields.String(),
         required = False,
         load_default = [],
@@ -55,15 +58,15 @@
             raise ValidationError(f"not a dict: {interp_selector_tree}")
         validate_tree_node(interp_selector_tree)
 
 
 tree_path_interp_factory_config_example = {
     interp_selector_tree_: {
         "some_command": "some_plugin_name",
-        default_tree_leaf_: f"{FuncTreeInterpFactory.__name__}.default",
+        surrogate_node_id_: f"{FuncTreeInterpFactory.__name__}.default",
     },
     ignored_func_ids_list_: [
         "some_ignored_func",
     ],
 }
 tree_path_interp_factory_config_desc = TypeDesc(
     dict_schema = InterpTreeInterpFactoryConfigSchema(),
```

### Comparing `argrelay-0.6.9/src/argrelay/plugin_interp/NoopInterpFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/plugin_interp/NoopInterpFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/AbstractClient.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/AbstractClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/RemoteClient.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/RemoteClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/RemoteClientCommandFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/RemoteClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/__main__.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
 
 def client_config_dict_to_object(client_config_dict):
     """
     Optimized dict -> object conversion avoiding import of `*Schema` for performance:
     """
     client_config = ClientConfig(
+        __comment__ = client_config_dict.get("use_local_requests", None),
         use_local_requests = client_config_dict.get("use_local_requests", False),
         optimize_completion_request = client_config_dict.get("optimize_completion_request", True),
         connection_config = ConnectionConfig(
             server_host_name = client_config_dict["connection_config"]["server_host_name"],
             server_port_number = client_config_dict["connection_config"]["server_port_number"],
         ),
         show_pending_spinner = client_config_dict.get("show_pending_spinner", True),
```

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/proc_parent.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/proc_parent.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_client/proc_split.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_client/proc_split.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/CustomFlaskApp.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/CustomFlaskApp.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/HelpHintCache.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/HelpHintCache.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/LocalServer.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/LocalServer.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/QueryEngine.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/QueryEngine.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/QueryResult.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/QueryResult.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_client.js` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/argrelay_client.js`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/gui_static/argrelay_style.css` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_static/argrelay_style.css`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/gui_templates/argrelay_main.html` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/gui_templates/argrelay_main.html`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/route_api.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/route_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             data_json = request.data.decode("utf-8")
             call_ctx = call_context_desc.dict_schema.loads(data_json)
         elif request.content_type == "application/json":
             call_ctx = call_context_desc.dict_schema.load(request.json)
         else:
             abort(415)
 
-        ElapsedTime.measure("after_input_context_creation")
+        ElapsedTime.measure("after_call_context_creation")
         ElapsedTime.is_debug_enabled = call_ctx.is_debug_enabled
         return call_ctx
 
     @blueprint_api.route(
         ServerAction.ProposeArgValues.value,
         methods = ["post"],
     )
```

### Comparing `argrelay-0.6.9/src/argrelay/relay_server/route_gui.py` & `argrelay-0.7.0.dev0/src/argrelay/relay_server/route_gui.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/runtime_context/AbstractPlugin.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_context/AbstractPlugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,24 @@
     ):
         self.server_config: ServerConfig = server_config
         self.plugin_instance_id: str = plugin_instance_id
         self.plugin_config_dict: dict = self.load_config(plugin_config_dict)
 
         self.validate_config()
 
+    # TODO_10_72_28_05: This will go away together with switch to FS_33_76_82_84 composite tree config:
+    def _compare_config_with_composite_tree(
+        self,
+    ):
+        """
+        Compares `CompositeInfoType` extracted from `composite_tree` with
+        data manually specified in `plugin_config_dict`.
+        """
+        pass
+
     def load_config(
         self,
         plugin_config_dict,
     ) -> dict:
         """
         Pre-proces the given config on load (e.g. populate default values).
```

### Comparing `argrelay-0.6.9/src/argrelay/runtime_context/EnvelopeContainer.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_context/EnvelopeContainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
+from typing import Union
 
 from argrelay.enum_desc.ArgSource import ArgSource
 from argrelay.runtime_context.SearchControl import SearchControl
 from argrelay.runtime_data.AssignedValue import AssignedValue
 
 
 @dataclass
@@ -34,14 +35,19 @@
     """
 
     found_count: int = field(default = 0)
     """
     Counter of `data_envelope`-s found in the last query.
     """
 
+    used_arg_bucket: Union[int, None] = field(default = None)
+    """
+    FS_97_64_39_94 `arg_bucket` (index) where args were consumed from for the current `envelope_container`.
+    """
+
     # TODO: Maybe rename to `context_types_to_values`?
     # TODO: Part of (or actually is?) `args_context`: FS_62_25_92_06:
     assigned_types_to_values: dict[str, AssignedValue] = field(default_factory = lambda: {})
     """
     All assigned args (from interpreted tokens) mapped as type:value which belong to `data_envelope`.
     """
```

### Comparing `argrelay-0.6.9/src/argrelay/runtime_context/InterpContext.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_context/InterpContext.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from __future__ import annotations
 
 from copy import deepcopy
 from dataclasses import field, dataclass
+from typing import Union
 
 from argrelay.enum_desc.ArgSource import ArgSource
 from argrelay.enum_desc.InterpStep import InterpStep
 from argrelay.enum_desc.ServerAction import ServerAction
+from argrelay.enum_desc.SpecialChar import SpecialChar
 from argrelay.enum_desc.TermColor import TermColor
 from argrelay.misc_helper_common import eprint
 from argrelay.misc_helper_common.ElapsedTime import ElapsedTime
 from argrelay.relay_server.HelpHintCache import HelpHintCache
 from argrelay.relay_server.QueryEngine import QueryEngine, populate_query_dict
 from argrelay.relay_server.QueryResult import QueryResult
 from argrelay.runtime_context.EnvelopeContainer import EnvelopeContainer
 from argrelay.runtime_context.ParsedContext import ParsedContext
 from argrelay.runtime_context.SearchControl import SearchControl
+from argrelay.runtime_context.arg_buckets_utils import arg_buckets_to_token_ipos_list
 
 function_container_ipos_ = 0
 
 
 @dataclass
 class InterpContext:
     """
@@ -38,22 +41,44 @@
     Reference to `ServerConfig.action_delegators`.
     """
 
     query_engine: QueryEngine = field()
 
     help_hint_cache: HelpHintCache = field()
 
-    unconsumed_tokens: list[int] = field(init = False)
+    excluded_tokens: list[int] = field(init = False, default_factory = lambda: [])
     """
-    Remaining tokens (their ipos) which are still unconsumed (in ascending order).
+    Tokens excluded by ways other than consumption into `consumed_arg_buckets`.
     """
 
-    consumed_tokens: list[int] = field(init = False, default_factory = lambda: [])
+    included_arg_buckets: list[list[int]] = field(init = False, default_factory = lambda: [])
     """
-    Already consumed tokens (their ipos) in the order of their consumption.
+    FS_97_64_39_94: arg buckets
+    
+    If `included_arg_buckets` are combined,
+    the result will contain both `remaining_arg_buckets` and `consumed_arg_buckets`.
+    Field `included_arg_buckets` is maximum set for arg buckets -
+    it is similar to maximum set `ParsedContext.all_tokens`,
+    but it cannot contain all tokens - it must exclude at least `SpecialChar.ArgBucketDelimiter` to start with.
+    """
+
+    remaining_arg_buckets: list[list[int]] = field(init = False)
+    """
+    Same as `included_arg_buckets` but for remaining tokens only.
+    """
+
+    consumed_arg_buckets: list[list[int]] = field(init = False, default_factory = lambda: [])
+    """
+    Same as `included_arg_buckets` but for consumed tokens only.
+    """
+
+    token_ipos_to_arg_bucket_map: dict[int, int] = field(init = False, default_factory = lambda: {})
+    """
+    Index reversed to `included_arg_buckets` -
+    for each `token_ipos` it gives the index of the `arg_bucket` it is in.
     """
 
     envelope_containers: list[EnvelopeContainer] = field(init = False, default_factory = lambda: [])
     """
     Each `envelope_container` wraps `data_envelope`-s matching query and some associated data.
     """
 
@@ -87,31 +112,68 @@
     interp_tree_abs_path: tuple[str, ...] = field(init = False, default = tuple([]))
     """
     Provides curr path within FS_01_89_09_24 interp tree.
     Takes part in implementation of FS_01_89_09_24 interp tree.
     """
 
     def __post_init__(self):
-        self.unconsumed_tokens = self._init_unconsumed_tokens()
+        self._init_arg_buckets()
+
+    def _init_arg_buckets(self):
+        self.included_arg_buckets.append([])
+        curr_bucket_index = len(self.included_arg_buckets) - 1
+        curr_arg_bucket = self.included_arg_buckets[curr_bucket_index]
+        for token_ipos in range(0, len(self.parsed_ctx.all_tokens)):
+
+            # Split and populate FS_97_64_39_94 arg buckets:
+            if self.parsed_ctx.all_tokens[token_ipos] == SpecialChar.ArgBucketDelimiter.value:
+                self.included_arg_buckets.append([])
+                curr_bucket_index = len(self.included_arg_buckets) - 1
+                curr_arg_bucket = self.included_arg_buckets[curr_bucket_index]
+                # Exclude `SpecialChar.ArgBucketDelimiter` unconditionally:
+                self.excluded_tokens.append(token_ipos)
+            else:
+
+                if self.parsed_ctx.server_action is ServerAction.ProposeArgValues:
+                    # FS_23_62_89_43 tangent arg value completion:
+                    # `ServerAction.ProposeArgValues` excludes tangent token because it is supposed to be completed:
+                    if token_ipos == self.parsed_ctx.tan_token_ipos:
+                        self.excluded_tokens.append(token_ipos)
+                    else:
+                        curr_arg_bucket.append(token_ipos)
+                        self.token_ipos_to_arg_bucket_map[token_ipos] = curr_bucket_index
+                else:
+                    # FS_23_62_89_43 tangent arg value completion:
+                    # Process all tokens (including tangent token) in case of `ServerAction.DescribeLineArgs`.
+                    # Obviously, same applies for `ServerAction.RelayLineArgs` (as there is no chance to propose more).
+                    curr_arg_bucket.append(token_ipos)
+                    self.token_ipos_to_arg_bucket_map[token_ipos] = curr_bucket_index
+
+        # Init remaining and consumed:
+        self.remaining_arg_buckets = deepcopy(self.included_arg_buckets)
+        for i in range(len(self.included_arg_buckets)):
+            self.consumed_arg_buckets.append([])
 
-    def _init_unconsumed_tokens(self):
-        if self.parsed_ctx.server_action is ServerAction.ProposeArgValues:
-            return [
-                token_ipos for token_ipos in range(0, len(self.parsed_ctx.all_tokens))
-                # FS_23_62_89_43:
-                # `ServerAction.ProposeArgValues` excludes tangent token because it is supposed to be completed:
-                if token_ipos != self.parsed_ctx.tan_token_ipos
-            ]
-        else:
-            return [
-                token_ipos for token_ipos in range(0, len(self.parsed_ctx.all_tokens))
-                # FS_23_62_89_43:
-                # Process all tokens (including tangent token) in case of `ServerAction.DescribeLineArgs`.
-                # Obviously, same applies for `ServerAction.RelayLineArgs` (as there is no chance to propose more).
-            ]
+    def next_remaining_token_ipos(
+        self,
+    ) -> Union[int, None]:
+        for arg_bucket in self.remaining_arg_buckets:
+            for token_ipos in arg_bucket:
+                return token_ipos
+        return None
+
+    def remaining_token_ipos_list(
+        self,
+    ) -> list[int]:
+        return arg_buckets_to_token_ipos_list(self.remaining_arg_buckets)
+
+    def consumed_token_ipos_list(
+        self,
+    ) -> list[int]:
+        return arg_buckets_to_token_ipos_list(self.consumed_arg_buckets)
 
     def alloc_searchable_containers(
         self,
         search_control_list: list[SearchControl],
     ):
         for search_control in search_control_list:
             envelope_container = EnvelopeContainer(search_control)
@@ -148,42 +210,49 @@
         self.curr_container.found_count = query_result.found_count
         ElapsedTime.measure(f"end_query_envelopes: {query_dict} {self.curr_container.found_count}")
 
     def consume_args(
         self,
         interp_n: int
     ):
-        # Query envelope values only - they will be used for consumption of command line args:
-        ElapsedTime.measure(f"[i={interp_n}]: before_init_query: {self.curr_interp}")
-        self.query_prop_values()
         while True:
-            # Reset to False as we just executed new query:
-            query_changed = False
-            arg_was_consumed = False
-
-            # Because each `prop_value` set (per `prop_type`) is treated independently,
-            # assignment of `prop_value`-s from args may set combinations
-            # which yields no search result in subsequent query.
-            # Logically, it is better to consume args one by one and running query after each consumption,
-            # but this is not done due to query overhead.
-            # Note that Tab-completion and selection (via manual step by human) in separate requests to server and
-            # separate `interpret_command` calls is close to that logically better approach.
-            if not query_changed:
-                ElapsedTime.measure(f"[i={interp_n}]: before_consume_key_args: {self.curr_interp}")
-                arg_was_consumed = self.curr_interp.consume_key_args()
-                query_changed = arg_was_consumed
-            if not query_changed:
-                ElapsedTime.measure(f"[i={interp_n}]: before_consume_pos_args: {self.curr_interp}")
-                arg_was_consumed = self.curr_interp.consume_pos_args()
-                query_changed = arg_was_consumed
 
-            if query_changed:
-                ElapsedTime.measure(f"[i={interp_n}]: before_reduce_query: {self.curr_interp}")
+            # FS_44_36_84_88 consume args one by one:
+            while True:
+                # Query envelope values only - they will be used for consumption of command line args:
+                ElapsedTime.measure(f"[i={interp_n}]: before_entry_query: {self.curr_interp}")
                 self.query_prop_values()
-                query_changed = False
+                # Reset to False as we just executed new query:
+                arg_was_consumed = False
+
+                # Because each `prop_value` set (per `prop_type`) is treated independently,
+                # assignment of `prop_value`-s from args may set combinations
+                # which yields no search result in subsequent query.
+                # Logically, it is better to consume args one by one and running query after each consumption,
+                # but this is not done due to query overhead.
+                # Note that Tab-completion and selection (via manual step by human) in separate requests to server and
+                # separate `interpret_command` calls is close to that logically better approach.
+                if not arg_was_consumed:
+                    ElapsedTime.measure(f"[i={interp_n}]: before_consume_key_args: {self.curr_interp}")
+                    arg_was_consumed = self.curr_interp.consume_key_args()
+                if not arg_was_consumed:
+                    ElapsedTime.measure(f"[i={interp_n}]: before_consume_pos_args: {self.curr_interp}")
+                    arg_was_consumed = self.curr_interp.consume_pos_args()
+
+                if arg_was_consumed:
+                    if self.curr_interp.consumes_args_at_once():
+                        # No known interp consuming at once depends on query - do not query, simply exit loop:
+                        break
+                    else:
+                        # Run next cycle to see if one more can be consumed:
+                        pass
+                else:
+                    break
+
+            query_changed = False
 
             if self.curr_container:
                 # Set implicit values (so that applying defaults knows what they are):
                 self.curr_container.populate_implicit_arg_values()
 
             if self.curr_interp.has_fill_control():
                 if self.parsed_ctx.server_action is ServerAction.DescribeLineArgs:
@@ -200,32 +269,27 @@
                 query_changed = (
                     self.curr_interp.delegate_fill_control()
                     or
                     query_changed
                 )
                 self._leave_only_hidden_by_defaults()
 
-
             # Query envelopes after all implicit and default values assigned:
             # TODO: We could probably select whether to query only envelopes or
             #       query their values depending on `ServerAction`.
             #       But init of next envelope depends on prev envelope found.
             if query_changed:
-                ElapsedTime.measure(f"[i={interp_n}]: before_final_query: {self.curr_interp}")
-                self.query_prop_values()
-                if self.curr_interp.consumes_args_at_once():
-                    break
-            elif arg_was_consumed:
-                # Run next cycle to see if one more can be consumed:
                 if self.curr_interp.consumes_args_at_once():
+                    # No known interp consuming at once depends on query - do not query, simply exit loop:
                     break
+                else:
+                    pass
             else:
                 break
 
-
     # TODO: Move all dynamic and non-serializable objects into `InterpRuntime` (or something like that) together with this loop:
     def interpret_command(
         self,
         first_interp_factory_id: str,
     ) -> None:
         """
         Implements FS_55_57_45_04 enum selector version of FS_15_79_76_85 line processor.
```

### Comparing `argrelay-0.6.9/src/argrelay/runtime_context/ParsedContext.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_context/ParsedContext.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 
 @dataclass(frozen = True)
 class ParsedContext(CallContext):
     """
     Internal immutable parsed view of :class:`InputContext`
 
+    Implements `FS_27_16_67_19` line syntax.
+
     `tan_token_*` = `tangent_token`, see FS_23_62_89_43.
     """
 
     all_tokens: list[str] = field(init = False)
     tan_token_ipos: int = field(init = False)
     tan_token_l_cpos: int = field(init = False)
     tan_token_r_cpos: int = field(init = False)
@@ -50,31 +52,43 @@
         call_ctx: CallContext,
     ):
         return cls(**dataclasses.asdict(call_ctx))
 
     @staticmethod
     def parse_input(
         call_ctx: CallContext,
-    ):
+    ) -> tuple[
+        list[str],
+        int,
+        int,
+        int,
+        str,
+        str,
+        str,
+    ]:
         """
         Given `|` is the cursor in this command line:
         ```
-        some_command some_su|b_command some_arg
+        some_command some_su|b_command some_arg % next_arg   last_arg
         ```
         ```
-                            |                       # non-existing char placed to indicate cursor cpos
-        0            1                 2            # token ipos
-        01234567890123456789 01234567890123456789   # char cpos (the least significant digit)
+                            |                                         # non-existing char placed to indicate cursor cpos
+                                                %                     # arg bucket separator
+        0            1                 2        3 4          5        # token ipos
+        01234567890123456789 0123456789012345678901234567890123456789 # char cpos (the least significant digit)
         ```
         Then function returns:
         (
             [                               # list of all tokens
                 "some_command",             # 0
                 "some_sub_command",         # 1 (tangent token = token "touched" by the cursor)
                 "some_arg",                 # 2
+                "%",                        # 3 arg bucket separator
+                "next_arg",                 # 4
+                "last_arg"                  # 5
             ],
             1                               # tangent token item position (ipos)
             13                              # left-most char position (cpos) of tangent token (including it)
             29                              # right-most char position (cpos) of tangent token (excluding it)
             "some_sub_command",             # tangent token string
             "some_su",                      # tangent token left part substring (preceding cursor position)
             "b_command",                    # tangent token right part substring (succeeding cursor position)
```

### Comparing `argrelay-0.6.9/src/argrelay/runtime_context/SearchControl.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_context/SearchControl.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/runtime_data/EnvelopeCollection.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_data/EnvelopeCollection.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/runtime_data/ServerConfig.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_data/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/runtime_data/StaticData.py` & `argrelay-0.7.0.dev0/src/argrelay/runtime_data/StaticData.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/sample_conf/argrelay.server.yaml` & `argrelay-0.7.0.dev0/src/argrelay/sample_conf/argrelay.server.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -70,172 +70,248 @@
     ClassCluster: ClassCluster
     ClassHost: ClassHost
     ClassService: ClassService
     access_type: access_type
 
 server_plugin_control:
     first_interp_factory_id: FirstArgInterpFactory.default
-    reusable_config_data:
 
-        # TODO: TODO_10_72_28_05: FS_33_76_82_84: global tree (non functional yet).
-        # TODO: Create schemas for each `node_type` with translator code from this tree to "legacy" structures:
-        #       *   add tests of their equivalence first
-        #       *   switch plugins to use it instead
-        #
-        #       This config is not function (not used yet) - it is a scratch board to see how this mess can be:
-        #       *   put into single global view (without composing it via recursive references to plugins)
-        #       *   simplified (without intermediate plugin instances performing single function but hard to follow in composition)
-        # `tree_node_type`-s: their "legacy" tree name: some explanation:
-        #       *   init_node: [no equivalent] : TODO: Do we need it?
-        #       *   zero_arg_node: first_arg_vals_to_next_interp_factory_ids:
-        #       *   interp_tree_node: interp_selector_tree:
-        #       *   func_tree_node: func_selector_tree:
-        #       *   tree_path_node: [no equivalent]: add extra tree level (but does nothing as the other types)
-        #       *   [no equivalent]: jump_tree: `jump_path` simply becomes config of a node (no need to have separate `jump_tree`)
-        #       *   [no equivalent]: tree_abs_path_to_interp_id: selecting which interp id to use simply becomes config of a node
-        global_tree:
-            node_type: init_node
-            sub_tree:
-                "relay_demo":
-                    node_type: zero_arg_node
-                    plugin_instance_id: InterpTreeInterpFactory.default
-                    sub_tree: &interp_tree_default
-                        "intercept": &intercept_invocation_func_interp_tree_node
-                            node_type: interp_tree_node
-                            plugin_instance_id: FuncTreeInterpFactory.intercept_invocation_func
-                            next_interp:
-                                jump_path:
-                                    -   "relay_demo"
-                                plugin_instance_id: InterpTreeInterpFactory.default
-                            sub_tree:
-                                "":
-                                    node_type: func_tree_node
-                                    func_id: intercept_invocation_func
-                        "help": &help_hint_func_interp_tree_node
-                            node_type: interp_tree_node
-                            plugin_instance_id: FuncTreeInterpFactory.help_hint_func
-                            next_interp:
-                                jump_path:
-                                    -   "relay_demo"
-                                plugin_instance_id: InterpTreeInterpFactory.default
-                            sub_tree:
-                                "":
-                                    node_type: func_tree_node
-                                    func_id: help_hint_func
-                        "enum":
-                            node_type: interp_tree_node
-                            plugin_instance_id: FuncTreeInterpFactory.query_enum_items_func
-                            next_interp:
-                                jump_path:
-                                    -   "relay_demo"
-                                plugin_instance_id: InterpTreeInterpFactory.default
-                            sub_tree:
-                                "":
-                                    node_type: func_tree_node
-                                    func_id: query_enum_items_func
-                        "": &default_func_interp_tree_node
-                            node_type: interp_tree_node
-                            plugin_instance_id: FuncTreeInterpFactory.default
-                            sub_tree:
-                                "echo":
-                                    node_type: func_tree_node
-                                    func_id: echo_args_func
-                                "list":
-                                    node_type: tree_path_node
-                                    sub_tree:
-                                        "host":
-                                            node_type: func_tree_node
-                                            func_id: list_host_func
-                                        "service":
-                                            node_type: func_tree_node
-                                            func_id: list_service_func
-                                "goto":
-                                    node_type: tree_path_node
-                                    sub_tree:
-                                        "repo":
-                                            node_type: func_tree_node
-                                            func_id: goto_git_repo_func
-                                        "host":
-                                            node_type: func_tree_node
-                                            func_id: goto_host_func
-                                        "service":
-                                            node_type: func_tree_node
-                                            func_id: goto_service_func
-                                "desc":
-                                    node_type: tree_path_node
-                                    sub_tree:
-                                        "tag":
-                                            node_type: func_tree_node
-                                            func_id: desc_git_tag_func
-                                        "commit":
-                                            node_type: func_tree_node
-                                            func_id: desc_git_commit_func
-                                        "host":
-                                            node_type: func_tree_node
-                                            func_id: desc_host_func
-                                        "service":
-                                            node_type: func_tree_node
-                                            func_id: desc_service_func
-                                "config":
-                                    node_type: tree_path_node
-                                    sub_tree:
-                                        "print_with_level":
-                                            node_type: func_tree_node
-                                            func_id: funct_id_print_with_severity_level
-                                        "print_with_exit":
-                                            node_type: func_tree_node
-                                            func_id: funct_id_print_with_exit_code
-                                        "print_with_io_redirect":
-                                            node_type: func_tree_node
-                                            func_id: funct_id_print_with_io_redirect
-                                        "double_execution":
-                                            node_type: func_tree_node
-                                            func_id: funct_id_double_execution
-                        "duplicates":
+    # TODO: TODO_10_72_28_05: FS_33_76_82_84: composite tree (non functional yet).
+    # TODO: Create schemas for each `node_type` with translator code from this tree to "legacy" structures:
+    #       *   TODO: add tests of their equivalence first
+    #       *   TODO: then, switch plugins to use it instead
+    #
+    #       This config is not function (not used yet) - it is a scratch board to see how this mess can be:
+    #       *   put into single global view (without composing it via recursive references to plugins)
+    #       *   simplified (without intermediate plugin instances performing single function but hard to follow in composition)
+    #
+    # `:`-delimited table (rows):
+    #           `tree_node_type`-s: their "legacy" tree name: some explanation
+    #
+    #       *   zero_arg_node: first_arg_vals_to_next_interp_factory_ids:
+    #       *   interp_tree_node: interp_selector_tree:
+    #       *   func_tree_node: func_selector_tree:
+    #       *   tree_path_node: [no equivalent]: add extra tree level (but does nothing as the other types)
+    #       *   [no equivalent]: jump_tree: `jump_path` simply becomes config of a node (no need to have separate `jump_tree`)
+    #       *   [no equivalent]: tree_abs_path_to_interp_id: selecting which interp id to use simply becomes config of a node
+    composite_forest:
+        tree_roots:
+            "relay_demo":
+                node_type: zero_arg_node
+                plugin_instance_id: InterpTreeInterpFactory.default
+                sub_tree:
+                    "intercept": &intercept_invocation_func_interp_tree_node
+                        node_type: interp_tree_node
+                        plugin_instance_id: FuncTreeInterpFactory.intercept_invocation_func
+                        next_interp:
+                            jump_path:
+                                -   "relay_demo"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                        sub_tree:
+                            "":
+                                node_type: func_tree_node
+                                func_id: intercept_invocation_func
+                    "help": &help_hint_func_interp_tree_node
+                        node_type: interp_tree_node
+                        plugin_instance_id: FuncTreeInterpFactory.help_hint_func
+                        next_interp:
+                            jump_path:
+                                -   "relay_demo"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                        sub_tree:
+                            "":
+                                node_type: func_tree_node
+                                func_id: help_hint_func
+                    "enum": &query_enum_items_func_interp_tree_node
+                        node_type: interp_tree_node
+                        plugin_instance_id: FuncTreeInterpFactory.query_enum_items_func
+                        next_interp:
+                            jump_path:
+                                -   "relay_demo"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                        sub_tree:
+                            "":
+                                node_type: func_tree_node
+                                func_id: query_enum_items_func
+                    "": &default_func_interp_tree_node
+                        node_type: interp_tree_node
+                        plugin_instance_id: FuncTreeInterpFactory.default
+                        next_interp:
+                            jump_path:
+                                -   "relay_demo"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                        sub_tree:
+                            "echo":
+                                node_type: func_tree_node
+                                func_id: echo_args_func
+                            "list":
+                                node_type: tree_path_node
+                                sub_tree:
+                                    "host":
+                                        node_type: func_tree_node
+                                        func_id: list_host_func
+                                    "service":
+                                        node_type: func_tree_node
+                                        func_id: list_service_func
+                            "diff":
+                                node_type: tree_path_node
+                                sub_tree:
+                                    "service":
+                                        node_type: func_tree_node
+                                        func_id: diff_service_func
+                            "goto":
+                                node_type: tree_path_node
+                                sub_tree:
+                                    "repo":
+                                        node_type: func_tree_node
+                                        func_id: goto_git_repo_func
+                                    "host":
+                                        node_type: func_tree_node
+                                        func_id: goto_host_func
+                                    "service":
+                                        node_type: func_tree_node
+                                        func_id: goto_service_func
+                            "desc":
+                                node_type: tree_path_node
+                                sub_tree:
+                                    "tag":
+                                        node_type: func_tree_node
+                                        func_id: desc_git_tag_func
+                                    "commit":
+                                        node_type: func_tree_node
+                                        func_id: desc_git_commit_func
+                                    "host":
+                                        node_type: func_tree_node
+                                        func_id: desc_host_func
+                                    "service":
+                                        node_type: func_tree_node
+                                        func_id: desc_service_func
+                            "config":
+                                node_type: tree_path_node
+                                sub_tree:
+                                    "print_with_level":
+                                        node_type: func_tree_node
+                                        func_id: funct_id_print_with_severity_level
+                                    "print_with_exit":
+                                        node_type: func_tree_node
+                                        func_id: funct_id_print_with_exit_code
+                                    "print_with_io_redirect":
+                                        node_type: func_tree_node
+                                        func_id: funct_id_print_with_io_redirect
+                                    "double_execution":
+                                        node_type: func_tree_node
+                                        func_id: funct_id_double_execution
+                    "duplicates":
+                        node_type: tree_path_node
+                        sub_tree:
                             "intercept":
                                 <<: *intercept_invocation_func_interp_tree_node
                                 next_interp:
                                     jump_path:
                                         -   "relay_demo"
                                         -   "duplicates"
                                     plugin_instance_id: InterpTreeInterpFactory.default
                             "help":
                                 <<: *help_hint_func_interp_tree_node
                                 next_interp:
                                     jump_path:
                                         -   "relay_demo"
                                         -   "duplicates"
                                     plugin_instance_id: InterpTreeInterpFactory.default
-                            "": *default_func_interp_tree_node
-                "some_command":
-                    node_type: zero_arg_node
-                    plugin_instance_id: InterpTreeInterpFactory.default
-                    sub_tree: *interp_tree_default
-                "service_relay_demo":
-                    node_type: zero_arg_node
-                    plugin_instance_id: InterpTreeInterpFactory.service
-                    sub_tree:
+                            "":
+                                <<: *default_func_interp_tree_node
+                                next_interp:
+                                    jump_path:
+                                        - "relay_demo"
+                                        - "duplicates"
+                                    plugin_instance_id: InterpTreeInterpFactory.default
+            "some_command":
+                node_type: zero_arg_node
+                plugin_instance_id: InterpTreeInterpFactory.default
+                sub_tree:
+                    "intercept":
+                        <<: *intercept_invocation_func_interp_tree_node
+                        next_interp:
+                            jump_path:
+                                -   "some_command"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                    "help":
                         <<: *help_hint_func_interp_tree_node
                         next_interp:
                             jump_path:
+                                -   "some_command"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                    "enum":
+                        <<: *query_enum_items_func_interp_tree_node
+                        next_interp:
+                            jump_path:
+                                -   "some_command"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                    "":
+                        <<: *default_func_interp_tree_node
+                        next_interp:
+                            jump_path:
+                                -   "some_command"
+                            plugin_instance_id: InterpTreeInterpFactory.default
+                    "duplicates":
+                        node_type: tree_path_node
+                        sub_tree:
+                            "intercept":
+                                <<: *intercept_invocation_func_interp_tree_node
+                                next_interp:
+                                    jump_path:
+                                        -   "some_command"
+                                        -   "duplicates"
+                                    plugin_instance_id: InterpTreeInterpFactory.default
+                            "help":
+                                <<: *help_hint_func_interp_tree_node
+                                next_interp:
+                                    jump_path:
+                                        -   "some_command"
+                                        -   "duplicates"
+                                    plugin_instance_id: InterpTreeInterpFactory.default
+                            "":
+                                <<: *default_func_interp_tree_node
+                                next_interp:
+                                    jump_path:
+                                        -   "some_command"
+                                        -   "duplicates"
+                                    plugin_instance_id: InterpTreeInterpFactory.default
+            "service_relay_demo":
+                node_type: zero_arg_node
+                plugin_instance_id: InterpTreeInterpFactory.service
+                sub_tree:
+                    "help":
+                        <<: *help_hint_func_interp_tree_node
+                        next_interp:
+                            jump_path:
+                                -   "service_relay_demo"
+                            plugin_instance_id: InterpTreeInterpFactory.service
+                    "":
+                        node_type: interp_tree_node
+                        plugin_instance_id: FuncTreeInterpFactory.service
+                        next_interp:
+                            jump_path:
                                 -   "service_relay_demo"
                             plugin_instance_id: InterpTreeInterpFactory.service
-                        "":
-                            node_type: interp_tree_node
-                            plugin_instance_id: FuncTreeInterpFactory.service
-                            sub_tree:
-                                "goto":
-                                    node_type: func_tree_node
-                                    func_id: goto_service_func
-                                "list":
-                                    node_type: func_tree_node
-                                    func_id: list_service_func
-                                "desc":
-                                    node_type: func_tree_node
-                                    func_id: desc_service_func
+                        sub_tree:
+                            "goto":
+                                node_type: func_tree_node
+                                func_id: goto_service_func
+                            "list":
+                                node_type: func_tree_node
+                                func_id: list_service_func
+                            "diff":
+                                node_type: func_tree_node
+                                func_id: diff_service_func
+                            "desc":
+                                node_type: func_tree_node
+                                func_id: desc_service_func
+
+    reusable_config_data:
 
         jump_tree: &jump_tree
             "relay_demo":
                 "intercept":
                     -   "relay_demo"
                 "help":
                     -   "relay_demo"
@@ -244,31 +320,43 @@
                 "duplicates":
                     "intercept":
                         -   "relay_demo"
                         -   "duplicates"
                     "help":
                         -   "relay_demo"
                         -   "duplicates"
+                    "":
+                        -   "relay_demo"
+                        -   "duplicates"
+                "":
+                    -   "relay_demo"
             "some_command":
                 "intercept":
                     -   "some_command"
                 "help":
                     -   "some_command"
                 "enum":
                     -   "some_command"
                 "duplicates":
                     "intercept":
                         -   "some_command"
                         -   "duplicates"
                     "help":
                         -   "some_command"
                         -   "duplicates"
+                    "":
+                        -   "some_command"
+                        -   "duplicates"
+                "":
+                    - "some_command"
             "service_relay_demo":
                 "help":
                     -   "service_relay_demo"
+                "":
+                    -   "service_relay_demo"
 
 plugin_instance_entries:
 
     FirstArgInterpFactory.default:
         plugin_module_name: argrelay.plugin_interp.FirstArgInterpFactory
         plugin_class_name: FirstArgInterpFactory
         plugin_dependencies:
@@ -329,15 +417,15 @@
             -   FuncTreeInterpFactory.help_hint_func
             -   FuncTreeInterpFactory.service
         plugin_config:
             interp_selector_tree:
                 "help": FuncTreeInterpFactory.help_hint_func
                 "": FuncTreeInterpFactory.service
 
-    # TODO: FS_33_76_82_84 `global_tree`: maintaining separate instance of `FuncTreeInterpFactory` plugin should be avoided.
+    # TODO: FS_33_76_82_84 `composite_tree`: maintaining separate instance of `FuncTreeInterpFactory` plugin should be avoided.
     #       See extended comment for `FuncTreeInterpFactory.help_hint_func`.
     FuncTreeInterpFactory.intercept_invocation_func:
         plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
         plugin_class_name: FuncTreeInterpFactory
         plugin_config:
             jump_tree: *jump_tree
             func_selector_tree: intercept_invocation_func
@@ -356,23 +444,26 @@
             jump_tree: *jump_tree
             func_selector_tree: query_enum_items_func
 
     FuncTreeInterpFactory.default:
         plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
         plugin_class_name: FuncTreeInterpFactory
         plugin_config:
+            jump_tree: *jump_tree
             func_selector_tree:
                 "echo": echo_args_func
                 "goto":
                     "repo": goto_git_repo_func
                     "host": goto_host_func
                     "service": goto_service_func
                 "list":
                     "host": list_host_func
                     "service": list_service_func
+                "diff":
+                    "service": diff_service_func
                 "desc":
                     "tag": desc_git_tag_func
                     "commit": desc_git_commit_func
                     "host": desc_host_func
                     "service": desc_service_func
                 "config":
                     "print_with_level": funct_id_print_with_severity_level
@@ -380,17 +471,19 @@
                     "print_with_io_redirect": funct_id_print_with_io_redirect
                     "double_execution": funct_id_double_execution
 
     FuncTreeInterpFactory.service:
         plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
         plugin_class_name: FuncTreeInterpFactory
         plugin_config:
+            jump_tree: *jump_tree
             func_selector_tree:
                 "goto": goto_service_func
                 "list": list_service_func
+                "diff": diff_service_func
                 "desc": desc_service_func
 
     NoopInterpFactory.default:
         plugin_module_name: argrelay.plugin_interp.NoopInterpFactory
         plugin_class_name: NoopInterpFactory
 
     NoopLoader.default:
@@ -477,32 +570,32 @@
 
     InterceptDelegator.default:
         plugin_module_name: argrelay.plugin_delegator.InterceptDelegator
         plugin_class_name: InterceptDelegator
         plugin_dependencies:
             -   FuncTreeInterpFactory.default
         plugin_config:
+            single_func_id: intercept_invocation_func
             tree_abs_path_to_interp_id:
                 "relay_demo":
                     "intercept": InterpTreeInterpFactory.default
                     "duplicates":
                         "intercept": InterpTreeInterpFactory.default
                 "some_command":
                     "intercept": InterpTreeInterpFactory.default
                     "duplicates":
                         "intercept": InterpTreeInterpFactory.default
-                "service_relay_demo":
-                    "help": InterpTreeInterpFactory.service
 
     HelpDelegator.default:
         plugin_module_name: argrelay.plugin_delegator.HelpDelegator
         plugin_class_name: HelpDelegator
         plugin_dependencies:
             -   FuncTreeInterpFactory.default
         plugin_config:
+            single_func_id: help_hint_func
             tree_abs_path_to_interp_id:
                 "relay_demo":
                     "help": InterpTreeInterpFactory.default
                     "duplicates":
                         "help": InterpTreeInterpFactory.default
                 "some_command":
                     "help": InterpTreeInterpFactory.default
@@ -513,21 +606,20 @@
 
     QueryEnumDelegator.default:
         plugin_module_name: argrelay.plugin_delegator.QueryEnumDelegator
         plugin_class_name: QueryEnumDelegator
         plugin_dependencies:
             -   FuncTreeInterpFactory.default
         plugin_config:
+            single_func_id: query_enum_items_func
             tree_abs_path_to_interp_id:
                 "relay_demo":
                     "enum": InterpTreeInterpFactory.default
                 "some_command":
                     "enum": InterpTreeInterpFactory.default
-                "service_relay_demo":
-                    "help": InterpTreeInterpFactory.service
 
     ServiceDelegator.default:
         plugin_module_name: argrelay.custom_integ.ServiceDelegator
         plugin_class_name: ServiceDelegator
 
     GitRepoDelegator.default:
         plugin_module_name: argrelay.custom_integ.GitRepoDelegator
```

#### html2text {}

```diff
@@ -35,93 +35,117 @@
     _*_ _(_1_)_ _T_a_b_ _i_s_ _o_n_l_y_ _u_s_e_d_ _t_o_ _c_o_m_p_l_e_t_e_ _`_c_o_m_m_o_n___i_n_f_i_x_`_ _-_ _r_e_q_u_e_s_t_ _t_o_ _p_r_o_v_i_d_e
       _s_u_g_g_e_s_t_i_o_n_s_ _i_s_ _s_e_n_t_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _o_n_ _i_d_l_e_ _t_i_m_e_o_u_t_.
     _*_ _(_2_)_ _S_e_a_r_c_h_ _r_e_q_u_e_s_t_ _(_A_l_t_+_S_h_i_f_t_+_Q_)_ _i_s_ _s_e_n_t_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _o_n_ _i_d_l_e_ _t_i_m_e_o_u_t_.
     _*_ _(_3_)_ _C_o_m_m_a_n_d_ _i_n_v_o_c_a_t_i_o_n_ _(_E_n_t_e_r_)_ _i_s_ _d_i_s_a_b_l_e_d_ _-_ _i_t_ _o_n_l_y_ _p_r_i_n_t_s_ _i_n_v_o_c_a_t_i_o_n
       _d_a_t_a_ _f_r_o_m_ _t_h_e_ _s_e_r_v_e_r_ _(_u_s_e_ _a_ _C_L_I_ _c_l_i_e_n_t_ _t_o_ _r_u_n_ _c_o_m_m_a_n_d_s_)_.
 class_to_collection_map: ClassCluster: ClassCluster ClassHost: ClassHost
 ClassService: ClassService access_type: access_type server_plugin_control:
-first_interp_factory_id: FirstArgInterpFactory.default reusable_config_data: #
-TODO: TODO_10_72_28_05: FS_33_76_82_84: global tree (non functional yet). #
-TODO: Create schemas for each `node_type` with translator code from this tree
-to "legacy" structures: # * add tests of their equivalence first # * switch
-plugins to use it instead # # This config is not function (not used yet) - it
-is a scratch board to see how this mess can be: # * put into single global view
-(without composing it via recursive references to plugins) # * simplified
-(without intermediate plugin instances performing single function but hard to
-follow in composition) # `tree_node_type`-s: their "legacy" tree name: some
-explanation: # * init_node: [no equivalent] : TODO: Do we need it? # *
+first_interp_factory_id: FirstArgInterpFactory.default # TODO:
+TODO_10_72_28_05: FS_33_76_82_84: composite tree (non functional yet). # TODO:
+Create schemas for each `node_type` with translator code from this tree to
+"legacy" structures: # * TODO: add tests of their equivalence first # * TODO:
+then, switch plugins to use it instead # # This config is not function (not
+used yet) - it is a scratch board to see how this mess can be: # * put into
+single global view (without composing it via recursive references to plugins) #
+* simplified (without intermediate plugin instances performing single function
+but hard to follow in composition) # # `:`-delimited table (rows): #
+`tree_node_type`-s: their "legacy" tree name: some explanation # # *
 zero_arg_node: first_arg_vals_to_next_interp_factory_ids: # * interp_tree_node:
 interp_selector_tree: # * func_tree_node: func_selector_tree: # *
 tree_path_node: [no equivalent]: add extra tree level (but does nothing as the
 other types) # * [no equivalent]: jump_tree: `jump_path` simply becomes config
 of a node (no need to have separate `jump_tree`) # * [no equivalent]:
 tree_abs_path_to_interp_id: selecting which interp id to use simply becomes
-config of a node global_tree: node_type: init_node sub_tree: "relay_demo":
-node_type: zero_arg_node plugin_instance_id: InterpTreeInterpFactory.default
-sub_tree: &interp_tree_default "intercept":
-&intercept_invocation_func_interp_tree_node node_type: interp_tree_node
-plugin_instance_id: FuncTreeInterpFactory.intercept_invocation_func
-next_interp: jump_path: - "relay_demo" plugin_instance_id:
-InterpTreeInterpFactory.default sub_tree: "": node_type: func_tree_node
-func_id: intercept_invocation_func "help": &help_hint_func_interp_tree_node
-node_type: interp_tree_node plugin_instance_id:
-FuncTreeInterpFactory.help_hint_func next_interp: jump_path: - "relay_demo"
-plugin_instance_id: InterpTreeInterpFactory.default sub_tree: "": node_type:
-func_tree_node func_id: help_hint_func "enum": node_type: interp_tree_node
+config of a node composite_forest: tree_roots: "relay_demo": node_type:
+zero_arg_node plugin_instance_id: InterpTreeInterpFactory.default sub_tree:
+"intercept": &intercept_invocation_func_interp_tree_node node_type:
+interp_tree_node plugin_instance_id:
+FuncTreeInterpFactory.intercept_invocation_func next_interp: jump_path: -
+"relay_demo" plugin_instance_id: InterpTreeInterpFactory.default sub_tree: "":
+node_type: func_tree_node func_id: intercept_invocation_func "help":
+&help_hint_func_interp_tree_node node_type: interp_tree_node
+plugin_instance_id: FuncTreeInterpFactory.help_hint_func next_interp:
+jump_path: - "relay_demo" plugin_instance_id: InterpTreeInterpFactory.default
+sub_tree: "": node_type: func_tree_node func_id: help_hint_func "enum":
+&query_enum_items_func_interp_tree_node node_type: interp_tree_node
 plugin_instance_id: FuncTreeInterpFactory.query_enum_items_func next_interp:
 jump_path: - "relay_demo" plugin_instance_id: InterpTreeInterpFactory.default
 sub_tree: "": node_type: func_tree_node func_id: query_enum_items_func "":
 &default_func_interp_tree_node node_type: interp_tree_node plugin_instance_id:
-FuncTreeInterpFactory.default sub_tree: "echo": node_type: func_tree_node
-func_id: echo_args_func "list": node_type: tree_path_node sub_tree: "host":
-node_type: func_tree_node func_id: list_host_func "service": node_type:
-func_tree_node func_id: list_service_func "goto": node_type: tree_path_node
+FuncTreeInterpFactory.default next_interp: jump_path: - "relay_demo"
+plugin_instance_id: InterpTreeInterpFactory.default sub_tree: "echo":
+node_type: func_tree_node func_id: echo_args_func "list": node_type:
+tree_path_node sub_tree: "host": node_type: func_tree_node func_id:
+list_host_func "service": node_type: func_tree_node func_id: list_service_func
+"diff": node_type: tree_path_node sub_tree: "service": node_type:
+func_tree_node func_id: diff_service_func "goto": node_type: tree_path_node
 sub_tree: "repo": node_type: func_tree_node func_id: goto_git_repo_func "host":
 node_type: func_tree_node func_id: goto_host_func "service": node_type:
 func_tree_node func_id: goto_service_func "desc": node_type: tree_path_node
 sub_tree: "tag": node_type: func_tree_node func_id: desc_git_tag_func "commit":
 node_type: func_tree_node func_id: desc_git_commit_func "host": node_type:
 func_tree_node func_id: desc_host_func "service": node_type: func_tree_node
 func_id: desc_service_func "config": node_type: tree_path_node sub_tree:
 "print_with_level": node_type: func_tree_node func_id:
 funct_id_print_with_severity_level "print_with_exit": node_type: func_tree_node
 func_id: funct_id_print_with_exit_code "print_with_io_redirect": node_type:
 func_tree_node func_id: funct_id_print_with_io_redirect "double_execution":
 node_type: func_tree_node func_id: funct_id_double_execution "duplicates":
-"intercept": <<: *intercept_invocation_func_interp_tree_node next_interp:
-jump_path: - "relay_demo" - "duplicates" plugin_instance_id:
-InterpTreeInterpFactory.default "help": <<: *help_hint_func_interp_tree_node
-next_interp: jump_path: - "relay_demo" - "duplicates" plugin_instance_id:
-InterpTreeInterpFactory.default "": *default_func_interp_tree_node
+node_type: tree_path_node sub_tree: "intercept": <<:
+*intercept_invocation_func_interp_tree_node next_interp: jump_path: -
+"relay_demo" - "duplicates" plugin_instance_id: InterpTreeInterpFactory.default
+"help": <<: *help_hint_func_interp_tree_node next_interp: jump_path: -
+"relay_demo" - "duplicates" plugin_instance_id: InterpTreeInterpFactory.default
+"": <<: *default_func_interp_tree_node next_interp: jump_path: - "relay_demo" -
+"duplicates" plugin_instance_id: InterpTreeInterpFactory.default
 "some_command": node_type: zero_arg_node plugin_instance_id:
-InterpTreeInterpFactory.default sub_tree: *interp_tree_default
-"service_relay_demo": node_type: zero_arg_node plugin_instance_id:
-InterpTreeInterpFactory.service sub_tree: <<: *help_hint_func_interp_tree_node
-next_interp: jump_path: - "service_relay_demo" plugin_instance_id:
-InterpTreeInterpFactory.service "": node_type: interp_tree_node
-plugin_instance_id: FuncTreeInterpFactory.service sub_tree: "goto": node_type:
-func_tree_node func_id: goto_service_func "list": node_type: func_tree_node
-func_id: list_service_func "desc": node_type: func_tree_node func_id:
-desc_service_func jump_tree: &jump_tree "relay_demo": "intercept": -
+InterpTreeInterpFactory.default sub_tree: "intercept": <<:
+*intercept_invocation_func_interp_tree_node next_interp: jump_path: -
+"some_command" plugin_instance_id: InterpTreeInterpFactory.default "help": <<:
+*help_hint_func_interp_tree_node next_interp: jump_path: - "some_command"
+plugin_instance_id: InterpTreeInterpFactory.default "enum": <<:
+*query_enum_items_func_interp_tree_node next_interp: jump_path: -
+"some_command" plugin_instance_id: InterpTreeInterpFactory.default "": <<:
+*default_func_interp_tree_node next_interp: jump_path: - "some_command"
+plugin_instance_id: InterpTreeInterpFactory.default "duplicates": node_type:
+tree_path_node sub_tree: "intercept": <<:
+*intercept_invocation_func_interp_tree_node next_interp: jump_path: -
+"some_command" - "duplicates" plugin_instance_id:
+InterpTreeInterpFactory.default "help": <<: *help_hint_func_interp_tree_node
+next_interp: jump_path: - "some_command" - "duplicates" plugin_instance_id:
+InterpTreeInterpFactory.default "": <<: *default_func_interp_tree_node
+next_interp: jump_path: - "some_command" - "duplicates" plugin_instance_id:
+InterpTreeInterpFactory.default "service_relay_demo": node_type: zero_arg_node
+plugin_instance_id: InterpTreeInterpFactory.service sub_tree: "help": <<:
+*help_hint_func_interp_tree_node next_interp: jump_path: - "service_relay_demo"
+plugin_instance_id: InterpTreeInterpFactory.service "": node_type:
+interp_tree_node plugin_instance_id: FuncTreeInterpFactory.service next_interp:
+jump_path: - "service_relay_demo" plugin_instance_id:
+InterpTreeInterpFactory.service sub_tree: "goto": node_type: func_tree_node
+func_id: goto_service_func "list": node_type: func_tree_node func_id:
+list_service_func "diff": node_type: func_tree_node func_id: diff_service_func
+"desc": node_type: func_tree_node func_id: desc_service_func
+reusable_config_data: jump_tree: &jump_tree "relay_demo": "intercept": -
 "relay_demo" "help": - "relay_demo" "enum": - "relay_demo" "duplicates":
 "intercept": - "relay_demo" - "duplicates" "help": - "relay_demo" -
-"duplicates" "some_command": "intercept": - "some_command" "help": -
-"some_command" "enum": - "some_command" "duplicates": "intercept": -
-"some_command" - "duplicates" "help": - "some_command" - "duplicates"
-"service_relay_demo": "help": - "service_relay_demo" plugin_instance_entries:
-FirstArgInterpFactory.default: plugin_module_name:
-argrelay.plugin_interp.FirstArgInterpFactory plugin_class_name:
-FirstArgInterpFactory plugin_dependencies: # Delegators for `func_tree`: -
-NoopDelegator.default - EchoDelegator.default - InterceptDelegator.default -
-HelpDelegator.default - QueryEnumDelegator.default - ServiceDelegator.default -
-GitRepoDelegator.default - ConfigOnlyDelegator.default # Interps for
-`interp_tree` per command (zero-arg): - InterpTreeInterpFactory.default -
-InterpTreeInterpFactory.service # Interps for normal funcs: -
-FuncTreeInterpFactory.default # Interps for special funcs: -
-FuncTreeInterpFactory.intercept_invocation_func -
+"duplicates" "": - "relay_demo" - "duplicates" "": - "relay_demo"
+"some_command": "intercept": - "some_command" "help": - "some_command" "enum":
+- "some_command" "duplicates": "intercept": - "some_command" - "duplicates"
+"help": - "some_command" - "duplicates" "": - "some_command" - "duplicates" "":
+- "some_command" "service_relay_demo": "help": - "service_relay_demo" "": -
+"service_relay_demo" plugin_instance_entries: FirstArgInterpFactory.default:
+plugin_module_name: argrelay.plugin_interp.FirstArgInterpFactory
+plugin_class_name: FirstArgInterpFactory plugin_dependencies: # Delegators for
+`func_tree`: - NoopDelegator.default - EchoDelegator.default -
+InterceptDelegator.default - HelpDelegator.default - QueryEnumDelegator.default
+- ServiceDelegator.default - GitRepoDelegator.default -
+ConfigOnlyDelegator.default # Interps for `interp_tree` per command (zero-arg):
+- InterpTreeInterpFactory.default - InterpTreeInterpFactory.service # Interps
+for normal funcs: - FuncTreeInterpFactory.default # Interps for special funcs:
+- FuncTreeInterpFactory.intercept_invocation_func -
 FuncTreeInterpFactory.help_hint_func -
 FuncTreeInterpFactory.query_enum_items_func plugin_config:
 first_arg_vals_to_next_interp_factory_ids: # This binding uses existing file
 system name `relay_demo`: "relay_demo": InterpTreeInterpFactory.default #
 Another equivalent binding # (if `some_command` is configured, it will behave
 as `relay_demo` above): "some_command": InterpTreeInterpFactory.default
 "service_relay_demo": InterpTreeInterpFactory.service ignored_func_ids_list: -
@@ -140,41 +164,42 @@
 FuncTreeInterpFactory.help_hint_func "": FuncTreeInterpFactory.default
 InterpTreeInterpFactory.service: plugin_module_name:
 argrelay.plugin_interp.InterpTreeInterpFactory plugin_class_name:
 InterpTreeInterpFactory plugin_dependencies: -
 FuncTreeInterpFactory.help_hint_func - FuncTreeInterpFactory.service
 plugin_config: interp_selector_tree: "help":
 FuncTreeInterpFactory.help_hint_func "": FuncTreeInterpFactory.service # TODO:
-FS_33_76_82_84 `global_tree`: maintaining separate instance of
+FS_33_76_82_84 `composite_tree`: maintaining separate instance of
 `FuncTreeInterpFactory` plugin should be avoided. # See extended comment for
 `FuncTreeInterpFactory.help_hint_func`.
 FuncTreeInterpFactory.intercept_invocation_func: plugin_module_name:
 argrelay.plugin_interp.FuncTreeInterpFactory plugin_class_name:
 FuncTreeInterpFactory plugin_config: jump_tree: *jump_tree func_selector_tree:
 intercept_invocation_func FuncTreeInterpFactory.help_hint_func:
 plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
 plugin_class_name: FuncTreeInterpFactory plugin_config: jump_tree: *jump_tree
 func_selector_tree: help_hint_func FuncTreeInterpFactory.query_enum_items_func:
 plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
 plugin_class_name: FuncTreeInterpFactory plugin_config: jump_tree: *jump_tree
 func_selector_tree: query_enum_items_func FuncTreeInterpFactory.default:
 plugin_module_name: argrelay.plugin_interp.FuncTreeInterpFactory
-plugin_class_name: FuncTreeInterpFactory plugin_config: func_selector_tree:
-"echo": echo_args_func "goto": "repo": goto_git_repo_func "host":
-goto_host_func "service": goto_service_func "list": "host": list_host_func
-"service": list_service_func "desc": "tag": desc_git_tag_func "commit":
+plugin_class_name: FuncTreeInterpFactory plugin_config: jump_tree: *jump_tree
+func_selector_tree: "echo": echo_args_func "goto": "repo": goto_git_repo_func
+"host": goto_host_func "service": goto_service_func "list": "host":
+list_host_func "service": list_service_func "diff": "service":
+diff_service_func "desc": "tag": desc_git_tag_func "commit":
 desc_git_commit_func "host": desc_host_func "service": desc_service_func
 "config": "print_with_level": funct_id_print_with_severity_level
 "print_with_exit": funct_id_print_with_exit_code "print_with_io_redirect":
 funct_id_print_with_io_redirect "double_execution": funct_id_double_execution
 FuncTreeInterpFactory.service: plugin_module_name:
 argrelay.plugin_interp.FuncTreeInterpFactory plugin_class_name:
-FuncTreeInterpFactory plugin_config: func_selector_tree: "goto":
-goto_service_func "list": list_service_func "desc": desc_service_func
-NoopInterpFactory.default: plugin_module_name:
+FuncTreeInterpFactory plugin_config: jump_tree: *jump_tree func_selector_tree:
+"goto": goto_service_func "list": list_service_func "diff": diff_service_func
+"desc": desc_service_func NoopInterpFactory.default: plugin_module_name:
 argrelay.plugin_interp.NoopInterpFactory plugin_class_name: NoopInterpFactory
 NoopLoader.default: plugin_module_name: argrelay.plugin_loader.NoopLoader
 plugin_class_name: NoopLoader ServiceLoader.default: plugin_module_name:
 argrelay.custom_integ.ServiceLoader plugin_class_name: ServiceLoader
 plugin_config: test_data_ids_to_load: #- TD_70_69_38_46 # no data -
 TD_63_37_05_36 # demo # WARNING: with `mongomock` and not `enable_query_cache`
 requests run up for TD_38_03_48_51 may run up to 10 mins: #- TD_38_03_48_51 #
@@ -201,34 +226,34 @@
 !include "data/ConfigOnlyLoader.default.data.yaml" NoopDelegator.default:
 plugin_module_name: argrelay.plugin_delegator.NoopDelegator plugin_class_name:
 NoopDelegator EchoDelegator.default: plugin_module_name:
 argrelay.plugin_delegator.EchoDelegator plugin_class_name: EchoDelegator
 InterceptDelegator.default: plugin_module_name:
 argrelay.plugin_delegator.InterceptDelegator plugin_class_name:
 InterceptDelegator plugin_dependencies: - FuncTreeInterpFactory.default
-plugin_config: tree_abs_path_to_interp_id: "relay_demo": "intercept":
+plugin_config: single_func_id: intercept_invocation_func
+tree_abs_path_to_interp_id: "relay_demo": "intercept":
 InterpTreeInterpFactory.default "duplicates": "intercept":
 InterpTreeInterpFactory.default "some_command": "intercept":
 InterpTreeInterpFactory.default "duplicates": "intercept":
-InterpTreeInterpFactory.default "service_relay_demo": "help":
-InterpTreeInterpFactory.service HelpDelegator.default: plugin_module_name:
+InterpTreeInterpFactory.default HelpDelegator.default: plugin_module_name:
 argrelay.plugin_delegator.HelpDelegator plugin_class_name: HelpDelegator
 plugin_dependencies: - FuncTreeInterpFactory.default plugin_config:
-tree_abs_path_to_interp_id: "relay_demo": "help":
-InterpTreeInterpFactory.default "duplicates": "help":
+single_func_id: help_hint_func tree_abs_path_to_interp_id: "relay_demo":
+"help": InterpTreeInterpFactory.default "duplicates": "help":
 InterpTreeInterpFactory.default "some_command": "help":
 InterpTreeInterpFactory.default "duplicates": "help":
 InterpTreeInterpFactory.default "service_relay_demo": "help":
 InterpTreeInterpFactory.service QueryEnumDelegator.default: plugin_module_name:
 argrelay.plugin_delegator.QueryEnumDelegator plugin_class_name:
 QueryEnumDelegator plugin_dependencies: - FuncTreeInterpFactory.default
-plugin_config: tree_abs_path_to_interp_id: "relay_demo": "enum":
+plugin_config: single_func_id: query_enum_items_func
+tree_abs_path_to_interp_id: "relay_demo": "enum":
 InterpTreeInterpFactory.default "some_command": "enum":
-InterpTreeInterpFactory.default "service_relay_demo": "help":
-InterpTreeInterpFactory.service ServiceDelegator.default: plugin_module_name:
+InterpTreeInterpFactory.default ServiceDelegator.default: plugin_module_name:
 argrelay.custom_integ.ServiceDelegator plugin_class_name: ServiceDelegator
 GitRepoDelegator.default: plugin_module_name:
 argrelay.custom_integ.GitRepoDelegator plugin_class_name: GitRepoDelegator
 ConfigOnlyDelegator.default: plugin_module_name:
 argrelay.custom_integ.ConfigOnlyDelegator plugin_class_name:
 ConfigOnlyDelegator plugin_config: # TODO_84_71_86_21: change to realistic
 examples: func_configs: funct_id_print_with_severity_level: func_envelope:
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_client/ClientConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/ClientConfigSchema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.ClientConfig import ClientConfig
 from argrelay.schema_config_core_client.ConnectionConfigSchema import connection_config_desc
 
 __comment___ = "__comment__"
 connection_config_ = "connection_config"
 use_local_requests_ = "use_local_requests"
@@ -12,64 +13,56 @@
 spinless_sleep_sec_ = "spinless_sleep_sec"
 
 
 # NOTE: Client does not use `Schema` to load config in prod code
 #       (only in tests due to heavy import caused by `Schema`).
 #       Therefore, validation and applying defaults is not done by this class.
 #       Duplicate the same requirements (for validation and defaults) in client prod code.
-class ClientConfigSchema(Schema):
+class ClientConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = ClientConfig
+
     # Allow this field in JSON (otherwise schema validation fails):
     __comment__ = fields.String(
         required = False,
+        load_default = "",
     )
 
     # Serve requests from local data or send to server
     # (used in test only - see `LocalClient` and FS_66_17_43_42 test infra):
     use_local_requests = fields.Boolean(
         required = False,
+        load_default = False,
     )
 
     # Use one of these (default = True):
     # *   if True: ProposeArgValuesRemoteOptimizedClientCommand
     # *   if False: ProposeArgValuesRemoteClientCommand
     optimize_completion_request = fields.Boolean(
         required = False,
+        load_default = True,
     )
 
     connection_config = fields.Nested(connection_config_desc.dict_schema)
 
     # Enables spinner for FS_14_59_14_06: pending requests.
     show_pending_spinner = fields.Boolean(
         required = False,
+        load_default = False,
     )
 
     spinless_sleep_sec = fields.Number(
         required = False,
         # Noticeable threshold is around 200 ms, but default to spin immediately:
-        default = 0.0,
+        load_default = 0.0,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return ClientConfig(
-            use_local_requests = input_dict.get(use_local_requests_, False),
-            optimize_completion_request = input_dict.get(optimize_completion_request_, True),
-            connection_config = input_dict[connection_config_],
-            show_pending_spinner = input_dict.get(show_pending_spinner_, False),
-            spinless_sleep_sec = input_dict.get(spinless_sleep_sec_, 0.0),
-        )
-
 
 client_config_desc = TypeDesc(
     dict_schema = ClientConfigSchema(),
     ref_name = ClientConfigSchema.__name__,
     dict_example = {
         connection_config_: connection_config_desc.dict_example,
     },
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_client/ConnectionConfigSchema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,36 @@
-from marshmallow import Schema, fields, RAISE, post_load
+from marshmallow import fields, RAISE
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.ConnectionConfig import ConnectionConfig
 from argrelay.server_spec.const_int import DEFAULT_IP_ADDRESS, DEFAULT_PORT_NUMBER
 
+server_host_name_ = "server_host_name"
+server_port_number_ = "server_port_number"
 
-class ConnectionConfigSchema(Schema):
+
+class ConnectionConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = ConnectionConfig
+
     server_host_name = fields.String(
-        default = DEFAULT_IP_ADDRESS,
+        load_default = DEFAULT_IP_ADDRESS,
     )
 
     server_port_number = fields.Integer(
-        default = DEFAULT_PORT_NUMBER,
+        load_default = DEFAULT_PORT_NUMBER,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return ConnectionConfig(
-            server_host_name = input_dict["server_host_name"],
-            server_port_number = input_dict["server_port_number"],
-        )
-
 
 connection_config_desc = TypeDesc(
     dict_schema = ConnectionConfigSchema(),
     ref_name = ConnectionConfigSchema.__name__,
     dict_example = {
-        "server_host_name": DEFAULT_IP_ADDRESS,
-        "server_port_number": DEFAULT_PORT_NUMBER,
+        server_host_name_: DEFAULT_IP_ADDRESS,
+        server_port_number_: DEFAULT_PORT_NUMBER,
     },
     default_file_path = "",
 )
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/EnvelopeCollectionSchema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 from __future__ import annotations
 
 from typing import Callable, Collection
 
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.EnvelopeCollection import EnvelopeCollection
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.schema_config_interp.DataEnvelopeSchema import data_envelope_desc
 from argrelay.schema_response.EnvelopeContainerSchema import data_envelopes_
 
 index_fields_ = "index_fields"
 
 
-class EnvelopeCollectionSchema(Schema):
+class EnvelopeCollectionSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = EnvelopeCollection
+
     index_fields = fields.List(
         fields.String(),
         required = False,
         load_default = [],
     )
 
     # TODO_00_79_72_55: do not store `data_envelopes`
     data_envelopes = fields.List(
         fields.Nested(data_envelope_desc.dict_schema),
-        load_default = [],
         required = False,
+        load_default = [],
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return EnvelopeCollection(
-            index_fields = input_dict[index_fields_],
-            data_envelopes = input_dict[data_envelopes_],
-        )
-
 
 envelope_collection_desc = TypeDesc(
     dict_schema = EnvelopeCollectionSchema(),
     ref_name = EnvelopeCollectionSchema.__name__,
     dict_example = {
         index_fields_: [
             "SomeTypeA",
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoClientConfigSchema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,34 @@
-from marshmallow import Schema, fields, RAISE, post_load
+from marshmallow import fields, RAISE
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.mongo_data.MongoClientConfig import MongoClientConfig
 
 client_connection_string_ = "client_connection_string"
 
 
-class MongoClientConfigSchema(Schema):
+class MongoClientConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = MongoClientConfig
+
     client_connection_string = fields.String()
     """
     See: https://www.mongodb.com/docs/manual/reference/connection-string/
 
     Full format:
     mongodb://[username:password@]host1[:port1][,...hostN[:portN]][/[defaultauthdb][?options]]
 
     The simplest:
     mongodb://localhost
     """
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return MongoClientConfig(
-            client_connection_string = input_dict[client_connection_string_],
-        )
-
 
 mongo_client_config_desc = TypeDesc(
     dict_schema = MongoClientConfigSchema(),
     ref_name = MongoClientConfigSchema.__name__,
     dict_example = {
         client_connection_string_: "mongodb://localhost",
     },
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoConfigSchema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from marshmallow import Schema, fields, RAISE, post_load
+from marshmallow import fields, RAISE
 
 from argrelay.enum_desc.DistinctValuesQuery import DistinctValuesQuery
-from argrelay.misc_helper_common import ensure_value_is_enum
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.mongo_data.MongoConfig import MongoConfig
 from argrelay.schema_config_core_server.MongoClientConfigSchema import mongo_client_config_desc
 from argrelay.schema_config_core_server.MongoServerConfigSchema import mongo_server_config_desc
 
 use_mongomock_ = "use_mongomock"
 distinct_values_query_ = "distinct_values_query"
 mongo_client_ = "mongo_client"
 mongo_server_ = "mongo_server"
 
 
-class MongoConfigSchema(Schema):
+class MongoConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = MongoConfig
+
     use_mongomock = fields.Boolean()
     """
     It might be the case that (test) `mongomock` lib actually provides necessary functionality and meet
     non-function requirements for many (prod) workloads without a need to deploy and administer MongoDB.
     https://github.com/mongomock/mongomock
     """
 
@@ -33,28 +35,14 @@
     See `DistinctValuesQuery`.
     """
 
     mongo_client = fields.Nested(mongo_client_config_desc.dict_schema)
 
     mongo_server = fields.Nested(mongo_server_config_desc.dict_schema)
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return MongoConfig(
-            use_mongomock = input_dict[use_mongomock_],
-            # TODO: Is calling `ensure_value_is_enum` even required?
-            distinct_values_query = ensure_value_is_enum(input_dict[distinct_values_query_], DistinctValuesQuery),
-            mongo_client = input_dict[mongo_client_],
-            mongo_server = input_dict[mongo_server_],
-        )
-
 
 mongo_config_desc = TypeDesc(
     dict_schema = MongoConfigSchema(),
     ref_name = MongoConfigSchema.__name__,
     dict_example = {
         use_mongomock_: True,
         distinct_values_query_: DistinctValuesQuery.original_find_and_loop.name,
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/MongoServerConfigSchema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from marshmallow import Schema, fields, RAISE, post_load
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.mongo_data.MongoServerConfig import MongoServerConfig
 
 database_name_ = "database_name"
 start_server_ = "start_server"
 server_start_command_ = "server_start_command"
 
 
-class MongoServerConfigSchema(Schema):
+class MongoServerConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = MongoServerConfig
+
     database_name = fields.String()
 
     start_server = fields.Boolean()
 
     server_start_command = fields.String()
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return MongoServerConfig(
-            database_name = input_dict[database_name_],
-            start_server = input_dict[start_server_],
-            server_start_command = input_dict[server_start_command_],
-        )
-
 
 mongo_server_config_desc = TypeDesc(
     dict_schema = MongoServerConfigSchema(),
     ref_name = MongoServerConfigSchema.__name__,
     dict_example = {
         database_name_: "argrelay",
         start_server_: False,
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/QueryCacheConfigSchema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,35 @@
 from marshmallow import Schema, fields, RAISE, post_load
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.relay_server.QueryCacheConfig import QueryCacheConfig
 
 enable_query_cache_ = "enable_query_cache"
 query_cache_ttl_sec_ = "query_cache_ttl_sec"
 query_cache_max_size_bytes_ = "query_cache_max_size_bytes"
 
 
-class QueryCacheConfigSchema(Schema):
+class QueryCacheConfigSchema(ObjectSchema):
     """
     Config schema for FS_39_58_01_91 query cache.
     """
 
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = QueryCacheConfig
+
     enable_query_cache = fields.Boolean()
 
     query_cache_ttl_sec = fields.Integer()
 
     query_cache_max_size_bytes = fields.Integer()
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return QueryCacheConfig(
-            enable_query_cache = input_dict[enable_query_cache_],
-            query_cache_ttl_sec = input_dict[query_cache_ttl_sec_],
-            query_cache_max_size_bytes = input_dict[query_cache_max_size_bytes_],
-        )
-
 
 query_cache_config_desc = TypeDesc(
     dict_schema = QueryCacheConfigSchema(),
     ref_name = QueryCacheConfigSchema.__name__,
     dict_example = {
         enable_query_cache_: True,
         query_cache_ttl_sec_: 60,
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerConfigSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/ServerConfigSchema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 from marshmallow import Schema, fields, RAISE, post_load
 
-from argrelay.custom_integ.ServiceArgType import ServiceArgType
 from argrelay.custom_integ.ServiceEnvelopeClass import ServiceEnvelopeClass
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
-from argrelay.runtime_data.EnvelopeCollection import EnvelopeCollection
 from argrelay.runtime_data.PluginEntry import PluginEntry
 from argrelay.runtime_data.ServerConfig import ServerConfig
 from argrelay.runtime_data.StaticData import StaticData
 from argrelay.schema_config_core_client.ConnectionConfigSchema import connection_config_desc
 from argrelay.schema_config_core_server.GuiBannerConfigSchema import gui_banner_config_desc
 from argrelay.schema_config_core_server.MongoConfigSchema import mongo_config_desc
 from argrelay.schema_config_core_server.QueryCacheConfigSchema import query_cache_config_desc
@@ -23,19 +22,21 @@
 gui_banner_config_ = "gui_banner_config"
 class_to_collection_map_ = "class_to_collection_map"
 server_plugin_control_ = "server_plugin_control"
 plugin_instance_entries_ = "plugin_instance_entries"
 static_data_ = "static_data"
 
 
-class ServerConfigSchema(Schema):
+class ServerConfigSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = ServerConfig
+
     connection_config = fields.Nested(
         connection_config_desc.dict_schema,
         required = True,
     )
 
     mongo_config = fields.Nested(
         mongo_config_desc.dict_schema,
@@ -88,32 +89,25 @@
 
     @post_load
     def make_object(
         self,
         input_dict,
         **kwargs,
     ):
+        # Build DAG:
         plugin_instance_id_activate_order_dag = {}
         for plugin_instance_id in input_dict[plugin_instance_entries_]:
             plugin_entry: PluginEntry = input_dict[plugin_instance_entries_][plugin_instance_id]
             plugin_instance_id_activate_order_dag[plugin_instance_id] = plugin_entry.plugin_dependencies
 
-        # Populate `plugin_instance_id` from `plugin_instance_entries` into each
-        return ServerConfig(
-            connection_config = input_dict[connection_config_],
-            mongo_config = input_dict[mongo_config_],
-            query_cache_config = input_dict[query_cache_config_],
-            gui_banner_config = input_dict[gui_banner_config_],
-            class_to_collection_map = input_dict[class_to_collection_map_],
-            server_plugin_control = input_dict[server_plugin_control_],
+        return type(self).model_class(
+            **input_dict,
             plugin_instance_id_activate_list = serialize_dag_to_list(
                 plugin_instance_id_activate_order_dag,
             ),
-            plugin_instance_entries = input_dict[plugin_instance_entries_],
-            static_data = input_dict[static_data_],
         )
 
 
 server_config_desc = TypeDesc(
     dict_schema = ServerConfigSchema(),
     ref_name = ServerConfigSchema.__name__,
     dict_example = {
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/ServerPluginControlSchema.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 from __future__ import annotations
 
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
+from argrelay.composite_tree.CompositeNodeSchema import base_node_desc
+from argrelay.composite_tree.CompositeForestSchema import composite_forest_desc
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.ServerPluginControl import ServerPluginControl
 
 first_interp_factory_id_ = "first_interp_factory_id"
+composite_forest_ = "composite_forest"
 reusable_config_data_ = "reusable_config_data"
 
 
-class ServerPluginControlSchema(Schema):
+class ServerPluginControlSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = ServerPluginControl
+
     first_interp_factory_id = fields.String(
         required = True,
     )
 
+    composite_forest = fields.Nested(
+        composite_forest_desc.dict_schema,
+        required = True,
+    )
+
     # This `dict` provides a place to store arbitrary data.
     # YAML allows reusing any (substantially complex) data via aliases:
     # https://stackoverflow.com/a/48946813/441652
     # But `marshmallow` does not allow arbitrary data by default
     # (and it is kept that way to let garbage slip through).
     # This `dict` is ignored on load -
     # the data is used by YAML loader before it even reaches the schema validation.
     # See also values merge:
     # https://stackoverflow.com/a/46644785/441652
     reusable_config_data = fields.Dict(
         required = False,
         load_default = {},
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return ServerPluginControl(
-            first_interp_factory_id = input_dict[first_interp_factory_id_],
-            # `reusable_config_data` is ignored
-        )
-
 
 server_plugin_control_desc = TypeDesc(
     dict_schema = ServerPluginControlSchema(),
     ref_name = ServerPluginControlSchema.__name__,
     dict_example = {
         first_interp_factory_id_: "SomeInterp",
+        composite_forest_: composite_forest_desc.dict_example,
     },
     default_file_path = "",
 )
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_core_server/StaticDataSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_core_server/StaticDataSchema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from __future__ import annotations
 
 from marshmallow import Schema, RAISE, fields, post_load
 
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.StaticData import StaticData
 from argrelay.schema_config_core_server.EnvelopeCollectionSchema import envelope_collection_desc
 
 envelope_collections_ = "envelope_collections"
 
 
 # TODO_00_79_72_55: remove in the future:
-class StaticDataSchema(Schema):
+class StaticDataSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = StaticData
+
     envelope_collections = fields.Dict(
         keys = fields.String(),
         values = fields.Nested(envelope_collection_desc.dict_schema),
         required = True,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return StaticData(
-            envelope_collections = input_dict[envelope_collections_],
-        )
-
 
 static_data_desc = TypeDesc(
     dict_schema = StaticDataSchema(),
     ref_name = StaticDataSchema.__name__,
     dict_example = {
         envelope_collections_: {
             ReservedEnvelopeClass.ClassFunction.name: envelope_collection_desc.dict_example,
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_interp/DataEnvelopeSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/DataEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/FuncEnvelopeSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/FunctionEnvelopeInstanceDataSchema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_interp/InitControlSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/InitControlSchema.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,36 @@
-from marshmallow import Schema, RAISE, fields, post_load
+from marshmallow import RAISE, fields
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_context.InitControl import InitControl
 
 init_types_to_values_ = "init_types_to_values"
 """
 Maps types to values for `init_control` (FS_46_96_59_05).
 """
 
 
-class InitControlSchema(Schema):
+class InitControlSchema(ObjectSchema):
     """
     Implements `init_control` (FS_46_96_59_05).
     """
 
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = InitControl
+
     init_types_to_values = fields.Dict(
         keys = fields.String(),
         values = fields.String(),
         required = True,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return InitControl(
-            init_types_to_values = input_dict[init_types_to_values_],
-        )
-
 
 init_control_desc = TypeDesc(
     dict_schema = InitControlSchema(),
     ref_name = InitControlSchema.__name__,
     dict_example = {
         init_types_to_values_: {
             "type_a": "TypeA",
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_interp/SearchControlSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_interp/SearchControlSchema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from marshmallow import Schema, RAISE, fields, validates_schema, ValidationError, post_load
 
 from argrelay.enum_desc.ReservedEnvelopeClass import ReservedEnvelopeClass
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_context.SearchControl import SearchControl
 
 collection_name_ = "collection_name"
 
 envelope_class_ = "envelope_class"
 """
@@ -15,26 +16,28 @@
 
 keys_to_types_list_ = "keys_to_types_list"
 """
 List of keys to use for named args during interpretation and arg types to use in query.
 """
 
 
-class SearchControlSchema(Schema):
+class SearchControlSchema(ObjectSchema):
     """
     Implements FS_31_70_49_15 # search_control
 
     Schema for search_control which specifies what arg types will be used in search of the `data_envelope`
     (and how they are mapped to named arg keys).
     """
 
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = SearchControl
+
     collection_name = fields.String(
         required = True,
     )
 
     envelope_class = fields.String(
         required = True,
     )
@@ -48,26 +51,14 @@
             # `prop_name`:
             values = fields.String(),
             required = True,
         ),
         required = True,
     )
 
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return SearchControl(
-            collection_name = input_dict[collection_name_],
-            envelope_class = input_dict[envelope_class_],
-            keys_to_types_list = input_dict[keys_to_types_list_],
-        )
-
     @validates_schema
     def validate_known(
         self,
         input_dict: dict,
         **kwargs,
     ):
         for key_to_type_entry in input_dict[keys_to_types_list_]:
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_config_plugin/PluginEntrySchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_config_plugin/PluginEntrySchema.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from marshmallow import Schema, fields, RAISE, post_load, pre_dump
+from marshmallow import fields, RAISE
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.runtime_data.PluginEntry import PluginEntry
 
 plugin_enabled_ = "plugin_enabled"
 plugin_config_ = "plugin_config"
 plugin_module_name_ = "plugin_module_name"
 plugin_class_name_ = "plugin_class_name"
 plugin_dependencies_ = "plugin_dependencies"
 
 
-class PluginEntrySchema(Schema):
+class PluginEntrySchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
+    model_class = PluginEntry
+
     plugin_enabled = fields.Boolean(
         required = False,
         load_default = True,
     )
 
     plugin_module_name = fields.String(
         required = True,
@@ -36,42 +39,14 @@
     )
 
     plugin_config = fields.Dict(
         required = False,
         load_default = {},
     )
 
-    @pre_dump
-    def make_dict(
-        self,
-        input_object: PluginEntry,
-        **kwargs,
-    ):
-        return {
-            plugin_enabled_: input_object.plugin_enabled,
-            plugin_module_name_: input_object.plugin_module_name,
-            plugin_class_name_: input_object.plugin_class_name,
-            plugin_dependencies_: input_object.plugin_dependencies,
-            plugin_config_: input_object.plugin_config,
-        }
-
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return PluginEntry(
-            plugin_enabled = input_dict[plugin_enabled_],
-            plugin_module_name = input_dict[plugin_module_name_],
-            plugin_class_name = input_dict[plugin_class_name_],
-            plugin_dependencies = input_dict[plugin_dependencies_],
-            plugin_config = input_dict[plugin_config_],
-        )
-
 
 _plugin_entry_example = {
     plugin_enabled_: True,
     plugin_module_name_: "SomePluginModule",
     plugin_class_name_: "SomePluginClass",
     plugin_dependencies_: [],
     plugin_config_: {
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_request/CallContextSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_request/CallContextSchema.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from marshmallow import Schema, fields, RAISE, post_load, pre_dump
+from marshmallow import fields, RAISE
 
 from argrelay.enum_desc.CompScope import CompScope
 from argrelay.enum_desc.ServerAction import ServerAction
-from argrelay.misc_helper_common import ensure_value_is_enum
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.server_spec.CallContext import CallContext
 
 server_action_ = "server_action"
 command_line_ = "command_line"
 cursor_cpos_ = "cursor_cpos"
 comp_scope_ = "comp_scope"
@@ -19,19 +19,21 @@
     command_line_: _sample_command_line,
     cursor_cpos_: len(_sample_command_line),
     comp_scope_: CompScope.ScopeInitial.name,
     is_debug_enabled_: False,
 }
 
 
-class CallContextSchema(Schema):
+class CallContextSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         ordered = True
 
+    model_class = CallContext
+
     server_action = fields.Enum(
         ServerAction,
         required = True,
         metadata = {
             "description": (
                 "Action to perform - see " + ServerAction.__name__ + " enum"
             ),
@@ -63,43 +65,14 @@
         required = True,
         metadata = {
             "description": "Enable extra debug output",
             "example": _call_context_example[is_debug_enabled_],
         },
     )
 
-    @pre_dump
-    def make_dict(
-        self,
-        input_object: CallContext,
-        **kwargs,
-    ):
-        return {
-            server_action_: input_object.server_action,
-            command_line_: input_object.command_line,
-            cursor_cpos_: input_object.cursor_cpos,
-            comp_scope_: ensure_value_is_enum(input_object.comp_scope, CompScope),
-            is_debug_enabled_: input_object.is_debug_enabled,
-        }
-
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        return CallContext(
-            server_action = ensure_value_is_enum(input_dict[server_action_], ServerAction),
-            command_line = input_dict[command_line_],
-            cursor_cpos = input_dict[cursor_cpos_],
-            # TODO: Is calling `ensure_value_is_enum` even required?
-            comp_scope = ensure_value_is_enum(input_dict[comp_scope_], CompScope),
-            is_debug_enabled = input_dict[is_debug_enabled_],
-        )
-
 
 call_context_desc = TypeDesc(
     dict_schema = CallContextSchema(),
     ref_name = CallContextSchema.__name__,
     dict_example = _call_context_example,
     default_file_path = "",
 )
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_response/ArgValuesSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_response/ArgValuesSchema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from marshmallow import Schema, fields, RAISE, pre_dump, post_load
+from marshmallow import fields, RAISE
 
+from argrelay.misc_helper_common.ObjectSchema import ObjectSchema
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.schema_response.ArgValues import ArgValues
 
 arg_values_ = "arg_values"
 
 _arg_values_example = {
     arg_values_: [
@@ -15,53 +16,31 @@
 
 
 # TODO_11_77_28_50: Make it possible to verify proposed arg_values in all `ServerAction`-s.
 # Append space to the command line (for surrogate token delimiter) in case of `ServerAction.RelayLineArgs`
 # to populate proposed arg_values to allow unconditionally assert proposed values in all tests
 # (for all `ServerAction`-s).
 
-class ArgValuesSchema(Schema):
+class ArgValuesSchema(ObjectSchema):
     class Meta:
         unknown = RAISE
         strict = True
 
     model_class = ArgValues
 
     arg_values = fields.List(
-        fields.String(default = ""),
-        default = [],
+        fields.String(
+            load_default = "",
+        ),
+        load_default = [],
         metadata = {
             "example": _arg_values_example[arg_values_],
         },
     )
 
-    @pre_dump
-    def make_dict(
-        self,
-        input_object: ArgValues,
-        **kwargs,
-    ):
-        return {
-            arg_values_: input_object.arg_values,
-        }
-
-    @post_load
-    def make_object(
-        self,
-        input_dict,
-        **kwargs,
-    ):
-        """
-        Implements inheritance as described here:
-        https://stackoverflow.com/a/65668854/441652
-        """
-        return type(self).model_class(
-            **input_dict,
-        )
-
 
 arg_values_desc = TypeDesc(
     dict_schema = ArgValuesSchema(),
     ref_name = ArgValuesSchema.__name__,
     dict_example = _arg_values_example,
     default_file_path = "",
 )
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_response/InterpResultSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_response/InterpResultSchema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from copy import deepcopy
 
-from marshmallow import RAISE, fields, pre_dump
+from marshmallow import RAISE, fields
 
+from argrelay.enum_desc.SpecialChar import SpecialChar
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.schema_response.ArgValuesSchema import ArgValuesSchema, arg_values_desc
 from argrelay.schema_response.EnvelopeContainerSchema import envelope_container_desc
 from argrelay.schema_response.InterpResult import InterpResult
 
 """
 Schema for the result of interpretation taken from :class:`InterpContext`
 """
 
 all_tokens_ = "all_tokens"
-consumed_tokens_ = "consumed_tokens"
+excluded_tokens_ = "excluded_tokens"
+consumed_arg_buckets_ = "consumed_arg_buckets"
 envelope_containers_ = "envelope_containers"
 tan_token_ipos_ = "tan_token_ipos"
 tan_token_l_part_ = "tan_token_l_part"
 
 
 class InterpResultSchema(ArgValuesSchema):
     """
@@ -30,59 +32,57 @@
     model_class = InterpResult
 
     all_tokens = fields.List(
         fields.String(),
         required = True,
     )
 
-    consumed_tokens = fields.List(
+    excluded_tokens = fields.List(
         fields.Integer(),
         required = True,
     )
 
+    consumed_arg_buckets = fields.List(
+        fields.List(
+            fields.Integer(),
+        ),
+        required = True,
+    )
+
     envelope_containers = fields.List(
         fields.Nested(envelope_container_desc.dict_schema),
         required = True,
     )
 
     tan_token_ipos = fields.Integer()
 
     tan_token_l_part = fields.String()
 
-    @pre_dump
-    def make_dict(
-        self,
-        input_object: InterpResult,
-        **kwargs,
-    ):
-        data_dict = super().make_dict(input_object)
-        data_dict.update({
-            all_tokens_: input_object.all_tokens,
-            consumed_tokens_: input_object.consumed_tokens,
-            envelope_containers_: input_object.envelope_containers,
-            tan_token_ipos_: input_object.tan_token_ipos,
-            tan_token_l_part_: input_object.tan_token_l_part,
-        })
-        return data_dict
-
 
 _interp_result_example = deepcopy(arg_values_desc.dict_example)
 _interp_result_example.update({
     all_tokens_: [
         "some_command",
         "unrecognized_token",
         "goto",
         "host",
         "prod",
+        SpecialChar.ArgBucketDelimiter.value,
+    ],
+    excluded_tokens_: [
+        5,
     ],
-    consumed_tokens_: [
-        0,
-        2,
-        3,
-        4,
+    consumed_arg_buckets_: [
+        [
+            0,
+            2,
+            3,
+            4,
+        ],
+        [],
     ],
     envelope_containers_: [
         envelope_container_desc.dict_example,
     ],
     tan_token_ipos_: 1,
     tan_token_l_part_: "unrecognized_",
 })
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_response/InvocationInput.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_response/InvocationInput.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
+from argrelay.runtime_context.InterpContext import InterpContext
 from argrelay.runtime_data.PluginEntry import PluginEntry
 from argrelay.schema_response.InterpResult import InterpResult
 
 
 @dataclass
 class InvocationInput(InterpResult):
     """
@@ -24,7 +25,25 @@
 
     custom_plugin_data: dict = field()
     """
     A placeholder dict for exclusive use by plugin.
 
     Whatever plugin server side needs to tell its plugin peer on the client side.
     """
+
+    @staticmethod
+    def with_interp_context(
+        interp_ctx: InterpContext,
+        delegator_plugin_entry: PluginEntry,
+        custom_plugin_data: dict,
+    ) -> InvocationInput:
+        return InvocationInput(
+            arg_values = interp_ctx.comp_suggestions,
+            all_tokens = interp_ctx.parsed_ctx.all_tokens,
+            excluded_tokens = interp_ctx.excluded_tokens,
+            consumed_arg_buckets = interp_ctx.consumed_arg_buckets,
+            envelope_containers = interp_ctx.envelope_containers,
+            tan_token_ipos = interp_ctx.parsed_ctx.tan_token_ipos,
+            tan_token_l_part = interp_ctx.parsed_ctx.tan_token_l_part,
+            delegator_plugin_entry = delegator_plugin_entry,
+            custom_plugin_data = custom_plugin_data,
+        )
```

### Comparing `argrelay-0.6.9/src/argrelay/schema_response/InvocationInputSchema.py` & `argrelay-0.7.0.dev0/src/argrelay/schema_response/InvocationInputSchema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 
-from marshmallow import RAISE, fields, pre_dump
+from marshmallow import RAISE, fields
 
 from argrelay.misc_helper_common.TypeDesc import TypeDesc
 from argrelay.plugin_delegator.ErrorDelegatorCustomDataSchema import error_delegator_custom_data_desc
 from argrelay.schema_config_plugin.PluginEntrySchema import plugin_entry_desc
 from argrelay.schema_response.InterpResultSchema import (
     InterpResultSchema,
     interp_result_desc,
@@ -27,27 +27,14 @@
         required = True,
     )
 
     custom_plugin_data = fields.Dict(
         required = False,
     )
 
-    @pre_dump
-    def make_dict(
-        self,
-        input_object: InvocationInput,
-        **kwargs,
-    ):
-        data_dict = super().make_dict(input_object)
-        data_dict.update({
-            delegator_plugin_entry_: input_object.delegator_plugin_entry,
-            custom_plugin_data_: input_object.custom_plugin_data,
-        })
-        return data_dict
-
 
 _invocation_input_example = deepcopy(interp_result_desc.dict_example)
 _invocation_input_example.update({
     delegator_plugin_entry_: plugin_entry_desc.dict_example,
     custom_plugin_data_: error_delegator_custom_data_desc.dict_example,
 })
```

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/CallContext.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/CallContext.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/DescribeLineArgsSpec.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/DescribeLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/ProposeArgValuesSpec.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/ProposeArgValuesSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/RelayLineArgsSpec.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/RelayLineArgsSpec.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/const_int.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/const_int.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/server_spec/server_data_schema.py` & `argrelay-0.7.0.dev0/src/argrelay/server_spec/server_data_schema.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/BaseTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/BaseTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/ClientServerTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/ClientServerTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/CustomTestCase.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/CustomTestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/CustomVerifier.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/CustomVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/End2EndTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/End2EndTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/EnvMockBuilder.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/EnvMockBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -935,27 +935,30 @@
 
 ########################################################################################################################
 # Test objects
 
 def default_test_parsed_context(
     command_line: str,
     cursor_cpos: int,
+    comp_type: CompType = CompType.PrefixShown,
 ) -> ParsedContext:
     return ParsedContext.from_instance(
-        default_test_input_context(
+        default_test_call_context(
             command_line,
             cursor_cpos,
+            comp_type,
         ),
     )
 
 
-def default_test_input_context(
+def default_test_call_context(
     command_line: str,
     cursor_cpos: int,
+    comp_type: CompType = CompType.PrefixShown,
 ) -> CallContext:
     return ShellContext(
         command_line = command_line,
         cursor_cpos = cursor_cpos,
-        comp_type = CompType.PrefixShown,
+        comp_type = comp_type,
         comp_key = UNKNOWN_COMP_KEY,
         is_debug_enabled = False,
     ).create_call_context()
```

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/InOutTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/InOutTestClass.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         actual_suggestions: list[str],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         container_ipos_to_options_hidden_by_default_value: Union[dict[int, dict[str, list[str]]], None],
         delegator_class: Union[Type[AbstractDelegator], None],
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
         expected_suggestions: Union[list[str], None],
         envelope_containers: list[EnvelopeContainer],
+        expected_container_ipos_to_used_arg_bucket: Union[dict[int, Union[int, None]], None],
     ):
         try:
 
             if expected_suggestions is not None:
                 self.assertEqual(expected_suggestions, actual_suggestions)
 
             if container_ipos_to_expected_assignments is not None:
@@ -67,14 +68,23 @@
 
             if envelope_ipos_to_field_values is not None:
                 self.verify_data_envelopes(
                     EnvMockBuilder.invocation_input.get_data_envelopes(),
                     envelope_ipos_to_field_values,
                 )
 
+            if expected_container_ipos_to_used_arg_bucket is not None:
+                # TODO_32_99_70_35: candidate for generic library of JSONPath verifiers:
+                for envelope_container_ipos, envelope_container in enumerate(envelope_containers):
+                    expected_used_arg_bucket = expected_container_ipos_to_used_arg_bucket[envelope_container_ipos]
+                    self.assertEqual(
+                        expected_used_arg_bucket,
+                        envelope_container.used_arg_bucket,
+                    )
+
         except:
 
             # Check if there are some obvious test input mistakes:
 
             if call_ctx.server_action is ServerAction.ProposeArgValues:
                 self.assertIsNone(delegator_class)
                 self.assertIsNone(envelope_ipos_to_field_values)
@@ -127,14 +137,19 @@
                 raise
 
     def verify_options_hidden_by_default_value(
         self,
         envelope_containers: list[EnvelopeContainer],
         container_ipos_to_options_hidden_by_default_value: Union[dict[int, dict[str, list[str]]], None],
     ):
+        """
+        Make sure that specified expected `options_hidden_by_default_value` list
+        (per `envelope_container` ipos, per `arg_type`) match what is populated into
+        `EnvelopeContainer.filled_types_to_values_hidden_by_defaults`.
+        """
         for container_ipos, options_hidden_by_default_value_per_type in container_ipos_to_options_hidden_by_default_value.items():
             try:
                 if options_hidden_by_default_value_per_type is None:
                     self.assertFalse(0 <= container_ipos < len(envelope_containers))
                 else:
                     self.assertTrue(0 <= container_ipos < len(envelope_containers))
                     for arg_type, options_hidden_by_default_value in options_hidden_by_default_value_per_type.items():
@@ -173,26 +188,37 @@
         then, the assigned value has `ArgSource.DefaultValue`.
         """
         for container_ipos, expected_assignments in container_ipos_to_expected_assignments.items():
             try:
                 if expected_assignments is not None:
                     if container_ipos in container_ipos_to_options_hidden_by_default_value:
                         for arg_type, assigned_value in expected_assignments.items():
-                            options_hidden_by_default_value_per_type = container_ipos_to_options_hidden_by_default_value[
-                                container_ipos
-                            ]
+                            options_hidden_by_default_value_per_type = (
+                                container_ipos_to_options_hidden_by_default_value[
+                                    container_ipos
+                                ]
+                            )
                             if arg_type in options_hidden_by_default_value_per_type:
-                                self.assertEqual(
-                                    assigned_value.arg_source,
-                                    ArgSource.DefaultValue,
-                                )
+                                if options_hidden_by_default_value_per_type[arg_type] is None:
+                                    self.assertNotEqual(
+                                        assigned_value.arg_source,
+                                        ArgSource.DefaultValue,
+                                    )
+                                else:
+                                    self.assertEqual(
+                                        assigned_value.arg_source,
+                                        ArgSource.DefaultValue,
+                                    )
             except:
-                print(f"container_ipos_to_expected_assignments:\n{container_ipos_to_expected_assignments}")
                 print(
-                    f"container_ipos_to_options_hidden_by_default_value:\n{container_ipos_to_options_hidden_by_default_value}")
+                    f"container_ipos_to_expected_assignments:\n{container_ipos_to_expected_assignments}"
+                )
+                print(
+                    f"container_ipos_to_options_hidden_by_default_value:\n{container_ipos_to_options_hidden_by_default_value}"
+                )
                 raise
 
     def verify_data_envelopes(
         self,
         data_envelopes,
         envelope_ipos_to_field_values,
     ):
```

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/JsonTestOutputVerifier.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/JsonTestOutputVerifier.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/LocalClient.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalClient.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/LocalClientCommandFactory.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalClientCommandFactory.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/LocalTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/LocalTestClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,27 +50,29 @@
             test_line,
             comp_type,
             expected_suggestions,
             container_ipos_to_expected_assignments,
             None,
             delegator_class,
             envelope_ipos_to_field_values,
+            None,
             LocalClientEnvMockBuilder(),
         )
 
     def verify_output_via_local_client(
         self,
         test_data: str,
         test_line: str,
         comp_type: CompType,
         expected_suggestions: Union[list[str], None],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         container_ipos_to_options_hidden_by_default_value: Union[dict[int, dict[str, list[str]]], None],
         delegator_class: Union[Type[AbstractDelegator], None],
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
+        expected_container_ipos_to_used_arg_bucket: Union[dict[int, Union[int, None]], None],
         init_env_mock_builder: EnvMockBuilder,
     ):
         (command_line, cursor_cpos) = parse_line_and_cpos(test_line)
 
         if envelope_ipos_to_field_values is not None:
             self.assertIsNotNone(delegator_class)
 
@@ -111,8 +113,9 @@
                 actual_suggestions,
                 container_ipos_to_expected_assignments,
                 container_ipos_to_options_hidden_by_default_value,
                 delegator_class,
                 envelope_ipos_to_field_values,
                 expected_suggestions,
                 interp_ctx.envelope_containers,
+                expected_container_ipos_to_used_arg_bucket,
             )
```

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/OpenFileMock.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/OpenFileMock.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/PopenMock.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/PopenMock.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,17 @@
                 # The call to `Popen` with CLI args matching one of the expected ones:
                 # all these fields will (potentially) be inspected through other calls to `Popen` - configure them:
                 return ConfiguredPopenMockDelegatee(
                     cli_args,
                     *p_output_config_tuple,
                 )
         else:
-            raise ValueError(f"unexpected CLI args: `{cli_args}` expected CLI args: `{self.expected_args_to_output.keys()}`")
+            raise ValueError(
+                f"unexpected CLI args: `{cli_args}` expected CLI args: `{self.expected_args_to_output.keys()}`"
+            )
 
 
 class ConfiguredPopenMockDelegatee:
 
     def __init__(
         self,
         args: Union[str, list[str]],
```

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/RemoteTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/RemoteTestClass.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         self,
         test_line: str,
         comp_type: CompType,
         expected_suggestions: Union[list[str], None],
         container_ipos_to_expected_assignments: Union[dict[int, dict[str, AssignedValue]], None],
         delegator_class: Union[Type[AbstractDelegator], None],
         envelope_ipos_to_field_values: Union[dict[int, dict[str, str]], None],
+        expected_container_ipos_to_used_arg_bucket: Union[dict[int, Union[int, None]], None],
         init_env_mock_builder: EnvMockBuilder,
     ):
         (command_line, cursor_cpos) = parse_line_and_cpos(test_line)
 
         if envelope_ipos_to_field_values is not None:
             self.assertIsNotNone(delegator_class)
 
@@ -90,8 +91,9 @@
                 actual_suggestions,
                 container_ipos_to_expected_assignments,
                 None,
                 delegator_class,
                 envelope_ipos_to_field_values,
                 expected_suggestions,
                 envelope_containers,
+                expected_container_ipos_to_used_arg_bucket,
             )
```

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/ServerOnlyTestClass.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/ServerOnlyTestClass.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/TestCase.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/TestCase.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay/test_infra/__init__.py` & `argrelay-0.7.0.dev0/src/argrelay/test_infra/__init__.py`

 * *Files identical despite different names*

### Comparing `argrelay-0.6.9/src/argrelay.egg-info/PKG-INFO` & `argrelay-0.7.0.dev0/src/argrelay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argrelay
-Version: 0.6.9
+Version: 0.7.0.dev0
 Summary: Tab-completion & data search server = total recall for Bash shell
 Home-page: https://github.com/argrelay/argrelay
 Author: uvsmtid
 Author-email: uvsmtid@gmail.com
 Project-URL: Bug Tracker, https://github.com/argrelay/argrelay/issues
 Keywords: argparse,argcomplete,bash,complete
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `argrelay-0.6.9/src/argrelay.egg-info/SOURCES.txt` & `argrelay-0.7.0.dev0/src/argrelay.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -40,18 +40,19 @@
 ./docs/feature_stories/FS_15_79_76_85.line_processor.md
 ./docs/feature_stories/FS_16_07_78_84.conf_dir_priority.md
 ./docs/feature_stories/FS_18_64_57_18.function_with_indefinite_input_data_envelopes_like_varargs.md
 ./docs/feature_stories/FS_20_88_05_60.named_args.md
 ./docs/feature_stories/FS_23_62_89_43.tangent_arg_value_completion.md
 ./docs/feature_stories/FS_24_50_40_64.arg_types_without_envelope_classes.md
 ./docs/feature_stories/FS_26_43_73_72.func_tree.md
+./docs/feature_stories/FS_27_16_67_19.line_syntax.md
 ./docs/feature_stories/FS_29_54_67_86.dir_structure.md
 ./docs/feature_stories/FS_31_70_49_15.search_control.md
 ./docs/feature_stories/FS_32_05_46_00.startwith_vs_contains.md
-./docs/feature_stories/FS_33_76_82_84.global_tree.md
+./docs/feature_stories/FS_33_76_82_84.composite_tree.md
 ./docs/feature_stories/FS_36_17_84_44.check_script.md
 ./docs/feature_stories/FS_37_57_36_29.envelopes_and_payloads.md
 ./docs/feature_stories/FS_39_58_01_91.query_cache.md
 ./docs/feature_stories/FS_41_40_39_44.suggest_from_interp_tree.md
 ./docs/feature_stories/FS_42_76_93_51.very_first_zero_arg_mapping_interp.md
 ./docs/feature_stories/FS_43_50_57_71.echo_args_func.md
 ./docs/feature_stories/FS_44_36_84_88.consume_args_one_by_one.md
@@ -82,14 +83,15 @@
 ./docs/feature_stories/FS_85_33_46_53.bootstrap_dev_env.md
 ./docs/feature_stories/FS_86_73_43_45.server_control_scripts.md
 ./docs/feature_stories/FS_88_66_66_73.intercept_invocation_func.md
 ./docs/feature_stories/FS_90_48_11_45.forced_assignment_from_entire_type_value_space.md
 ./docs/feature_stories/FS_91_88_07_23.jump_tree.md
 ./docs/feature_stories/FS_92_75_93_01.clean_command_line.md
 ./docs/feature_stories/FS_94_30_49_28.help_doc.md
+./docs/feature_stories/FS_97_64_39_94.arg_buckets.md
 ./docs/feature_stories/FS_98_55_40_77.invoke_control.md
 ./docs/feature_stories/FS_99_81_19_25.no_space_in_options.md
 ./docs/feature_stories/readme.md
 ./docs/release_notes/readme.md
 ./docs/release_notes/v0.0.0.dev0.md
 ./docs/release_notes/v0.0.0.dev27.md
 ./docs/release_notes/v0.0.0.dev28.md
@@ -114,23 +116,27 @@
 ./docs/task_refs/TODO_11_77_28_50.suggestions_in_all_responses.md
 ./docs/task_refs/TODO_24_22_11_49.avoid_removing_last_history_command.md
 ./docs/task_refs/TODO_26_08_72_06.interp_vs_delegator.md
 ./docs/task_refs/TODO_26_15_31_78.categorize_git_repo_existence.md
 ./docs/task_refs/TODO_27_61_22_18.make_shell_vars_local.md
 ./docs/task_refs/TODO_32_99_70_35.JSONPath_to_verify_response_data.md
 ./docs/task_refs/TODO_37_15_12_91.Popen_mock.md
+./docs/task_refs/TODO_40_10_18_32.add_custom_base_to_all_schemas.md
 ./docs/task_refs/TODO_42_81_01_90.assert_data_instead_of_print_out.md
+./docs/task_refs/TODO_43_41_95_86.use_server_logger_to_disable_stdout.md
 ./docs/task_refs/TODO_45_75_75_65.remove_instance_data_leave_envelop_payload.md
 ./docs/task_refs/TODO_51_29_08_00.combine_interp_factory_with_interp.md
 ./docs/task_refs/TODO_54_68_18_12.support_defaults_for_config_only_delegator.md
 ./docs/task_refs/TODO_64_79_28_85.make_publish_package_upgrade_all_packages_before_test.md
 ./docs/task_refs/TODO_66_66_75_78.split_arg_and_prop_concepts.md
-./docs/task_refs/TODO_70_48_96_29.be_able_to_assert_unconsumed_arg_vals.md
+./docs/task_refs/TODO_70_48_96_29.be_able_to_assert_remaining_arg_vals.md
 ./docs/task_refs/TODO_74_73_60_93.support_expected_envelope_count_in_config_only_delegator.md
+./docs/task_refs/TODO_75_52_01_67.arg_buckets_to_support_multiple_var_args.md
 ./docs/task_refs/TODO_78_94_31_68.split_argrelay_into_multiple_packages.md
+./docs/task_refs/TODO_79_67_28_83.recursive_dict_schema.md
 ./docs/task_refs/TODO_81_49_24_81.json_or_repr_before_intercept_jump.md
 ./docs/task_refs/TODO_84_71_86_21.realistic_useful_config_only_command_example.md
 ./docs/task_refs/TODO_94_66_41_94.separate_config_for_plugins.md
 ./docs/task_refs/TODO_99_87_25_42.next_incompatible_changes.md
 ./docs/task_refs/readme.md
 ./docs/test_data/TD_27_59_80_86.single_data_envelope_arg_suggestion_and_consumption.md
 ./docs/test_data/TD_38_03_48_51.large_data_set.md
@@ -155,14 +161,23 @@
 ./src/argrelay/client_command_remote/DescribeLineArgsRemoteClientCommand.py
 ./src/argrelay/client_command_remote/ProposeArgValuesRemoteClientCommand.py
 ./src/argrelay/client_command_remote/ProposeArgValuesRemoteOptimizedClientCommand.py
 ./src/argrelay/client_command_remote/RelayLineArgsRemoteClientCommand.py
 ./src/argrelay/client_command_remote/__init__.py
 ./src/argrelay/client_spec/ShellContext.py
 ./src/argrelay/client_spec/__init__.py
+./src/argrelay/composite_tree/CompositeForest.py
+./src/argrelay/composite_tree/CompositeForestSchema.py
+./src/argrelay/composite_tree/CompositeInfoType.py
+./src/argrelay/composite_tree/CompositeNode.py
+./src/argrelay/composite_tree/CompositeNodeSchema.py
+./src/argrelay/composite_tree/CompositeNodeType.py
+./src/argrelay/composite_tree/CompositeTreeWalker.py
+./src/argrelay/composite_tree/DictTreeWalker.py
+./src/argrelay/composite_tree/__init__.py
 ./src/argrelay/custom_integ/BaseConfigDelegator.py
 ./src/argrelay/custom_integ/BaseConfigDelegatorConfigSchema.py
 ./src/argrelay/custom_integ/ConfigOnlyDelegator.py
 ./src/argrelay/custom_integ/ConfigOnlyDelegatorConfigSchema.py
 ./src/argrelay/custom_integ/ConfigOnlyLoader.py
 ./src/argrelay/custom_integ/ConfigOnlyLoaderConfigSchema.py
 ./src/argrelay/custom_integ/FuncConfigSchema.py
@@ -209,14 +224,15 @@
 ./src/argrelay/handler_request/__init__.py
 ./src/argrelay/handler_response/AbstractClientResponseHandler.py
 ./src/argrelay/handler_response/DescribeLineArgsClientResponseHandler.py
 ./src/argrelay/handler_response/ProposeArgValuesClientResponseHandler.py
 ./src/argrelay/handler_response/RelayLineArgsClientResponseHandler.py
 ./src/argrelay/handler_response/__init__.py
 ./src/argrelay/misc_helper_common/ElapsedTime.py
+./src/argrelay/misc_helper_common/ObjectSchema.py
 ./src/argrelay/misc_helper_common/TypeDesc.py
 ./src/argrelay/misc_helper_common/__init__.py
 ./src/argrelay/misc_helper_server/__init__.py
 ./src/argrelay/mongo_data/MongoClientConfig.py
 ./src/argrelay/mongo_data/MongoClientWrapper.py
 ./src/argrelay/mongo_data/MongoConfig.py
 ./src/argrelay/mongo_data/MongoServerConfig.py
@@ -225,14 +241,15 @@
 ./src/argrelay/plugin_config/AbstractConfigurator.py
 ./src/argrelay/plugin_config/DefaultConfigurator.py
 ./src/argrelay/plugin_config/DefaultConfiguratorConfig.py
 ./src/argrelay/plugin_config/DefaultConfiguratorConfigSchema.py
 ./src/argrelay/plugin_config/__init__.py
 ./src/argrelay/plugin_delegator/AbstractDelegator.py
 ./src/argrelay/plugin_delegator/AbstractJumpDelegator.py
+./src/argrelay/plugin_delegator/AbstractJumpDelegatorConfigSchema.py
 ./src/argrelay/plugin_delegator/EchoDelegator.py
 ./src/argrelay/plugin_delegator/ErrorDelegator.py
 ./src/argrelay/plugin_delegator/ErrorDelegatorCustomDataSchema.py
 ./src/argrelay/plugin_delegator/HelpDelegator.py
 ./src/argrelay/plugin_delegator/InterceptDelegator.py
 ./src/argrelay/plugin_delegator/NoopDelegator.py
 ./src/argrelay/plugin_delegator/QueryEnumDelegator.py
@@ -246,15 +263,14 @@
 ./src/argrelay/plugin_interp/FuncTreeInterpFactory.py
 ./src/argrelay/plugin_interp/FuncTreeInterpFactoryConfigSchema.py
 ./src/argrelay/plugin_interp/InterpTreeInterp.py
 ./src/argrelay/plugin_interp/InterpTreeInterpFactory.py
 ./src/argrelay/plugin_interp/InterpTreeInterpFactoryConfigSchema.py
 ./src/argrelay/plugin_interp/NoopInterp.py
 ./src/argrelay/plugin_interp/NoopInterpFactory.py
-./src/argrelay/plugin_interp/TreeWalker.py
 ./src/argrelay/plugin_interp/__init__.py
 ./src/argrelay/plugin_loader/AbstractLoader.py
 ./src/argrelay/plugin_loader/NoopLoader.py
 ./src/argrelay/plugin_loader/__init__.py
 ./src/argrelay/relay_client/AbstractClient.py
 ./src/argrelay/relay_client/AbstractClientCommand.py
 ./src/argrelay/relay_client/AbstractClientCommandFactory.py
@@ -283,14 +299,15 @@
 ./src/argrelay/runtime_context/AbstractPlugin.py
 ./src/argrelay/runtime_context/EnvelopeContainer.py
 ./src/argrelay/runtime_context/InitControl.py
 ./src/argrelay/runtime_context/InterpContext.py
 ./src/argrelay/runtime_context/ParsedContext.py
 ./src/argrelay/runtime_context/SearchControl.py
 ./src/argrelay/runtime_context/__init__.py
+./src/argrelay/runtime_context/arg_buckets_utils.py
 ./src/argrelay/runtime_data/AssignedValue.py
 ./src/argrelay/runtime_data/ClientConfig.py
 ./src/argrelay/runtime_data/ConnectionConfig.py
 ./src/argrelay/runtime_data/EnvelopeCollection.py
 ./src/argrelay/runtime_data/PluginEntry.py
 ./src/argrelay/runtime_data/ServerConfig.py
 ./src/argrelay/runtime_data/ServerPluginControl.py
```

