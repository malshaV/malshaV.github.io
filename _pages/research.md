---
title: "Research"
permalink: /research/
author_profile: true
---

### Designing a Cost Effective Dry Contact sEMG Sensor System for Controlling a Bionic Hand
<br>

<p>
<img src="/images/TMA.PNG" alt="TMA" style="float: left; width: 40%; margin-right: 5%; margin-bottom: 0.5em;">
</p>


<p align="justify">
Surface Electromyogram (sEMG) signals from the forearm is widely used as a source for gesture controlled
applications and prosthesis control.This project involves development of a real-time gesture recognition algorithm using forearm sEMG signals and development of a cost effective electrode system to acquire forearm signals, with the aim of controlling a bionic arm. Most commonly used approach in hand gesture recognition tasks is to extract a set of temporal and frequency domain
features from acquired sEMG recordings and then classify them using different learning algorithms such as SVM and LDA. In these studies the sEMG recordings from electrodes placed on the forearm  are treated as individual and uncorrelated entities. However we observed a correlated nature between the signal channels whenever a gesture is elicited. Hence we came up with a novel idea of Temporal Muscle Activation Maps that can represent the individual and mutual activation
patterns of forearm muscles which was then used in real-time gesture recognition. The code and the demo of this work can be found [here.](https://github.com/Laknath1996/Real-Time-Hand-Gesture-Recognition-with-TMA-Maps)
In order to acquire sEMG signals from the forearm we developed a active, dry-contact electrode sensors to acquire high quality sEMG signals, and a final device to interface our novel finger gesture recognition algorithm with the sensors. The electrode design was fabricated and assembled on a double-sided flex printed circuit, with a small form-factor and these electrodes were interfaced with an ADS1299 Performance Demonstration Kit with STM32 F411RE Nucleo board to obtain the sEMG signals required for the gesture classification.
The electrode sensors were evaluated with a finger gesture classification experiment, and the CMRR of the sensor was experimentally characterized as well. ([TMA_maps_paper](https://ieeexplore.ieee.org/document/9054227),[Electrodes_paper](https://arxiv.org/abs/2009.02575))
</p>


### Retinal and Conjunctival Vascular Tortuosity Analysis
<br>
<p align="justify">
In this research we analysed the association of retinal and conjunctival vascular tortuosity with diabetes. Previous studies in the literature suggests that the vascular tortuosity is a bio marker for any systemic diseases and these studies also suggests that the vascular tortuosity varies with the thickness of the vessels.
This creates a need of a framework that can extract vessels of a desired thickness. To this end, we propose a framework that can extract vessels of specified thicknesses from retinal fundus images or external eye images. The proposed framework consist of a vessel probability map generation step followed by few post processing steps.
The vessel probability maps are obtained using fully convolutional neural network architecture; Iternet which is trained separately to obtain vessel probability maps for retinal and external eye images. The vessels of desired thicknesses are extracted using the generated vessel probability maps and a hessian based multiscale vessel enhancement techniques.
The extracted vessels were skeletonized and  tortuosity was computed using several tortuosity indices. These calculated tortuosity values were used to analyze the association of diabetes with retinal and conjunctival vascular tortuosities.
</p>


### Deep Learning based Phase Unwrapping
<br>
<p align="justify">
Phase unwrapping is a prevalent problem in Quantitative Susceptibility Mapping (QSM) in Magnetic Resonance Imaging. The objective of phase unwrapping is to recover the true phase from a wrapped phase signal. Conventional phase unwrapping techniques are prone to errors at lower SNR values and expend a high computational time. Recently, few studies have explored the possibility of using deep learning based techniques to perform phase unwrapping under severe noise conditions and with a lower computational time. However, these deep learning based methods require large datasets for training, thus limiting the application in real- world scenarios.
Most wrapped phase images contain global spatial structures that can provide information relevant to the mapping between the wrapped phase and true phase images. However,  the existing deep learning based phase unwrapping techniques are comprised of typical Fully Convolutional Networks which ignore the spatial relationships among different local regions of a given image.
To address these shortcomings, we proposed a spatial-quad directional LSTM based encoder- decoder network architecture which predicts the true phase image for a given wrapped phase image.
The Spatial Quad-Directional Block learns the global spatial relationships between image regions passing four sequences formed by traversing the input feature maps through LSTM layers.
We trained the proposed network by using pairs of simulated wrapped phase images and true phase images and the phase images were created by adding and subtracting Gaussians of different shapes and positions.
</p>