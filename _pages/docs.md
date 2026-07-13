---
permalink: /docs/
title: "Documentation"
excerpt: "A complete index of CANlab documentation: object references, workflows, visualization guides, walkthroughs, and tutorials."
author_profile: false
toc: true
toc_label: "On this page"
toc_sticky: true
---
{% include base_path %}

{% assign docs = "https://github.com/canlab/CanlabCore/blob/master/docs" %}
{% assign surf = "https://github.com/canlab/CanlabCore/blob/master/docs" %}

This page indexes the documentation for the CANlab tools: reference docs in the [CanlabCore repository]({{ docs }}/Object_methods.md), the runnable [walkthroughs](/walkthroughs/) and [tutorials](/tutorials/) on this site, and the [Interactive fMRI](/objectoriented/) overview. Reference docs are Markdown files rendered on GitHub; walkthroughs and tutorials are on this site.

**Start here:** [Interactive fMRI analysis](/objectoriented/) for the philosophy and object model, the [Object methods index]({{ docs }}/Object_methods.md) for the class-by-class reference, or the [Quick-start walkthrough](/_pages/canlab_help_1_installing_tools/canlab_help_1_installing_tools.html) to install and run.

## Object references

Per-class references — properties, methods grouped by category, and worked examples. See the [Object methods index]({{ docs }}/Object_methods.md) for the class hierarchy and overview.

| Class | What it holds |
| --- | --- |
| [`fmri_data`]({{ docs }}/fmri_data_methods.md) | The workhorse image object; most analysis methods live here |
| [`image_vector`]({{ docs }}/image_vector_methods.md) | Abstract base; source of shared methods |
| [`statistic_image`]({{ docs }}/statistic_image_methods.md) | Statistic maps (t / p / effect size) with thresholding |
| [`atlas`]({{ docs }}/atlas_methods.md) | Atlases / parcellations with labels and probability maps |
| [`fmri_surface_data`]({{ surf }}/fmri_surface_data_methods.md) | *New.* CIFTI-style surface / grayordinate data |
| [`region`]({{ docs }}/region_methods.md) | Contiguous clusters / ROIs as a unit of analysis |
| [`fmridisplay`]({{ docs }}/fmridisplay_methods.md) | Figure-handle container for layered brain montages |
| [`glm_map`]({{ docs }}/glm_map_methods.md) | *New.* First- and second-level GLM / regression estimator |
| [`fmri_glm_design_matrix`]({{ docs }}/fmri_glm_design_matrix_methods.md) | First-level GLM design matrix (onsets, basis set, X) |
| [`predictive_model`]({{ docs }}/predictive_model_methods.md) | *New.* Fitted multivariate prediction model and artifacts |
| [`canlab_dataset`]({{ docs }}/canlab_dataset_methods.md) | Subject × variable behavioral / clinical data |
| [`brainpathway`]({{ docs }}/brainpathway_methods.md) | Connectivity / pathway model (single- & multi-subject) |
| [`fmri_timeseries`]({{ docs }}/fmri_timeseries_methods.md) | Raw timeseries container |
| [`fmri_mask_image`]({{ docs }}/fmri_mask_image_methods.md) | Binary mask (legacy) |

## Workflows

End-to-end recipes that chain several methods together. Each comes as a **roadmap** (choose the right approach) and a **how-to** (runnable code). See the [Workflows overview]({{ docs }}/Workflows.md).

| Workflow | Roadmap | How-to |
| --- | --- | --- |
| ROI / atlas data extraction | [roadmap]({{ docs }}/workflows/ROI_extraction_methods_roadmap.md) | [how-to]({{ docs }}/workflows/extract_roi_data_howto.md) |
| First-level fMRI GLM (`glm_map`) | [roadmap]({{ docs }}/workflows/glm_map_first_level_roadmap.md) | [how-to]({{ docs }}/workflows/glm_map_first_level_howto.md) |
| Second-level group GLM (`glm_map`) | [roadmap]({{ docs }}/workflows/glm_map_second_level_roadmap.md) | [how-to]({{ docs }}/workflows/glm_map_second_level_howto.md) |
| Surface & grayordinate data | [`fmri_surface_data`]({{ surf }}/fmri_surface_data_methods.md) | [how-to]({{ surf }}/workflows/fmri_surface_data_howto.md) |
| Loading & using image sets | — | [how-to]({{ surf }}/workflows/load_image_set_howto.md) |

## Visualization

A multi-page guide to rendering images and results — montages, 3-D surfaces, colormaps, the interactive controller, and atlases/regions.

- [Visualization walkthrough — index]({{ docs }}/visualization_walkthrough/index.md)
  - [Getting started]({{ docs }}/visualization_walkthrough/01_getting_started.md)
  - [Montages]({{ docs }}/visualization_walkthrough/02_montages.md)
  - [Surfaces]({{ docs }}/visualization_walkthrough/03_surfaces.md)
  - [Colormaps]({{ docs }}/visualization_walkthrough/04_colormaps.md)
  - [Interactive controller]({{ docs }}/visualization_walkthrough/05_controller.md)
  - [Atlases and regions]({{ docs }}/visualization_walkthrough/06_atlases_and_regions.md)
- [`canlab_niivue` — portable interactive web viewer]({{ docs }}/canlab_niivue_guide.md) ([live demo](/#interactive-brain-viewer))

## Concepts & reference

- [Atlases, regions, and patterns]({{ docs }}/atlases_regions_and_patterns.md) — how atlases, region objects, and signature patterns relate.
- [Recasting objects]({{ docs }}/recasting_objects.md) — converting between object types.
- [Sample datasets]({{ docs }}/sample_datasets.md) — built-in datasets and how to load them (`load_image_set`).
- [Toolbox folders]({{ docs }}/toolbox_folders.md) — how CanlabCore is organized.

## Long-form tutorials

Multi-part didactic tutorials with runnable code.

- **Multivariate classification & decoding with SVM**
  - [Part 1 — classification with SVM]({{ docs }}/markdown_tutorials/multivariate_classification_with_SVM/multivariate_decoding_part1_classification_with_SVM.md)
  - [Part 2 — classification and regression]({{ docs }}/markdown_tutorials/multivariate_classification_with_SVM/multivariate_decoding_part2_classification_and_regression.md)
  - [Part 3 — the `predictive_model` API]({{ docs }}/markdown_tutorials/multivariate_classification_with_SVM/multivariate_decoding_part3_predictive_model_api.md)
  - [Part 4 — cross-classification]({{ docs }}/markdown_tutorials/multivariate_classification_with_SVM/multivariate_decoding_part4_cross_classification.md)
  - [Part 5 — algorithms and tuning]({{ docs }}/markdown_tutorials/multivariate_classification_with_SVM/multivariate_decoding_part5_algorithms_and_tuning.md)

## Walkthroughs & tutorials on this site

- [**Walkthroughs**](/walkthroughs/) — step-by-step, runnable analyses (installing tools, group stats, ROI analysis, prediction, mediation, meta-analysis, visualization).
- [**fMRI tutorials**](/tutorials/) — longer-form didactic tutorials using MATLAB live scripts.
- [**Batch system**](/batch/) — the second-level analysis batch-script system.
- [**Interactive fMRI analysis**](/objectoriented/) — philosophy, object model, and a simple analysis flow.

## Help and issues

- In MATLAB, `doc <class_name>` (e.g. `doc fmri_data`) or `methods <class_name>` lists a class's properties and methods.
- Report bugs or documentation errors on the [CanlabCore issues page](https://github.com/canlab/CanlabCore/issues).
