---
permalink: /
title: "CANlab neuroimaging analysis tools"
excerpt: "The CANlab imaging analysis tools consist of a set of linked Github repositories. This site serves as the point of entry for using these tools."
author_profile: true
sidebar:
  - title: "What's new"
    text: |
      A short, hand-maintained log. Full history in the [commit log](https://github.com/canlab/CanlabCore/commits/master).

      - **2026** — Interactive **volume and surface visualization**, including a portable [NiiVue web viewer](/docs/).
      - **2026** — **scikit-learn-style predictive-modeling API** (`predictive_model`) for interactive multivariate prediction.
      - **2026** — New **`glm_map`** object and interactive API for first- and second-level GLM analysis.
      - **2026** — **CIFTI-style surface objects** (`fmri_surface_data`) — native CIFTI/GIFTI, no external toolbox.
      - **2026** — **Unit tests** now run on every push and nightly.
      - **2026** — **Updated documentation**: new [Docs page](/docs/) with object references, workflows, and visualization guides.
#redirect_from:
#  * /about/
#  * /about.html
---
{% include base_path %}

The CANlab imaging analysis tools are a set of linked [Github repositories](#repositories) that enable **interactive** analysis of fMRI and other neuroimaging data using objects with simple methods (commands) customized for neuroimaging. Take preprocessed data or single-subject results, load them into lightweight data objects, and explore with commands like `plot`, `predict`, `montage`, and `surface`.

> **New here?** Start with the [Setup page]({{ "/setup/" | relative_url }}) and the [Quick-start walkthrough]({{ "/_pages/canlab_help_1_installing_tools/canlab_help_1_installing_tools.html" | relative_url }}). Looking for something specific? Try the [search page]({{ "/search/" | relative_url }}).

## Interactive brain viewer

Results objects render to a portable, self-contained web viewer with one command — `canlab_niivue(t)`. Try it below: switch **layouts**, recolor with the **Colormap** menu, outline the region at the crosshair with **Atlas region**, raise the **Threshold**, fade layers, and click to move the crosshair (its MNI coordinate, value, and atlas region print below the image).

<iframe src="{{ "/assets/niivue/emotionreg_ttest.html" | relative_url }}"
        width="100%" height="520"
        style="border:1px solid #d4d8dd; border-radius:6px;"
        loading="lazy"
        title="Interactive CANlab NiiVue brain viewer — emotionreg t-test"></iframe>

*One-sample t-test on the CANlab `emotionreg` sample dataset (p &lt; .005 uncorrected, k ≥ 10), warm/cool blobs over a 2&nbsp;mm MNI underlay. If the frame is blank, [open the demo directly]({{ "/assets/niivue/emotionreg_ttest.html" | relative_url }}). See the [NiiVue viewer guide](https://github.com/canlab/CanlabCore/blob/master/docs/canlab_niivue_guide.md).*

## Repositories

The tools are distributed across linked GitHub repositories. **`CanlabCore` and `Neuroimaging_Pattern_Masks` are the foundation and are meant to be used together** — the core object-oriented code plus the masks, signature patterns, and meta-analysis maps it operates on.

| Core repository | Description |
| --- | --- |
| [**CanlabCore**](https://github.com/canlab/CanlabCore) | Object-oriented fMRI analysis tools used across all other toolboxes |
| [**Neuroimaging_Pattern_Masks**](https://github.com/canlab/Neuroimaging_Pattern_Masks) | Masks, predictive signature patterns, atlases, and meta-analysis maps |

Additional toolboxes are semi-stand-alone but require `CanlabCore`:

| Toolbox | Description |
| --- | --- |
| [M3 Multilevel Mediation Toolbox](https://github.com/canlab/MediationToolbox) | Single- and multi-level mediation for any data type, including brain images |
| [CANlab Robust Regression Toolbox](https://github.com/canlab/RobustToolbox) | Robust regression for 2nd-level (group) analysis |
| [MKDA Coordinate-Based Meta-Analysis Toolbox](https://github.com/canlab/Canlab_MKDA_MetaAnalysis) | Coordinate-based meta-analysis and multivariate tools |
| [CANlab_help_examples](https://github.com/canlab/CANlab_help_examples) | Walkthroughs and the 2nd-level batch-script system |

Other CANlab repositories contain code and data for experiments and procedures:

| Repository | Description |
| --- | --- |
| [Paradigms_Public](https://github.com/canlab/Paradigms_Public) | Experimental paradigms |
| [FMRI_simulations](https://github.com/canlab/FMRI_simulations) | Brain movies, effect-size and power analyses |
| [CANlab_data_public](https://github.com/canlab/CANlab_data_public) | Published datasets |
| [DCC](https://github.com/canlab/Lindquist_Dynamic_Correlation) | Martin Lindquist's dynamic correlation toolbox |
| [CanlabScripts](https://github.com/canlab/CanlabScripts) | In-lab Matlab / Python / bash utilities |

## Why interactive analysis?

Much of neuroimaging has moved toward standardized pipelines — an essential foundation. But discovery also requires *exploring* data: visualizing it in many ways, understanding its quirks and outliers, and adapting analyses to the question at hand. The CANlab toolboxes were built for this. They provide a high-level language for neuroimaging data, so complex operations become single, readable commands. Some values we aspire to:

* **Interactivity & transparency** — cross-validated multivariate prediction, surface/slice rendering, and results tables are each one command. A basic group analysis, including publication-quality figures and tables, takes about five lines of readable code.
* **Reproducibility & fewer errors** — simple, shared commands are easy to reproduce, and core object code is re-used and vetted across analyses and users. Executable walkthroughs and unit tests check that core functions still produce expected results.
* **Efficiency** — a batch system runs standard QC and analyses and saves date-stamped HTML reports with figures and statistics, good for archiving, sharing, and writing papers.
* **Extensibility** — the object framework is extensible: images are stored in a flat, space-efficient `voxels × images` matrix familiar to data scientists, and core code handles rendering results back into brain space with anatomical labeling.

For the full rationale — the object model, storage design, and how new methods plug in — see the [**Interactive fMRI analysis page**](/objectoriented/).

## Core objects

Interactive analysis is organized around a small set of objects with simple, high-level methods. Click a class for its full documentation.

| Object | Description |
| --- | --- |
| [`fmri_data`](https://github.com/canlab/CanlabCore/blob/master/docs/fmri_data_methods.md) | The workhorse: holds images plus metadata; most analysis methods (`predict`, `regress`, `ica`, `ttest`) live here |
| [`statistic_image`](https://github.com/canlab/CanlabCore/blob/master/docs/statistic_image_methods.md) | Statistic maps (t / p / effect size) with thresholding state |
| [`atlas`](https://github.com/canlab/CanlabCore/blob/master/docs/atlas_methods.md) | Brain atlases / parcellations with labels and probability maps |
| [`region`](https://github.com/canlab/CanlabCore/blob/master/docs/region_methods.md) | Data grouped by contiguous cluster / ROI as a unit of analysis |
| [`fmri_surface_data`](https://github.com/canlab/CanlabCore/blob/master/docs/fmri_surface_data_methods.md) | *New.* CIFTI-style cortical-surface / grayordinate data — native CIFTI/GIFTI, no external toolbox |
| [`fmridisplay`](https://github.com/canlab/CanlabCore/blob/master/docs/fmridisplay_methods.md) | Container for slice/surface figure handles, for layered visualization |
| [`glm_map`](https://github.com/canlab/CanlabCore/blob/master/docs/glm_map_methods.md) | *New.* scikit-learn-style estimator for first- and second-level GLM / regression |
| [`predictive_model`](https://github.com/canlab/CanlabCore/blob/master/docs/predictive_model_methods.md) | *New.* A fitted multivariate prediction model and its artifacts |

See the [Object methods index](https://github.com/canlab/CanlabCore/blob/master/docs/Object_methods.md) for the complete class list, and the [**Docs page**](/docs/) for all references, workflows, and visualization guides.

## Learn more

- [**Interactive fMRI analysis**](/objectoriented/) — the philosophy, object model, and a simple analysis flow.
- [**Docs**](/docs/) — object references, workflows, visualization guides, walkthroughs, and tutorials.
- [**Walkthroughs**](/walkthroughs/) — step-by-step, runnable analyses.
- [**Setup**](/setup/) — install the toolboxes and dependencies.

## Issues and bugs

Please raise issues or document errors on the [CANlab Github page](https://github.com/canlab/CanlabCore/issues).
