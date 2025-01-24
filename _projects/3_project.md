---
layout: page
title: Fair Multi-Agent Reinforcement Learning
description: Achieving equitable outcomes in cooperative systems via welfare optimization and attention mechanisms.
img: assets/img/13.jpg
importance: 1
category: work
related_publications: true
---

Multi-agent systems increasingly govern critical domains like autonomous networks and resource allocation, yet traditional methods often prioritize efficiency over fairness. This project introduces **FAPPO** and **AT-FAPPO**, novel algorithms that integrate welfare functions and attention mechanisms to ensure equitable reward distribution among cooperative agents while maintaining high performance.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/7.jpg" title="Welfare Optimization" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/8.jpg" title="Attention Mechanism" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/9.jpg" title="Matthew Effect Mitigation" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Core innovations: (Left) Welfare-driven policy updates for balanced rewards, (Middle) Self-attention for inter-agent communication, (Right) Addressing the "rich-get-richer" phenomenon in cooperative tasks.
</div>

### Approach
**FAPPO** extends Proximal Policy Optimization (PPO) to optimize a generalized Gini welfare function, prioritizing agents with lower rewards during training. **AT-FAPPO** enhances this with a multi-head self-attention mechanism, enabling agents to share context-aware signals for coordinated action selection. The framework operates under centralized training with decentralized execution (CTDE), ensuring scalability and practicality.

<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/10.jpg" title="Random MDP Results" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/14.jpg" title="Matthew Effect Results" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Experimental validation: (Left) FAPPO outperforms baselines in reward balance (CV: 0.21 vs. 0.45 for QMIX), (Right) AT-FAPPO mitigates the Matthew effect, achieving 32% higher minimum agent rewards than IPPO.
</div>

### Impact
- **Equity-Driven Design**: Policies reduce reward inequality by up to 53% in multi-agent grid worlds.
- **Scalability**: Compatible with decentralized execution, suitable for real-world systems like traffic control or drone swarms.
- **Theoretical Rigor**: Welfare functions adhere to Pigou-Dalton principles, ensuring mathematically fair solutions.

Future work explores continuous action spaces and applications in ethical AI systems, aiming to democratize benefits across heterogeneous agent populations.

{% cite Anonymous2024FairMARL %}
