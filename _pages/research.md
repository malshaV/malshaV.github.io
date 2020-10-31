---
title: "Research"
permalink: /research/
author_profile: true
---

UNDER CONSTRUCTION

### Designing a Cost Effective Dry Contact sEMG Sensor System for Controlling a Bionic Hand
<br>

<p>
<img src="/images/TMA.PNG" alt="TMA" style="float: left; width: 40%; margin-right: 5%; margin-bottom: 0.5em;">
<img src="/images/Hand.jpg" alt="Hand" style="float: left; width: 40%; margin-right: 5%; margin-bottom: 0.5em;">
<p style="clear: both;">
</p>


Surface Electromyogram (sEMG) signals from the forearm is widely used as a source for gesture controlled
applications and prosthesis control.This project involves development of a real-time gesture recognition algorithm using forearm sEMG signals and development of a cost effective electrode system to acquire forearm signals, with the aim of controlling a bionic arm. Most commonly used approach in hand gesture recognition tasks is to extract a set of temporal and frequency domain
features from acquired sEMG recordings and then classify them using different learning algorithms such as SVM and LDA. In these studies the sEMG recordings from electrodes placed on the forearm  are treated as individual and uncorrelated entities. However we observed a correlated nature between the signal channels whenever a gesture is elicited. Hence we came up with a novel idea of Temporal Muscle Activation Maps that can represent the individual and mutual activation
patterns of forearm muscles which was then used in real-time gesture recognition. The code and the demo of this work can be found [here.](https://github.com/Laknath1996/Real-Time-Hand-Gesture-Recognition-with-TMA-Maps)
In order to acquire sEMG signals from the forearm we developed a active, dry-contact electrode sensors to acquire high quality sEMG signals, and a final device to interface our novel finger gesture recognition algorithm with the sensors. The electrode design was fabricated and assembled on a double-sided flex printed circuit, with a small form-factor and these electrodes were interfaced with an ADS1299 Performance Demonstration Kit with STM32 F411RE Nucleo board to obtain the sEMG signals required for the gesture classification.
The electrode sensors were evaluated with a finger gesture classification experiment, and the CMRR of the sensor was experimentally characterized as well. ([TMA_maps_paper](https://ieeexplore.ieee.org/document/9054227),[Electrodes_paper](https://arxiv.org/abs/2009.02575))