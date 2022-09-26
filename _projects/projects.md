
**Energy Disaggregation at Substations with Behind-the-Meter Solar Generation**
------
Energy disaggregation at the substation level (EDS) estimates the energy consumption of each type of load from the aggregated measurements. At the substation level, most meters only measure at the net point so the obtained measurements are aggregated loads. It may be difficult to identify a set of pure measurements
of a certain type of load. The distribution operator may know all the loads connected to a substation, it may not know whether a particular type of load is consuming energy or not within a given time interval. Thus, each aggregate measurement is the total consumption of multiple types of loads, and the types that exist in this measurement are not fully known. We call it “partially labeled aggregate data.” We for the first time addresses the so-called “partial labels” issue in energy disaggregation and develops a model-free EDS method to separate individual loads, including BTM solar, from the total energy consumption in real-time. 



**Energy disaggregation at the substation level and illustration of partial labels**
<p align="center">
  <img src="/images/BTM_illustration.png" width="335" />
  <img src="/images/PartialLabel_illust.png" width="330" /> 
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

**The framework of proposed model**
<div  align="center">
<img src='/images/figure1-1.png' width='500'>
</div>



**Bayesian Robust Hankel Matrix Completion with Uncertainty Modeling for Synchrophasor Data Recovery**
------
Synchrophasor data suffer from quality issues like missing and bad data. Exploiting the low-rankness of the Hankel matrix of the synchrophasor data, we formulate the data recovery problem as a robust low-rank Hankel matrix completion problem and proposes a Bayesian data recovery method that estimates the posterior distribution of synchrophasor data from partial observations. In contrast to the deterministic approaches, our proposed Bayesian method provides an uncertainty index to evaluate the confidence of each estimation. To the best of our knowledge, this is the first method that provides confidence measure for synchrophasor data recovery. Numerical experiments on synthetic data and recorded synchrophasor data demonstrate that our method outperforms existing low-rank matrix completion methods.

<div  align="center">
<img src='/images/RobustMatrixCompletion.png' width='475'>
</div>
 
**Backdoor Model Detection Under Data-Scarce Regime**
------
[TrojanNet:](https://github.com/wangren09/TrojanNetDetector) We proposed **backdoor model detectors** that can effectively recognize **poisoned models** and reveal the **corresponding backdoor triggers** under the **data-limited** and **data-free** regimes.

**Trojan (backdoor) attack, frameworks, and trigger detection:**
<div  align="center">
<img src='/images/DFTND_Framework.png' width='400'>
<img src='/images/Trojan3.JPG' width='240'>
</div>


**Simultaneous Achievement of Data Privacy And Information Accuracy: Provable Privacy Protection in the Data Collection/Processing Phase**
------
We developed a **data privacy preserving framework** through quantization. We further developed an efficient data recovery method based on the nonconvex optimization and high-dimensional statistics such that the recovery error diminishes to zero. The method guarantees that any intruder accessing a small amount of data cannot reveal accurate information even with the knowledge of the quantization rule. Towards security enhancement, We developed a **distributed algorithm** such that multiple data owners could collect and process data separately and then collaboratively recover the data without sharing the raw information directly.

**Privacy protection:**
<div  align="center">
<img src='/images/Quantization_tensor.png' width='550'>
</div>

**Information extraction with prior knowledge:**
<div  align="center">
<img src='/images/DP2.png' width='330'>
</div>


**Multi-Trigger-Key: Privacy Protection in the Model Inference Phase**
------
We introduced a **Multi-Trigger-Key framework** that associates each protected task with a specifically designed trigger-key. The true information can be revealed by adding the trigger-key if the user is authorized.

**Multi-Trigger-Key Framework:**
<div  align="center">
<img src='/images/multi_trig_key.png' width='450'>
</div>





**Smart Grid Robustness and Uncertain Optimization with High-Penetration of Renewable Energy**
------
We proposed methods to **analyze the power grid robustness** and optimize the **economic dispatch** when considering highly stochastic renewable energy.


<video width="320" height="240" controls>
    <source src="/images/demo_OpenECA (3).mp4" type="video/mp4">
</video>





<!-- 
**Twitter Sentiment Analysis with Recurrent Neural Networks**
------
We implemented a recurrent neural network (LSTM) based on TensorFlow for the task of sentiment analysis on natural language data. Sentiment analysis refers to the natural language processing task of classifying some collection of the text by its polarity. We analyzed the data from Twitter ([Sentiment140 dataset](http://www.sentiment140.com/)) and try to classify it as either "positive" or "negative". The tweets can be viewed as sequences of words in natural language and form the sequantial input to the RNN model. The goal is to understand the attitude of the person that generates the text.

<div align="center">
<img src='/images/RNN.png'>
</div>
-->
