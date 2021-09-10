
# RL-Medical

Multiagent Deep Reinforcement Learning for Anatomical Marker Detection using PyTorch.

## Introduction

Accurate detection of anatomical markerss is an essential step in several medical imaging tasks. This repository implements a novel communicative multi-agent reinforcement learning system to automatically detect markers in 3D medical images. This algorithm enables the agents to learn explicit communication channels, as well as implicit communication signals by sharing certain weights of the architecture among all the agents.

10 brain MRI scans each with 20 markers annotated from the ADNI dataset are included in the `data` folder for convenience.

## Results
Here are a few examples of the learned agents on unseen data:

* An  example  of  our  proposed  algorithm  system  consisting  of  5  agents.  These agents are looking for 5 different markers in a brain MRI scan. Each agent’s ROI is represented by a yellow box and centered around a blue point, while the red point is the target marker. ROI is sampled with 3mm spacing at the beginning of every episode. The length of the circumference of red disks denotes the distance between the current and target markers in z-axis.
<p align="center">
<img src="./doc/brain_5_agents.gif">
</p>

* Similarly, 5 algorithm agents in fetal ultrasounds scans.
<p align="center">
<img src="./doc/fetal_5_agents.gif">
</p>

* Detecting the apex point in short-axis cardiac MRI [(HQ video)](doc/cardiac_apex.mp4)
<p align="center">
<img src="./doc/cardiac_apex.gif" width="255">
</p>

* Detecting the anterior commissure (AC) point in adult brain MRI [(HQ video)](doc/brain_ac.mp4)
<p align="center">
<img src="./doc/brain_ac.gif" width="255">
</p>

* Detecting the cavum septum pellucidum (CSP) point in fetal head ultrasound [(HQ video)](doc/fetal_csp.mp4)
<p align="center">
<img src="./doc/fetal_csp.gif" width="255">
</p>
