---
layout: project_page
permalink: /

title: "MOPS: Multi-Object Photoreal Simulation Dataset for Computer Vision in Robot Manipulation"
authors:
    Maximilian X. Li, Paul Mattes, Nils Blank, Rudolf Lioutikov
affiliations:
    Intuitive Robots Lab, Karlsruhe Institute of Technology, Germany
paper: ./static/Li2026_MOPS.pdf
code: https://github.com/LiXiling/mops-data
#video: https://www.youtube.com/results?search_query=turing+machine
#data: https://huggingface.co/docs/datasets
---

<!-- Abstract -->
<div class="columns is-centered has-text-centered">
  <div class="column is-four-fifths">
    <h2 class="section-heading">Abstract</h2>
    <div class="content has-text-justified abstract-text">
      Datasets bridging computer vision and robotics by providing high-quality visual annotations
      in manipulation-relevant scenes remain limited.
      This work introduces the <strong>Multi-Object Photoreal Simulation (MOPS)</strong> dataset, which provides
      comprehensive ground truth annotations for photorealistic simulated environments. MOPS employs
      a zero-shot asset augmentation pipeline based on Large Language Models (LLM) to automatically
      normalize 3D object scale and generate part-level affordances. The dataset features pixel-level
      segmentations for tasks crucial to robotic perception, including fine-grained part segmentation
      and affordance prediction (e.g., <em>"graspable"</em> or <em>"pushable"</em>). By combining detailed
      annotations with photorealistic simulation, MOPS generates a vast, diverse collection of scenes
      to accelerate progress in robot perception and manipulation. We validate MOPS through vision and
      robot learning benchmarks.
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Alpha Release Notice -->
<div class="notification is-warning is-light alpha-notice">
  <div class="columns is-vcentered">
    <div class="column is-narrow">
      <span class="tag is-warning is-medium"><strong>Alpha</strong></span>
    </div>
    <div class="column">
      <strong>Early Alpha Release</strong> — MOPS is under active development. The public API may change and some features are still in progress.
    </div>
  </div>
  <div class="repo-links mt-3">
    <a href="https://github.com/LiXiling/mops-data" class="repo-pill is-available">
      <span class="repo-icon">⚙️</span>
      <span><code>mops-data</code> — Image generation in ManiSkill3</span>
      <span class="repo-status">Available</span>
    </a>
    <a class="repo-pill is-coming-soon">
      <span class="repo-icon">🤖</span>
      <span><code>mops-il</code> — Full robot trajectories in RoboCasa v0.1</span>
      <span class="repo-status">Coming Soon</span>
    </a>
  </div>
</div>

<hr class="section-divider">

<!-- Annotation Modalities Image Gallery -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Annotation Modalities</h2>
  <p class="section-subheading">MOPS provides rich, multi-modal ground truth for every scene</p>
</div>

<div class="columns is-multiline modality-gallery">
  <div class="column is-half-tablet is-one-quarter-desktop">
    <div class="modality-card">
      <figure class="image">
        <img src="./static/image/rgb.png" alt="RGB Render">
      </figure>
      <div class="modality-label">
        <span class="modality-dot" style="background:#4a90d9;"></span>
        RGB
      </div>
    </div>
  </div>
  <div class="column is-half-tablet is-one-quarter-desktop">
    <div class="modality-card">
      <figure class="image">
        <img src="./static/image/depth.png" alt="Depth Map">
      </figure>
      <div class="modality-label">
        <span class="modality-dot" style="background:#e67e22;"></span>
        Depth
      </div>
    </div>
  </div>
  <div class="column is-half-tablet is-one-quarter-desktop">
    <div class="modality-card">
      <figure class="image">
        <img src="./static/image/normal.png" alt="Surface Normals">
      </figure>
      <div class="modality-label">
        <span class="modality-dot" style="background:#27ae60;"></span>
        Surface Normals
      </div>
    </div>
  </div>
  <div class="column is-half-tablet is-one-quarter-desktop">
    <div class="modality-card">
      <figure class="image">
        <img src="./static/image/segm.png" alt="Part / Affordance Segmentation">
      </figure>
      <div class="modality-label">
        <span class="modality-dot" style="background:#8e44ad;"></span>
        Segmentation
      </div>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Key Features -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Key Features</h2>
</div>

<div class="columns is-multiline feature-grid">
  <div class="column is-half">
    <div class="feature-card">
      <div class="feature-icon">🎨</div>
      <h3 class="feature-title">Photorealistic Simulation</h3>
      <p class="feature-text">High-quality visual rendering via ManiSkill3 and SAPIEN, optimized for computer vision tasks in robotic manipulation.</p>
    </div>
  </div>
  <div class="column is-half">
    <div class="feature-card">
      <div class="feature-icon">🤖</div>
      <h3 class="feature-title">LLM-Powered Annotation</h3>
      <p class="feature-text">Zero-shot asset augmentation pipeline using large language models for automatic part-level labeling and semantic understanding.</p>
    </div>
  </div>
  <div class="column is-half">
    <div class="feature-card">
      <div class="feature-icon">🏷️</div>
      <h3 class="feature-title">Pixel-Level Segmentation</h3>
      <p class="feature-text">Detailed ground truth for fine-grained part segmentation and affordance prediction (e.g., <em>graspable</em>, <em>pushable</em>).</p>
    </div>
  </div>
  <div class="column is-half">
    <div class="feature-card">
      <div class="feature-icon">🏠</div>
      <h3 class="feature-title">Diverse Environments</h3>
      <p class="feature-text">Rich indoor scenes including kitchen environments, cluttered tabletops, and isolated object scenarios at scale.</p>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Technical Overview -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Technical Overview</h2>
</div>

