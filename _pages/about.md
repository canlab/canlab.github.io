---
permalink: /
title: "CANlab neuroimaging analysis tools"
excerpt: "The CANlab imaging analysis tools consist of a set of linked Github repositories. This site serves as the point of entry for using these tools."
author_profile: true
#redirect_from:
#  * /about/
#  * /about.html
---
{% include base_path %}

The CANlab imaging analysis tools consist of a set of linked [Github repositories](/repositories.md).

They enable interactive data analysis for fMRI and other types of neuroimaging data using objects with simple methods (or commands) customized for neuroimaging data analysis.  

## Interactive analysis: Philosophy and principles

Much of neuroimaging analysis, like other areas of science, has moved towards pipelines: Standardized processing streams that produce reliable results with optimized procedures. This is an essential part of any technology, and an important effort. At same time, however, there is a need for creativity and exploration of data and techniques in order to discover new ways of doing things. And there is a need to understand data — its characteristics, its quirks and outliers, and its behavior under different conditions — in order to avoid spurious results and understand what is true. Exploration and discovery require the ability to visualize data in a variety of ways, interact with it, and create analyses that fit the questions at hand.  

There are many established pipelines for neuroimaging analysis, but relatively few tools that provide flexibility and the ability to interact with data. The CANlab toolboxes were designed with interactive analysis in mind.  The tools provide a high-level language for interacting with neuroimaging data. The idea is to take preprocessed data or even the results of single-subject analyses—the output of established preprocessing pipelines—and import them into lightweight, flexible data objects specialized for neuroimaging visualization and analysis.  These objects allow for interactive analysis with simple commands, like “plot”, “predict”, and “montage”.  

There are several advantages to this type of framework. We’re not saying the code is perfect — it’s necessarily a work in progress — but here are some of the values we aspire to:

* **Interactivity:** Complex operations can be done with simple commands. For example, single commands perform (a) stratified, cross validated multivariate prediction (b) rendering imaging results on brain slices or surfaces, and many other functions. This operations can thus be done interactively, allowing analysts to explore the distribution of data and the consequences of altering analysis choices.

* **Transparency:** Scripts that use these commands become simple to read, write, and interpret, increasing transparency and reducing coding errors. A basic group fMRI analysis, including generating publication-quality figures and tables of results, can be performed in only a few (about 5) lines of code.

Organization of the toolbox around a few core objects makes it easier to discover what they can do (their methods). A series of executable walkthroughs—and HTML reports with expected output—demonstrate some of the core functionality.

* **Reproducibility:** The use of simple, transparent commands makes it easy to share the code needed to reproduce an analysis in a format that others can understand and use.

* **Minimization of errors:** Core object functions are re-used and vetted across analyses and users, reducing coding errors. The walkthroughs serve as a basic unit test for many core functions, providing a test that analyses are running and producing expected results whatever platform and software versions are being used.  (A full unit test would be desirable, and is planned.)

* **Efficiency:** A batch system built on simple object commands runs a variety of standard quality control checks and analyses, and saves date-stamped HTML reports with figures and statistics. This provides a base set of analyses that reduces coding time and reduces coding errors. This is good for archiving and reproducibility, and good for efficiently writing papers.

* **Shareability:** The data objects are designed to be space efficient, and store imaging data in a fraction of the disk space it takes to store full images.

In the batch system, standardized variable names make it easy to understand the structure of the folders and files, which promotes meaningful sharing. Date-stamped HTML reports provide a record of analyses, figures and statistics that can be archived and shared.

* **Extensibility:** The object-oriented framework is extensible, allowing developers and data scientists to add new methods or object types.

New analytic techniques can be easily “plugged in”. The objects store images in a flat 2-D matrix (voxels x images) that is very familiar to data scientists from all fields, and can be subjected to custom analyses. Core object code handles the rendering of these results back into brain space, including visualization and anatomical labeling. This makes neuroimaging accessible to a variety of data scientists developing sophisticated new analyses.

## Walkthroughs and batch scripts

