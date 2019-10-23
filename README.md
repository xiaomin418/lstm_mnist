# lstm_mnist
This project uses lstm neural networks to train the data of MNIST.

## deep learning代码

LSTM.py

利用LSTM实现手写数字识别的demo

解释mnist数据集：
Training set images: train-images-idx3-ubyte.gz (9.9 MB, 解压后 47 MB, 包含 60,000 个样本)
Training set labels: train-labels-idx1-ubyte.gz (29 KB, 解压后 60 KB, 包含 60,000 个标签)
Test set images: t10k-images-idx3-ubyte.gz (1.6 MB, 解压后 7.8 MB, 包含 10,000 个样本)
Test set labels: t10k-labels-idx1-ubyte.gz (5KB, 解压后 10 KB, 包含 10,000 个标签)

图片是以字节的形式进行存储, 我们需要把它们读取到 NumPy array 中, 以便训练和测试算法.
网上对MNIST数据集介绍：
TRAINING SET LABEL FILE (train-labels-idx1-ubyte):

[offset] [type]          [value]          [description] 
0000     32 bit integer  0x00000801(2049) magic number (MSB first) 
0004     32 bit integer  60000            number of items 
0008     unsigned byte   ??               label(rows) 
0009     unsigned byte   ??               label(cols)
........ 
xxxx     unsigned byte   ??               label
The labels values are 0 to 9.
