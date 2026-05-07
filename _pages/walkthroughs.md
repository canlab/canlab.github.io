---
permalink: /walkthroughs/
title: "Object-oriented analysis walkthroughs"
excerpt: "Code to run each walkthrough is included in the CANlab core toolbox or on Neurovault."
author_profile: false
toc: true
toc_label: "Walkthroughs"
toc_sticky: true
# redirect_from:
#  * /objectoriented/
#  * /objectoriented.md
---
{% include base_path %}

This series of walkthroughs is designed to illustrate the CANlab interactive analysis tools, and some analysis principles as well. Code to run each walkthrough is included in the CANlab core toolbox or on Neurovault. See the main [CANlab intro page](/) for the philosophy behind the interactive analysis approach.

These walkthroughs focus on **using CANlab code** and are not didactic. For more extensive explanation of fMRI concepts, see the [didactic tutorials](/tutorials) using Matlab live scripts.

**Tip:** Use the [search page]({{ "/search/" | relative_url }}) to find a walkthrough by topic.

## 1. Getting started

Install the toolboxes, load a sample dataset, and learn the basic visualization and reporting commands.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 1.1 | [Installing tools](canlab_help_1_installing_tools/canlab_help_1_installing_tools.html) | |
| 1.2 | [Getting help](canlab_help_1b_getting_help/canlab_help_1b_getting_help.html) | [.mlx](canlab_help_1b_getting_help/canlab_help_1b_getting_help.mlx) |
| 1.3 | [Load a sample dataset](canlab_help_2_load_a_sample_dataset/canlab_help_2_load_a_sample_dataset.html) | |
| 1.4 | [Basic image visualization](canlab_help_2b_basic_image_visualization/canlab_help_2b_basic_image_visualization.html) | |
| 1.5 | [Loading datasets used in tutorials](canlab_help_2c_loading_datasets/canlab_help_2c_loading_datasets.html) | |
| 1.6 | [Publishing results reports](canlab_help_2d_publish_a_report/canlab_help_2d_publish_a_report.html) | |
| 1.7 | Basic Matlab debugging | [.mlx](/tutorials/matlab/basic_matlab_debugging.mlx) |
| 1.8 | [Voxel and image spaces in fmri_data objects](Voxel_and_image_spaces_in_CANlab_fmri_data_objects.html) | [.mlx](Voxel_and_image_spaces_in_CANlab_fmri_data_objects.mlx) |

## 2. Basic analyses

Group statistics, ROI analysis, masking, surface rendering, and design matrices.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 2.1 | [Group t-test](canlab_help_3_voxelwise_t_test_walkthrough/canlab_help_3_voxelwise_t_test_walkthrough.html) | |
| 2.2 | [Atlases and ROI analysis](canlab_help_3b_atlases_and_ROI_analysis/canlab_help_3b_atlases_and_ROI_analysis.html) | |
| 2.3 | [Masking and writing NIfTI image files](canlab_help_4_masking_and_writing_nifti_files/canlab_help_4_masking_and_writing_nifti_files.html) | |
| 2.4 | [3-D visualization on brain surfaces](canlab_help_4b_3D_visualization/canlab_help_4b_3D_visualization.html) | |
| 2.5 | [Create and explore 1st-level design matrices](first_level_design_matrix_exploration/first_level_design_matrix_exploration.html) | |
| 2.6 | [Regression — interactive analysis](canlab_help_5_regression_walkthrough/canlab_help_5_regression_walkthrough.html) | |
| 2.7 | [Interpreting maps with Neurosynth topic similarity and wedge plots](neurosynth_topic_similarity_and_wedge_plot/neurosynth_topic_similarity_and_wedge_plot.html) | |
| 2.8 | [Annotating a results map (gradients, neurochemical maps, networks, Neurosynth topics)](canlab_help_annotate_thresholded_results_map/canlab_help_annotate_thresholded_results_map.html) | |

## 3. Multivariate predictive models

