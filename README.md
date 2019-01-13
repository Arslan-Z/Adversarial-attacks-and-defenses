# Adversarial-attacks-and-defenses
A curated list of adversarial learning resources

	
Some current models are quite vulnerable to adversarial examples, for example, inputs that are almost indistinguishable from natural data and yet classified incorrectly by the network. 

Adversarial examples expose regions of the input space where the model performs poorly, which can aid in understanding and improving the model. 

By using these examples as training data, adversarial training learns models that are more robust, and may even perform better on non-adversarial examples. 


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
 * 
 
 
 
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
