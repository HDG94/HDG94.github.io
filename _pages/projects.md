---
layout: page
permalink: /projects/
title: projects
description: Below is a list of selected projects during my PhD.
nav: true
---


**Multiagent Model-based Credit Assignment for Continuous Control**


<div class="embed-responsive embed-responsive-16by9">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/gFyVPm4svEY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>



**Abstract:** Deep reinforcement learning (RL) has recently shown great promise in robotic continuous control tasks. Nevertheless, prior research in this vein center around the centralized learning setting that largely relies on the communication availability among all the components of a robot. However, agents in the real world often operate in a decentralised fashion without communication due to latency requirements, limited power budgets and safety concerns. By formulating robotic components as a system of decentralised agents, this work presents a decentralised multiagent reinforcement learning framework for continuous control. To this end, we first develop a cooperative multiagent PPO framework that allows for centralized optimisation during training and decentralised operation during execution. However, the system only receives a global reward signal which is not attributed towards each agent. To address this challenge, we further propose a generic game-theoretic credit assignment framework which computes agent-specific reward signals. Last but not least, we also incorporate a model-based RL module into our credit assignment framework, which leads to significant improvement in sample efficiency. We demonstrate the effectiveness of our framework on experimental results on Mujoco locomotion control tasks.

---
**MDP Abstraction with Successor Features**

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/rlg/abstraction.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/rlg/smdp.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/rlg/minecraft.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Abstract:** Abstraction plays an important role for generalisation of knowledge and skills, and is key to sample efficient learning. In this work, we study joint temporal and state abstraction in reinforcement learning, where temporally-extended actions in the form of options induce temporal abstractions, while aggregation of similar states with respect to abstract options induce state abstractions. Many existing abstraction schemes ignore the interplay of state and temporal abstraction, consequently, considered option policies often cannot be directly transferred to new environments due to changes in the state space and transition dynamics. To address these issues, we propose a novel abstraction scheme building on successor features. This includes an algorithm for transferring abstract options across different environments, and a state abstraction mechanism which allows us to perform efficient planning with the transferred options. We achieve improved empirical performance on transfer and planning on a set of benchmark tasks.

---
**Multi-Agent Hierarchical Reinforcement Learning with Dynamic Termination**

<div class="row justify-content-sm-center">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/rlg/options.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>

**Abstract:** In a multi-agent system, an agent's optimal policy will typically depend on the policies chosen by others. Therefore, a key issue in multi-agent systems research is that of predicting the behaviours of others, and responding promptly to changes in such behaviours. One obvious possibility is for each agent to broadcast their current intention, for example, the currently executed option in a hierarchical reinforcement learning framework. However, this approach results in inflexibility of agents if options have an extended duration and are dynamic. While adjusting the executed option at each step improves flexibility from a single-agent perspective, frequent changes in options can induce inconsistency between an agent's actual behaviour and its broadcast intention. In order to balance flexibility and predictability, we propose a dynamic termination Bellman equation that allows the agents to flexibly terminate their options. We evaluate our model empirically on a set of multi-agent pursuit and taxi tasks, and show that our agents learn to adapt flexibly across scenarios that require different termination behaviours.


---
**Replication-robust payoff-allocation for machine learning data markets**

<div class="row justify-content-sm-center">
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="assets/img/rlg/options.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        TODO
    </div>
</div>
