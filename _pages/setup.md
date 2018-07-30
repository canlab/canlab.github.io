---
permalink: /setup/
title: "Initial Setup and Requirements"
author_profile: true
redirect_from:

---
{% include base_path %}

This page walks through Matlab and Github setup and then provides an introduction to CAN Lab object-oriented tools.

Install Matlab
======
You can [install Matlab](https://www.mathworks.com/) from the Mathworks website.

Set up CAN Lab tools from Github
======
There are two options for this step: 1) Download a .zip file with the code, or 2) Install Github on your computer and Clone
the repository (recommended).  With the 2nd option you will get updates, but it requires more steps and some knowledge of how Github works.

First, go to the [Github CANlab tools site](https://github.com/canlab/CanlabCore):
![canlabcore repo view](/docs/images/canlabcore.png)

Using the green "Clone or Download" drop down you can either download a zip file of the repository or clone using git with
a web URL for the repository (these are options 1 and 2 above, respectively).

Walkthrough
======
There is a Matlab script in the [CanlabCore repository](https://github.com/canlab/CanlabCore) that will help download the repositories you need from Github and add them to your Matlab path.  This walkthough shows you how to do it:

[Setup walkthrough](/canlab_help_1_installing_tools.html)


Repositories
======
The CANlab imaging analysis tools consist of a set of linked repositories. Several of these are needed for interactive data analysis using our [object-oriented framework](/objectoriented/), including [CanlabCore](https://github.com/canlab/CanlabCore), [CANlab_help_examples](https://github.com/canlab/CANlab_help_examples), and [Neuroimaging_Pattern_Masks](https://github.com/canlab/Neuroimaging_Pattern_Masks).
Other toolboxes are semi-stand-alone but require [CanlabCore](https://github.com/canlab/CanlabCore).

CANlab Core Tools                             https://github.com/canlab/CanlabCore
CANlab Neuroimaging_Pattern_Masks repository  https://github.com/canlab/Neuroimaging_Pattern_Masks
CANlab_help_examples                          https://github.com/canlab/CANlab_help_examples

M3 Multilevel mediation toolbox               https://github.com/canlab/MediationToolbox
CANlab robust regression toolbox              https://github.com/canlab/RobustToolbox
MKDA coordinate-based meta-analysis toolbox   https://github.com/canlab/Canlab_MKDA_MetaAnalysis

Other CANlab repositories contain code and data for experiments and procedures:

Paradigms_Public - experimental paradigms     https://github.com/canlab/Paradigms_Public
FMRI_simulations - brain movies, effect size/power https://github.com/canlab/FMRI_simulations
CANlab_data_public - Published datasets       https://github.com/canlab/CANlab_data_public
DCC - Martin Lindquist's dynamic correlation toolbox  https://github.com/canlab/Lindquist_Dynamic_Correlation
CanlabScripts - in-lab Matlab/python/bash     https://github.com/canlab/CanlabScripts
