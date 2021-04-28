---
permalink: /tutorials/
title: "fMRI tutorials with Matlab Live Scripts"
excerpt: "Code to run each walkthrough is included in the CANlab Core toolbox, and datasets are included or downloaded from Neurovault."
author_profile: true
# redirect_from:
#  * /objectoriented/
#  * /objectoriented.md
---
{% include base_path %}

This series of walkthroughs is designed to illustrate the principles of fMRI acquisition, design, and analysis. They use the CANlab Core interactive analysis tools.
Code to run each walkthrough is included in the CANlab Core toolbox, and datasets are included or downloaded from Neurovault. See the main [CANlab intro page](/) for more on the philosophy behind the interactive analysis approach.

This is *not* a comprehensive introduction to Matlab. It's assumed that you will use other resources to supplement your basic understanding how to work with Matlab, including:

| Matlab's comprehensive built-in examples (type "doc" within Matlab)
| Function help (type "help my_fun", where my_fun is the name of a function)
| [Matlab Academy](https://matlabacademy.mathworks.com/) (free!), including the "Matlab Onramp" module and others)
| Other great resources, e.g., Michael X. Cohen's [YouTube lectures](https://www.youtube.com/channel/UCUR_LsXk7IYyueSnXcNextQ) and [Matlab book](https://mitpress.mit.edu/books/matlab-brain-and-cognitive-scientists)   

| Basic signal processing             
| ------------       |
| [1.1. T1 decay and basic Matlab orientation](tutorials/html/Lab1_T1_decay_and_basic_matlab.html) | [Download Matlab Live Script](tutorials/matlab/Lab1_T1_decay_and_basic_matlab.mlx) |  
| [1.2. Sine waves and the Fourier Transform](canlab_help_2_load_a_sample_dataset/sin_cos_fft.html) | [Download Matlab Live Script](tutorials/matlab/sin_cos_fft.mlx) |

| The General Linear Model and fMRI designs             
| ------------       |
| [2.1. fMRI Design Matrices and inference](tutorials/html/Construction_and_inference_with_simple_design.html) | [Download Matlab Live Script](tutorials/matlab/Construction_and_inference_with_simple_design.mlx) |
| [2.2. fMRI Design Matrices: Multiple regressors](tutorials/html/Design_construction_multiple_regressors.html) | [Download Matlab Live Script](tutorials/matlab/Design_construction_multiple_regressors.mlx) |
| [2.3. Efficiency, colinearity, and variance inflation](tutorials/html/Efficiency_colinearity_and_variance_inflation.html) | [Download Matlab Live Script](tutorials/matlab/Efficiency_colinearity_and_variance_inflation.mlx) |
| [2.4. High-pass Filtering](tutorials/html/high_pass_filtering.html) | [Download Matlab Live Script](tutorials/matlab/high_pass_filtering.mlx) |

| First-level models with SPM               
| ------------       |
| [3.1. Setting SPM defaults](tutorials/html/***.html) | [Download Matlab Live Script](tutorials/matlab/***.mlx) |
| [3.2. The Pinel localizer dataset](tutorials/html/***.html) | [Download Matlab Live Script](tutorials/matlab/***.mlx) |
| [3.3. First-level model using the SPM GUI](tutorials/html/***.html) | [Download Matlab Live Script](tutorials/matlab/***.mlx) |
| [3.4. First-level model using CANlab tools](tutorials/html/***.html) | [Download Matlab Live Script](tutorials/matlab/***.mlx) |

| Second-level models with CANlab tools            
| ------------       |
| [2.1. group t-test](canlab_help_3_voxelwise_t_test_walkthrough/canlab_help_3_voxelwise_t_test_walkthrough.html)
| [2.2. atlases and ROI analysis](canlab_help_3b_atlases_and_ROI_analysis/canlab_help_3b_atlases_and_ROI_analysis.html)
| [2.3. Masking and writing Nifti image files](canlab_help_4_masking_and_writing_nifti_files/canlab_help_4_masking_and_writing_nifti_files.html)
| [2.4. 3-D visualization on brain surfaces](canlab_help_4b_3D_visualization/canlab_help_4b_3D_visualization.html)
| [2.5. Create and explore 1st-level design matrices](first_level_design_matrix_exploration/first_level_design_matrix_exploration.html)
| [2.6. regression, interactive analysis](canlab_help_5_regression_walkthrough/canlab_help_5_regression_walkthrough.html)
| [2.7. Interpreting maps with Neurosynth topic similarity and wedge plots](neurosynth_topic_similarity_and_wedge_plot/neurosynth_topic_similarity_and_wedge_plot.html)

| Multivariate predictive models           
| ------------       |
| [3.1. multivariate prediction with continuous outcomes](canlab_help_7_multivariate_prediction_basics/canlab_help_7_multivariate_prediction_basics.html)
| 3.2  Effect sizes with SVMs
| [3.3. Apply a Multivariate Pattern of Interest](canlab_help_9_apply_a_multivariate_pattern_of_interest/canlab_help_9_apply_a_multivariate_pattern_of_interest.html)
| [3.4. Bayes Factor Maps](EmoReg_BayesFactor_walkthrough/EmoReg_BayesFactor_walkthrough.html)
| [3.5. Interpreting maps with riverplots](canlab_help_8_riverplot_cerebellar_atlas_example.m/canlab_help_8_riverplot_cerebellar_atlas_example.html)

| Mediation analysis          
| ------------       |
| [4.1. mediation analysis](mediation_example_script_1/mediation_example_script_1.html)
| [4.2. additional output report from publish_mediation_report.m](mediation_brain_sample_report/mediation_brain_results_report.html)

| Coordinate-based Meta-analysis          
| ------------       |
| [5.1. MKDA meta-analysis 1](canlab_meta_analysis_walkthrough1.m/canlab_meta_analysis_walkthrough1.html)

## Other tutorials

[13. more visualization](visualize_neuroimaging_data/visualize_neuroimaging_data.html)

[14. CANLab single trials demo](canlab_single_trials_demo/demo_norming_comparison.html)

## Behavioral data and Plots

[15. the canlab_dataset object](canlab_dataset_basic_usage/canlab_dataset_basic_usage.html)

[16. time series and bar plots](atlas_2012_behavioral_plot_example_figure/atlas_2012_behavioral_plot_example_figure.html)

[17. mixed effects models in Matlab and CANLab glmfit_multilevel](canlab_mixed_model_example/canlab_mixed_model_example.html)

## Tutorials in progress
Please note that the tutorials which follow are works in progress and of primary interest to advanced users.

[Interpreting within and between subject components of PCR models](mlpcr_demo/mlpcr_demo.html)
