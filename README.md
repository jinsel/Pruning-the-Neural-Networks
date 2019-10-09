# Pruning-the-Neural-Networks
![Pruning the Neural Network](https://github.com/jinsel/Pruning-the-Neural-Networks/blob/master/image/1*4dJE_vHfGpPBtXLLXLmnBQ.png)
# **Purning**
Pruning is one of the methods for inference to efficiently produce models smaller in size, more memory-efficient, more power-efficient and faster at inference with minimal loss in accuracy, other such techniques being weight sharing and quantization. Out of several aspects that deep learning takes as an inspiration from the area of Neuroscience. Pruning in deep learning is also a biologically inspired.

## Purning helps to solve the problems of:
1) Model are getting larger<br>
2) Speed of the machine if you use CPU<br>
3) Energy Efficiency (Memory Usage)


## **Here we are comparing two different Purning techniques<br> <br>**
1) **Weight Pruning** <br> 
2) **Unit/Neuron Pruning**

#### Weight pruning
1)Set individual weights in the weight matrix to zero. This corresponds to deleting connections.<br>

2)Here, to achieve *sparsity* of k% we rank the individual weights in weight matrix W according to their magnitude, and then set to zero the smallest k%.

Tensors with several values set to zero can be considered *sparse*. This results in important benefits:
* *Compression*. Sparse tensors are amenable to compression by only keeping the non-zero values and their corresponding coordinates.
* *Speed*. Sparse tensors allow us to skip otherwise unnecessary computations involving the zero values.

#### Unit/Neuron Pruning
1)Set entire columns to zero in the weight matrix to zero, in effect deleting the corresponding output neuron.<br>

2)Here to achieve *sparsity* of k% we rank the columns of a weight matrix according to their *L2-norm* and delete the smallest k%.

#### Graph between accuracy and sparsity of Weight Pruning and Unit Pruning
![Graph](https://github.com/jinsel/Pruning-the-Neural-Networks/blob/master/image/index.png)

### Getting Started
If you want to do some research or work on Pruning the Neural Network then follow the under instructions.<br>
#### Clone 
1) Fork the Repository<br>
2) Clone this repo to your local machine using https://github.com/jinsel/Pruning-the-Neural-Networks
#### Installation
#### Tensorflow 
(Requires the latest pip)<br>
$ pip install --upgrade pip <br>
$ pip install tensorflow 

(If you want to use GPU then)<br> 
$ pip install tensorflow-gpu 

##### For Numpy 
$ pip install numpy

#### If you are using the Google Colab then:
**Enable the GPU with**: Runtime > Change runtime type > Hardware accelator and make sure GPU is selected.


## Reference:
### Research Paper and Blog
1) [To prune, or not to prune: exploring the efficacy of pruning for model compression,](https://arxiv.org/pdf/1710.01878.pdf) Michael H. Zhu, Suyog Gupta, 2017 <br>

2) [Learning to Prune Filters in Convolutional Neural Networks](https://arxiv.org/pdf/1801.07365.pdf), Qiangui Huang et. al, 2018<br>

3) https://jacobgil.github.io/deeplearning/pruning-deep-learning  Pruning deep neural networks to make them fast and small<br>

4)  [Optimize machine learning models with Tensorflow Model Optimization Toolkit](https://www.tensorflow.org/model_optimization)<br>

5)  https://www.tensorflow.org/model_optimization/guide/pruning/train_sparse_models <br>

6) https://towardsdatascience.com/pruning-deep-neural-network-56cae1ec5505 Pruning Deep Neural Networks

### Videos
1)  https://www.youtube.com/watch?v=CrDRr2fxbsg&t=656s Toward Efficient Deep Neural Network Deployment: Deep Compression and EIE, Song Han <br>

2)  https://www.youtube.com/watch?v=vouEMwDNopQ Deep Compression, DSD Training and EIE<br>





