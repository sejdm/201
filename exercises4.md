% MTH 201, Curves and surfaces
% Practice problem set 4

1. Compute the signed curvature of the circle parametrized by $\gamma(t) = (5\mathrm{cos}(t), -5\mathrm{sin}(t))$.

2. If $\gamma : (a, b) \to \mathbb{R}^2$ parametrizes a curve, compute the curvature of the curve parametrized by $\tilde{\gamma}(t) = \gamma(-t)$ in terms of the curvature of $\gamma$. What about the relation between the signed curvatures of $\gamma$ and $\tilde{\gamma}$?

3. Compare the signed curvatures of a curve and its reflection, i.e. $\gamma(t)$ and $-\gamma(t)$.

1. By finding a unit speed parametrization of a circle of radius $r$, compute its curvature. Let $\gamma(t)$ be some other *constant* speed parametrization of a circle of radius $r$, where $v := \|\dot{\gamma}(t)\|$ is the (constant) speed, and prove that $\|\ddot{\gamma}(t)\| = v^2/r$ (Do you recognize the significance of this?).

1. Can you draw a curve whose signed curvature in terms of a unit speed parametrization is $\kappa_s(t)=t$?

1. Prove that if $\gamma(t)$ is a unit speed parametrization and it is periodic with period $T$, i.e. $\gamma(t+T)= \gamma(t)$, then the integral $\int_0^T\kappa_s(t)$ is always an integer multiple of $2\pi$. Hopefully, from the $2\pi$ in the expected answer, you have guessed the formula of $\kappa_s(t)$ that will prove useful!

1. Examine the formula for the curvature function to check if it is smooth everywhere. If not, when is it not smooth? What about the signed curvature? Why is there a difference?


3. Derive a formula for the signed curvature $\kappa_s(t)$ in terms of any given parametrization $\gamma(t)$ (not necessarily an arc-length parametrization). Hint: this is almost exactly like the derivation of the general formula for the curvature that you worked out in questions 2 and 3 of the last exercise set. This time, try deriving it without looking at the sub-parts.


3. Prove that any curve with constant curvature $k\neq0$ must be a circle of radius $1/k$. Hint: During the last lecture we proved that we can always find an arc length parametrization of a curve so that the curvature function matches a given function $k(t)$. The proof essentially derived a formula for the parametrization in terms of $k(t)$. Use that to compute the parametrization when you know that $k(t)$ is constant.

4. Recall that the signed unit normal, $\mathbf{N}_s(t)$, and the unit tangent vector, $\mathbf{T}(t)$, of a curve are orthogonal to each other for each point $\gamma(t)$ of a *planar* curve. Therefore, any vector at the point $\gamma(t)$ can be written as a linear combination of these two vectors. Remember that the coefficients of a vector, written in terms of an orthonormal basis, can be computed by taking the dot product with the corresponding basis vector. Use this to compute the following vectors in terms of linear combinations of $\mathbf{T}(t)$ and $\mathbf{N}_s(t)$. In your answer, all the coefficients will involve the signed curvature function $\kappa_s(t)$.
	a) $\dot{\mathbf{T}}(t)$
	a) $\dot{\mathbf{N}}_s(t)$
	b) $\ddot{\mathbf{N}}_s(t)$
	
5. For a regular plane curve parametrized by $\gamma(t)$, the curve parametrized by $\gamma_c(t) := \gamma(t) + c \mathbf{N}_s(t)$ for some fixed number $c$, is said to be "parallel to the curve parametrized by $\gamma(t)$". 
	a) What is the curve parallel to a circle of radius $r$?
	a) Prove that the $\dot{\gamma}_c(t)$ is a scalar multiple of $\dot{\gamma}(t)$.
	b) Compute the signed curvature of $\gamma_c(t)$ in terms of the signed curvature fuction, $k(t)$, for $\gamma$. You will need to assume that $k(t) \neq 1/c$. Hint: Just as in the previous exercise, it may be useful to express $\ddot{\gamma}_c(t)$ in terms of $\mathbf{N}_s(t)$ and $\mathbf{T}(t)$, where $\mathbf{N}_s(t)$ and $\mathbf{T}(t)$ are the unit normal and unit tangent vectors, respectively, of $\gamma(t)$ and compute the coefficients by taking the dot product with appropriate vectors.

6. If a curve parametrized by $\gamma$ has signed curvature function $\kappa_s(t)$, what is the signed curvature of the curve parametrizaed by $c\gamma(t)$, where $c$ is some constant?
