# The Metacognitive Paradox of OCD
Loosen AM, Zaboski BA, Moore AS, Bohner C, Pushkarskaya H, Pittenger C*, Hauser TU* (2026).
The metacognitive paradox of OCD: confidence is globally reduced but shows increased
sensitivity to local evidence. *Translational Psychiatry*.

## Overview
This repository contains the data analysis and Bayesian learner implementation for a study
conducted at University College London (UCL) and the Yale School of Medicine. Patients
with OCD and healthy control participants played a novel intra- and extra-dimensional shift
task with integrated confidence ratings.

The repository includes Python code for the implementation of a Bayesian Observer model
to capture how confidence ratings should develop under a Bayes-optimal framework, given
task information and decision evidence (1). It also includes code to reproduce the
behavioral analysis (2) reported in the manuscript.

---
## Setup
Download the data from [OSF](https://osf.io/c6tnx/) and place the CSV files in a folder named `data/` at the root of this repository. Create the environment from `environment.yml`. Run `BayesianObserver` first, which writes the certainty estimates that the other notebooks read.

## Content of the Repository
1. **Bayesian Observer Model**:
   - BayesianObserver: Produces certainty trajectories of a Bayes-optimal learner that
     knows the task structure and infers the currently rewarded rule from trial-by-trial
     feedback, exposed to the specific task run of a given participant.

2. **Behavioral Analysis**
   - PreprocBehavAnalysis: Analyzes group-level differences in behavioral and (meta-)cognitive task measures.
   - BayesianObserver-BehavAnalysis: Links the certainty estimates from the Bayesian Observer to behavioral data.
---