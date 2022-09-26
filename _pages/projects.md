---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---
**Overview**
------
My current research is working on some of the basic questions in power systems:  1. How can data-driven methods estimate the renewable energies such as solar generations without fully labeled historical data? 2. Can algorithm provide uncertainty measure to measure the reliability of the disaggregation results?
3. How to provide a confidence measure for synchrophasor data recovery and how to recover simultaneous and consecutive data corruptions?  4. How to recover the missing/bad data with nonlinear dynamics?



**Energy Disaggregation at Substations with Behind-the-Meter Solar Generation**
------
Energy disaggregation at the substation level (EDS) estimates the energy consumption of each type of load from the aggregated measurements. At the substation level, most meters only measure at the net point so the obtained measurements are aggregated loads. It may be difficult to identify a set of pure measurements
of a certain type of load. The distribution operator may know all the loads connected to a substation, it may not know whether a particular type of load is consuming energy or not within a given time interval. Thus, each aggregate measurement is the total consumption of multiple types of loads, and the types that exist in this measurement are not fully known. We call it “partially labeled aggregate data.” We for the first time addresses the so-called “partial labels” issue in energy disaggregation and develops a model-free EDS method to separate individual loads, including BTM solar, from the total energy consumption in real-time. 



**Energy disaggregation at the substation level and illustration of partial labels**
<p align="center">
  <img src="/images/BTM_illustration.png" width="300" />
  <img src="/images/PartialLabel_illust.png" width="300" /> 
</p>

**Proposed mathmatical model**
<p align="center">
  <img src="/images/partiallabel_equation.png" width="335" />
  <img src="/images/Dictionary-1.png" width="335" /> 
</p>



**Bayesian Energy Disaggregation at Substations with Uncertainty Modeling**
------
The existing energy disaggregation method cannot provide any reliability measure of the disaggregation results, while the disaggregation accuracy can vary significantly for different data due to the volatility of loads such as the solar generation. We proposes a Bayesian-dictionary-learning-based approach to disaggregate the loads and provides an uncertainty measure of the returned estimation. Our approach learns the probability distributions of the load patterns and the decomposition coefficients from recorded data with partial labels at the offline stage. In real-time disaggregation of the obtained aggregate data, our approach computes the mean and covariance of the probability distribution of each load consumption, estimates the load using the mean, and computes the uncertainty index based on the covariance. 

**Diaggregation results of existing method (without the uncertainty measure):**
<div  align="center">
<img src='/images/net.png' width='200'>
<img src='/images/Case21Fig1 (1).png' width='200'>
  <img src='/images/Case21Fig2 (1).png' width='200'>
  <img src='/images/Case21Fig3 (1).png' width='200'>
</div>

**Diaggregation results of proposed method (provide the uncertainty measure)**
<div  align="center">
<img src='/images/net.png' width='200'>
<img src='/images/Case4Fig1 (1).png' width='200'>
  <img src='/images/Case4Fig2 (1).png' width='200'>
  <img src='/images/Case4Fig3 (1).png' width='200'>
</div>

**The framework of proposed graphic model**
<div  align="center">
<img src='/images/figure1-1.png' width='500'>
</div>



**Bayesian Robust Hankel Matrix Completion with Uncertainty Modeling for Synchrophasor Data Recovery**
------
Synchrophasor data suffer from quality issues like missing and bad data. Exploiting the low-rankness of the Hankel matrix of the synchrophasor data, we formulate the data recovery problem as a robust low-rank Hankel matrix completion problem and proposes a Bayesian data recovery method that estimates the posterior distribution of synchrophasor data from partial observations. In contrast to the deterministic approaches, our proposed Bayesian method provides an uncertainty index to evaluate the confidence of each estimation. To the best of our knowledge, this is the first method that provides confidence measure for synchrophasor data recovery.

**Recovery results of proposed method (provide the uncertainty measure)**

Additional Gaussian noise is added during time 5.6 to 6.6 seconds. The subfigures are (a) the observed data, (b) the estimated data, (c) the estimated data in one channel (d) the uncertainty index for the channel in (c).

<div  align="center">
<img src='/images/M2obR0.png' width='200'>
<img src='/images/M2estimationR0.png' width='200'>
  <img src='/images/M2uncertaintyR0.png' width='200'>
  <img src='/images/M2varianceR0.png' width='200'>
</div>

**The framework of proposed graphic model**

<div  align="center">
<img src='/images/RobustMatrixCompletion.png' width='675'>
</div>
 


**Bayesian High-Rank Hankel Matrix Completion for Synchrophasor Data Recovery**
------
The existing works exploit the Hankel low-rankness of the PMU data. However,many PMU data do not satisfy the low-rank property because of the nonlinear dynamics. Applying the approximate low-rankness to the PMU data recovery sometimes leads to degradation of the recovery performance. We develop a new Bayesian method to implicitly map the high-rank nonlinear data into the high dimensional space by the kernel trick. We propose to exploit the lifted low-rankness of the Hankel matrix of the data in the high dimensional space, although the rank of the data in the original low dimensional space is high. 

**Comparison of recovery results of proposed high-rank method with two low-rank methods**

The subfigures are (a) the observed data, (b) the estimated data by our method, (c) the estimated data by Bayesian low-rank method (d) the estimated data by deterministic low-rank method.

<div  align="center">
<img src='/images/obM3.png' width='200'>
<img src='/images/NewM3.png' width='200'>
  <img src='/images/SAPM3.png' width='200'>
  <img src='/images/OldM3.png' width='200'>
</div>




**Streaming Synchrophasor Data Quality (SSDQ) Software for EPRI**
------
I also mentor several undergraduate students to implement the our developed data recovery algorithms on Matlab and OpenPDC/OpenECA platform. OpenPDC is an open source platform for streaming synchrophasor data, used by ISO New England, the Tennessee Valley Authority (TVA), Southern Company, Southwest Power
Pool (SPP).


**Demo of developed software on OpenECA and Matlab GUI Platform**
<video width="320" height="240" controls>
    <source src="/images/demo_OpenECA (3).mp4" type="video/mp4">
</video>

<video width="320" height="240" controls>
     <source src="/images/demo_SSDQ2 (2).mp4" type="video/mp4">
</video>


<!-- 
**Twitter Sentiment Analysis with Recurrent Neural Networks**
------
We implemented a recurrent neural network (LSTM) based on TensorFlow for the task of sentiment analysis on natural language data. Sentiment analysis refers to the natural language processing task of classifying some collection of the text by its polarity. We analyzed the data from Twitter ([Sentiment140 dataset](http://www.sentiment140.com/)) and try to classify it as either "positive" or "negative". The tweets can be viewed as sequences of words in natural language and form the sequantial input to the RNN model. The goal is to understand the attitude of the person that generates the text.

<div align="center">
<img src='/images/RNN.png'>
</div>
-->
