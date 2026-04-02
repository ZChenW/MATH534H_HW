# Weak Maximum Principle

## Theorem

Let \(u(x,t)\) be continuous on the closed rectangle

\[
R=[0,L]\times[0,T]
\]

and suppose \(u\) satisfies the heat equation in the interior:

\[
u_t-k u_{xx}=0, \qquad k>0.
\]

Define the parabolic boundary

\[
\Gamma=\{(x,t)\in R : t=0 \text{ or } x=0 \text{ or } x=L\}.
\]

Then

\[
\max_{(x,t)\in R} u(x,t) = \max_{(x,t)\in \Gamma} u(x,t).
\]

That is, the maximum of \(u\) on \(R\) is attained on \(\Gamma\).

---

## Proof

We prove this by contradiction.

Assume the conclusion is false. Then the maximum of \(u\) on \(R\) is attained at some interior point \((x_0,t_0)\), where

\[
0<x_0<L, \qquad 0<t_0\le T.
\]

Now define the auxiliary function

\[
v(x,t)=u(x,t)+\varepsilon x^2,
\qquad \varepsilon>0.
\]

Since \(v\) is continuous on the compact set \(R\), it attains a maximum somewhere on \(R\). Suppose this maximum occurs at an interior point \((x_1,t_1)\).

At an interior maximum point of \(v\), we have

\[
v_t(x_1,t_1)=0
\]

and

\[
v_{xx}(x_1,t_1)\le 0.
\]

Because

\[
v_t=u_t, \qquad v_{xx}=u_{xx}+2\varepsilon,
\]

it follows that

\[
u_t(x_1,t_1)=0
\]

and

\[
u_{xx}(x_1,t_1)=v_{xx}(x_1,t_1)-2\varepsilon \le -2\varepsilon <0.
\]

Now evaluate the heat equation at \((x_1,t_1)\):

\[
u_t(x_1,t_1)-k u_{xx}(x_1,t_1)
=0-k(\text{negative number})>0.
\]

This contradicts the fact that \(u\) satisfies

\[
u_t-k u_{xx}=0.
\]

Therefore, \(v\) cannot attain its maximum at an interior point. So the maximum of \(v\) must occur on \(\Gamma\). Hence

\[
\max_R (u+\varepsilon x^2)=\max_\Gamma (u+\varepsilon x^2).
\]

Since \(0\le x^2\le L^2\) on \(R\), we have

\[
u(x,t)\le u(x,t)+\varepsilon x^2\le u(x,t)+\varepsilon L^2.
\]

Therefore,

\[
\max_R u
\le
\max_R (u+\varepsilon x^2)
=
\max_\Gamma (u+\varepsilon x^2)
\le
\max_\Gamma u+\varepsilon L^2.
\]

So

\[
\max_R u \le \max_\Gamma u+\varepsilon L^2.
\]

Since this holds for every \(\varepsilon>0\), letting \(\varepsilon\to 0\) gives

\[
\max_R u\le \max_\Gamma u.
\]

On the other hand, since \(\Gamma\subset R\), we clearly have

\[
\max_\Gamma u\le \max_R u.
\]

Combining the two inequalities, we obtain

\[
\max_R u=\max_\Gamma u.
\]

Thus the theorem is proved.

\(\square\)
