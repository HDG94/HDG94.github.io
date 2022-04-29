---
layout: page
permalink: /projects/
title: projects
description: Below is a list of selected projects during my PhD.
nav: true
---

<br>
<br>

***
## **Multiagent Model-based Credit Assignment for Continuous Control**

<div class="embed-responsive embed-responsive-16by9">
  <iframe width="480" height="270" src="https://www.youtube.com/embed/gFyVPm4svEY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<div class="caption">
    This short video shows the formulation and demo.
</div>

**Abstract:** Deep reinforcement learning (RL) has recently shown great promise in robotic continuous control tasks. Nevertheless, prior research in this vein center around the centralized learning setting that largely relies on the communication availability among all the components of a robot. However, agents in the real world often operate in a decentralised fashion without communication due to latency requirements, limited power budgets and safety concerns. By formulating robotic components as a system of decentralised agents, this work presents a decentralised multiagent reinforcement learning framework for continuous control. To this end, we first develop a cooperative multiagent PPO framework that allows for centralized optimisation during training and decentralised operation during execution. However, the system only receives a global reward signal which is not attributed towards each agent. To address this challenge, we further propose a generic game-theoretic credit assignment framework which computes agent-specific reward signals. Last but not least, we also incorporate a model-based RL module into our credit assignment framework, which leads to significant improvement in sample efficiency. We demonstrate the effectiveness of our framework on experimental results on Mujoco locomotion control tasks.

<br>
<br>

***
## **MDP Abstraction with Successor Features**

<div class="row justify-content-sm-center">
    <div class="col-sm-7 mt-3 mt-md-0">
        <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/abstraction.jpg" title="We Combined Temporal + State Abstraction " class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="caption">
            We Combined Temporal Abstraction + State Abstraction
        </div>
    </div>
    <div class= "col-sm-5 mt-3 mt-md-0" >
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.html path="assets/img/minecraft.png" title="Minecraft Setting" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="w-100"></div>
        <div class="col-sm mt-3 mt-md-0">
            {% include figure.html path="assets/img/smdp.png" title="Abstract SMDP Generated via Our Algorithm" class="img-fluid rounded z-depth-1" %}
        </div>
        <div class="caption">
            Abstract SMDP Generated via Our Algorithm
        </div>
    </div>
</div>

**Appendix:** you can [download pdf](https://HDG94.github.io/assets/img/abstractions_appendix.pdf) here.

**Abstract:** **Abstraction** plays an important role for generalisation of knowledge and skills, and is key to sample efficient learning. In this work, we study **joint temporal and state abstraction** in reinforcement learning, where temporally-extended actions in the form of options induce temporal abstractions, while aggregation of similar states with respect to abstract options induce state abstractions. Many existing abstraction schemes ignore the interplay of state and temporal abstraction, consequently, considered option policies often cannot be directly transferred to new environments due to changes in the state space and transition dynamics. To address these issues, we propose a novel abstraction scheme building on successor features. This includes an algorithm for transferring abstract options across different environments, and **Successor Homomorphism**, i.e., a state abstraction mechanism which allows us to perform efficient planning with the transferred options. We achieve improved empirical performance on transfer and planning on a set of benchmark tasks.


<br>
<br>

***
## **Multi-Agent Hierarchical Reinforcement Learning with Dynamic Termination**

<div class="row justify-content-sm-center">
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
    <div class="col-sm-6 mt-3 mt-md-0">
        {% include figure.html path="assets/img/options.png" title="Dynamic Termination Hierarchical RL" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-2 mt-3 mt-md-0">
    </div>
</div>

**Abstract:** In a multi-agent system, an agent's optimal policy will typically depend on the policies chosen by others. Therefore, a key issue in multi-agent systems research is that of predicting the behaviours of others, and responding promptly to changes in such behaviours. One obvious possibility is for each agent to broadcast their current intention, for example, the currently executed **option** in a hierarchical reinforcement learning framework. However, this approach results in inflexibility of agents if options have an extended duration and are dynamic. While adjusting the executed option at each step improves flexibility from a single-agent perspective, frequent changes in options can induce inconsistency between an agent's actual behaviour and its broadcast intention. In order to **balance flexibility and predictability**, we propose a **dynamic termination Bellman equation** that allows the agents to flexibly terminate their options. We evaluate our model empirically on a set of multi-agent pursuit and taxi tasks, and show that our agents learn to adapt flexibly across scenarios that require different termination behaviours.


<br>
<br>

***
## **Replication-robust payoff-allocation for Submodular Cooperative Games**

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/submodular.jpg" title="Example Submodular Settings" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Example Submodular Settings
</div>

**Abstract:** **Submodular functions** have been a powerful mathematical model for a wide range of real-world applications. Recently, submodular functions are becoming increasingly important in machine learning (ML) for modelling notions such as information and redundancy among entities such as data and features. Among these applications, a key question is **payoff allocation**, i.e., how to evaluate the importance of each entity towards the collective objective? To this end, classic solution concepts from **cooperative game theory** offer principled approaches to payoff allocation. However, despite the extensive body of game-theoretic literature, payoff allocation in submodular games are relatively under-researched. In particular, an important notion that arises in the emerging submodular applications is redundancy, which may occur from various sources such as abundant data or malicious manipulations where a player replicates its resource and act under multiple identities. Though many game-theoretic solution concepts can be directly used in submodular games, naively applying them for payoff allocation in these settings may incur robustness issues against replication.
In this paper, we systematically study the replication manipulation in submodular games and investigate replication robustness, a metric that quantitatively measures the robustness of solution concepts against replication. Using this metric, we present conditions which theoretically characterise the robustness of **semivalues**, a wide family of solution concepts including the Shapley and Banzhaf value. Moreover, we empirically validate our theoretical results on an emerging submodular ML application, i.e., the ML data market.

<br>
<br>

***
## **Behavioural Strategies in Weighted Boolean Games**

**Abstract:** This paper studies the computation of mixed Nash equilibria in weighted Boolean games. In weighted Boolean games, players aim to maximise the total expected weight of a set of formulas by selecting behavioural strategies, that is, randomisations over the truth assignments for each propositional variable under their unique control. Behavioural strategies thus present a compact representation of mixed strategies. Two results are algorithmically significant: (a) behavioural equilibria satisfy a specific independence property; and (b) they allow for exponentially fewer supports than mixed equilibria. These findings suggest two ways in which one can leverage existing algorithms and heuristics for computing mixed equilibria: a naive approach where we check mixed equilibria for the aforesaid independence property, and a more sophisticated approach based on support enumeration. In addition, we explore a direct numerical approach inspired by finding correlated equilibria using linear programming. In an extensive experimental study, we compare the performance of these three approaches.
