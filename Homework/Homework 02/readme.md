# Homework 02

### 内容一：图像的泊松融合
1. 将某张图（从某张图⾥⾯取⼀部分或者这张图本身）放到另外⼀张图的某个位置，采⽤泊松融合⽅法进⾏图像融合；
2. 根据所讲述的算法原理构造相应的线性⽅程组进⾏求解。


### 内容二： 基于0范数的图像光滑
1. 掌握Image Smoothing via L0 Gradient Minimization的算法原理；
2. 并根据算法原理读懂作者所提供的[代码](http://www.cse.cuhk.edu.hk/~leojia/projects/L0smoothing/L0smoothing.zip)，并⽤代码所附图像之外的⾄少五张图像进⾏测试，并修改算法中的不少于五组不同参数来测试算法效果。

## 作业要求：
- 编程语⾔不限；
- ⽤Eigen库来实现矩阵、向量的表示，线性⽅程组的求解；
- 泊松融合的矩阵，要⽤Eigen中的稀疏矩阵格式来构造；
- 尝试Eigen中所提供的不同Sparse Linear Solver进⾏求解，并对⽐不同solver的求解效率。
