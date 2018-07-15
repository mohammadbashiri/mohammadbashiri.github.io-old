---
title: "Presentation at Franklin Lab"
layout: post
date: 2018-07-02 00:00
tag:
- Presentation
- FranklinLab
- Journal Club
category: blog
author: mohammadbashiri
---

## Population Coding of Conditional Probability Distributions in Dorsal Premotor Cortex

Today I presented a new paper at Franklin Lab (Sport department, Technical University of Munich) about a paper ([link]) recently publish by <a href="http://kordinglab.com/" terget="_balnk">KordingLab</a> in Nature Communication.

The authors of the paper are Joshua I. Glaser, Matthew G. Perich, Pavan Ramkumar, Lee E. Miller & Konrad P. Kording

### A short summary of the paper:

In day-to-day motor movements, we are always constrained by the physics of our body as well as the environment which in turn limits the numebr of possible movements that we can perform. In other words, considering the state of our body in the world, some movements may be more probable than others. The result is essentially a probability distribution over possible movements. The question is How does the brain represent these probability distributions?

More specifically, we are interested in the followings:

- How does such distribution effect the behavioral performance
- If the probability of possible upcoming movements effect our behavior, how is that information encoded on the neural level?
- Where in the cortex such neurons exist? (primary motor cortex versions dorsal premotor cortex)
- Single neuron versus population coding of the probability distirbution
- is the confidence in the upcoming target, position dependent (distance w.r.t the center of the workspace)?
- Are these neurons really representing upcoming movements? or they just happen to have an activity that matches our hypothesis (control)


<b>The task</b>: We have a square-shape workspace. The monkey reached sequentially to four targets, before receiving a reward. Due to the border of the workspace, upcoming targets were more likely to be presented approximately opposite to the current hand position.


Answers in short:

- The position of the hand w.r.t the borders of the workspace does actually influence the hand movement, both in trajectory and latency: Early in the reaches, trajectories were biased towards the expected target direction, defined as the  most probable direction given the distribution of target presentation. in the case of latencies, shorter latencies where elicited when the target appeared close to the expected direction. Note that latency and trajectories are not independent (i.e., deviation from trajectory, increases the latency).

- A subgroupo of neurons in dorsal premotor cortex (PMd), named "potential neurons" seem to increase their activity if the upcoming target is more probable to be similar to their preferred direction (PD).

- It appears that the population of PR neurons in PMd works together to represent probability distribution of available upcoming movements given the current hand position

- The confidence of such distribution (decoded from neural activity) increases (lower std deviation) as we move further from the center and closer to the border, which actually means neural activity is eliciting a statistical representation of possible upcoming movements.

- as a control a visuomotor task was perform. In short, the idea is that if neurons are representating a probablity distribution of possible upcoing movements given the physical state of our body in the environment, then if we now rotate the target, while keeping it visually similar, the probability distributions should also rotate. And they do!


[link]: https://www.nature.com/articles/s41467-018-04062-6

## 