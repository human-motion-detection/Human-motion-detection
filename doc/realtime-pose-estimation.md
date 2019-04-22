<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
# Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields
基于部分亲和域的实时多人2D图像姿态检测

## 介绍

## 方法
1. 系统输入一张大小为$w\times h$的彩色图像, 输出图像中每个人的关键点
2. 前馈神经网络同时预测身体部位的一组置信图$S$,和一组编码了部分之间关联程度的部分亲和域向量$L$，其中$J$表示共有的身体部位数，$C$表示两个部位之间的连接数
> $$\textbf S_j \in \mathbb R^{w \times h}, j \in \{1 \dots J\}$$
> $$\textbf L_c \in \mathbb R^{w \times h \times 2}, c \in \{1, \dots, C\}$$

3. 最后通过贪婪推算，解析置信图与亲和域，输出图像中所有人的2D关键点

## 结果

## 讨论

