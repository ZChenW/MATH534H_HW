# Math534H Lec8

> 对应原文件：`M534H - L8.pdf`  
> 说明：按页面顺序转写，难辨处标 `[原文难辨]`。

## 第 1 页

- Lecture 8
- 延续上次内容
- 例子中主部类似
  $$
  5y\,u_{xx} + 8u_{xy} + 2u_{yy}=0
  $$
  [系数按 OCR 近似识别]
- 计算判别量后，得到在不同区域分别是：
  - elliptic
  - hyperbolic
  - parabolic

## 第 2 页

- 问：这种分类从哪里来？
- 先看
  $$
  \Delta<0
  $$
  的 elliptic case
- 目标：做变量变换，使方程看起来像 Laplace equation

## 第 3 页

- 引入新变量
  $$
  \xi=\xi(x,y),\qquad \eta=\eta(x,y)
  $$
- 然后把 $u_x,u_y$、二阶导数写成新变量形式
- 希望消掉混合项

## 第 4 页

- 经过选择合适的新变量，得到
  $$
  Lu = u_{\xi\xi}+u_{\eta\eta}
  $$
- 这就是 Laplace equation 的主部

## 第 5 页

- 类似地，若判别量大于零，则会得到 wave-equation type 的结构
- 若判别量等于零，则得到 parabolic type

## 第 6-9 页

- 后续内容推广到更高维
- 关键词可辨识为：
  - in higher dimensions
  - symmetric matrix
  - linear algebra fact
- 主旨：二阶主部对应实对称矩阵，可由线性代数方法化简
