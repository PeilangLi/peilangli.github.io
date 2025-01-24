---
layout: page
title: From Explainability to Interpretability: Interpretable Policies in Reinforcement Learning
description: Bridging the gap between explainable and interpretable reinforcement learning with Shapley values.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: true
---

Reinforcement learning has achieved remarkable performance in complex domains, but the inherent black-box nature of deep neural network policies makes them difficult to interpret and trust, especially in critical applications. This project introduces a novel model-agnostic approach that leverages Shapley values to transform deep reinforcement learning policies into interpretable representations.

<div class="row"> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/1.jpg" title="Shapley Value Analysis" class="img-fluid rounded z-depth-1" %} </div> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/2.jpg" title="Cluster Visualization" class="img-fluid rounded z-depth-1" %} </div> <div class="col-sm mt-3 mt-md-0"> {% include figure.liquid loading="eager" path="assets/img/3.jpg" title="Interpretable Decision Boundaries" class="img-fluid rounded z-depth-1" %} </div> </div>
The framework provides global insights into policy behavior, surpassing traditional local explainability. It supports both off-policy and on-policy algorithms, including Deep Q-Network (DQN), Proximal Policy Optimization (PPO), and Advantage Actor-Critic (A2C). The interpretable policies maintain model effectiveness and demonstrate enhanced stability in environments like CartPole and MountainCar.

<div class="caption"> Visualizations include Shapley value analysis (left), action clustering (middle), and decision boundaries for interpretable policies (right). </div>
This work represents a step toward developing transparent, trustworthy AI solutions for high-stakes real-world applications.