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

