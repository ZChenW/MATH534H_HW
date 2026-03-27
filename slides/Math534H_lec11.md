# Math534H Lec11

> 对应原文件：`Math 534H - L11.pdf`  
> 说明：按页面顺序转写，难辨处标 `[原文难辨]`。

## 第 1 页

- Lecture 11
- 参考 Strauss 中的习题，要求求解一个带混合导数的二阶方程
- 给出初值
  $$
  u(x,0)=x^2,\qquad u_t(x,0)=e^x
  $$
  [第二个初值按 OCR 推断]
- 下面给出 short sketch of what you need to do

## 第 2 页

- 第一步：complete squares
- 第二步：change of coordinates
- 化到标准双曲型后，解应写成
  $$
  u(x,t)=F(x-t)+G(4x+t)
  $$
  [系数按 OCR 近似识别]

## 第 3 页

- 再把初值条件代回去，求出 $F,G$
- 写
  $$
  h(x,t)=F(x-t)+J(x+4t)
  $$
  [原文中一个函数名像是 $J$]
- 对 $t=0$ 求值、求导
- 得到关于 $F',G'$ 或对应导数的方程组

## 第 4 页

- 解出 $F$ 与 $G$
- 最后得到显式表达式 [最终公式 OCR 不清]

## 第 5 页

- 新标题：
  - Causality and Energy
  - Finite Propagation Speed
- 回顾 D'Alembert's formula

## 第 6 页

- 对
  $$
  u_{tt}-c^2u_{xx}=0
  $$
  若
  $$
  u(x,0)=p(x),\qquad u_t(x,0)=q(x)
  $$
  则
  $$
  u(x,t)=\frac{p(x+ct)+p(x-ct)}{2}
  +\frac{1}{2c}\int_{x-ct}^{x+ct}q(y)\,dy
  $$

## 第 7 页

- 备注：
  - 若初值只有某种正则性，波动方程不会像热方程那样产生更强正则化
  - 文中有 “NO regularization effect” 的意思

## 第 8 页

- Finite propagation
- Domain of dependence
- Domain of influence

## 第 9 页

- 初始位置的影响产生一对波
- 它们都以速度 $c$ 传播
- 且振幅与原来有关

## 第 10 页

- 初始速度的影响也以速度 $c$ 向外传播
- 因此波的每一部分都不会比 $c$ 更快

## 第 11 页

- Causality principle：
  - 某点的解只由其依赖域中的初始数据决定

## 第 12 页

- 本讲结论：
  - 双曲型方程满足有限传播速度
  - 波动方程具有因果性
  - D'Alembert 公式把这些性质显式展示出来
