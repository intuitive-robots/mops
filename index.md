---
layout: project_page
permalink: /

title: Multi-Objective Photoreal Simulation (MOPS) Dataset for Computer Vision in Robotic Manipulation
authors:
    Maximilian X. Li, Paul Mattes, Nils Blank, Korbinian F. Rudolf, Paul W. Loedige, Rudolf Lioutikov
affiliations:
    Inutitive Robots Lab, KIT, Germany
paper: /mops/static/li2025mops-preprint.pdf
#video: https://www.youtube.com/results?search_query=turing+machine
#code: https://github.com/topics/turing-machines
#data: https://huggingface.co/docs/datasets
---

![Turing Machine](/static/image/MOPS_rm_fig.png)

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
We introduce the Multi-Object Photoreal Simulation (MOPS) dataset, addressing the lack of computer vision datasets specifically designed for robot manipulation. MOPS provides photorealistic simulated environments with comprehensive ground truth annotations, using a zero-shot asset augmentation pipeline based on large language models. This pipeline annotates 3D assets at the part level and normalizes assets across libraries. The dataset delivers pixel-level segmentation for critical robotics tasks including part segmentation and affordance prediction. By combining detailed annotations with photorealistic simulation, MOPS generates diverse indoor scenes to accelerate progress in robot perception, manipulation, and interaction with real-world environments.
        </div>
    </div>
</div>

---
### Attention
> 🚧 MOPS is currently still under construction and should be treated as an early alpha release 🚧
> 
> Currently, the code is split up into two repos: 
> - `mops-data` for photorealistic image generation in ManiSkill3
> - `mops-casa` for full robot trajectories in RoboCasa

## Code
To Be Released

## Citation
```
@article{li2025mops,
  title={Multi-Objective Photoreal Simulation (MOPS) Dataset for Computer Vision in Robotic Manipulation},
  author={
    Maximilian Xiling Li,
    Paul Mattes,
    Nils Blank,
    Korbinian Franz Rudolf,
    Paul Werker L\"odige,
    Rudolf Lioutikov},
  year={2025}
}
```
