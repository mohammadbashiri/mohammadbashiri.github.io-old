---
title: "Non-invasive Deep Brain Stimulation via Temporal Interference: A Computational Study"
layout: post
date: 2018-04-20 22:10
tag:
- Non-invasive DBS
- Temporal Interference
- Finite-element analysis
projects: true
hidden: false
description: "A project on modeling the effect of non-invasive deep brain stimulation via temporal interference on neurons with different membrane characteristics."
category:
author: mohammadbashiri
externalLink: false
---

# Non-Invasive Deep Brain Stimulation

This repository contains all the code used for simulation of non-invasive Deep Brain Stimulation (DBS) via Temporal Interference (TI).

## About the project

The project is inspired by a paper published on June 2017 [1], which proposed a new
method for Non-invasive DBS via two (or more) temporally interfering signals. Using the
codes available in this repo, one can visualize the distribution of electric fields (E-field) in
a spherical head model. Furthermore, using the computed electric field distribution, we
can also see the response of neurons at any point in the conductive medium (head model).

![model_concept](https://github.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/Head_model_Concept.png?raw=true)

Given that you have an E-field distribution from finite-element analysis (FEA) of any arbitrary head model,
which was also part of this project (but not covered here), a different script could be used to visualize
the distribution.

A a summary, the main focus of this repository is two-fold:
- Visualization of E-field distribution either generated from FEA or an analytical solution
- Testing the response of different neuron models at different locations within the E-field
distribution


## Electric field (E-field) distribution

In this project, I used a spherical head model, to keep things simple. The computation and
visualization of the E-field is done in Matlab (so look into the Matlab folder if you are
interested). Fir this purpose, you can choose the electrode configuration you would like to
see the distribution for, and run the code. An example of the output might look like the
following:

![e_field](https://github.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/E-field_example.png?raw=true)

## Neuron response

Once we have an E-field distribution, we probably want to see how would a neuron respond to
such electric field at different locations (after all that is the whole point - stimulating
neurons). Let us see the input and response of a neuron that is located at the center of
the distribution shown above.

![neuron_response](https://github.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/Neuron_response.png?raw=true)

## Neuron models

Here I have included several neuron models, which enables me to test the method for different
neurons models (essentially for different membrane characteristics). Neuron models included in
this repo are:

* Hodgkin Huxley (tuned to mammals) - implement in Matlab and Python
* Adaptive Exponential Integrate & Fire -  implemented in Python
* Auditory brainstem - implemented in Matlab
* Izhikevich - implemented in Python

### Reference
[1] N. Grossman et al., “Noninvasive Deep Brain Stimulation via Temporally Interfering Electric Fields,” Cell, vol. 169, no. 6,
p. 1029–1041.e16, 2017.

---

You can find the codes for this project on my github, [here](https://github.com/mohammadbashiri/non-invasive-deep-brain-stimulation).
