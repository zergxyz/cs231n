Stanford cs231n'18
=========
Stanfor cs231n是一门介绍CNN基础概念和知识的课程。这一课程前半部分的重点在于介绍组成CNN的各种模块，包括FC, Conv, Relu, BN等等。特别是在它的assignment1和2中，作者很用心的一步一步、循序渐进的带领初学者动手编程实现每一个模块。这样，在平时的工作中，我们不但可以像搭积木一样，将这些模块一层一层的叠加起来组成我们的CNN，更重要的是，我们可以更深入的了解数据在这些模块中是怎样流动的，以及梯度又是如何在这些模块中backpropagate的。基于此，在这里将学习cs231n课程中的学习心得记录下来，内容包括：

1. 各个模块backpropagation公式的推导过程，以及在编写程序中遇到的问题解决过程。这一点很重要，因为在以后的工作中，不论是使用TensorFlow还是PyTorch,我们只需要考虑forward过程来搭建CNN，至于梯度如何backpropagate，软件会自动帮我们处理好。所以我们只知道CNN会backpropagation，但很少有机会知道它是怎样backpropagation的。而这门课程恰恰可以让我们了解每一个CNN模块backpropagation的公式推导及编程实现，这对今后处理梯度消失/爆炸的问题会很有帮助。
2. 学习作者调试CNN模块的思路和流程，包括初始值的检验，gradie check，minibatch overfitting等等。如1所述，即使我们知道了CNN的梯度是如何计算的，CNN搭建起来是如何验证的，但将它编程实现又是另外一个问题，这里面有很多细节值得我们注意。基于此，这里将按照作业的流程将其中出现的所有函数自己动手写一遍，深入了解一下作者搭建调试CNN网络的过程。

[Lecture 1](https://github.com/FortiLeiZhang/cs231n/blob/master/document/Lecture%201%20--%20%20Introduction%20to%20Convolutional%20Neural%20Networks%20for%20Visual%20Recognition.md)
