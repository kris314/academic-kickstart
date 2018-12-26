+++
title = "Feature Learning and Embedding Techniques"

date = 2017-05-20T00:00:00
# lastmod = 2018-09-09T00:00:00

draft = false  # Is this a draft? true/false
toc = true  # Show table of contents? true/false
type = "docs"  # Do not modify.


# Add menu entry to sidebar.
# linktitle = "Example Page"
[menu.teaching]
  parent = "Courses"
  weight = 1
+++

In recent years, in the field of vision and other AI problems, there has been a paradigm shift in the way we represent features. Feature learning has been a common buzzword due to the resurgence of neural networks with much bigger architectures, data and efficient optimization techniques. Deep Learning as referred to these learnable machines due to their enormous number of parameters has taken its own place in the field of machine learning with a large research community base, trying to solve complex real world problems. The course is divided into four parts:

## **BoWs and Encoding Techniques**
In the first part of the course, we begin with the state of art feature descriptors used prior to deep learning (before 2012). 

### Sub-Topics
* Bag of Words (BoWs)
    * Learning visual vocabulary
    * Coding and Pooling
    * Ranking and Retrieval
    * Geometric Verification
    * Inspiration from IR domain
* Advanced coding schemes
    * Kernel code books, Sparse Coding and Locally constrained linear coding.
    * VLADs, Fisher Vector and Super Vector

#### Course Material: [Link](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T1-BoWandBeyond.pdf)

## **Convolutional neural networks**
In the major theme of the course, we start with fundamentals of a convolutional neural network (CNN), different layers, loss functions and also visualize the features learnt implicitly in each individual layer. We also discuss some of the major architectures proposed from 2012-2016 which got attention since they were winning entries of Large Scale Visual Recognition challenge. We also see how these architectures enable building image retrieval applications. Here we begin with the metric learning problem which uses ranking and similarity based loss functions. We later present a case study of some recent architectures used for instance based  retrieval using deep neural networks while also revisiting some of the concepts from pooling, feature aggregation used from prior deep learning era.

### Sub-Topics
* Paradigm Shift: Feature engineering to feature learning
    * Simple feed forward network
    * Convolutional Network
    * Basics, Activation functions, Layers
        * Training and Loss functions
        * Generalization: Dropouts
    * Visualizing CNNs using
        * Deconvnets and Saliency maps
    * Transfer Learning
    * Some Practical Aspects
* Advanced NN architectures - Case Studies
    * LeNet, AlexNet, Overfeat, VGG, GoogLeNet, ResNet
* CNNs: Beyond 0/1 Loss Functions: Metric Learning
    * Basics in Metric Learning (Mahalanobis, LMNN)
    * Constrastive Loss (Siamese Architecture) and applications (dimensionality reduction and face verification)
    * Triplet Loss, Mining hard examples and application (face verification)
* Instance level retrieval and matching
    * Visual instance retrieval
        * Image retrieval using Deep Networks
    * Neural Codes for Image Retrieval
        * Multi-Scale Orderless Pooling
        * Sum Pooled Convolutional Features
        * Integral Max Pooling
        * Magnet Loss
    * Case Study: Deep Image Retrieval (Gordo et. al. ECCV’16)

#### Course Material: [Link1](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T2-CNNs.pdf), [Link2](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T3-ModernCNNArchitectures.pdf), [Link3](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T4-DistanceMetricLearningBeyond0-1Loss.pdf), [Link4](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T5-VisualInstanceRetrieval.pdf)

## **Soft Attention Models in Deep Networks**
In the third part of the course, we delve into generative methods where we start with a LSTM model used as a predictive network. We later introduce a recent class of generative models called as variational autoencoders (VAE). We further introduce a new learning module called as attention interface which empowers learning with sequential data such as handwriting, text and speech. As a case study, we present the DRAW architecture which uses LSTM architecture and utilizes the concepts from VAE and attention mechanism to generate 2D images.

### Sub-Topics
* Motivation for attention models
* Primer on Prediction using RNNs
    * Handwriting prediction
    * Handwriting synthesis
* Basics in variational autoencoders
* Deep Recurrent Attentive Writer

#### Course Material: [Link](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T6-SoftAttentionModelsinDeepNetworks.pdf)

## **Word Embedding techniques**
In the last part of the course, we introduce the concept of word embedding technique which is used in many NLP application to encode the discrete words into continous space where the semantic relationships are explicit. Here we discuss neural language modeling and present the prominent embedding technique using word2vec.

### Sub-Topics
* Introduction to language modelling and classical topic modeling methods.
* Neural language model and discussion on issues of tradtional softmax layer.
* Recent word embedding models:-
    * C&W Model
    * Word2Vec (Continous BoWs and Skip grams)
        * Hierarchical Softmax
        * Noise Contrastive Estimation
        * Negative Sampling

#### Course Material: [Link](https://researchweb.iiit.ac.in/~praveen.krishnan/compreExam/slides/T7-WordEmbedding.pdf)