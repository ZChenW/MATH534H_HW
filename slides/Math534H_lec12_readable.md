# Math 534H - 2026年春 - Lecture 12

## 第1页

**波动方程守恒能量。**

1. 我们将假设初始条件 $\phi$ 和 $\psi$ 在某个区间 $[-R,R]$ 外消失。

   这意味着 $u(x,t)$（因此 $u_x(x,t)$ 和 $u_t(x,t)$）在 $|x|>R+ct$ 时消失。

- $\rho$：弦的密度，$\rho>0$
- $T$：张力向量的大小（常数），$T>0$
- $(\rho,T\ \text{与}\ x,t\ \text{无关})$，并且

$$

  c^2=\frac{T}{\rho}

$$

- $c$：波速

## 第2页

例如，对弦来说，方程是

$$

\rho u_{tt}=Tu_{xx},\qquad x\in\mathbb{R}.

$$

也即

$$

u_{tt}-\frac{T}{\rho}u_{xx}=0
\quad\Longleftrightarrow\quad
u_{tt}-c^2u_{xx}=0.

$$

**动能（Kinetic Energy）**

$$

KE=\frac12\rho\int_{-\infty}^{\infty}u_t^2\,dx

$$

**势能（PE）**

$$

PE=\frac12T\int_{-\infty}^{\infty}u_x^2\,dx

$$

其中

$$

u_t=u_t(x,t),\qquad u_x=u_x(x,t).

$$

于是

$$

E=KE+PE

$$

对 $u$ 的能量泛函为

$$

E[u](t)=\frac12\rho\int_{-\infty}^{\infty}u_t^2(x,t)\,dx
+\frac12T\int_{-\infty}^{\infty}u_x^2(x,t)\,dx.

$$

## 第3页

**能量守恒（Conservation of Energy）意味着**

$$

E[u](t)=E[u](0)\ \to\ \text{constant}.

$$

即

$$

\frac{dE}{dt}=0=\frac{dKE}{dt}+\frac{dPE}{dt}.

$$

我们来证明这一点。 不失一般性（WLOG），取

$$

\rho=1=T,\qquad c^2=1.

$$

则

$$

\frac{dKE}{dt}=\frac12\int_{-\infty}^{\infty}\frac{d}{dt}(u_t^2)\,dx
=\frac12\cdot 2\int_{-\infty}^{\infty}u_tu_{tt}\,dx.

$$

但由

$$

u_{tt}-u_{xx}=0

$$

可得

$$

u_{tt}=u_{xx}.

$$

所以

$$

\frac{dKE}{dt}=\int_{-\infty}^{\infty}u_tu_{xx}\,dx
\stackrel{\mathrm{IBP}}{=}
u_tu_x\Big|_{-\infty}^{\infty}
-\int_{-\infty}^{\infty}u_{tx}u_x\,dx.

$$

边界项为 0。

## 第4页

因此

$$

\frac{dKE}{dt}=-\int_{-\infty}^{\infty}u_{tx}u_x\,dx.

$$

其中

$$

u_{tx}u_x=\frac12\frac{d}{dt}(u_x^2).

$$

于是

$$

\frac{dKE}{dt}=-\frac12\frac{d}{dt}\int_{-\infty}^{\infty}u_x^2\,dx
\qquad\text{(1)}

$$

另一方面

$$

\frac{dPE}{dt}=\frac12\frac{d}{dt}\int_{-\infty}^{\infty}u_x^2\,dx
\qquad\text{(2)}

$$

所以

$$

\frac{dE}{dt}=\frac{dKE}{dt}+\frac{dPE}{dt}=0,

$$

证毕，如所愿。

## 第5页

**另一个例子（Another Examples）**

1. **阻尼弦方程（Damped string equation）**。

   这来自弦/波问题中存在显著阻力时——比如空气阻力起作用。

   设 $\Gamma$ 为阻力因子（resistance factor），

$$

   \Gamma>0.

$$

   则方程为

$$

   u_{tt}-c^2u_{xx}+\Gamma u_t=0.

$$

   对这个方程，仍然像之前一样定义

$$

   E=KE+PE.

$$

   即

$$

   E[u](t)=\frac12\rho\int_{-\infty}^{\infty}u_t^2\,dx
   +\frac12T\int_{-\infty}^{\infty}u_x^2\,dx.

$$

   重复前面的计算，不过现在写成：

## 第6页

$$

u_{tt}=c^2u_{xx}-\Gamma u_t
\qquad\text{（多出来一项！）}

$$

所以现在你会得到

$$

\frac{dKE}{dt}
=-\frac12T\frac{d}{dt}\int_{-\infty}^{\infty}u_x^2\,dx
-\rho\Gamma\int_{-\infty}^{\infty}u_t^2\,dx.

$$

并且

$$

\frac{dPE}{dt}=\frac12T\frac{d}{dt}\int_{-\infty}^{\infty}u_x^2\,dx.

$$

于是

$$

\frac{dE}{dt}=\frac{dKE}{dt}+\frac{dPE}{dt}
=-\rho\Gamma\int_{-\infty}^{\infty}u_t^2\,dx\le 0.

$$

因此

$$

E[u](t)\le E[u](0),

$$

也就是说能量是**递减的（decreasing）**。

## 第7页

2. 现在假设在你的弦问题中，存在一个**横向弹性力（transverse elastic force）**。

   我们会有一个与位移 $u$ 成正比的额外项（就像在一根盘绕的弦中一样）。

   那么方程变为

$$

   u_{tt}-c^2u_{xx}+ku=0,
   \qquad k>0.

$$

   如果你去计算 $\frac{dE}{dt}$，其中 $E$ 与之前相同，
   最后会多出一个形如

$$

   -\rho k\int_{-\infty}^{\infty}u_tu\,dx

$$

   的额外项，**这个项没有固定符号！**

## 第8页

所以我们需要**修改能量**！

怎么找呢？

从

$$

0=u_{tt}-c^2u_{xx}+ku

$$

开始。

乘以 $u_t$，得到

$$

0=(u_{tt}-c^2u_{xx}+ku)u_t

$$

即

$$

0=u_{tt}u_t-c^2u_{xx}u_t+kuu_t.

$$

其中

$$

u_{tt}u_t=\frac12\frac{d}{dt}(u_t^2),
\qquad
kuu_t=\frac12k\frac{d}{dt}(u^2).

$$

接下来对两边关于 $x$ 积分，并像之前一样对右边第二项做分部积分（IBP）。

## 第9页

为简便起见，这里假设

$$

c^2=1,\qquad k=1,\qquad T=1,\qquad \rho=1.

$$

那么我们将得到

$$

0=\frac12\frac{d}{dt}\left[\int \bigl(u_t^2+u_x^2+u^2\bigr)\,dx\right].

$$

把这个新的能量记作

$$

\widetilde{E}[u](t).

$$

这个新的 $\widetilde{E}[u]$ 在时间中是守恒的。

最后这一部分我们下次再详细做。

---

注：由于原 PDF 为手写讲义，个别符号位置和少数字样可能存在轻微辨识歧义；以上内容已尽量按原文逐页、逐式翻译并保留原有结构。
