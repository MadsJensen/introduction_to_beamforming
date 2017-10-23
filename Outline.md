# Introduction to source localization with beamfomers


## 1. General idea of workshop

Background information and hands-on sessions. <br/>
Hands-on will be done with MNE-Python.


## 2. Prerequisites for the course

1. MNE-Python and dependencies should be installed on computer (refer to MNE homepage, conda environment?)



## 3. Outline

1. What is source localization? <br/> From topo plot to source plot, activity measured at scalp as superposition of source activity: how can we get back to source space?

2. What is a beamformer? <br/> Source localization as ill-posed problem, beamformer as one technique to solve it.

3. How does a beamformer work?  <br/> Short overview of necessary steps (coregistration, forward model, creating and applying a filter = inverse solution) before addressing those steps in greater detail.

4. The forward model. <br/> What is the forward model, why do I need it and how do I compute it? <br/> _Hands on #1: Preparing your data: coregistration, segmentation, and meshes_ <br/>

5. The spatial filter.  <br/> What does the spatial filter do? Which ingredients are needed (special consideration here: covariance matrix).  <br/> _Hands on #2: Preparing your data for computing a covariance matrix_  <br/>  _Hands on #3: Constructing a spatial filter_

6. Applying the spatial filter. <br/> Relation between filter (i.e., covariance matrix) and data input (common filters etc.), source reconstruction of evoked signals vs single trials, ...  <br/>
_Hands on #4: Applying the spatial filter and visualizing the results_

7. Sandbox: playing around with beamformer inputs?

8. Discussion/questions etc. for those who cannot get enough :smile:


## 4. Questions / problems / brainstorming

- Which example data set should we use?
- Would we want to tackle the following topics:
  - use of noise covariance (whitening) - also relates to the usage of different sensor types so might be relevant here
  - for minimum norm people: what are the practical differences of MNE and beamforming solutions?
  - how much of point 4 should be computed during the workshop (computation time)
  - just for completeness: ``reduce_rank`` option is implemented now, but MNE-Python does warn the user when it is _needed_ (i.e., with spherical models), so we do not need to get in detail
- Workshop code management: ``ipynb`` or code snippets