Cross-validated multivariate prediction, applying signature patterns, and Bayesian results.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 3.1 | [Multivariate prediction with continuous outcomes](canlab_help_7_multivariate_prediction_basics/canlab_help_7_multivariate_prediction_basics.html) | |
| 3.2 | Effect sizes with SVMs *(in progress)* | |
| 3.3 | [Apply a multivariate pattern of interest](canlab_help_9_apply_a_multivariate_pattern_of_interest/canlab_help_9_apply_a_multivariate_pattern_of_interest.html) | |
| 3.4 | [Bayes Factor maps](EmoReg_BayesFactor_walkthrough/EmoReg_BayesFactor_walkthrough.html) | |
| 3.5 | [Interpreting maps with riverplots](canlab_help_8_riverplot_cerebellar_atlas_example.m/canlab_help_8_riverplot_cerebellar_atlas_example.html) | |

## 4. Mediation analysis

Single- and multi-level mediation effect parametric mapping (the M3 toolbox).

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 4.1 | [Mediation and M3 Toolbox basics](tutorials/html/mediation_1_basics.html) | [.mlx](tutorials/matlab/mediation_1_basics.mlx) |
| 4.2 | [Single-level Mediation Effect Parametric Mapping (fMRI)](tutorials/html/mediation_brain_single_level_walkthrough1.html) | [.mlx](tutorials/matlab/mediation_brain_single_level_walkthrough1.mlx) |
| 4.2b | [Sample MEPM report from publish_mediation_report.m](mediation_brain_sample_report/mediation_brain_results_report.html) | |
| 4.3 | [Multilevel Mediation Effect Mapping (fMRI)](tutorials/html/mediation_brain_multilevel_walkthrough1.html) | [.mlx](tutorials/matlab/mediation_brain_multilevel_walkthrough1.mlx) |

## 5. Coordinate-based meta-analysis

MKDA-style meta-analysis of published activation coordinates.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 5.1 | [MKDA meta-analysis 1](canlab_meta_analysis_walkthrough1.m/canlab_meta_analysis_walkthrough1.html) | |

## 6. Multivariate Pathway Identification (MPathI) and connectivity

Prepare time-series data and run multivariate pathway identification.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 6.1 | [Prep time-series data for connectivity](tutorials/html/canlab_help_prep_for_connectivity.html) | [.mlx](tutorials/matlab/canlab_help_prep_for_connectivity.mlx) |
| 6.2 | [MPathI pathway dissociation](tutorials/html/canlab_help_MPathI_multivariate_pathway.html) | [.mlx](tutorials/matlab/canlab_help_MPathI_multivariate_pathway.mlx) |

## 7. Visualization extras

Additional brain-rendering and surface-projection examples.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 7.1 | [More visualization](visualize_neuroimaging_data/visualize_neuroimaging_data.html) | |
| 7.2 | [Surface rendering](canlab_help_surface_projection/mnisurf_projection_tutorial.html) | |
| 7.3 | [CANlab single-trials demo](canlab_single_trials_demo/demo_norming_comparison.html) | |

## 8. Behavioral data and plots

Working with the canlab_dataset object and generating publication plots.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 8.1 | [The canlab_dataset object](canlab_dataset_basic_usage/canlab_dataset_basic_usage.html) | |
| 8.2 | [Time series and bar plots](atlas_2012_behavioral_plot_example_figure/atlas_2012_behavioral_plot_example_figure.html) | |
| 8.3 | [Mixed-effects models with glmfit_multilevel](canlab_mixed_model_example/canlab_mixed_model_example.html) | |

## 9. In progress (advanced)

These tutorials are works in progress and of primary interest to advanced users.

| # | Walkthrough | Live script |
|---|-------------|-------------|
| 9.1 | [Within- and between-subject components of PCR models](mlpcr_demo/mlpcr_demo.html) | |
| 9.2 | [Building ML pipelines with CANlab tools](canlab_pipelines_walkthrough/estimateBestRegionPerformance.html) | |
| 9.3 | [Understanding the CANlab atlases object](using_canlab_atlases/using_canlab_atlases.html) | |
