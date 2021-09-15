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

* Matlab's comprehensive built-in examples (type "doc" within Matlab)
* Function help (type "help my_fun", where my_fun is the name of a function)
* [Matlab Academy](https://matlabacademy.mathworks.com/) (free!), including the "Matlab Onramp" module and others)
* Other great resources, e.g., Michael X. Cohen's [YouTube lectures](https://www.youtube.com/channel/UCUR_LsXk7IYyueSnXcNextQ) and [Matlab book](https://mitpress.mit.edu/books/matlab-brain-and-cognitive-scientists), Kendrick Kay's [Matlab-based stats course](https://www.cmrr.umn.edu/~kendrick/statsmatlab/)   

These are didactic tutorials using Matlab live scripts. There is also a complementary set of [code walkthroughs](/walkthroughs) on using the CANlab object-oriented tools, with some overlap but unique information and code examples.

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
| [2.5. Nuisance Covariates](tutorials/html/nuisance_covariates.html) | [Download Matlab Live Script](tutorials/matlab/nuisance_covariates.mlx) |

| First-level models with whole-brain data               
| ------------       |
| [3.1. Setting SPM defaults](tutorials/html/setting_SPM_defaults.html) | [Download Matlab Live Script](tutorials/matlab/setting_SPM_defaults.mlx) |
| Get the Pinel localizer dataset used [here](https://dartbrains.org/content/Download_Data.html) or on Dropbox [here (Neurospin version)(https://www.dropbox.com/sh/fmw6gy7dzhzcnh5/AAA3OsHvRXUKUKCyl18SCxpQa?dl=0) or [here (BIDS)(https://www.dropbox.com/sh/wly58x4r0bqneb2/AADeE6AVHGcJMrClqHzX9GMFa?dl=0)|  |
| [3.2. Preprocessing basics using SPM](tutorials/html/preproc_basics_spm12.html) | [Download Matlab Live Script](tutorials/matlab/preproc_basics_spm12.mlx) |
| [3.3. First-level model using the SPM GUI](tutorials/html/first_level_spm12.html) | [Download Matlab Live Script](tutorials/matlab/first_level_spm12.mlx) |
| [3.4. First-level model using CANlab regress()](tutorials/html/first_level_canlab.html) | [Download Matlab Live Script](tutorials/matlab/first_level_canlab.mlx) |

| Second-level models with CANlab tools            
| ------------       |
| See [walkthroughs](/walkthroughs) |

| Multivariate predictive models           
| ------------       |
| Datasets | (On Dropbox; See also links in tutorials)   |
| [Kragel270 fmri_data object](https://www.dropbox.com/s/k8zxio26cfx0uv3/kragel_2018_nat_neurosci_270_subjects_test_images.mat?dl=0) | [Paper](https://www.nature.com/articles/s41593-017-0051-7) |
| [BMRK3 pain dataset fmri_data object](https://www.dropbox.com/s/i7wnvzph4n1wdwt/bmrk3_6levels_pain_dataset.mat?dl=0) | [Paper](https://www.nejm.org/doi/full/10.1056/nejmoa1204471) |
| [Rejection vs Pain dataset](https://www.dropbox.com/sh/zryqei5o7j1e2gj/AAAj4XDhwCuSI25QC94w4LT0a?dl=0) | [Paper](https://www.nature.com/articles/ncomms6380?origin=ppub) and [this](https://www.pnas.org/content/108/15/6270.short) |
| | |
| [3.1. SVM on unpaired data using predict()](tutorials/html/canlab_SVM_on_unpaired_data_Kragel270.html) | [Download Matlab Live Script](tutorials/matlab/canlab_SVM_on_unpaired_data_Kragel270.mlx) |
| [3.2. multivariate prediction with continuous outcomes](canlab_help_7_multivariate_prediction_basics/canlab_help_7_multivariate_prediction_basics.html)

## Other tutorials

[CANlab code walkthroughs](/walkthroughs)
