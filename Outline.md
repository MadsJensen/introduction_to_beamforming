# Introduction to source localization with beamformers @ CFIN


## 1. General idea of the workshop

This workshop will contain background information about beamforming, intermixed with hands-on sessions where we will apply a beamformer pipeline to MEG data. <br/>
The hands-on will be done in [MNE-Python](https://www.martinos.org/mne/stable/index.html).


## 2. Prerequisites for the course

MNE-Python and dependencies should be installed on the computer, further information will be available before the workshop.



## 3. Outline

1. What is source localization? <br/> From topo plot to source plot -  how can we get back to source space?

2. What is a beamformer? <br/> Source localization as ill-posed problem, beamformer as one technique to solve it.

3. How does a beamformer work?  <br/> Short overview of necessary steps (coregistration, forward model, creating and applying a filter) before addressing those steps in greater detail.

4. The forward model. <br/> What is the forward model, why do I need it and how do I compute it? <br/> _Hands on #1: Preparing your data: coregistration, segmentation, and meshes_ <br/>

5. The spatial filter.  <br/> What does the spatial filter do? Which ingredients are needed (special consideration here: covariance matrix).  <br/> _Hands on #2: Preparing your data for computing a covariance matrix_  <br/>  _Hands on #3: Constructing a spatial filter_

6. Applying the spatial filter. <br/> Relation between filter (i.e., covariance matrix) and data input (common filters etc.), source reconstruction of evoked signals vs single trials, ...  <br/>
_Hands on #4: Applying the spatial filter and visualizing the results_

7. Sandbox: playing with the data

8. Discussion/questions etc. 
