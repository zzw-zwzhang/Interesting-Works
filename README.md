# Interesting-Works
<!-- https://latex.codecogs.com/gif.latex? -->

## SGD
- [Communication Efficient SGD via Gradient Sampling with Bayes Prior](https://openaccess.thecvf.com/content/CVPR2021/papers/Song_Communication_Efficient_SGD_via_Gradient_Sampling_With_Bayes_Prior_CVPR_2021_paper.pdf), 2021 CVPR  
- [On the Origin of Implicit Regularization in Stochastic Gradient Descent](https://arxiv.org/pdf/2101.12176.pdf), 2021 ICLR
- [A Diffusion Theory For Deep Learning Dynamics: Stochastic Gradient Descent Exponentially Favors Flat Minima](https://arxiv.org/pdf/2002.03495.pdf), 2021 ICLR
- [On the Validity of Modeling SGD with Stochastic Differential Equations (SDEs)](https://arxiv.org/pdf/2102.12470.pdf), 2021 NeurIPS
- [Rethinking the Limiting Dynamics of SGD: Modified Loss, Phase Space Oscillations, and Anomalous Diffusion](https://arxiv.org/pdf/2107.09133.pdf), 2021 NeurIPS
  1) Other works have questionedthe correctness of the using the central limit theorem to model the gradient noise as Gaussian [20], arguing that the weak dependence between batches and heavy-tailed structure in the gradient noiseleads the CLT to break down.
  2) The two conditions needed for the CLT (Central Limit Theorem) to hold are not exactly met in the setting of SGD. Independent and identically distributed. Generally we perform SGD by making a complete pass through the entire dataset before using a sample again which introduces a weak dependence between samples. **While the covariance matrix without replacement more accurately models the dependence between samples within a batch, it fails to account for the dependence between batches.** *Finite variance*. A differentline of work has questioned the Gaussian assumption entirely because of the need for finite variance random variables. This work instead suggests using the generalized central limit theorem implying the noise would be a heavy-tailed α-stable random variable. Thus, the previous assumption is implicitly assuming the i.i.d. and finite variance conditions apply for large enough datasets and small enough batches.
  3) Reference: [What is the difference between finite and infinite variance](https://stats.stackexchange.com/questions/94402/what-is-the-difference-between-finite-and-infinite-variance/100161)  
     &emsp; &emsp; &emsp;&emsp; [ANITA: An Optimal Loopless Accelerated Variance-Reduced Gradient Method](https://arxiv.org/pdf/2103.11333.pdf), 2021 arXiv  
     &emsp; &emsp; &emsp;&emsp; [Accelerating Stochastic Gradient Descent using Predictive Variance Reduction](https://proceedings.neurips.cc/paper/2013/file/ac1dd209cbcc5e5d1c6e28598e8cbbe8-Paper.pdf), 2013 NeurIPS  
   4) Large variance slows down the convergence.

- [On the Interplay between Noise and Curvature and its Effecton Optimization and Generalization](https://arxiv.org/pdf/1906.07774.pdf), 2020 AISTATS
  1) The relationship between the Hessian and the covariance matrix.  
  ![](https://latex.codecogs.com/gif.latex?\Sigma(\theta)%20\approx%20\frac{\sigma^2}{N}%20\sum_{i=1}^{N}%20x_i%20x_i^T%20=%20\frac{\sigma^2}{N}%20X^T%20X%20=%20\sigma^2%20H)
  2) The speed at which one can minimize an expected loss using stochastic methods dependson two properties: the curvature of the loss and the variance of the gradients.
  3) The distinction between the Fisher matrix, the Hessian, and the covariance matrix of the gradients.
  
- [Three Factors Influencing Minima in SGD](https://arxiv.org/pdf/1711.04623.pdf), 2018 ICANN
- [Entropy-SGD: Biasing Gradient Descent Into Wide Valleys](https://arxiv.org/pdf/1611.01838.pdf), 2017 ICLR
- [Optimization Methods for Large-Scale Machine Learning](https://arxiv.org/pdf/1606.04838.pdf), 2018 SIAM Review
- [On the Relation Between the Sharpest Directions of DNN Loss and the SGD Step Length](https://arxiv.org/pdf/1807.05031.pdf), 2019 ICLR


## Information Bottleneck
- [Disentangled Information Bottleneck](https://arxiv.org/pdf/2012.07372.pdf), 2021 AAAI


## Batch Normalization
- [Metadata Normalization](https://arxiv.org/pdf/2104.09052.pdf), 2021 CVPR
- [Cross-Iteration Batch Normalization](https://arxiv.org/pdf/2002.05712.pdf), 2021 CVPR
- [Stochastic Whitening Batch Normalization](https://arxiv.org/pdf/2106.04413.pdf), 2021 CVPR
- [Learning Intra-Batch Connections for Deep Metric Learning](https://arxiv.org/pdf/2102.07753.pdf), 2021 ICML
- [Padé Activation Units: End-to-end Learning of Flexible Activation Functions in Deep Networks](https://arxiv.org/pdf/1907.06732.pdf), 2020 ICLR


## Physics & ML
- [Hidenori Tanaka](https://sites.google.com/view/htanaka/home)


## Random Matrix Theory
- [Geometry of Neural Network Loss Surfaces via Random Matrix Theory](https://dl.acm.org/doi/pdf/10.5555/3305890.3305970), 2017 ICML
- [Nonlinear Random Matrix Theory for Deep Learning](https://papers.nips.cc/paper/2017/file/0f3d014eead934bbdbacb62a01dc4831-Paper.pdf), 2017 NeurIPS
  1) Analysis of the eigenvalues of the data covariance matrix.
- [Random Matrix Theory Proves that Deep Learning Representations of GAN-data Behave as Gaussian Mixtures](http://proceedings.mlr.press/v119/seddik20a/seddik20a.pdf), 2020 ICML
- [Applicability of Random Matrix Theory in Deep Learning](https://arxiv.org/pdf/2102.06740v1.pdf), 2021 arXiv
- [Random Matrices in Machine Learning](https://afia.asso.fr/wp-content/uploads/2018/09/Stats-IA_RCouillet-2.pdf), 2018
- [Why Deep Learning Works:Implicit Self-Regularization in Deep Neural Networks](http://helper.ipam.ucla.edu/publications/mlpws2/mlpws2_16011.pdf), 2019 Slide


## Covariance Matrix
- [Hidenori Tanaka](https://sites.google.com/view/htanaka/home)
- [Matrix Power Normalized Covariance Pooling For Deep Convolutional Networks](http://peihuali.org/iSQRT-COV/index.html)


## Image Generation
- [Infinite Nature: Perpetual View Generation of Natural Scenes from a Single Image](https://infinite-nature.github.io/), 2021 ICCV Oral
- [Repopulating Street Scenes](https://grail.cs.washington.edu/projects/repop/), 2021 CVPR
- [No Shadow Left Behind: Removing Objects and their Shadows using Approximate Lighting and Geometry](http://grail.cs.washington.edu/projects/shadowremoval/), 2021 CVPR
- [Repopulating Street Scenes](https://arxiv.org/pdf/2103.16183.pdf), 2021 CVPR
- [People as Scene Probes](https://arxiv.org/pdf/2007.09209.pdf), 2020 ECCV
- [TediGAN: Text-Guided Diverse Face Image Generation and Manipulation](https://github.com/IIGROUP/TediGAN), 2021 CVPR
- [Object-Centric Learning with Slot Attention](https://arxiv.org/pdf/2006.15055.pdf), 2020 NeurIPS
- [Decomposing 3D Scenes into Objects via Unsupervised Volume Segmentation](https://stelzner.github.io/obsurf/), 2021 arXiv


## Virtual Try-On
- [Self-Supervised Collision Handling via Generative 3D Garment Models for Virtual Try-On](https://arxiv.org/pdf/2105.06462.pdf), 2021 CVPR
- [SMPLicit: Topology-aware Generative Model for Clothed People](https://arxiv.org/pdf/2103.06871.pdf), 2021 CVPR
