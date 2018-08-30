---
title: "Non-invasive Deep Brain Stimulation via Temporal Interference: A Computational Study"
layout: post
date: 2016-01-23 22:10
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

![model_concept](https://raw.githubusercontent.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/Head_model_Concept.png)

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

![e_field](https://github.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/Head_model_Concept.png?raw=true)

## Neuron response

Once we hae an E-field distribution, we probably want to see how would a neuron respond to
such electric field at different locations (after all that is the whole point - stimulating
neurons). Let us see the input and response of a neuron that is located at the center of
the distribution shown above.

![neuron_response](https://raw.githubusercontent.com/mohammadbashiri/non-invasive-deep-brain-stimulation/blob/master/Figures/Neuron_response.png)

## Neuron models

Here I have included several neuron models, which enables me to test the method for different
neruons models (essentially for different membrane characteristics). Neuron models included in
this repo are:

* Hodgkin Huxley (tuned to mammals) - implement in Matlab and Python
* Adaptive Exponential Integrate & Fire -  implemented in Python
* Auditory brainstem - implemented in Matlab
* Izhikevich - implemented in Python

## Running the codes

To familiarize with, and run, the codes do the following steps:

* Clone the repo
* Install the dependencies
    ```bash
    $ pip install numpy scipy matplotlib ipython jupyterlab
    ```
* Go through the examples. Examples are available in the corresponding Python and Matlab folders.

### You see a bug?

If you see anything wrong with the code, or you would like to suggest a change, I would be more
than happy to communicate. There are two ways to communicate (and/or contribute):
- Easiest way (which might also take some time for the change to be implemented) is to
email me at mohammadbashiri93@gmail.com, with the description of the problem you are facing.
- Through Git
- Fork the repo, clone it from your own account, make a (descriptive) branch, implement
the change, push it to your own remote repo, make a pull request to my repo.

### Reference
[1] N. Grossman et al., “Noninvasive Deep Brain Stimulation via Temporally Interfering Electric Fields,” Cell, vol. 169, no. 6,
p. 1029–1041.e16, 2017.