A series of step-by-step analysis walkthroughs are in the [CANlab_help_examples repository](https://github.com/canlab/CANlab_help_examples), in the `example_help_files` folder.

These are executable Matlab files (.m files) that can be run. They can also be published to HTML files (see canlab_help_publish.m). A set of HTML files with figures and printouts of these help examples is in the `published_html` folder.

A system of batch scripts is in the [CANlab_help_examples repository](https://github.com/canlab/CANlab_help_examples), in the `Second_level_analysis_template_scripts` folder.


## types of objects

| Object            | Description                                                                 |
| --------          | --------------------------------------------------------------------------- |
| fmri_data         | Stores neuroimaging datasets; operate on datasets by calling object methods |
| statistic_image   | Stores statistic images with stats and P-values                             |
| atlas             | Stores atlas data with probability maps and integers for unique regions     |
| region            | Stores data grouped by region/network, treating region as a unit of analysis|
| fmridisplay       | Container for handles for brain slices and surfaces, allowing visualization |


## fmri_data object features and philosophy

  * **Flat format:** Store image data in a flat (2-d), space-efficient voxels x images matrix
  * **Save space:** Tools to remove out-of-image voxels and empty (zero/NaN) voxels, store data in single-precision format
  * **Analysis-friendly:** 2-d matrices can be read and analyzed in multiple packages/algorithms
  * Meta-data included to convert back to 3-d image volume space,
    with easy tools (methods) to reconstruct and visualize images
    Built-in resampling makes it easy to compare/combine datasets with different voxel sizes and image bounding boxes. Reduces overhead for statisticians/data scientists unfamiliar with neuroimaging to apply their algorithms.
  * Multiple images can be stored in a single object
  * Methods have short, intuitive names, and perform high-level functions specialized for neuroimaging. e.g., some example methods are:
  * **Visualization** (plot, orthviews, surface, montage, histogram, isosurface methods)
  * **Image manipulation** (apply_mask, get_wh_image, resample_space, compare_space, flip, threshold methods)
  * **Data extraction** (apply_atlas, apply_parcellation, extract_gray_white_csf, extract_roi_averages)
  * **Analysis** (ica, mahal, image_math, and many more in the fmri_data subclass)
  * **Provenance:** Ability to track and update history of changes to objects
  * **Documentation:** In Matlab, type `doc object_class` name (e.g., `doc fmri_data`) for properties, methods, and examples.  





## Examples * UNDER CONSTRUCTION
======

These examples require the [CAN Lab Core Tools Repository](https://github.com/canlab/CanlabCore).
Running the examples in your own environment also serves as a preliminary unit test frame for the CAN Lab tools.

Please document errors by posting issues on the [CAN Lab Github page](https://github.com/canlab/CanlabScripts/issues).

For information on software requirements and getting set up to run second-level scripts see our [Setup and System Requirements](/setup.md) page.

For a tutorial on how to use CAN LAb scripts to create a second-level analysis pipeline dealing with groups of subjects, please see our [Second-Level
Analysis Tutorial](/second_level.md)



Data Quality Control
======
<details>
<summary>Data Quality Control Examples</summary>

1. Main list one

   * First

   * Second

   * Third

```
Testing out code blocks within details dropdowns!
```
</details>


Univariate Contrasts
======
<details>
<summary>Univariate Contrasts Examples</summary>
1. Main list one

   * First
   * Second
   * Third
</details>


Cross Validated SVMs
======
<details>
<summary>Cross Validated SVM Examples</summary>
1. Main list one
   * First
   * Second
   * Third
</details>

Network-Based Analysis
======
<details>
<summary>Network-Based Analysis Examples</summary>
1. Main list one
   * First
   * Second
   * Third
</details>

Brain Signature Responses
======
<details>
<summary>Brain Signature Response Examples</summary>
1. Main list one
   * First
   * Second
   * Third
</details>

Parcel-Based Analysis
======
<details>
<summary>Parcel-Based Examples</summary>
1. Main list one
   * First
   * Second
   * Third
</details>
