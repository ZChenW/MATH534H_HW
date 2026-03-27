# Lecture 13

## Review (14:36 ~ 14:45)

## Continue from (++) page 8 of lecture 12

继续前言

$$
0 = \int_{-\infty}^{\infty} (u_{tt}u_t - c^2 u_{xx}u_t + ku\,u_t)\,dx
$$

$$
\int_{-\infty}^{\infty} u_{xx}u_t\,dx
= \left[ u_x u_t \right]_{-\infty}^{\infty}- \int_{-\infty}^{\infty} u_{xt}u_x\,dx
= 0 - \frac12 \frac{d}{dt}\int_{-\infty}^{\infty} u_x^2\,dx
$$

$$
0 = \frac{1}{2}\frac{d}{dt}\int_{-\infty}^{\infty}
\left( u_t^2 + c^2 u_x^2 + k u^2 \right)\,dx
$$

Constant in time:

$$\overline{E}[u](t) = \overline{E}[u](0)$$

$$\frac{d}{dt} \overline{E}[u][t] == 0$$

The energy is conserved in time.

## Heat Equation (15:07 ~)

为什么u(x, -t) is also a solution of wave equation, but heat equation not?

Diffusion on Heating equation in 1D x \in R

Heat equation is time-reversible

$$u_t - R u_{xx}, k > 0$$

- Properities of solution:
  - Remark: IVP
    - $u_t - k u_{xx} = 0$
    - $u(x, 0) = \phi$ 告诉你“最开始温度长什么样”
  - Maximum Principle 热方程的解在内部不会自己产生新的最大值。最大值只能出现在初始时刻或者空间边界上。
    - $x \in [0, L]$
    - $t \in [0, T]$
    - $R = [0, L] * [0, T]$ Former a Close Rectangle

|
|
x---------------------k
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
| | | | | | | | | | | |
0---------------------t-------

Remark: Uniqueness and stablility of solution to IVP for H, could be approached
in two ways:

- Using "Eneray method"
- Maximum Principle
  There is not max prin for the wave equation
  - ## Theorem (weak Maximum Principle):

### Weak Maximum Principle 的标准形式

设 \(u(x,t)\) 在矩形区域

\[
R=[0,L]\times[0,T]
\]

上满足热方程

\[
u*t-k u*{xx}=0,\qquad k>0
\]

并且 \(u\) 足够光滑、在闭区域上连续。

那么：

\[
\max\_{\overline R} u
\]

一定出现在这个区域的 **抛物边界** 上，而不是内部。

这里的抛物边界通常是

\[
([0,L]\times\{0\})\cup (\{0\}\times[0,T])\cup(\{L\}\times[0,T])
\]

也就是：

- 底边 \(t=0\)：初始时刻
- 左边 \(x=0\)
- 右边 \(x=L\)

### Weak Min Principle 的标准形式

### Proof Maximum Principle
