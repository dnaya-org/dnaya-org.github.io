---
title: "Motivation"
date: 2020-12-15T13:20:39-03:00
draft: true
---

Two common machine learning tasks are *data classification* and *data
clustering*. Among the techniques to solve them, graph-based (or
complex-network-based) ones show interesting properties.  Such methods usually
have two steps:

1. *Graph formation*: a graph representation of the dataset is constructed
   following some specific rules.
2. *Optimization*: a objective function (a loss function and a regularizer) is
   associated with the graph structure.  The optimal solution also solves the
   underlying machine-learning task.

Particularly, clustering tasks can be solved using *community detection*
methods -- for example, using modularity optimization.  Similarly, graph-based
semi-supervised learning solves classification problems in a transductive
manner.

Among the advantages of such methods, we highlight:

- *Versatility*.  Several methods can be employed to construct the graph that
  represents the dataset, including techniques to deal with tabular data,
  images, time series, etc.  As a result, they work well in many different contexts.
- *Robust even with few data samples*.  They don't require large datasets to
  achieve good results.  In the classification scenario, few labeled samples
  are required.
- *Explicit and interpretable*.  The objective function is known, so it is
  usually easy to understand the results.

However, they exhibit a major drawback: solving the optimization problem is
usually unfeasible for large datasets.  The obvious work-around is using
heuristics to find suboptimal solutions.

Early heuristic optimization methods, such as genetic algorithms (GA) and ant
colony optimization (ACO), exploit nature- and bio-inspired processes that
minimize a cost inherently. However, they rely on ad-hoc computational models for
the actions and interactions of autonomous agents with the intent to assess
their effects on the system as a whole.  As a result, they show strong
stochastic behavior leading to a series of downsides, such as instability and
low comprehension of the global dynamics.

In this specific context (graph-based methods), recent advances in Network
Science and Complex Systems gave rise to interesting heuristics based on
collective dynamics to solve machine learning problems.

> Consult
> [Verri's thesis](https://teses.usp.br/teses/disponiveis/55/55134/tde-18102018-113054/en.php)
> for a more detailed motivation of using collective dynamics as heuristics to
> solve these problems.

In the next section, we expose collective dynamics to solve machine learning
tasks.
