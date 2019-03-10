# Adversarial-attacks-and-defenses
A curated list of adversarial learning resources

	
With the widespread application of artificial intelligence and machine learning technology in various fields, some recent work has demonstrated that some current models are quite vulnerable to adversarial examples, for example, inputs that are almost indistinguishable from natural data and yet classified incorrectly by the network. 
Adversarial examples expose regions of the input space where the model performs poorly, which can aid in understanding and improving the model. 

## Table of Contents
### Attacks     
 - [CV](#CV)
 - [NLP](#NLP)
 - [RL](#RL)
### Defenses
- [Modify the training process](#Modify the training process)
- [Modify the input data](#Modify the input data)
- [Modify Network](#Modify Network)
- [Networks adjunction](#Networks adjunction)
 

## CV
 **Classification**
 * [DeepFool: a simple and accurate method to fool deep neural networks](https://arxiv.org/abs/1511.04599), S. Moosavi-Dezfooli et al., CVPR 2016
 * [The Limitations of Deep Learning in Adversarial Settings](https://arxiv.org/abs/1511.07528), N. Papernot et al., ESSP 2016
 * [Transferability in Machine Learning: from Phenomena to Black-Box Attacks using Adversarial Samples](https://arxiv.org/abs/1605.07277), N. Papernot et al., arxiv 2016
 * [Adversarial Examples In The Physical World](https://arxiv.org/pdf/1607.02533v3.pdf), A. Kurakin et al., ICLR workshop 2017 
 * [Delving into Transferable Adversarial Examples and Black-box Attacks](https://arxiv.org/abs/1611.02770) Liu et al., ICLR 2017
 * [Towards Evaluating the Robustness of Neural Networks](https://arxiv.org/abs/1608.04644) N. Carlini et al., SSP 2017
 * [Practical Black-Box Attacks against Deep Learning Systems using Adversarial Examples](https://arxiv.org/abs/1602.02697), N. Papernot et al., Asia CCS 2017
 * [Privacy and machine learning: two unexpected allies?](http://www.cleverhans.io/privacy/2018/04/29/privacy-and-machine-learning.html), I. Goodfellow et al.
 
## NLP
**Speech Recognition**
* [Audio Adversarial Examples: Targeted Attacks on Speech-to-Text](https://arxiv.org/abs/1801.01944), N. Carlini et al., arxiv 2018

**Questiona Answering System**
* [Adversarial Examples for Evaluating Reading Comprehension Systems](https://arxiv.org/abs/1707.07328), R. Jia et al., EMNLP 2017

 
 ## RL
* [Adversarial attacks on neural network policies](https://arxiv.org/abs/1702.02284), S. Huang et al, ICLR workshop 2017
* [Tactics of Adversarial Attacks on Deep Reinforcement Learning Agents](https://arxiv.org/abs/1703.06748), Y. Lin et al, IJCAI 2017
* [Delving into adversarial attacks on deep policies](https://arxiv.org/abs/1705.06452), J. Kos et al., ICLR workshop 2017
 
 
 
## Modify the training process

**Adversarial Training**
  
Adversarial training provides a means of regularizing supervised learning algorithms to reduce overfitting. 
It uses labels while training models which use supervised cost because the labels appears in the cost function that the adversarial perturbation is designed to maximize. 
However, this method requires making small perturbations to numerous entries of the input vector and will increase the training/data size. 

***Virtual Adversarial Training***
 * [Adversarial training methods for semi-supervised text classification.](https://arxiv.org/abs/1605.07725),  Miyato, T.; Dai, A. M.; and Goodfellow, I. 2016. 
They proposed virtual adversarial training method for semi-supervised text classification and it can smooth the output contribution of neuron networks.

***Stability training***


**Foveation-based defense**

* [Foveation-based Mechanisms Alleviate Adversarial Examples.](https://arxiv.org/abs/1511.06292)
Foveation is defined as a transformation of the image that selects a region in which the CNN is applied, discarding the information from the other regions.
The foveation provides an input to the CNN that always has the same size, even if the size of the selected region varies. 
In this way, the foveation may produce a change of the position and scale of the objects in the input of the CNN. 
It is well-known that the representations learned by the CNNs are robust to changes of scale and position of the objects, and the transformation produced by the foveation does not negatively affect the performance of the CNN. 
Also, the foveation mechanism does not introduce non-linearities, it does not modify pixel values from the original image, and the interpolations for re-sizing the image are linear. Without loss of generality, the foveation mechanism can be used as a crop of a region that includes most of the object or the whole object.


##Attacks wth GAN
* [Generating Natural Adversarial Examples.](https://arxiv.org/abs/1710.11342)
* [Learning Universal Adversarial Perturbations with Generative Models.](https://arxiv.org/abs/1708.05207)
