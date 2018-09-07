% MTH 201, Curves and surfaces
% Practice problem set 1

1. Let $\gamma_1 : (a, b) \to \mathbb{R}^3$ and $\gamma_2 : (a, b) \to \mathbb{R}^3$ be two smooth functions. Prove the following
   a) $\frac{d}{dt} (\gamma_1(t) + \gamma_2(t)) = \frac{d}{dt}\gamma_1(t) + \frac{d}{dt}\gamma_2(t)$
   a) $\frac{d}{dt} (\gamma_1(t) - \gamma_2(t)) = \frac{d}{dt}\gamma_1(t) - \frac{d}{dt}\gamma_2(t)$
   a) $\frac{d}{dt} (c\gamma_1(t)) = c\frac{d}{dt}\gamma_1(t)$ where $c$ is some real number.
   a) $\frac{d}{dt} (f(t)\gamma_1(t)) = f'(t)  \gamma_1(t) + f(t) \frac{d}{dt}\gamma_1(t)$ where $f : \mathbb{R} \to \mathbb{R}$ is a smooth _real valued_ function.
   a) $\frac{d}{dt} \gamma_1(f(t)) = f'(t) \frac{d}{dt}\gamma_1(f(t))$ where $f : \mathbb{R} \to \mathbb{R}$ is a smooth _real valued_ function. This will be referred to as the "chain rule", below.
   a) $\frac{d}{dt} (\gamma_1(t)\cdot \gamma_2(t)) = \frac{d}{dt}\gamma_1(t) \cdot \gamma_2(t) + \gamma_1(t)\cdot \frac{d}{dt}\gamma_2(t)$. The symbol $\cdot$ refers to the "dot product".

1. Consider the parametrization $\gamma(t) = (a\ cos(t), a\ sin(t), bt)$ for some  fixed real numbers $a>0$ and $b>0$.
	a) What curve does this parametrization define? Can you imagine its shape?
	b) Compute the speed of the parametrization, i.e. $\|\dot{\gamma}(t)\|$, for each $t$.
	c) Which of these points, $(a, 0, 0)$, $(a, a, 0)$, $(-a, 0, \pi b)$, $(a, 0, 2\pi b)$, lie on the curve described by $\gamma$?
	c) Can you think of a "unit speed" reparametrization, $\tilde{\gamma}$, describing the same curve, i.e. so that $\|\frac{d\tilde{\gamma}}{dt}\| = 1$? You must also describe the reparametrization map $\phi$ so that $\tilde{\gamma}(t) = \gamma (\phi(t))$.
	b) Compute the arc length function $s(t) = \int_0^t \|\dot{\gamma}(u)\|du$. Use this to compute the arc length of the part of the curve between the points $(a, 0, 0)$ and $(a, 0, 2\pi b)$ (after, of course, verifying that they do indeed lie on the curve).
	c) Compute $\|\frac{d}{dt} \gamma(s^{-1}(t))\|$.
 

1.  Consider a line segment between two points $p=(x_1, x_2, x_3)$ and $q=(y_1, y_2, y_3)$ in $\mathbb{R}^3$. 
	a) Find a parametrization of the line segment.
	b) Use the parametrization to show that the arc length of the line segment is equal to $\|p - q\|$.

1.  This exercise will help you to prove that the line segment joining two points on the curve parametrized by some parametrization, $\gamma : (a, b) \to \mathbb{R}^3$, is the shortest curve joining the two points $p = \gamma(t_0)$ and $q = \gamma(t_1)$. Note that by the previous exercise, the length of the line segment between points $p$ and $q$ is $\|\gamma(t_1) - \gamma(t_0)\|$.
	a) Prove the Cauchy-Schwartz inequality, i.e.  $|\mathbf{v} \cdot \mathbf{w}|\leq \|\mathbf{v}\| \|\mathbf{w}\|$ for any pair of vectors $\mathbf{v}$ and $\mathbf{w}$ (this follows easily from the definition of the dot product $\mathbf{v}\cdot\mathbf{w} = \|\mathbf{v}\|\|\mathbf{w}\|cos(\theta)$ where $\theta$ is the angle between the two vectors.).
	a) Show that for any vector $\mathbf{v}$, we can figure out its norm by taking the dot product with the unit vector in the same direction, i.e. $\|\mathbf{v}\| = \mathbf{v} \cdot \frac{\mathbf{v}}{\|\mathbf{v}\|}$.
	a) Use the second fundamental theorem of calculus to show that $(\gamma(t_1) - \gamma(t_0)) \cdot \mathbf{v} = \int_{t_0}^{t_1} \dot{\gamma} (t)\cdot\mathbf{v}dt$.
	a) By the previous two parts, the distance between points $\gamma(t_0)$ and $\gamma(t_1)$ on the curve is $\|\gamma(t_1) - \gamma(t_0)\|= \int_{t_0}^{t_1}\dot{\gamma}(t) \cdot \frac{\gamma(t_1) - \gamma(t_0)}{\|\gamma(t_1) - \gamma(t_0)\|}dt$ (Why?). This will allow you to use Cauchy-Schwartz inequality to relate this integral with integral defining the arc length and complete the proof of the inequality, $\|\gamma(t_1) - \gamma(t_0)\| \leq \int_{t_0}^{t_1} \|\dot{\gamma} (t)\|dt$.

3.  Consider the arc-length function $s(t) = \int_{t_0}^t \|\dot{\gamma}(u)\|du$, where $\gamma$ is some parametrization of a curve. Further, assume that $\dot{\gamma}(t)\neq 0$ for any $t$ in the domain of $\gamma$ (while solving the parts of this exercise below, can you identify the parts of your argument that need this assumption?).
	a) Use the second fundamental theorem of calculus to show that $s'(t) = \|\dot{\gamma}(t)\|$ and therefore that $s'(t) > 0$.
	b) Use the solution to the previous part to compute the derivative of $s^{-1}(t)$, which is the inverse of $s(t)$ (in the next lecture, we will see why this inverse exists and why it is smooth). 
	c) Let $\tilde{\gamma}(t) := \gamma(s^{-1}(t))$, and use the chain rule and the previous parts to show that $\|\frac{d}{dt} \tilde{\gamma}(t)\|=1$. In other words, you can use the arc-length function to reparametrize $\gamma$ to a "unit speed" parametrization.

4.  Prove that if $\gamma : (a, b) \to \mathbb{R}^3$ is a parametrization of a curve such that $\|\dot{\gamma}(t)\| = 1$ for any $t$ in the interval $(a, b)$, then $s(t) = t$, where $s(t)$ is the arc length function $s(t) = \int_0^t \|\dot{\gamma}(u)\|du$. Observe that $s(t)=t$ means that the arc-length of the curve until a point $\gamma(t)$ is equal to the parameter $t$ and therefore such a $\gamma$ is also called an "arc length parametrization".

5.  Use the chain rule to show that if $\|\frac{d}{dt}\gamma(\phi(t))\| = 1$ then $\dot{\gamma}(\phi(t)) \neq 0$. Therefore, we can only hope to reparametrize $\gamma$ to obtain a unit speed parametrization if $\dot{\gamma}(t) \neq 0$ for any $t$  that is in the interval on which $\gamma$ is defined.


5.  Show that if $\dot{\gamma}(t) \neq 0$ then $\frac{d}{dt}{\gamma}(\phi(t)) \neq 0$. Therefore, the property that $\dot{\gamma}(t) \neq 0$ for any $t$ in the interval on which it is defined, does not change on reparametrizing
