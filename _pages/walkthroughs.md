---
permalink: /walkthroughs/
title: "Object-oriented analysis walkthroughs"
excerpt: "Code to run each walkthrough is included in the CANlab core toolbox or on Neurovault."
author_profile: true
# redirect_from:
#  * /objectoriented/
#  * /objectoriented.md
---
{% include base_path %}

This series of walkthroughs is designed to illustrate the CANlab interactive analysis tools, and some analysis principles as well.
Code to run each walkthrough is included in the CANlab core toolbox or on Neurovault. See the main [CANlab intro page](/) for more on the philosophy behind the interactive analysis approach. These walkthroughs are mainly about using CANlab code and are not didactic. There is also another set of [didactic tutorials](/tutorials) using Matlab live scripts with more extensive explanations.

| Getting started             
| ------------       |
| [1.1. Installing tools](canlab_help_1_installing_tools/canlab_help_1_installing_tools.html)
| [1.2. Getting help](canlab_help_1b_getting_help/canlab_help_1b_getting_help.html) <> [Matlab Live Script](canlab_help_1b_getting_help/canlab_help_1b_getting_help.mlx)
| [1.3. Load a sample dataset](canlab_help_2_load_a_sample_dataset/canlab_help_2_load_a_sample_dataset.html)
| [1.4.  basic image visualization](canlab_help_2b_basic_image_visualization/canlab_help_2b_basic_image_visualization.html)
| [1.5.  Loading some datasets used in tutorials](canlab_help_2c_loading_datasets/canlab_help_2c_loading_datasets.html)
| [1.6.  Publishing results reports](canlab_help_2d_publish_a_report/canlab_help_2d_publish_a_report.html)
| [1.7.  Basic Matlab debugging (live script)](/tutorials/matlab/basic_matlab_debugging.mlx)
| [1.8.  Voxel and image spaces in CANlab fmri_data objects](Voxel_and_image_spaces_in_CANlab_fmri_data_objects.html) <> [Matlab live script](Voxel_and_image_spaces_in_CANlab_fmri_data_objects.mlx)

| Basic analyses             
| ------------       |
| [2.1. group t-test](canlab_help_3_voxelwise_t_test_walkthrough/canlab_help_3_voxelwise_t_test_walkthrough.html)
| [2.2. atlases and ROI analysis](canlab_help_3b_atlases_and_ROI_analysis/canlab_help_3b_atlases_and_ROI_analysis.html)
| [2.3. Masking and writing Nifti image files](canlab_help_4_masking_and_writing_nifti_files/canlab_help_4_masking_and_writing_nifti_files.html)
| [2.4. 3-D visualization on brain surfaces](canlab_help_4b_3D_visualization/canlab_help_4b_3D_visualization.html)
| [2.5. Create and explore 1st-level design matrices](first_level_design_matrix_exploration/first_level_design_matrix_exploration.html)
| [2.6. regression, interactive analysis](canlab_help_5_regression_walkthrough/canlab_help_5_regression_walkthrough.html)
| [2.7. Interpreting maps with Neurosynth topic similarity and wedge plots](neurosynth_topic_similarity_and_wedge_plot/neurosynth_topic_similarity_and_wedge_plot.html)
| [2.8. Annotating a results map with transmodal and transcriptomic gradients, neurochemical maps, resting-state networks, and Neurosynth topics](canlab_help_annotate_thresholded_results_map/canlab_help_annotate_thresholded_results_map.html)


| Multivariate predictive models           
| ------------       |
| [3.1. multivariate prediction with continuous outcomes](canlab_help_7_multivariate_prediction_basics/canlab_help_7_multivariate_prediction_basics.html)
| 3.2  Effect sizes with SVMs
| [3.3. Apply a Multivariate Pattern of Interest](canlab_help_9_apply_a_multivariate_pattern_of_interest/canlab_help_9_apply_a_multivariate_pattern_of_interest.html)
| [3.4. Bayes Factor Maps](EmoReg_BayesFactor_walkthrough/EmoReg_BayesFactor_walkthrough.html)
| [3.5. Interpreting maps with riverplots](canlab_help_8_riverplot_cerebellar_atlas_example.m/canlab_help_8_riverplot_cerebellar_atlas_example.html)

| Mediation analysis          
| ------------       |
| [4.1. Mediation and M3 Toolbox basics](tutorials/html/mediation_1_basics.html) | [Download Matlab Live Script](tutorials/matlab/mediation_1_basics.mlx) |  
| [4.2. Single-level Mediation Effect Parametric Mapping (fMRI)](tutorials/html/mediation_brain_single_level_walkthrough1.html) | [Download Matlab Live Script](tutorials/matlab/mediation_brain_single_level_walkthrough1.mlx) |  
| [   additional single-level MEPM output report from publish_mediation_report.m](mediation_brain_sample_report/mediation_brain_results_report.html) |  |
| [4.3. Multilevel Mediation Effect Mapping (fMRI)](tutorials/html/mediation_brain_multilevel_walkthrough1.html) | [Download Matlab Live Script](tutorials/matlab/mediation_brain_multilevel_walkthrough1.mlx) |

| Coordinate-based Meta-analysis          
| ------------       |
| [5.1. MKDA meta-analysis 1](canlab_meta_analysis_walkthrough1.m/canlab_meta_analysis_walkthrough1.html)

| Multivariate Pathway Identification (MPathI) and connectivity       
| ------------       |
| [6.1. Prep time series data for connectivity](tutorials/html/canlab_help_prep_for_connectivity.html) | [Download Matlab Live Script](tutorials/matlab/canlab_help_prep_for_connectivity.mlx) |  
| [6.2. MPathI pathway dissociation](tutorials/html/canlab_help_MPathI_multivariate_pathway.html) | [Download Matlab Live Script](tutorials/matlab/canlab_help_MPathI_multivariate_pathway.mlx) |  


## Other tutorials

[13. more visualization](visualize_neuroimaging_data/visualize_neuroimaging_data.html)

[14. more visualization: surface rendering](canlab_help_surface_projection/mnisurf_projection_tutorial.html)

[15. CANLab single trials demo](canlab_single_trials_demo/demo_norming_comparison.html)

## Behavioral data and Plots

[16. the canlab_dataset object](canlab_dataset_basic_usage/canlab_dataset_basic_usage.html)

[17. time series and bar plots](atlas_2012_behavioral_plot_example_figure/atlas_2012_behavioral_plot_example_figure.html)

[18. mixed effects models in Matlab and CANLab glmfit_multilevel](canlab_mixed_model_example/canlab_mixed_model_example.html)

## Tutorials in progress
Please note that the tutorials which follow are works in progress and of primary interest to advanced users.

[Interpreting within and between subject components of PCR models](mlpcr_demo/mlpcr_demo.html)

[Building and using ML pipelines using Canlab tools](canlab_pipelines_walkthrough/estimateBestRegionPerformance.html)

[Understanding the CANLAb atlases objects](using_canlab_atlases/using_canlab_atlases.html)
