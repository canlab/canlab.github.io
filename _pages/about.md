---
permalink: /
title: "CANlab neuroimaging analysis tools"
excerpt: "The CANlab imaging analysis tools consist of a set of linked Github repositories. This site serves as the point of entry for using these tools."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
{% include base_path %}

The CANlab imaging analysis tools consist of a set of linked [Github repositories](/repositories.md). They enable interactive data analysis for fMRI and other types of neuroimaging data using objects with simple methods (or commands) customized for neuroimaging data analysis.  

This page contains examples consisting of walkthroughs, results, and figures that demonstrate what the code can do and how to do it.

Object-oriented features and philosophy:
======

  - Store image data in a flat (2-d), space-efficient voxels x images matrix
  - Save space: Tools to remove out-of-image voxels and empty (zero/NaN) voxels, store data in single-precision format
  - Analysis-friendly: 2-d matrices can be read and analyzed in multiple packages/algorithms
  - Meta-data included to convert back to 3-d image volume space,
    with easy tools (methods) to reconstruct and visualize images
    Built-in resampling makes it easy to compare/combine datasets with different voxel sizes and image bounding boxes
    Reduces overhead for statisticians/data scientists unfamiliar with neuroimaging to apply their algorithms.
  - Multiple images can be stored in a single object
  - Methods have short, intuitive names, and perform high-level functions specialized for neuroimaging:
  - Visualization (plot, orthviews, surface, montage, histogram, isosurface methods)
  - Image manipulation (apply_mask, get_wh_image, resample_space, compare_space, flip, threshold methods)
  - Data extraction (apply_atlas, apply_parcellation, extract_gray_white_csf, extract_roi_averages)
  - Analysis (ica, mahal, image_math, and many more in the fmri_data subclass)
  - Provenance: Ability to track and update history of changes to objects





Examples - UNDER CONSTRUCTION
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

   - First

   - Second

   - Third

```
Testing out code blocks within details dropdowns!
```
</details>


Univariate Contrasts
======
<details>
<summary>Univariate Contrasts Examples</summary>
1. Main list one

   - First
   - Second
   - Third
</details>


Cross Validated SVMs
======
<details>
<summary>Cross Validated SVM Examples</summary>
1. Main list one
   - First
   - Second
   - Third
</details>

Network-Based Analysis
======
<details>
<summary>Network-Based Analysis Examples</summary>
1. Main list one
   - First
   - Second
   - Third
</details>

Brain Signature Responses
======
<details>
<summary>Brain Signature Response Examples</summary>
1. Main list one
   - First
   - Second
   - Third
</details>

Parcel-Based Analysis
======
<details>
<summary>Parcel-Based Examples</summary>
1. Main list one
   - First
   - Second
   - Third
</details>
