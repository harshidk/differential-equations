First [[Classifying Differential Equations|order]] differential equations come in the general form
$$ \frac{dy}{dx}=f(x,y) $$

---

**Separable differential equations** have the property:

$$
\frac{dx}{dy}=f(x,y)=p(x)q(y)
$$

If a differential equation is separable, that means that we can find a solution via:

$$
\int q(y)^{-1}dy=\int p(x) dx
$$

---

Consider the equation:

$$
\frac{dy}{dx}=\frac{x^2}{1-y^2}
$$

We know that this equation is separable because $\frac{x^2}{1-y^2}$ can be written as $x^2(1-y^2)^-1$. Therefore we can find a solution via:

$$
\int 1-y^2 dy=\int x^2dx
$$

Evaluating the integral and moving everything to one side leaves:

$$
-x^3+3y-y^3=c
$$

---

Sadly, most differential equations don't have the form $\frac{dx}{dy}=f(x,y)$.

First order linear differential are differential equations that can be written in the form:

$$
\frac{dy}{dt}+p(t)y=g(t)
$$

We can always find a solution to a first order linear differential equation provided that a solution exists; the method to finding one is known as the method of integrating factors and is only slightly more involved than the method for separable equations.

To start by solving $\frac{dy}{dt}+p(t)y=g(t)$, first multiply by an undefined function $\mu(t)$.

$$
\mu(t)\frac{dy}{dt}+\mu(t)p(t)y=\mu(t)g(t)
$$

Notice that the left hand side is similar to the derivative of the product $\mu(t)y$ given that the derivative of $\frac{d\mu(t)}{dt}=p(t)\mu(t)$ and that $\mu(t)$ is positive for all $t$. Funnily enough, this resembles a separable equation and we can solve for $\mu(t)$.

$$
\int\frac{d\mu(t)}{\mu(t)}=\int p(t)dt

$$

$$
\ln\mu (t)=\int p(t)dt+k,
$$

Choosing $k=0$ we can obtain the simplest possible function for $\mu(t)$:

$$
\mu(t)=\exp\int p(t)dt
$$

Note that $\mu(t)$ is positive for all $t$. Now we can return to our original equation and rewrite $\frac{\mu(t)dy}{dt}+\mu(t)p(t)y$ as $[\mu(t)y]^{'}$. We now have

$$
\frac{d}{dt}[\mu(t)y]=\mu(t)g(t)
$$

And after integrating both side and moving $\mu(t)$ over, we are left with:

$$
y=\frac{1}{\mu(t)}\int u(t)g(t)dt+\frac{C}{\mu(t)}
$$

The five steps for solving first order partial differential equations are:

- Write the equation in form $y'+p(t)y=g(t)$
- Calculate the integrating factor $\mu(t)=e^{\int p(t)dt}$
- Multiply the original equation by $\mu(t)$ and write it in the form $[\mu(t)y]^{'}=\mu(t)g(t)$.
- Integrate both sides of the equation
- Solve for y

---

Consider the problem:

$$
ty^{'}+2y=4t^2
$$

$$y(1)=2$$
First rewrite the differential in standard form by dividing by $t$.

$$
y'+\frac{2}{t}y=4t
$$

Then we can choose $\mu(t)=e^{\int \frac{2}{t}dt}=e^{2\ln t}=t^2$. Multiplying both sides by $\mu(t)$ results in the equation.

$$
t^2y'+2ty=4t^3
$$

The left-hand side can be rewritten as $[t^2y]'$ and integrating both sides leaves us with:

$$
t^2y=t^4+C
$$

Solving for $y$ leaves us with:

$$
y=t^2+\frac{C}{t^2}
$$

Now we can apply the initial condition $y(1)=2$,

$$
2=1+\frac{C}{1^2}, C=1
$$

Finally, the explicit solution of $y$ is:

$$
y=t^2+\frac{1}{t^2}: t>0
$$

Note that the $t>0$ is required due to the discontinuity at $t=0$. It is not enough to say $t\neq 0$ as then the solution to the differential equation would not be continuous on the range $(-\inf, \inf)$ -- a required property of the solution. Therefore, the domain must be restricted on $t>0$.

---
