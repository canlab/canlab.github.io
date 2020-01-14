---
permalink: /setup/
title: "Initial Setup and Requirements"
author_profile: true
redirect_from:

---
{% include base_path %}

This page walks through Matlab and Github setup and then provides an introduction to CAN Lab object-oriented tools.
Here is a [Quick start walkthrough for the CANlab tools](/canlab_help_1_installing_tools/canlab_help_1_installing_tools.html).

## Install Matlab

You can install Matlab from the [Mathworks website](https://www.mathworks.com/). Free trial versions are available. You will need two toolboxes: The statistics and machine learning toolbox and the signal processing toolbox.  

## Install Statistical Parametric Mapping (SPM)

Our toolboxes use SPM's image reading and writing functions, and the spm_orthviews viewer. SPM is a [free download from their site](https://www.fil.ion.ucl.ac.uk/spm/)

## Install git and Github

We recommend that you use version control, particularly Github. Then you can Clone repositories and download changes with one click, and you can contribute by flagging issues or modifying/extending the code and creating Pull Requests to add to the core tools. The simplest starting point is to first [install git on your computer](https://git-scm.com/). Then [install Github Desktop](https://help.github.com/en/desktop/getting-started-with-github-desktop/installing-github-desktop). If you are new to Git, check out [this intro tutorial](https://guides.github.com/activities/hello-world/). As you start to want to use it to manage projects and contribute, see [this flowchart](https://guides.github.com/introduction/flow/) and learn about the [Git command line interface](https://dev.to/dhruv/essential-git-commands-every-developer-should-know-2fl). This is optional here, but we suggest git and Github Desktop.

## Install CANlab core tools from Github

There are two options for this step: 1) Download a .zip file with the code, or 2) Install Github on your computer and Clone
the repository (recommended).  With the 2nd option you will get updates (see above). It requires a bit more setup time, but it's well worth it!

First, go to the [Github CANlab tools site](https://github.com/canlab/CanlabCore):
![canlabcore repo view](/images/canlabcore.png)

Using the green "Clone or Download" drop down you can either download a zip file of the repository or clone using git with
a web URL for the repository (these are options 1 and 2 above, respectively). You can download other repositories this way, or use the quick-start walkthrough below.

## Quick-start Walkthrough

There is a Matlab script in the [CanlabCore repository](https://github.com/canlab/CanlabCore) that will help download the repositories you need from Github and add them to your Matlab path.  This walkthough shows you how to do it:

[Setup walkthrough](/canlab_help_1_installing_tools/canlab_help_1_installing_tools.html)

## Repositories

The CANlab imaging analysis tools consist of a set of linked repositories.
Links and descriptions are on the [repositories page](/repositories.md)
