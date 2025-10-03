---
layout: project_page
permalink: /

title: "SRBTrack: Terrain-Adaptive Tracking of a Single-Rigid-Body Character Using Momentum-Mapped Space-Time Optimization"
venue: "SIGGRAPH Asia 2025"
authors:
    Hanyang Cao<sup>1*</sup>,&nbsp;
    <a href="https://heyuanyao-pku.github.io/" target="_blank" rel="noopener">Heyuan Yao</a><sup>2*</sup>,&nbsp;
    <a href="https://libliu.info/" target="_blank" rel="noopener">Libin Liu</a><sup>2</sup>,&nbsp;
    <a href="http://calab.hanyang.ac.kr/?node=Taesoo" target="_blank" rel="noopener">Taesoo Kwon</a><sup>1†</sup>
affiliations:
    <sup>1</sup> Hanyang University;&nbsp;&nbsp;<sup>2</sup> Peking University<br/>
    <sup>*</sup> equal contribution;&nbsp;<sup>†</sup> corresponding author
paper: https://www.cs.virginia.edu/~robins/Turing_Paper_1936.pdf
video: https://www.youtube.com/watch?v=yf_V8TVO71s
code: coming soon
---

<!-- Using HTML to center the abstract -->
<div class="columns is-centered has-text-centered">
    <div class="column is-four-fifths">
        <h2>Abstract</h2>
        <div class="content has-text-justified">
Generating realistic and robust motion for virtual characters under complex physical conditions, such as irregular terrain, real-time control scenarios, and external disturbances, remains a key challenge in computer graphics. While deep reinforcement learning has enabled high-fidelity physics-based character animation, such methods often suffer from limited generalizability, as learned controllers tend to overfit to the environments they were trained in. In contrast, simplified models, such as single rigid bodies, offer better adaptability, but traditionally require hand-crafted heuristics and can only handle short motion segments. In this paper, we present a general learning framework that trains a single-rigid-body (SRB) character controller from long and unstructured datasets, without the reliance on human-crafted rules. Our method enables zero-shot adaptation to diverse environments and unseen motion styles. The resulting controller generates expressive and physically plausible motions in real time and seamlessly integrates with high-level kinematic motion planners without retraining, enabling a wide range of downstream tasks.
        </div>
    </div>
</div>

---

<h3 style="text-align: center;">Overview</h3>
<div style="text-align:center;">
    <img src="https://raw.githubusercontent.com/hanyang9/SRBTrack/main/static/image/overview_final.pdf" alt="overview" width="640">
    <p>The SRB tracking policy, trained using a combination of reinforcement and supervised learning on flat terrain, generalizes to uneven terrain at inference. A QP solver computes contact forces from predicted actions, while a full-body motion predictor outputs future states. The states are refined via momentum-mapped space–time optimization for rendering.</p>
</div>

<h3 style="text-align: center;">Terrain Adaptation</h3>
> All blinded! All executed by a single policy! All trained on flat terrain only!
<div style="display: flex; justify-content: center; gap: 20px; margin: 20px 0;">
  <div style="text-align:center;">
    <video width="300" controls autoplay muted loop playsinline>
      <source src="https://raw.githubusercontent.com/hanyang9/SRBTrack/main/static/Video/SRB_hill.mp4" type="video/mp4">
    </video>
    <p>Hopping on hill.</p>
  </div>

  <div style="text-align:center;">
    <video width="300" controls autoplay muted loop playsinline>
      <source src="https://raw.githubusercontent.com/hanyang9/SRBTrack/main/static/Video/SRB_pyramid.mp4" type="video/mp4">
    </video>
    <p>Walking on pyramid with ball interaction.</p>
  </div>

  <div style="text-align:center;">
    <video width="300" controls autoplay muted loop playsinline>
      <source src="https://raw.githubusercontent.com/hanyang9/SRBTrack/main/static/Video/SRB_stepping_stones.mp4" type="video/mp4">
    </video>
    <p>Walking on stepping stones.</p>
  </div>

</div>


<h2 style="text-align: center;">Video</h2>
<div style="text-align:center; margin: 20px 0;">
  <iframe width="800" height="450" 
          src="https://www.youtube.com/embed/yf_V8TVO71s" 
          title="YouTube video player" 
          frameborder="0" 
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" 
          allowfullscreen>
  </iframe>
</div>
---
