---
layout: project_page
permalink: /

title: Multi-Objective Photoreal Simulation (MOPS) Dataset for Computer Vision in Robotic Manipulation
authors:
    Maximilian X. Li, Paul Mattes, Nils Blank, Korbinian F. Rudolf, Paul W. Loedige, Rudolf Lioutikov
affiliations:
    Intuitive Robots Lab, KIT, Germany
paper: ./static/li2025mops-preprint.pdf
code: https://github.com/LiXiling/mops-data
#video: https://www.youtube.com/results?search_query=turing+machine
#data: https://huggingface.co/docs/datasets
---

![MOPS Dataset Overview](/static/image/MOPS_rm_fig.png)

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
            We introduce the <strong>Multi-Object Photoreal Simulation (MOPS) dataset</strong>, addressing the lack of computer vision datasets specifically designed for robot manipulation. MOPS provides photorealistic simulated environments with comprehensive ground truth annotations, using a zero-shot asset augmentation pipeline based on large language models. This pipeline annotates 3D assets at the part level and normalizes assets across libraries. The dataset delivers pixel-level segmentation for critical robotics tasks including part segmentation and affordance prediction. By combining detailed annotations with photorealistic simulation, MOPS generates diverse indoor scenes to accelerate progress in robot perception, manipulation, and interaction with real-world environments.
        </div>
    </div>
</div>

---

## 🚧 Alpha Release Notice

> **Important**: MOPS is currently under active development and should be treated as an **early alpha release**. The public API may change, and some features are still in development.

Currently, the code is split into two repositories:
- **[`mops-data`](https://github.com/LiXiling/mops-data)** - Photorealistic image generation in ManiSkill3 ✅
- **`mops-casa`** - Full robot trajectories in RoboCasa 🚧 *Coming Soon*

---

## 🎯 Key Features

### 🎨 Photorealistic Simulation
High-quality visual rendering optimized for computer vision applications in robotic manipulation tasks.

### 🤖 LLM-Powered Annotation  
Zero-shot asset augmentation pipeline using large language models for comprehensive part-level annotations.

### 🎯 Pixel-Level Segmentation
Detailed ground truth for part segmentation and affordance prediction tasks.

### 🏠 Diverse Environments
Rich indoor scenes including kitchen environments, cluttered tabletops, and single object scenarios.

---

## 🔧 Technical Overview

**Asset Management**: Normalized asset pipeline across multiple 3D libraries with automatic part-level annotation and semantic understanding.

**Multi-Modal Annotations**: Comprehensive ground truth including RGB, depth, segmentation masks, affordance maps, and 6D pose information.

**Simulation Framework**: Built on ManiSkill3 and SAPIEN for physics-accurate simulation with photorealistic rendering capabilities.

---

## 🚀 Getting Started

### Prerequisites
- Python 3.10
- CUDA-compatible GPU  
- 16GB+ RAM recommended

### Quick Installation
```bash
conda create -n mops python=3.10
conda activate mops

pip install mani_skill
git clone https://github.com/LiXiling/mops-data

cd mops-data
pip install -e .
```

**[📖 Full Installation Guide →](https://github.com/LiXiling/mops-data#installation)**

---

## 📊 Dataset Highlights

- **Photoreal Quality**: Leverages advanced rendering for realistic visual data
- **Comprehensive Annotations**: Part-level segmentation and affordance labeling
- **Scalable Pipeline**: Automated asset processing and scene generation
- **Robot-Centric Design**: Tailored for manipulation and interaction tasks

---

## 📝 Citation

If you use MOPS in your research, please cite our work:

```bibtex
@article{li2025mops,
  title={Multi-Objective Photoreal Simulation (MOPS) Dataset for Computer Vision in Robotic Manipulation},
  author={
    Maximilian Xiling Li and
    Paul Mattes and
    Nils Blank and
    Korbinian Franz Rudolf and
    Paul Werker L\"odige and
    Rudolf Lioutikov
  },
  year={2025}
}
```

---

## 🏛️ Acknowledgments

This work is supported by the **Intuitive Robots Lab** at KIT, Germany.