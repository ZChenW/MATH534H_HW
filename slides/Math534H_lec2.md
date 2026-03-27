# Math534H Lec2

> 对应原文件：`M534H -  L2.pdf`  
> 说明：按页面顺序转写。手写内容难辨处记为 `[原文难辨]`。

## 第 1 页

- Math 534H, Spring 2026, Lecture 2
- 主题：Examples of Nonlinear Equations
- ⑧ Burgers' equation
- 拟线性，一阶
  $$
  u_t - 2u u_x = 0
  $$
  或按版面理解为
  $$
  u_t + 2u u_x = 0
  $$
- 这是无粘（nonviscous）版本
- 它控制一维无粘流体的流动
- 也用于交通流建模
- 粘性版本加入耗散项
  $$
  u_t + 2u u_x = \nu u_{xx}
  $$
- 讲义文字强调：
  - steepening term
  - dissipation term
  - shock forming

## 第 2 页

- ⑨ Porous medium equation
- 拟线性，二阶
  $$
  u_t = \operatorname{div}(u^m \nabla u), \qquad t>0
  $$
- 当 $m=1$ 时，接近线性热方程情形
- 该方程出现在 filtration 的背景里
- 例如模拟水在土壤中渗透运动
- 本页后半还出现一个二阶半线性例子
- 以及 cubic nonlinear Schrödinger equation
- 用途包括：
  - fiber optics
  - BEC
  - water waves
  - plasma physics
- 讲义写到：
  - dispersive equation
  - $\lambda=1$ defocusing
  - $\lambda=-1$ focusing

## 第 3 页

- ⑪ Minimal surface equation
- 拟线性，二阶
  $$
  \operatorname{div}\left(\frac{\nabla u}{\sqrt{1+|\nabla u|^2}}\right)=0
  $$
- 区域在 $\mathbb{R}^2$ 中，边界为闭曲线
- 该方程的解的图像使面积最小
- 即在给定边界下，在所有曲面中面积最小
- 例子：soap bubbles 是极小曲面
- ⑫ 一个来自 geometric optics 的例子：
  - Eikonal equation
  - 一阶
  - fully nonlinear

## 第 4 页

- 转入：Transport equations with constant coefficients
- 在 $(x,t)\in\mathbb{R}^2$ 上
  $$
  u_t + c u_x = 0
  $$
- 提问：How do we solve this?
- 讲义说明：之后将会通过“构造”显式解来证明解存在

## 第 5 页

- [原文大段难辨]
- 本页继续常系数输运方程的求解准备
- 应在说明显式构造的想法与特征线背景

## 第 6 页

- [原文大段难辨]
- 内容接续输运方程

## 第 7 页

- [原文大段难辨]
- 本讲结束于从非线性例子切换到一阶输运方程
