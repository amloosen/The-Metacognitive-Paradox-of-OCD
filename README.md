# The-Metacognitive-Paradox-of-OCD
Loosen et al. (in preparation) The metacognitive paradox of OCD: confidence is globally reduced but shows increased sensitivity to local evidence

## Overview
This repository contains the data analysis and model implementation for a study conducted at the University College London (UCL) and Yale School of Medicine.
Participants played a novel intra- and extra-dimensional shift task with integrated confidence ratings.  

This repository contains code in Python for the behaviorala analysis (1) and the implementation of a Bayesian Observer model to capture how confidence ratings should develop under a Bayes-optimal framework (2), given task information and decision evidence. The resulting parameters from this model are analyzed in relation to the group status (3; patient vs. control).

---
# Required
Please download the data on [OSF](https://osf.io/c6tnx/). Download the data from OSF and place the CSV files in a folder named data/ at the root of this repository.
Add an empty sub-folder called "figures".

## Content of the Repository
1. **Data Analysis**:
   - Exploring group-level differences in task performance and confidence ratings.
      -  PreprocBehavAnalysis
    
2. **Bayesian Observer Model**:  
   - BayesianObserver: Simulates confidence trajectories of a Bayes-optimal observer, who knows task rules and is exposed to the specific task run of a given participant.
   - BayesianObserver-BehavAnalysis: As to be run after the BayesianObserver and links resulting parameters to behavioral data.
     
---
