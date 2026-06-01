# Photometric Stereo Prior Boosted Sparse Multi-View Stereo

[![Conference](https://img.shields.io/badge/ICIP-2026-blue)](#)
[![Code](https://img.shields.io/badge/code-coming%20soon-lightgrey)](#code-status)

Official repository for **Photometric Stereo Prior Boosted Sparse Multi-View Stereo**.

> Code and detailed instructions are coming soon.

## Overview

Sparse multi-view stereo (MVS) often suffers from artifacts when only a limited number of viewpoints are available. This project explores how to boost sparse-view reconstruction with photometric-stereo priors without requiring real multi-illumination capture.

The key idea is to first estimate coarse geometry and reflectance from sparse multi-view images, synthesize virtual multi-illumination images through a relighting module, and then use a pretrained photometric stereo network to infer detail-rich normal priors for geometry refinement.

## Pipeline

![Pipeline](assets/pipeline.png)

The framework contains two main stages:

1. **Sparse-view inverse neural rendering**  
   Estimate coarse surface geometry and material properties, including albedo, roughness, metalness, and normals, from sparse multi-view inputs.

2. **Photometric stereo prior boosting**  
   Generate virtual multi-illumination images, predict surface normals with a frozen photometric stereo backbone, and use the predicted normals as priors to refine the reconstruction.

## Code Status

The implementation is currently being cleaned and will be released soon.

Planned release contents:

- Data preparation scripts
- Multi-illumination rendering module
- Photometric-stereo prior integration
- Training and evaluation scripts
- Example configuration files
- Reproduction instructions for synthetic and real-world experiments

## Repository Structure

```text
icip2026/
├── assets/          # Figures and README resources
├── configs/         # Experiment configuration files, coming soon
├── data/            # Dataset links or preparation notes, coming soon
├── docs/            # Additional documentation, coming soon
├── examples/        # Demo examples, coming soon
├── scripts/         # Utility scripts, coming soon
├── src/             # Source code, coming soon
├── third_party/     # External dependencies or setup notes, coming soon
├── checkpoints/     # Pretrained or released model checkpoints, coming soon
└── outputs/         # Example outputs and visualization results, coming soon
```

## Citation

If you find this work useful, please consider citing our paper. The BibTeX entry will be updated after the official proceedings information is available.

```bibtex
@inproceedings{zhang2026photometric,
  title     = {Photometric Stereo Prior Boosted Sparse Multi-View Stereo},
  author    = {Zhang, Jilong and Yang, Songyun and Han, Yufei and Ma, Zhanyu and Guo, Heng},
  booktitle = {Proceedings of the IEEE International Conference on Image Processing},
  year      = {2026}
}
```

## Acknowledgement

This project builds on sparse-view inverse rendering and photometric stereo research. More details will be provided with the code release.
