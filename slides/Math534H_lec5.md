# Math534H Lec5

> 对应原文件：`M534H - L5.pdf`  
> 说明：按页面顺序转写，难辨处标 `[原文难辨]`。

## 第 1 页

- Lecture 5
- 用不同方法求解
  $$
  a u_x + b u_y + c u = 0
  $$
- 使用 coordinate method
- 更一般地做，而不只局限于前一讲中的例子

## 第 2 页

- 设新的变量为 [原文书写较乱]
- 一处清晰可辨的选择是
  $$
  z=bx-ay
  $$
- 再回代并用链式法则把 $u_x,u_y$ 表为新变量导数
- 得到方程在新变量中简化

## 第 3 页

- 化简后得到某个关于新变量的一阶方程
- 积分可得
  $$
  u(z,y)=e^{g(z)} e^{-\frac{c}{a^2+b^2}(\cdots)}
  $$
  [原文公式局部难辨]
- 进一步写成
  $$
  u(x,y)=p(bx-ay)\,[原文难辨因子]
  $$
- 其中 $p$ 是任意一元函数

## 第 4 页

- 课堂作业：检查上式确实满足
  $$
  a u_x + b u_y + c u = 0
  $$
- 下次讨论：
  $$
  u_t + b u_x = F(x,t)
  $$
- 并配合初值条件
  $$
  u(x,0)=g(x)
  $$

## 第 5 页

- 阅读部分：
  - auxiliary conditions
  - Dirichlet boundary conditions
  - Neumann boundary conditions
  - Robin boundary conditions
  - well-posedness：existence, uniqueness, stability
