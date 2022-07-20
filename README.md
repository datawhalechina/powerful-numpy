# 巨硬的NumPy

`巨硬的NumPy` 教程包括两部分：《从小白到入门》和《从入门到熟练》。

- 《从小白到入门》旨在帮助没有基础的同学快速掌握 `numpy` 的常用功能，保证日常绝大多数场景的使用。
- 《从入门到熟练》目的是帮助有进一步需要的同学对 `numpy` 进行更深入地了解，主要包括基本概念、操作，原理分析和例子。

设计思想：

- 两部分侧重点不同的教程
- 章节互相独立可单独学习


## 从小白到入门

### 原则

- 偏实用高频 API
- 展示实际用法
- 简单直接

### 大纲

>已列出重要接口。

- [创建和生成](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#创建和生成)
    - [从 python 列表或元组创建](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#从-python-列表或元组创建)
    - [使用 arange 生成](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#使用-arange-生成)
    - [使用 linspace/logspace 生成](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#使用-linspace/logspace-生成)
        - [`np.linspace`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.linspace)
    - [使用 ones/zeros 创建](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#使用-ones/zeros-创建)
    - [使用 random 生成](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#使用-random-生成)
    - [从文件读取](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#从文件读取)
- [统计和属性](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#统计和属性)
    - [尺寸相关](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#尺寸相关)
        - [`np.shape`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.shape)
    - [最值分位](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#最值分位)
        - [`np.max/min`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.max/min)
    - [平均求和标准差](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#平均求和标准差)
        - [`np.average`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.average)
        - [`np.sum`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.sum)
- [形状和转换](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#形状和转换)
    - [改变形状](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#改变形状)
        - [`np.expand_dims`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.expand_dims)
        - [`np.squeeze`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.squeeze)
        - [`np.reshape/arr.reshape`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.reshape/arr.reshape)
    - [反序](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#反序)
    - [转置](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#转置)
        - [`arr.T`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#arr.T)
        - [`np.transpose`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.transpose)
- [分解和组合](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#分解和组合)
    - [切片和索引](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#切片和索引)
        - [`index/slice`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#index/slice)
    - [拼接](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#拼接)
        - [`np.concatenate`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.concatenate)
        - [`np.stack`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.stack)
    - [重复](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#重复)
    - [分拆](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#分拆)
        - [`np.split`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.split)
- [筛选和过滤](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#筛选和过滤)
    - [条件筛选](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#条件筛选)
    - [提取](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#提取)
    - [抽样](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#抽样)
    - [最值 Index](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#最值-Index)
        - [`np.argmax/argmin`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.argmax/argmin)
        - [`np.argsort`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.argsort)
- [矩阵和运算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#矩阵和运算)
    - [算术](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#算术)
    - [矩阵](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#矩阵)
        - [`arr.dot`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#arr.dot)
        - [`np.matmul`](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#np.matmul)
- [小结和心得](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#小结和心得)
    - [内容小结](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#内容小结)
    - [心得技巧](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#心得技巧)
- [巩固和练习](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#巩固和练习)
    - [基础题目 1](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#基础题目1)
    - [基础题目 2](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#基础题目2)
    - [进阶题目](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#进阶题目)
- [解答和参考](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#解答和参考)
    - [基础题目 1](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#基础题目1)
    - [基础题目 2](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#基础题目2)
    - [进阶题目](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#进阶题目)
- [文献和资料](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/introduction/ch-all.ipynb#文献和资料)

## 从入门到熟练

### 原则

- 系统全面
- 原理介绍
- 例子辅助理解

### 大纲

- [核心概念](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb)
    - [常量](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#常量)
    - [数据类型](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#数据类型)
    - [结构化数组](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#结构化数组)
    - [时间数组](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#时间数组)
    - [数组对象](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#数组对象)
    - [自定义数组容器](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#自定义数组容器)
    - [子类化与标准子类](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch01-core_concepts.ipynb#子类化与标准子类)
- [操作变换](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb)
    - [广播](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#广播)
    - [通函数](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#通函数)
    - [基本操作](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#基本操作)
    - [排序搜索](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#排序搜索)
    - [集合操作](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#集合操作)
    - [函数式编程](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#函数式编程)
    - [测试](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch02-manipulation.ipynb#测试)
- [数值计算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb)
    - [数学函数](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#数学函数)
    - [数值分析](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#数值分析)
    - [导数和微积分](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#导数和微积分)
    - [多项式](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#多项式)
    - [逻辑运算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#逻辑运算)
    - [二进制运算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#二进制运算)
    - [字符串](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch03-numeric_calculation.ipynb#字符串)
- [线性代数](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb)
    - [数组乘法](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#数组乘法)
    - [基础概念](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#基础概念)
    - [矩阵运算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#矩阵运算)
    - [Einsum](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#Einsum)
    - [Padding](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#Padding)
    - [卷积](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#卷积)
    - [掩码运算](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch04-linear_algebra.ipynb#掩码运算)
- [概率统计](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb)
    - [基本指标](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#基本指标)
    - [相关性](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#相关性)
    - [柱状图](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#柱状图)
    - [计数](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#计数)
    - [随机生成器](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#随机生成器)
    - [随机排列](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#随机排列)
    - [随机分布](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch05-probability_statistics.ipynb#随机分布)
- [不止NumPy](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb)
    - [Numba](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#Numba)
    - [JAX](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#JAX)
    - [Cython](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#Cython)
    - [CuPy](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#CuPy)
    - [Sparse](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#Sparse)
    - [Dask](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#Dask)
    - [Xarray](https://nbviewer.org/github/datawhalechina/powerful-numpy/blob/main/src/skilled/ch06-morethan_numpy.ipynb#Xarray)


## 社区反馈


反馈来自社区。格式：`微信昵称：意见`。谢谢诸位反馈。

- 潭：语速有点快；切片和索引希望详细点。
- 我的名字：重点部分放慢速度，非重点也许可以跳过。
- Channer：常用的、不容易理解的参数可以重点讲一下，举一些简单的例子。
