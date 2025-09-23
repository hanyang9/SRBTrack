---
layout: project_page
permalink: /

title: "SRBTrack: Terrain-Adaptive Tracking of a Single-Rigid-Body Character Using Momentum-Mapped Space-Time Optimization"
authors:
    Hanyang</a><sup>1*</sup>,&nbsp;
    <a href="https://heyuanyao-pku.github.io/" target="_blank" rel="noopener">Heyuan Yao</a><sup>2*</sup>,&nbsp;
    <a href="https://libliu.info/" target="_blank" rel="noopener">Libin Liu</a><sup>2</sup>,&nbsp;
    <a href="http://calab.hanyang.ac.kr/?node=Taesoo" target="_blank" rel="noopener">Taesoo Kwon</a><sup>1†</sup>
affiliations:
    <sup>1</sup> Hanyang University;&nbsp;&nbsp;<sup>2</sup> Peking University<br/>
    <sup>*</sup> equal contribution;&nbsp;<sup>†</sup> corresponding author
paper: https://www.cs.virginia.edu/~robins/Turing_Paper_1936.pdf
video: https://www.youtube.com/results?search_query=turing+machine
code: https://github.com/topics/turing-machines
data: https://huggingface.co/docs/datasets
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

> Note: This is an example of a Jekyll-based project website template: [Github link](https://github.com/shunzh/project_website).


## Key Ideas
1. Turing first presented the concept of a "computable number," which refers to a number that can be computed by an algorithm or a definite step-by-step process.
2. He introduced the notion of a Turing machine, an abstract computational device consisting of an infinite tape divided into cells and a read-write head. The machine can read and write symbols on the tape, move the head left or right, and transition between states based on a set of rules.
3. Turing demonstrated that the set of computable numbers is enumerable, meaning it can be listed in a systematic way, even though it is not necessarily countable.
4. He proved the existence of non-computable numbers, which cannot be computed by any Turing machine.
5. Turing showed that the Entscheidungsproblem is undecidable, meaning there is no algorithm that can determine, for any given mathematical statement, whether it is provable or not.

![Turing Machine](/static/image/Turing_machine.png)

*Figure 1: A representation of a Turing Machine. Source: [Wiki](https://en.wikipedia.org/wiki/Turing_machine).*

## Significance
Turing's paper laid the foundation for the theory of computation and had a profound impact on the development of computer science. The Turing machine became a fundamental concept in theoretical computer science, serving as a theoretical model for studying the limits and capabilities of computation. Turing's work also influenced the development of programming languages, algorithms, and the design of modern computers.

## Citation
```
@article{turing1936computable,
  title={On computable numbers, with an application to the Entscheidungsproblem},
  author={Turing, Alan Mathison},
  journal={Journal of Mathematics},
  volume={58},
  number={345-363},
  pages={5},
  year={1936}
}
```
