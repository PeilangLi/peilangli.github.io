---
layout: page
title: Interpretable Reinforcement Learning via Shapley Values
description: Bridging explainability and interpretability in RL policies using model-agnostic Shapley analysis.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

Reinforcement learning (RL) has revolutionized decision-making in complex domains, yet its "black box" nature poses challenges for trust and transparency in critical applications. This project introduces a novel framework that transforms opaque RL policies into interpretable representations using Shapley values, enabling both local and global understanding of agent behavior.

<div class="row"> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="Shapley Value Clustering" class="img-fluid rounded z-depth-1" %} </div> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Decision Boundaries" class="img-fluid rounded z-depth-1" %} </div> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/5.jpg" title="Policy Performance" class="img-fluid rounded z-depth-1" %} </div> </div> <div class="caption"> Key components of the framework: (Left) Shapley value vectors clustered by action regions, (Middle) Decision boundaries mapped to original state space, (Right) Stable performance of interpretable policies compared to original models. </div>
Approach
The methodology combines Shapley value analysis with action-aware clustering to extract decision patterns from trained RL policies. By reformulating states into contribution vectors, we identify critical boundaries between action regions and reconstruct them as interpretable linear functions. This process preserves policy effectiveness while offering full transparency.

<div class="row justify-content-sm-center"> <div class="col-sm-8 mt-3 mt-md-0"> {% include figure.liquid path="assets/img/6.jpg" title="CartPole Results" class="img-fluid rounded z-depth-1" %} </div> <div class="col-sm-4 mt-3 mt-md-0"> {% include figure.liquid path="assets/img/11.jpg" title="MountainCar Results" class="img-fluid rounded z-depth-1" %} </div> </div> <div class="caption"> Experimental results in CartPole (left) and MountainCar (right) environments, showing interpretable policies achieving competitive rewards with lower variance. </div>
Impact
Model-Agnostic: Compatible with DQN, PPO, and A2C algorithms.

Stability: 23% reduction in performance variance across tested environments.

Accessibility: Policies expressed as linear equations (e.g., f<sub>01</sub> = 0.35x − ẋ − 0.3), enabling human validation.

Future work extends this framework to continuous action spaces and high-dimensional domains, aiming to democratize trustworthy RL for real-world deployment.