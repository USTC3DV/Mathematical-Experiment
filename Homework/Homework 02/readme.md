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

## 说明：
1. 我们同时提供关于泊松融合的 Matlab 和 C++ 框架；
2. C++ 框架下，要求 `VS 2019`、`Qt 5.15.2 的 MSVC 2019 64-bit`、 `Eigen 3.4.0`、`Opencv` 或以上版本，我们已编译好并生成了解决方案 `Poisson.sln`；
- 如果你没有 C++ 基础，请先阅读并学习简单的[C++类以及封装、多态、继承](./C++学习笔记.md)知识学习，再去读懂框架中相关类及其成员的定义与实现；
- 有关 [QT的安装与配置](./框架/QT安装与配置.md) 请参见相关文档以及内部链接指导；
- Opencv 和 Eigen 的配置较为简单或类似与 QT 的环境配置，请自行查阅相关官方文档进行学习配置；
- 在读懂 C++ 框架的前提下，具体本次作业需要实现什么，请参见[说明文档](./框架/代码框架说明及待做事项.md)。
3. Matlab框架下，只需补充 `blendImagePoisson.m` 文件中的 `TODO: compute blended image` 内容。
