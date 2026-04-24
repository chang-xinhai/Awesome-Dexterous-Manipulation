<div align="center">

<h1 id="awesome-dexterous-manipulation">Awesome-Dexterous-Manipulation</h1>

<p>
  <strong>A curated map of papers, hardware, sensors, methods, datasets, benchmarks, and infrastructure for dexterous robot manipulation.</strong>
</p>

<!-- [![Awesome](https://awesome.re/badge.svg)](https://awesome.re) -->
<!-- [![PR's Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com) -->

<p>
  <a href="#-1-hardware--sensor-systems"><img alt="Hardware" src="https://img.shields.io/badge/Hardware-Dexterous%20Hands-a8d8ff?style=for-the-badge"></a>
  <a href="#-2-dexterity-capabilities--tasks"><img alt="Tasks" src="https://img.shields.io/badge/Tasks-In--Hand%20Dexterity-b8e6c9?style=for-the-badge"></a>
  <a href="#-3-methodology"><img alt="Methods" src="https://img.shields.io/badge/Methods-Learning%20%26%20Control-ffd6a5?style=for-the-badge"></a>
  <a href="#-4-infrastructure"><img alt="Infrastructure" src="https://img.shields.io/badge/Infrastructure-Sim%20%26%20Data-d7c5ff?style=for-the-badge"></a>
  <a href="#-5-surveys--reviews"><img alt="Surveys" src="https://img.shields.io/badge/Surveys-Field%20Map-ffb7b2?style=for-the-badge"></a>
</p>

</div>

## About

**Awesome-Dexterous-Manipulation** is a curated list for the ecosystem around dexterous robot manipulation: dexterous hands, tactile sensing, hand-centric tasks, robot learning, optimal control, teleoperation, benchmarks, datasets, and simulators.

This list is intentionally **dexterity-first**. It includes strong adjacent manipulation work only when it materially helps understand, build, evaluate, or deploy dexterous manipulation systems.

## Must Read

Start here if you want the shortest path through the field.

| Goal | Start with |
| :-- | :-- |
| Understand classic dexterous manipulation | [A Mathematical Introduction to Robotic Manipulation](https://www.cds.caltech.edu/~murray/mlswiki/index.php/Main_Page), [A framework for planning dexterous manipulation](https://dblp.org/rec/conf/icra/TrinkleH91) |
| Learn modern in-hand RL | [Learning Dexterous In-Hand Manipulation](https://arxiv.org/abs/1808.00177), [Learning Complex Dexterous Manipulation with Deep RL and Demonstrations](https://arxiv.org/abs/1709.10087), [In-Hand Object Rotation via Rapid Motor Adaptation](https://arxiv.org/abs/2210.04887) |
| Study dexterous hands | [LEAP Hand](https://v1.leaphand.com/), [Shadow Dexterous Hand](https://www.shadowrobot.com/dexterous-hand-series/), [Allegro Hand](https://github.com/Wonikrobotics-git/allegro_hand_ros_v5) |
| Study tactile sensing | [TacThru](https://tacthru.yuyang.li/), [GelSight](https://gelsight.com/), [DIGIT](https://digit.ml/), [ReSkin](https://reskin.dev/), [Awesome Touch](https://github.com/linchangyi1/Awesome-Touch) |
| Find benchmarks and datasets | [DexYCB](https://dex-ycb.github.io/), [DexGraspNet](https://pku-epic.github.io/DexGraspNet/), [Adroit](https://github.com/Farama-Foundation/D4RL/wiki/Tasks#adroit), [Shadow Hand environments](https://isaac-sim.github.io/IsaacLab/main/source/overview/environments.html) |
| Build with simulators | [Isaac Lab](https://isaac-sim.github.io/IsaacLab/), [MuJoCo](https://mujoco.org/), [SAPIEN](https://sapien.ucsd.edu/), [PyBullet](https://github.com/bulletphysics/bullet3) |
| Explore data collection | [DexCap](https://arxiv.org/abs/2403.07788), [DexUMI](https://arxiv.org/abs/2505.21864), [DexWild](https://dexwild.github.io/), [Open-TeleVision](https://arxiv.org/abs/2407.01512) |

## News

- [2026-04-24] Added focused in-hand rotation, tactile manipulation, and Yuyang Li project-cluster resources.
- [2026-04-24] Initialized **Awesome-Dexterous-Manipulation** with hardware, task, methodology, infrastructure, and survey taxonomy.
- [2026-04-24] Added initial seed resources for dexterous hands, tactile sensing, dexterous RL, teleoperation, simulators, and datasets.

## Contents

- [Awesome-Dexterous-Manipulation](#awesome-dexterous-manipulation)
  - [About](#about)
  - [Must Read](#must-read)
  - [News](#news)
  - [Hardware & Sensor Systems](#-1-hardware--sensor-systems)
    - [Dexterous Hands](#11-dexterous-hands)
    - [Tactile Sensors](#12-tactile-sensors)
    - [Multi-Modal Fusion Setups](#13-multi-modal-fusion-setups)
  - [Dexterity Capabilities & Tasks](#-2-dexterity-capabilities--tasks)
    - [Prehensile Manipulation](#21-prehensile-manipulation)
    - [Non-Prehensile Manipulation](#22-non-prehensile-manipulation)
    - [Dynamic & Agile Manipulation](#23-dynamic--agile-manipulation)
    - [Complex & Specialized Tasks](#24-complex--specialized-tasks)
  - [Methodology](#-3-methodology)
    - [Reinforcement Learning](#31-reinforcement-learning)
    - [Imitation Learning](#32-imitation-learning)
    - [Vision-Language-Action & Foundation Models](#33-vision-language-action-vla--foundation-models)
    - [Trajectory Optimization & Optimal Control](#34-trajectory-optimization--optimal-control)
    - [Data Collection Paradigms](#35-data-collection-paradigms)
  - [Infrastructure](#-4-infrastructure)
    - [Simulators](#41-simulators)
    - [Benchmarks & Datasets](#42-benchmarks--datasets)
  - [Surveys & Reviews](#-5-surveys--reviews)
  - [Acknowledgement](#acknowledgement)
  - [Citation](#citation)

<h2 id="-1-hardware--sensor-systems">🦾 1. Hardware & Sensor Systems</h2>

Physical systems and sensing layers for dexterous manipulation.

<a id="11-dexterous-hands"></a>

### 1.1 Dexterous Hands

#### Anthropomorphic Hands

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2024-10-28 | 16 DoF, 8 Motors, Open Hardware | Carnegie Mellon | [LEAP Hand v2](https://v2.leaphand.com/) | RSS 2025 Demo | [hardware](https://v2.leaphand.com/) |
| 2024-08-12 | Vision-Tactile, Dexterous Hand, Compliant | MIT | [EyeSight Hand: Design of a Fully-Actuated Dexterous Robot Hand with Integrated Vision-Based Tactile Sensors and Compliant Actuation](https://arxiv.org/abs/2408.06265) | IROS 2024 | [project](https://eyesighthand.github.io/) |
| 2023-09-14 | Low-Cost, Anthropomorphic, Open Source | Carnegie Mellon | [LEAP Hand: Low-Cost, Efficient, and Anthropomorphic Hand for Robot Learning](https://arxiv.org/abs/2309.06440) | RSS 2024 | [project](https://v1.leaphand.com/) / [github](https://github.com/leap-hand/LEAP_Hand_API) |
| 2022-12-06 | Robust Hand, Industrial, Product | Shadow Robot | [Shadow Dexterous Hand Series](https://www.shadowrobot.com/dexterous-hand-series/) | Website | [hardware](https://www.shadowrobot.com/dexterous-hand-series/) |
| 2018-07-30 | Tendon Actuation, Dexterous Hand, Design | University of Washington | [The Yale OpenHand Project: Optimizing Open-Source Hand Designs for Ease of Fabrication and Adoption](https://ieeexplore.ieee.org/document/8412004) | RA-L 2018 | [project](https://www.eng.yale.edu/grablab/openhand/) |

#### Non-Anthropomorphic & Multi-Finger Grippers

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2020-08-08 | Three-Finger, Open Source, Learning | MPI-IS | [TriFinger: An Open-Source Robot for Learning Dexterity](https://arxiv.org/abs/2008.03596) | CoRL 2021 | [project](https://sites.google.com/view/trifinger) / [github](https://github.com/open-dynamic-robot-initiative/trifinger_simulation) |
| 2016-08-23 | Multi-Finger, Research Hand, Simulation | Wonik Robotics | [Allegro Hand](https://github.com/Wonikrobotics-git/allegro_hand_ros_v5) | GitHub | [ros-v5](https://github.com/Wonikrobotics-git/allegro_hand_ros_v5) / [ros-v4](https://github.com/Wonikrobotics-git/allegro_hand_ros_v4) |
| 2015-05-26 | Adaptive Gripper, Three-Finger, Industrial | Robotiq | [3-Finger Adaptive Robot Gripper](https://robotiq.com/products/3-finger-adaptive-robot-gripper) | Website | [hardware](https://robotiq.com/products/3-finger-adaptive-robot-gripper) |
| 2014-05-31 | Underactuated, Open Hardware, Grasping | Yale | [OpenHand: A Library of Robot Hand Designs](https://www.eng.yale.edu/grablab/openhand/) | Website | [project](https://www.eng.yale.edu/grablab/openhand/) |

<a id="12-tactile-sensors"></a>

### 1.2 Tactile Sensors

#### Vision-Based Tactile

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-12-10 | Visuo-Tactile, Multimodal, Contact | Peking University | [Simultaneous Tactile-Visual Perception for Learning Multimodal Robot Manipulation](https://arxiv.org/abs/2512.09851) | RA-L 2026 | [project](https://tacthru.yuyang.li/) / [github](https://github.com/YuyangLee/TacThru) / [data](https://huggingface.co/datasets/YuyangLee/TacThru) |
| 2024-12-19 | Tactile Hand, High-Resolution Touch, Grasping | Peking University | [Embedding high-resolution touch across robotic hands enables adaptive human-like grasping](https://arxiv.org/abs/2412.14482) | Nature Machine Intelligence 2025 | [website](https://www.nature.com/articles/s42256-025-01053-3) |
| 2024-08-12 | Finger Vision, Hand-Integrated, Dexterous | MIT | [EyeSight Hand](https://arxiv.org/abs/2408.06265) | IROS 2024 | [project](https://eyesighthand.github.io/) |
| 2023-09-19 | Contact-Rich, Low-Cost, Optical | MIT | [GelSight Svelte: A Human Finger-Shaped Single-Camera Tactile Robot Finger with Large Sensing Coverage and Proprioceptive Sensing](https://arxiv.org/abs/2309.10885) | ICRA 2024 | [project](https://gelsight-svelte.github.io/) |
| 2023-08-28 | 3D Shape, 6D Force, Compact | Tsinghua | [9DTact: A Compact Vision-Based Tactile Sensor for Accurate 3D Shape Reconstruction and Generalizable 6D Force Estimation](https://arxiv.org/abs/2308.14277) | arXiv | [project](https://linchangyi1.github.io/9DTact/) |
| 2020-05-29 | High-Resolution, Low-Cost, DIGIT | Meta AI | [DIGIT: A Novel Design for a Low-Cost Compact High-Resolution Tactile Sensor with Application to In-Hand Manipulation](https://arxiv.org/abs/2005.14679) | RA-L 2020 | [project](https://digit.ml/) / [github](https://github.com/facebookresearch/digit-design) |
| 2017-09-20 | GelSight, Optical Tactile, Contact Geometry | MIT | [GelSight: High-Resolution Robot Tactile Sensors for Estimating Geometry and Force](https://gelsight.com/) | Website | [hardware](https://gelsight.com/) |

#### Capacitive & Piezoresistive

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2024-09-12 | Magnetic Skin, Plug-and-Play, Contact | Carnegie Mellon | [AnySkin: Plug-and-play Skin Sensing for Robotic Touch](https://arxiv.org/abs/2409.08276) | arXiv | [project](https://any-skin.github.io/) |
| 2021-10-29 | Magnetic Skin, Replaceable, Low-Cost | Meta AI | [ReSkin: Versatile, Replaceable, Lasting Tactile Skins](https://arxiv.org/abs/2111.00071) | CoRL 2021 | [project](https://reskin.dev/) / [github](https://github.com/facebookresearch/ReSkin) |
| 2019-06-06 | Tactile Glove, Human Grasp, Large-Scale | MIT | [Learning the Signatures of the Human Grasp Using a Scalable Tactile Glove](https://www.nature.com/articles/s41586-019-1234-z) | Nature 2019 | [project](https://www.science.org/doi/10.1126/science.aau9923) |
| 2018-09-19 | E-Skin, Directional Pressure, Bioinspired | Stanford | [A Hierarchically Patterned, Bioinspired E-Skin Able to Detect the Direction of Applied Pressure for Robotics](https://www.science.org/doi/10.1126/scirobotics.aau6914) | Science Robotics 2018 | [paper](https://www.science.org/doi/10.1126/scirobotics.aau6914) |
| 2015-03-18 | Capacitive Array, Three-Axis Force, Flexible | Southeast University | [Flexible Capacitive Tactile Sensor Array With Truncated Pyramids as Dielectric Layer for Three-Axis Force Measurement](https://ieeexplore.ieee.org/document/7061975) | JMEMS 2015 | [paper](https://ieeexplore.ieee.org/document/7061975) |

<a id="13-multi-modal-fusion-setups"></a>

### 1.3 Multi-Modal Fusion Setups

#### Visuo-Tactile Integration

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2026-01-21 | Tactile, Force/Torque, Contact-Rich | TU Munich | [TacUMI: A Multi-Modal Universal Manipulation Interface for Contact-Rich Tasks](https://arxiv.org/abs/2601.14550) | arXiv | [github](https://github.com/Tac-UMI/TacUMI) |
| 2025-12-10 | See-Through-Skin, TacThru-UMI, Diffusion Policy | Peking University | [Simultaneous Tactile-Visual Perception for Learning Multimodal Robot Manipulation](https://arxiv.org/abs/2512.09851) | RA-L 2026 | [project](https://tacthru.yuyang.li/) / [github](https://github.com/YuyangLee/TacThru) |
| 2025-11-08 | Vision+Tactile, Fine Manipulation, Bimanual | Tsinghua | [ViTaMIn-B](https://chuanyune.github.io/ViTaMIn-B_page/) | arXiv | [project](https://chuanyune.github.io/ViTaMIn-B_page/) |
| 2025-08-04 | Tactile Control, Articulated Objects, Proactive | Peking University | [TacMan-Turbo: Proactive Tactile Control for Robust and Efficient Articulated Object Manipulation](https://arxiv.org/abs/2508.02204) | T-ASE 2026 | [paper](https://arxiv.org/abs/2508.02204) |
| 2025-04-08 | Robot-Free, Visuo-Tactile, Contact-Rich | Tsinghua | [ViTaMIn: Learning Contact-Rich Tasks Through Robot-Free Visuo-Tactile Manipulation Interface](https://arxiv.org/abs/2504.06156) | arXiv | [project](https://chuanyune.github.io/ViTaMIn_page/) |
| 2024-03-04 | Tactile, Articulated Objects, Prior-Free | Peking University | [Tac-Man: Tactile-Informed Prior-Free Manipulation of Articulated Objects](https://arxiv.org/abs/2403.01694) | T-RO 2024 | [project](https://tacman-aom.github.io/) |
| 2023-09-18 | Vision+Touch, In-Hand Rotation, Sim2Real | UC Berkeley | [General In-Hand Object Rotation with Vision and Touch](https://arxiv.org/abs/2309.09979) | CoRL 2023 | [project](https://haozhi.io/rotateit/) |
| 2022-09-30 | Multimodal, Contact-Rich, Learning | MIT | [Visuo-Tactile Transformers for Manipulation](https://arxiv.org/abs/2210.00121) | CoRL 2022 | [paper](https://arxiv.org/abs/2210.00121) |

#### Proprioception & Force-Torque

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2026-01-15 | Force, Compliance, Contact-Rich | Stanford | [In-the-Wild Compliant Manipulation with UMI-FT](https://arxiv.org/abs/2601.09988) | ICRA 2026 | [github](https://github.com/real-stanford/UMI-FT) |
| 2025-09-23 | Force-Guided, Wrist F/T, Contact-Rich | GIST | [ManipForce](https://sites.google.com/view/manipforce/) | ICRA 2026 | [project](https://sites.google.com/view/manipforce/) / [github](https://github.com/gist-ailab/ManipForce) |
| 2022-10-10 | Proprioception, Adaptation, Sim2Real | UC Berkeley | [In-Hand Object Rotation via Rapid Motor Adaptation](https://arxiv.org/abs/2210.04887) | arXiv | [paper](https://arxiv.org/abs/2210.04887) |
| 2019-10-16 | Proprioception, Vision, Rubik's Cube | OpenAI | [Solving Rubik's Cube with a Robot Hand](https://arxiv.org/abs/1910.07113) | arXiv | [blog](https://openai.com/index/solving-rubiks-cube/) |

<h2 id="-2-dexterity-capabilities--tasks">🖐️ 2. Dexterity Capabilities & Tasks</h2>

Hand-centric capabilities, organized by manipulation taxonomy rather than by only individual benchmark names.

<a id="21-prehensile-manipulation"></a>

### 2.1 Prehensile Manipulation

#### In-Hand Reorientation / Rotation

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-10-09 | In-Hand Rotation, Neural Dynamics, Sim2Real | Tsinghua | [DexNDM: Closing the Reality Gap for Dexterous In-Hand Rotation via Joint-Wise Neural Dynamics Model](https://arxiv.org/abs/2510.08556) | ICLR 2026 | [project](https://meowuu7.github.io/DexNDM/) |
| 2025-05-12 | In-the-Wild, DexHand, Human-to-Robot | CMU | [DexWild](https://dexwild.github.io/) | RSS 2025 | [project](https://dexwild.github.io/) |
| 2025-01-09 | Any-Axis, Hierarchical Skills, Pose Estimation | UC Berkeley | [From Simple to Complex Skills: The Case of In-Hand Object Reorientation](https://arxiv.org/abs/2501.05439) | arXiv | [paper](https://arxiv.org/abs/2501.05439) |
| 2024-07-10 | In-Hand Translation, Tactile Skin, Shear | Meta FAIR | [Learning In-Hand Translation Using Tactile Skin With Shear and Normal Force Sensing](https://arxiv.org/abs/2407.07885) | arXiv | [project](https://jessicayin.github.io/tactile-skin-rl/) |
| 2023-09-18 | In-Hand Rotation, Vision+Touch, Sim2Real | UC Berkeley | [General In-Hand Object Rotation with Vision and Touch](https://arxiv.org/abs/2309.09979) | CoRL 2023 | [project](https://haozhi.io/rotateit/) |
| 2022-11-21 | Visual Dexterity, Depth, Novel Objects | MIT | [Visual Dexterity: In-Hand Reorientation of Novel and Complex Object Shapes](https://arxiv.org/abs/2211.11744) | Science Robotics 2023 | [project](https://taochenshh.github.io/projects/visual-dexterity/) |
| 2022-10-10 | In-Hand Reorientation, Adaptation, Disturbance | UC Berkeley | [In-Hand Object Rotation via Rapid Motor Adaptation](https://arxiv.org/abs/2210.04887) | arXiv | [paper](https://arxiv.org/abs/2210.04887) |
| 2019-10-16 | Rubik's Cube, Vision, Domain Randomization | OpenAI | [Solving Rubik's Cube with a Robot Hand](https://arxiv.org/abs/1910.07113) | arXiv | [blog](https://openai.com/index/solving-rubiks-cube/) |
| 2018-08-01 | In-Hand Manipulation, Shadow Hand, RL | OpenAI | [Learning Dexterous In-Hand Manipulation](https://arxiv.org/abs/1808.00177) | IJRR 2020 | [dblp](https://dblp.org/rec/journals/ijrr/OpenAI20) / [blog](https://openai.com/index/learning-dexterity/) |
| 2017-09-28 | Demonstrations, Object Manipulation, Adroit | University of Washington | [Learning Complex Dexterous Manipulation with Deep Reinforcement Learning and Demonstrations](https://arxiv.org/abs/1709.10087) | RSS 2018 | [github](https://github.com/aravindr93/hand_dapg) |

#### Finger Gaiting / Regrasping

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2021-09-27 | Finger Gaiting, Intrinsic Sensing, Tactile | Columbia | [On the Feasibility of Learning Finger-gaiting In-hand Manipulation with Intrinsic Sensing](https://arxiv.org/abs/2109.12720) | arXiv | [project](https://roamlab.github.io/learnfg/) / [pdf](https://roamlab.github.io/learnfg/paper.pdf) |
| 1991-04-01 | Contact Planning, Classic, ICRA | Rensselaer Polytechnic Institute | [A framework for planning dexterous manipulation](https://dblp.org/rec/conf/icra/TrinkleH91) | ICRA 1991 | [author-bib](https://www.cse.lehigh.edu/~trink/trink_bib.html) |

#### Tool Use & Extrinsic Dexterity

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2014-05-31 | Extrinsic Dexterity, External Forces, Robot Hand | Carnegie Mellon | [Extrinsic Dexterity: In-Hand Manipulation with External Forces](https://publications.ri.cmu.edu/extrinsic-dexterity-in-hand-manipulation-with-external-forces) | ICRA 2014 | [paper](https://publications.ri.cmu.edu/extrinsic-dexterity-in-hand-manipulation-with-external-forces) |

<a id="22-non-prehensile-manipulation"></a>

### 2.2 Non-Prehensile Manipulation

#### Pushing, Sliding & Flipping

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2016-09-28 | Pushing, Planar Manipulation, Learning | MIT | [Learning to Push by Grasping: Using Multiple Tasks for Effective Learning](https://arxiv.org/abs/1609.09025) | ICRA 2017 | [paper](https://arxiv.org/abs/1609.09025) |

#### Rolling & Pivoting

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 1998-05-20 | Rolling, Finger Gaiting, Contact Planning | Texas A&M | [Dextrous Manipulation by Rolling and Finger Gaiting](https://www.cs.cmu.edu/~lihan/Research/Gait98.html) | ICRA 1998 | [pdf](https://www.cse.lehigh.edu/~trink/Papers/HTicra98.pdf) |

<a id="23-dynamic--agile-manipulation"></a>

### 2.3 Dynamic & Agile Manipulation

#### Catching, Throwing & Juggling

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2019-10-16 | Rubik's Cube, Disturbance, Dynamic Recovery | OpenAI | [Solving Rubik's Cube with a Robot Hand](https://arxiv.org/abs/1910.07113) | arXiv | [blog](https://openai.com/index/solving-rubiks-cube/) |

#### Pen Spinning / Twirling / Fine Motor Skills

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2024-07-26 | Pen Spinning, Sim2Real, Real Fine-Tuning | UC San Diego | [Lessons from Learning to Spin "Pens"](https://arxiv.org/abs/2407.18902) | arXiv | [project](https://penspin.github.io/) |
| 2023-04-09 | Piano Playing, Fine Motor Control, RL | Google Research | [RoboPianist: Dexterous Piano Playing with Deep Reinforcement Learning](https://arxiv.org/abs/2304.04150) | CoRL 2023 | [project](https://kzakka.com/robopianist/) / [openreview](https://openreview.net/forum?id=HDYMjiukjn) |

<a id="24-complex--specialized-tasks"></a>

### 2.4 Complex & Specialized Tasks

#### Bimanual Dexterous Manipulation

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-10-09 | Bimanual, Human Videos, Humanoid | Shanghai AI Lab | [DexMan: Learning Bimanual Dexterous Manipulation from Human and Generated Videos](https://arxiv.org/abs/2510.08475) | arXiv | [paper](https://arxiv.org/abs/2510.08475) |
| 2025-05-28 | DexHand, Robot-Free, UMI | Stanford | [DexUMI: Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation](https://arxiv.org/abs/2505.21864) | RSSW 2025 | [data](https://umi-data.github.io/) |
| 2024-11-19 | Bimanual Dexterity, Asymmetry, RL | Georgia Tech | [AsymDex: Asymmetry and Relative Coordinates for RL-based Bimanual Dexterity](https://arxiv.org/abs/2411.13020) | arXiv | [project](https://star-lab.cc.gatech.edu/papers/Yang-AsymDex-preprint/) |
| 2024-10-17 | Bimanual, Dexterity, Real Robot | Google DeepMind | [ALOHA Unleashed: A Simple Recipe for Robot Dexterity](https://arxiv.org/abs/2410.13126) | arXiv | [project](https://aloha-unleashed.github.io/) |
| 2024-01-08 | Bimanual, Mobile, Teleoperation | Stanford | [Mobile ALOHA: Learning Bimanual Mobile Manipulation with Low-Cost Whole-Body Teleoperation](https://arxiv.org/abs/2401.02117) | arXiv | [project](https://mobile-aloha.github.io/) / [github](https://github.com/MarkFzp/mobile-aloha) |

#### Deformable Object Manipulation

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-07-30 | Deformable, Mobile Manipulation, Benchmark | University of Washington | [MoDeSuite: Robot Learning Task Suite for Benchmarking Mobile Manipulation with Deformable Objects](https://arxiv.org/abs/2507.21796) | arXiv | [project](https://sites.google.com/view/modesuite/home) |
| 2022-10-24 | Differentiable Physics, Deformable, Benchmark | UC Berkeley | [DaXBench: Benchmarking Deformable Object Manipulation with Differentiable Physics](https://arxiv.org/abs/2210.13066) | ICLR 2023 | [github](https://github.com/AdaCompNUS/DaXBench) |
| 2020-11-14 | Cloth, Benchmark, Deformable | UC Berkeley | [SoftGym: Benchmarking Deep Reinforcement Learning for Deformable Object Manipulation](https://arxiv.org/abs/2011.07215) | CoRL 2020 | [project](https://sites.google.com/view/softgym) / [github](https://github.com/Xingyu-Lin/softgym) |

<h2 id="-3-methodology">🧠 3. Methodology</h2>

Learning, planning, control, and data-pipeline methods for dexterous manipulation.

<a id="31-reinforcement-learning"></a>

### 3.1 Reinforcement Learning

#### Sim-to-Real Transfer

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-10-09 | Neural Dynamics, In-Hand Rotation, Sim2Real | Tsinghua | [DexNDM](https://arxiv.org/abs/2510.08556) | ICLR 2026 | [project](https://meowuu7.github.io/DexNDM/) |
| 2025-02-27 | Humanoid, DexHand, Sim2Real | NVIDIA | [Sim-to-Real Reinforcement Learning for Vision-Based Dexterous Manipulation on Humanoids](https://arxiv.org/abs/2502.20396) | arXiv | [project](https://toruowo.github.io/recipe/) |
| 2025-01-09 | Hierarchical Skills, Any-Axis, Sim2Real | UC Berkeley | [From Simple to Complex Skills: The Case of In-Hand Object Reorientation](https://arxiv.org/abs/2501.05439) | arXiv | [paper](https://arxiv.org/abs/2501.05439) |
| 2024-11-19 | Bimanual Dexterity, RL, Sim2Real | Georgia Tech | [AsymDex](https://arxiv.org/abs/2411.13020) | arXiv | [project](https://star-lab.cc.gatech.edu/papers/Yang-AsymDex-preprint/) |
| 2024-07-26 | Pen Spinning, Real Fine-Tuning, Sim2Real | UC San Diego | [Lessons from Learning to Spin "Pens"](https://arxiv.org/abs/2407.18902) | arXiv | [project](https://penspin.github.io/) |
| 2022-10-10 | Adaptation, Domain Randomization, Shadow Hand | UC Berkeley | [In-Hand Object Rotation via Rapid Motor Adaptation](https://arxiv.org/abs/2210.04887) | arXiv | [paper](https://arxiv.org/abs/2210.04887) |
| 2019-10-16 | Rubik's Cube, Automatic Domain Randomization | OpenAI | [Solving Rubik's Cube with a Robot Hand](https://arxiv.org/abs/1910.07113) | arXiv | [blog](https://openai.com/index/solving-rubiks-cube/) |
| 2018-08-01 | In-Hand Manipulation, Domain Randomization | OpenAI | [Learning Dexterous In-Hand Manipulation](https://arxiv.org/abs/1808.00177) | IJRR 2020 | [dblp](https://dblp.org/rec/journals/ijrr/OpenAI20) / [blog](https://openai.com/index/learning-dexterity/) |

#### Reward Design & State Estimation

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-10-09 | Human Video, Contact Rewards, Humanoid | Shanghai AI Lab | [DexMan](https://arxiv.org/abs/2510.08475) | arXiv | [paper](https://arxiv.org/abs/2510.08475) |
| 2024-07-10 | Tactile Skin, Shear/Normal Force, Translation | Meta FAIR | [Learning In-Hand Translation Using Tactile Skin With Shear and Normal Force Sensing](https://arxiv.org/abs/2407.07885) | arXiv | [project](https://jessicayin.github.io/tactile-skin-rl/) |
| 2023-09-18 | Vision+Touch, State Estimation, Rotation | UC Berkeley | [General In-Hand Object Rotation with Vision and Touch](https://arxiv.org/abs/2309.09979) | CoRL 2023 | [project](https://haozhi.io/rotateit/) |
| 2017-09-28 | Demonstrations, Sparse Rewards, Adroit | University of Washington | [Learning Complex Dexterous Manipulation with Deep RL and Demonstrations](https://arxiv.org/abs/1709.10087) | RSS 2018 | [github](https://github.com/aravindr93/hand_dapg) |

<a id="32-imitation-learning"></a>

### 3.2 Imitation Learning

#### Behavior Cloning & Action Chunking

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-05-28 | Human Hand, Robot-Free, DexHand | Stanford | [DexUMI: Using Human Hand as the Universal Manipulation Interface for Dexterous Manipulation](https://arxiv.org/abs/2505.21864) | RSSW 2025 | [data](https://umi-data.github.io/) |
| 2025-03-27 | Bimanual Transfer, DexHand, Residual Learning | Tsinghua | [ManipTrans: Efficient Dexterous Bimanual Manipulation Transfer via Residual Learning](https://arxiv.org/abs/2503.21860) | CVPR 2025 | [project](https://maniptrans.github.io/) / [github](https://github.com/Halowangqx/ManipTrans) |
| 2024-10-17 | Bimanual, Imitation, Robot Dexterity | Google DeepMind | [ALOHA Unleashed](https://arxiv.org/abs/2410.13126) | arXiv | [project](https://aloha-unleashed.github.io/) |
| 2024-01-08 | Bimanual, Mobile, Low-Cost Teleop | Stanford | [Mobile ALOHA](https://arxiv.org/abs/2401.02117) | arXiv | [project](https://mobile-aloha.github.io/) |
| 2023-04-13 | ACT, Action Chunking, Bimanual | Stanford | [Learning Fine-Grained Bimanual Manipulation with Low-Cost Hardware](https://arxiv.org/abs/2304.13705) | RSS 2023 | [project](https://tonyzhaozh.github.io/aloha/) / [github](https://github.com/tonyzhaozh/act) |

#### Diffusion Policies

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-05-21 | 3D Diffusion, Point Cloud, Dexterous | Zhejiang University | [DP3: 3D Diffusion Policy for Generalizable Visuomotor Policy Learning](https://arxiv.org/abs/2403.03954) | ICRA 2025 | [project](https://3d-diffusion-policy.github.io/) |
| 2024-12-19 | Dexterous Fine-Tuning, Real-World Hands | UC Berkeley | [DEFT: Dexterous Fine-Tuning for Real-World Hand Policies](https://dexterous-finetuning.github.io/) | Website | [project](https://dexterous-finetuning.github.io/) |
| 2024-10-31 | Bimanual, Diffusion Foundation, Manipulation | Tsinghua | [RDT-1B: a Diffusion Foundation Model for Bimanual Manipulation](https://arxiv.org/abs/2410.07864) | arXiv | [project](https://rdt-robotics.github.io/rdt-robotics/) / [github](https://github.com/thu-ml/RoboticsDiffusionTransformer) |
| 2023-03-01 | Diffusion Policy, Visuomotor, Robot Learning | Columbia | [Diffusion Policy: Visuomotor Policy Learning via Action Diffusion](https://arxiv.org/abs/2303.04137) | RSS 2023 | [project](https://diffusion-policy.cs.columbia.edu/) / [github](https://github.com/real-stanford/diffusion_policy) |

<a id="33-vision-language-action-vla--foundation-models"></a>

### 3.3 Vision-Language-Action (VLA) & Foundation Models

#### Dexterous VLA Models

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2026-03-01 | DexHand, VLM, Planning | Tsinghua | [UniHM: Unified Dexterous Hand Manipulation with Vision Language Model](https://arxiv.org/abs/2603.00732) | arXiv | [project](https://unihm.github.io/) |
| 2024-06-13 | OpenVLA, Generalist Policy, Robot Learning | Stanford | [OpenVLA: An Open-Source Vision-Language-Action Model](https://arxiv.org/abs/2406.09246) | CoRL 2024 | [project](https://openvla.github.io/) / [github](https://github.com/openvla/openvla) |
| 2023-10-13 | Cross-Embodiment, RT-X, Large-Scale | Google DeepMind | [Open X-Embodiment: Robotic Learning Datasets and RT-X Models](https://arxiv.org/abs/2310.08864) | ICRA 2024 | [project](https://robotics-transformer-x.github.io/) |

#### Zero-shot / Few-shot Dexterity

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2026-03-12 | Humanoid, Demonstrations, Reproducible | Physical Intelligence Lab | [HumDex: Humanoid Dexterous Manipulation Made Easy](https://arxiv.org/abs/2603.12260) | arXiv | [github](https://github.com/physical-superintelligence-lab/HumDex) |
| 2025-07-05 | Human Hand, Few-Shot, Robot-Free | Peking University | [RwoR: Generating Robot Demonstrations from Human Hand Collection for Policy Learning without Robot](https://arxiv.org/abs/2507.03930) | IROS 2025 | [project](https://rwor.github.io/) |
| 2024-10-31 | Egocentric Video, Imitation, Scaling | Georgia Tech | [EgoMimic: Scaling Imitation Learning via Egocentric Video](https://arxiv.org/abs/2410.24221) | arXiv | [project](https://egomimic.github.io/) / [github](https://github.com/SimarKareer/EgoMimic) |

<a id="34-trajectory-optimization--optimal-control"></a>

### 3.4 Trajectory Optimization & Optimal Control

#### Trajectory Optimization

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2022-09-28 | Trajectory Optimization, RL, Dexterous | University of Washington | [Solving Complex Dexterous Manipulation Tasks With Trajectory Optimisation and Reinforcement Learning](https://dexterous-manipulation.github.io/) | CoRL 2022 | [project](https://dexterous-manipulation.github.io/) |

#### Kinematics & Motion Planning

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2024-03-12 | Mocap, Retargeting, DexHand | Stanford | [DexCap: Scalable and Portable Mocap Data Collection System for Dexterous Manipulation](https://arxiv.org/abs/2403.07788) | arXiv | [github](https://github.com/j96w/DexCap) |
| 1994-01-01 | Kinematics, Grasping, Classic Textbook | Caltech | [A Mathematical Introduction to Robotic Manipulation](https://www.cds.caltech.edu/~murray/mlswiki/index.php/Main_Page) | Book | [pdf](https://www.cds.caltech.edu/~murray/books/MLS/pdf/mls94-complete.pdf) |

<a id="35-data-collection-paradigms"></a>

### 3.5 Data Collection Paradigms

#### Vision-based Teleoperation

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-05-28 | Human Hand, DexHand, Robot-Free | Stanford | [DexUMI](https://arxiv.org/abs/2505.21864) | RSSW 2025 | [data](https://umi-data.github.io/) |
| 2024-07-02 | Teleoperation, Immersive, Active Vision | UC San Diego | [Open-TeleVision: Teleoperation with Immersive Active Visual Feedback](https://arxiv.org/abs/2407.01512) | CoRL 2024 | [github](https://github.com/OpenTeleVision/TeleVision) |
| 2024-03-12 | VR, Bimanual, Teleoperation | NYU | [OPEN TEACH: A Versatile Teleoperation System for Robotic Manipulation](https://arxiv.org/abs/2403.07870) | arXiv | [github](https://github.com/aadhithya14/Open-Teach) |
| 2024-02-15 | Robot-Free Teaching, Portable, UMI | Stanford | [Universal Manipulation Interface](https://arxiv.org/abs/2402.10329) | RSS 2024 | [project](https://umi-gripper.github.io/) |

#### Exoskeleton & Glove-based

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-02-11 | Haptic Glove, Force Feedback, Teleoperation | University of Bristol | [DOGlove: Dexterous Manipulation with a Low-Cost Open-Source Haptic Force Feedback Glove](https://arxiv.org/abs/2502.07730) | RSS 2025 | [project](https://do-glove.github.io/) |
| 2024-08-21 | Visual-Exoskeleton, Retargeting, Teleop | UC San Diego | [ACE](https://arxiv.org/abs/2408.11805) | CoRL 2024 | [project](https://ace-teleop.github.io/) |
| 2019-06-06 | Tactile Glove, Human Demonstrations, Grasp | MIT | [Learning the Signatures of the Human Grasp Using a Scalable Tactile Glove](https://www.nature.com/articles/s41586-019-1234-z) | Nature 2019 | [paper](https://www.nature.com/articles/s41586-019-1234-z) |

#### Passive Video & Internet Data Extraction

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2026-02-09 | RGB Video, Dexterous Policies, Human Video | Carnegie Mellon | [Dexterous Manipulation Policies from RGB Human Videos via 4D Hand-Object Trajectory Reconstruction](https://arxiv.org/abs/2602.09013) | arXiv | [project](https://videomanip.github.io/) |
| 2025-10-09 | Human Videos, Bimanual, Generated Videos | Shanghai AI Lab | [DexMan](https://arxiv.org/abs/2510.08475) | arXiv | [paper](https://arxiv.org/abs/2510.08475) |
| 2024-10-31 | Egocentric Video, Imitation, Scaling | Georgia Tech | [EgoMimic](https://arxiv.org/abs/2410.24221) | arXiv | [project](https://egomimic.github.io/) |
| 2022-03-30 | Human Video, Telekinesis, Dexterous Hand | Stanford | [Robotic Telekinesis: Learning a Robotic Hand Imitator by Watching Humans on YouTube](https://arxiv.org/abs/2202.10448) | RSS 2022 | [project](https://robotic-telekinesis.github.io/) |

<h2 id="-4-infrastructure">🛠️ 4. Infrastructure</h2>

Reusable simulators, benchmark suites, datasets, robot descriptions, and training resources.

<a id="41-simulators"></a>

### 4.1 Simulators

#### GPU-Accelerated

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-04-17 | Tactile Simulation, GPU, Vision-Based Touch | Peking University | [Taccel: Scaling Up Vision-based Tactile Robotics via High-performance GPU Simulation](https://arxiv.org/abs/2504.12908) | NeurIPS 2025 Spotlight | [project](https://taccel-simulator.github.io/) / [github](https://github.com/Genesis-Embodied-AI/Taccel) |
| 2024-06-14 | Isaac Lab, GPU Sim, RL Environments | NVIDIA | [Isaac Lab](https://isaac-sim.github.io/IsaacLab/) | GitHub | [github](https://github.com/isaac-sim/IsaacLab) / [docs](https://isaac-sim.github.io/IsaacLab/) |
| 2021-08-02 | GPU Physics, Massive RL, Dexterous Tasks | NVIDIA | [Isaac Gym: High Performance GPU-Based Physics Simulation for Robot Learning](https://arxiv.org/abs/2108.10470) | NeurIPS 2021 | [paper](https://arxiv.org/abs/2108.10470) |
| 2021-08-01 | Isaac Sim, Omniverse, Robotics Simulation | NVIDIA | [Isaac Sim](https://developer.nvidia.com/isaac/sim) | Website | [docs](https://docs.isaacsim.omniverse.nvidia.com/) |

#### CPU-based & High-Fidelity Physics

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2022-05-24 | MuJoCo, Contact Dynamics, Open Source | DeepMind | [MuJoCo: A Physics Engine for Model-Based Control](https://mujoco.org/) | Website | [github](https://github.com/google-deepmind/mujoco) / [paper](https://ieeexplore.ieee.org/document/6386109) |
| 2020-09-04 | SAPIEN, Manipulation, Simulation | UC San Diego | [SAPIEN: A SimulAted Part-Based Interactive ENvironment](https://arxiv.org/abs/2003.08515) | CVPR 2020 | [project](https://sapien.ucsd.edu/) / [github](https://github.com/haosulab/SAPIEN) |
| 2016-10-27 | PyBullet, Robotics Simulation, Open Source | Erwin Coumans | [PyBullet](https://github.com/bulletphysics/bullet3) | GitHub | [docs](https://github.com/bulletphysics/bullet3/blob/master/docs/pybullet_quickstart_guide/PyBulletQuickstartGuide.md.html) / [pypi](https://pypi.org/project/pybullet/) |
| 2012-12-11 | Contact Dynamics, Model-Based Control | University of Washington | [MuJoCo: A Physics Engine for Model-Based Control](https://ieeexplore.ieee.org/document/6386109) | IROS 2012 | [website](https://mujoco.org/) |

<a id="42-benchmarks--datasets"></a>

### 4.2 Benchmarks & Datasets

#### Dexterous Grasping Datasets

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2023-10-24 | Multi-Object, DexHand, Synthetic Dataset | Peking University | [Grasp Multiple Objects with One Hand](https://arxiv.org/abs/2310.15599) | RA-L 2024 | [project](https://multigrasp.github.io/) |
| 2023-01-30 | Large-Scale, DexHand, Grasp Synthesis | Peking University | [DexGraspNet: A Large-Scale Robotic Dexterous Grasp Dataset for General Objects Based on Simulation](https://arxiv.org/abs/2210.02697) | ICRA 2023 | [project](https://pku-epic.github.io/DexGraspNet/) / [github](https://github.com/PKU-EPIC/DexGraspNet) |
| 2022-10-03 | Hand-Agnostic, MultiDex, Grasp Synthesis | BIGAI | [GenDexGrasp: Generalizable Dexterous Grasping](https://arxiv.org/abs/2210.00722) | ICRA 2023 | [project](https://sites.google.com/view/gendexgrasp/home) / [github](https://github.com/tengyu-liu/GenDexGrasp) |
| 2021-04-16 | Hand-Object, RGB-D, Pose, YCB | NVIDIA | [DexYCB: A Benchmark for Capturing Hand Grasping of Objects](https://arxiv.org/abs/2104.04631) | CVPR 2021 | [project](https://dex-ycb.github.io/) |
| 2020-09-01 | Human Grasp, Object Pose, Contact | University of Tuebingen | [GRAB: A Dataset of Whole-Body Human Grasping of Objects](https://arxiv.org/abs/2008.11200) | ECCV 2020 | [project](https://grab.is.tue.mpg.de/) |
| 2019-12-17 | Hand-Object, 3D Reconstruction, HO-3D | IIT Delhi | [HOnnotate: A Method for 3D Annotation of Hand and Object Poses](https://arxiv.org/abs/1907.01481) | CVPR 2020 | [project](https://www.tugraz.at/index.php?id=40231) |

#### Teleoperation & Task Benchmarks

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2025-04-25 | Platform, Dataset, Benchmark, Simulation | Peking University | [RoboVerse: Towards a Unified Platform, Dataset and Benchmark for Scalable and Generalizable Robot Learning](https://arxiv.org/abs/2504.18904) | RSS 2025 | [project](https://roboverseorg.github.io/) / [github](https://github.com/RoboVerseOrg) |
| 2024-03-19 | In-the-Wild, Large-Scale, Robot Data | Stanford | [DROID: A Large-Scale In-The-Wild Robot Manipulation Dataset](https://arxiv.org/abs/2403.12945) | arXiv | [project](https://droid-dataset.github.io/) |
| 2023-10-13 | Cross-Embodiment, RT-X, Multi-Dataset | Google DeepMind | [Open X-Embodiment](https://arxiv.org/abs/2310.08864) | ICRA 2024 | [project](https://robotics-transformer-x.github.io/) |
| 2022-10-24 | Deformable, Differentiable Physics, Benchmark | UC Berkeley | [DaXBench](https://arxiv.org/abs/2210.13066) | ICLR 2023 | [github](https://github.com/AdaCompNUS/DaXBench) |
| 2020-04-15 | Dexterous Hand, Offline RL, Adroit | UC Berkeley | [D4RL: Datasets for Deep Data-Driven Reinforcement Learning](https://arxiv.org/abs/2004.07219) | arXiv | [github](https://github.com/Farama-Foundation/D4RL) |
| 2019-10-24 | Manipulation Benchmark, Meta-World, RL | Stanford | [Meta-World: A Benchmark and Evaluation for Multi-Task and Meta Reinforcement Learning](https://arxiv.org/abs/1910.10897) | CoRL 2019 | [github](https://github.com/Farama-Foundation/Metaworld) |

<h2 id="-5-surveys--reviews">📚 5. Surveys & Reviews</h2>

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |
| 2021-05-18 | Tactile Sensing, Review, Robots | University of Bristol | [A Review of Tactile Sensors for Robotic Applications](https://www.mdpi.com/1424-8220/21/11/3938) | Sensors 2021 | [paper](https://www.mdpi.com/1424-8220/21/11/3938) |
| 2018-12-01 | Dexterous Manipulation, Hand-Centric Taxonomy | Stanford | [A Hand-Centric Classification of Human and Robot Dexterous Manipulation](https://doi.org/10.1109/TOH.2018.2866787) | IEEE ToH 2018 | [paper](https://doi.org/10.1109/TOH.2018.2866787) |

## Acknowledgement

This list follows the single-file, compact-table style of [Awesome-UMI](https://github.com/chang-xinhai/Awesome-UMI) and cross-checks scope against related public resources:

- [Dexterous-Manipulation](https://github.com/kingchou007/Dexterous-Manipulation)
- [awesome-humanoid-manipulation](https://github.com/Tsunami-kun/awesome-humanoid-manipulation)
- [Awesome-Robotics-Manipulation](https://github.com/BaiShuanghao/Awesome-Robotics-Manipulation)
- [Awesome-Touch](https://github.com/linchangyi1/Awesome-Touch)
- [awesome-robot-descriptions](https://github.com/robot-descriptions/awesome-robot-descriptions)

## Citation

If this repository helps your work, please cite or link it as:

```bibtex
@misc{awesome_dexterous_manipulation,
  title        = {Awesome-Dexterous-Manipulation},
  author       = {Xinhai Chang},
  year         = {2026},
  howpublished = {\url{https://github.com/chang-xinhai/Awesome-Dexterous-Manipulation}},
}
```