<div class="columns">
  <div class="column">
    <div class="tech-item">
      <span class="tech-label">Asset Pipeline</span>
      <p>Normalized asset management across multiple 3D libraries with automatic part-level annotation and semantic scene understanding.</p>
    </div>
  </div>
  <div class="column">
    <div class="tech-item">
      <span class="tech-label">Multi-Modal Ground Truth</span>
      <p>Comprehensive annotations including RGB, depth, surface normals, segmentation masks, affordance maps, and 6D pose information.</p>
    </div>
  </div>
  <div class="column">
    <div class="tech-item">
      <span class="tech-label">Simulation Framework</span>
      <p>Built on ManiSkill3 and SAPIEN for physics-accurate simulation with photorealistic rendering and programmable scene generation.</p>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Dataset Comparison -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Dataset Comparison</h2>
  <p class="section-subheading">MOPS provides significantly broader taxonomic coverage than existing datasets</p>
</div>

<div class="columns is-centered">
  <div class="column is-four-fifths">
    <div class="comparison-table-wrap">
      <table class="comparison-table">
        <thead>
          <tr>
            <th>Dataset</th>
            <th>Level</th>
            <th>Aff. Labels</th>
            <th>Obj. Cat.</th>
            <th>Objects</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>RGB-D Part</td>
            <td><span class="level-tag">Part</span></td>
            <td>7</td>
            <td>17</td>
            <td>105</td>
          </tr>
          <tr>
            <td>3D-AffNet</td>
            <td><span class="level-tag">Part</span></td>
            <td>16</td>
            <td>23</td>
            <td><strong>22,949</strong></td>
          </tr>
          <tr class="table-section-divider">
            <td>MOPS-Partnet</td>
            <td><span class="level-tag">Part</span></td>
            <td>24</td>
            <td>46</td>
            <td>2,345</td>
          </tr>
          <tr>
            <td>MOPS-Robocasa</td>
            <td><span class="level-tag level-tag-object">Object</span></td>
            <td>44</td>
            <td>101</td>
            <td>1,008</td>
          </tr>
          <tr class="table-highlight">
            <td><strong>MOPS (Total)</strong></td>
            <td><span class="level-tag level-tag-mixed">Mixed</span></td>
            <td><strong>56</strong></td>
            <td><strong>137</strong></td>
            <td>3,353</td>
          </tr>
        </tbody>
      </table>
      <p class="table-caption">While 3D-AffNet has more instances, MOPS provides significantly higher taxonomic coverage across object categories and affordance types.</p>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Robot Manipulation Results -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Robot Manipulation Results</h2>
  <p class="section-subheading">Imitation learning on 24 RoboCasa tasks, evaluated over 10 environment seeds each</p>
</div>

<div class="columns is-centered is-vcentered">
  <div class="column is-narrow">
    <div class="results-stats">
      <div class="stat-box">
        <div class="stat-number">21.25<span class="stat-unit">%</span></div>
        <div class="stat-label">Success Rate</div>
        <div class="stat-sublabel">RGB + MOPS Affordances</div>
      </div>
      <div class="stat-box stat-box-gain">
        <div class="stat-number">+7.92<span class="stat-unit">pp</span></div>
        <div class="stat-label">Absolute Gain</div>
        <div class="stat-sublabel">over RGB-only baseline</div>
      </div>
    </div>
  </div>
  <div class="column">
    <div class="comparison-table-wrap">
      <table class="comparison-table">
        <thead>
          <tr>
            <th>Policy Inputs</th>
            <th>Success Rate</th>
            <th>Gain</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>RGB only</td>
            <td>13.33%</td>
            <td><span class="gain-neutral">&mdash;</span></td>
          </tr>
          <tr class="table-highlight">
            <td><strong>RGB + MOPS Affordances</strong></td>
            <td><strong>21.25%</strong></td>
            <td><span class="gain-positive">+7.92</span></td>
          </tr>
        </tbody>
      </table>
      <p class="table-caption">MOPS affordance annotations provide a consistent boost to imitation learning performance across 24 RoboCasa manipulation tasks.</p>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Getting Started -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Getting Started</h2>
</div>

<div class="columns is-centered">
  <div class="column is-four-fifths">
    <div class="install-box">
      <p class="install-prereqs"><strong>Prerequisites:</strong> Python 3.10 &nbsp;·&nbsp; CUDA-compatible GPU &nbsp;·&nbsp; 16 GB+ RAM</p>
      <pre><code class="language-bash">conda create -n mops python=3.10
conda activate mops

pip install mani_skill
git clone https://github.com/LiXiling/mops-data
cd mops-data
pip install -e .</code></pre>
      <p class="mt-3"><a href="https://github.com/LiXiling/mops-data#installation" class="external-link button is-link is-light is-small is-rounded">📖 Full Installation Guide →</a></p>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Citation -->
<div class="has-text-centered mb-5">
  <h2 class="section-heading">Citation</h2>
  <p class="section-subheading">If you use MOPS in your research, please cite our work</p>
</div>

<div class="columns is-centered">
  <div class="column is-four-fifths">
    <div class="citation-box">
      <pre><code>@article{li2026mops,
  title   = {Multi-Objective Photoreal Simulation (MOPS) Dataset
             for Computer Vision in Robot Manipulation},
  author  = {Maximilian Xiling Li and Paul Mattes and
             Nils Blank and Rudolf Lioutikov},
  year    = {2026}
}</code></pre>
    </div>
  </div>
</div>

<hr class="section-divider">

<!-- Acknowledgments -->
<div class="has-text-centered acknowledgments">
  <p>This work is supported by the <strong>Intuitive Robots Lab</strong> at Karlsruhe Institute of Technology, Germany.</p>
</div>