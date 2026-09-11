Consider the general system

$$
\begin{pmatrix}
{dx}/{dt} \\
{dy}/{dt}
\end{pmatrix}
=
\begin{pmatrix}
p_{11}(t)x+p_{12}(t)y+g_1(t) \\
p_{21}(t)x+p_{22}(t)y+g_{2}(t)
\end{pmatrix}
$$

The system can also be rewritten as

$$
\frac{d\mathbf{x}}{dt} = \mathbf{P}(t)\mathbf{x}+g(t)
$$

where

$$
\begin{align}
\mathbf{x}&=\begin{pmatrix}
x \\
y
\end{pmatrix},  &   \mathbf{P}(t) &= \begin{pmatrix} p_{11}(t) & p_{12}(t)  \\ p_{21}(t)  & p_{22}(t)\end{pmatrix}, & g(t)&=\begin{pmatrix} g_{1}(t) \\  g_{2}(t)\end{pmatrix}
\end{align}.
$$

The above system is known as a [[Classifying Differential Equations|first order]] linear system of dimension two because it consists of [[First Order Differential Equations|first order equations]] and because its state space (the xy-plane) is two-dimensional.
