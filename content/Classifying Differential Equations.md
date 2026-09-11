The methods of classifying different differential equations are primary based on three properties: **ordinary, order, and linearity**.

---

Ordinary differential equations are differential equations where the unknown function depend on a single independent variable. Therefore, the only derivatives that appear in the equation are ordinary derivates. For instance, consider the equation:
$$ \frac{du}{dt}=-k(u-T_{0}) $$
is an ordinary differential equation since it only depends on one independent variable, u. Then consider the equation:

$$
\frac{\partial{u}}{\partial{t}}=D\frac{\partial^2{u}}{\partial x^2}
$$

This is a partial differential equation because it depends on the two independent variables t and x. This equation is known as the heat equation.

---

The **order** of a differential equation is the order of the highest derivative that appears in the equation. The equation:

$$
ay^{''}+by^{'}+cy = f(t)
$$

is a second order ODE because the highest derivative contained in the equation is two.

---

An nth order differential equation is said to be **linear** if it can be written in the form

$$
a_{0}(t)y^{(n)}+a_{1}(t)y^{(n-1)}+\dots+a_{n}(t)y=g(t)^2.
$$

The equation is said to be homogeneous if $g(t)$ is zero for all $t$. Otherwise the equation is nonhomogeneous.

An ODE that cannot be written in the above form is said to be nonlinear. Common reasons that an ODE is nonlinear are:

- the dependent variable y or its derivatives are arguments in a nonlinear function $\sin y$, $e^{-y}$, or $\sqrt{1+y^2}$),
- y or any of its derivatives appear as products or raised to power other than one, such as $y^2$ and $yy^{'}$

We can show that the equation

$$
x^3y^{'''}+3x^2y{''}+4y=\sin \ln(x)
$$

is a linear differential equation as $a_0=x^3$, $a_1=3x^2$, $a_2=0$, $a_3=4$, and $g(x)=\sin\ln x$.
Additionally since $g(x)$ is not zero for all values of x, the equation is nonhomogeneous.
