# 巨硬的NumPy

`巨硬的NumPy` 教程包括两部分：《从小白到入门》和《从入门到精通》。

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

开发中……

### 原则

- 系统全面
- 原理介绍
- 例子辅助理解

### 大纲

- 概念
    - 常量
    - 数组对象
    - 标量
    - 数据类型
- 操作
    - 创建
    - 转换
    - 变形
    - 排列
    - 拆分
    - 组合
    - 索引
    - 切片
    - 选择
    - 广播
- 统计
    - 基本描述
    - 均值方差
    - 相关性
    - 排序
- 分布
    - 离散
    - 连续
    - 抽样
- 函数
    - 四则运算
    - 三角函数
    - 指数对数
    - 四舍五入
    - 复数运算
- 线代
    - 向量积
    - 分解
    - 特征值
    - 范数
    - 逆矩阵



## Response How To Teach And Learn


反馈来自社区，微信昵称：意见，谢谢诸位反馈。

- 潭：语速有点快；切片和索引希望详细点。
- 我的名字：重点部分放慢速度，非重点也许可以跳过
- Channer：常用的、不容易理解的参数可以重点讲一下，举一些简单的例子
