% MTH 201, Curves and surfaces
% Practice problem set 10



1. Compute the first fundamental form with respect to the surface patch $\sigma(x, y) = (f(x)\mathrm{cos}(y), f(x)\mathrm{sin}(y), g(x))$. Why do you think your answer does not involve $g$?


1. Find a surface patch for each of the following surfaces, and compute the first fundamental form of that patch.
	a) A sphere. $\sigma(x, y) = (x, y, \sqrt{1 - x^2 - z^2})$
	c) A generalized cylinder over a plane curve $\gamma$. $\sigma(x, y) = \gamma(x) + y\mathbb{\delta}(x)$, where $\delta$ is orthogonal to the plane that contains $\gamma$.
   
   
1. If $\sigma$ is a regular surface patch of a surface, $\tilde{\sigma} = \sigma \circ \Theta$, another surface patch, where $\Theta$ is a coordinate transformation, then show that their respective first fundamental forms $E\mathrm{d}x^2 + 2 F\mathrm{d}x\mathrm{d}y + G\mathrm{d}y^2$ and $\tilde{E}\mathrm{d}\tilde{x}^2 + 2 \tilde{F}\mathrm{d}\tilde{x}\mathrm{d}\tilde{y} + \tilde{G}\mathrm{d}\tilde{y}^2$ are related by
$$\left({\begin{array}{cc}
   \tilde{E} & \tilde{F} \\
   \tilde{F} & \tilde{G} \\
  \end{array} } \right) = 
  (\mathrm{Jac}(\Theta))^t 
  \left( {\begin{array}{cc}
   E & F \\
   F & G \\
  \end{array} } \right)
  \mathrm{Jac}(\Theta)$$

1. Let $\gamma$ be the unit speed parametrization of a regular *space* curve. 
	a) Prove that the surface patch $\sigma(x,y) = \gamma(x) + y \dot{\gamma}(x)$ is regular, then the curvature $\kappa$ is strictly positive.
	a) Prove that if $\gamma$ is a *plane* curve, then $\sigma$ is a surface patch of a plane.
	b) Compute the first fundamental form of $\sigma$ ($\gamma$ may be non-planar). Show that there exists a *plane* curve $\tilde{\gamma}$ so that $\tilde{\sigma}(x,y) = \tilde{\gamma}(x) + y \dot{\tilde{\gamma}}(x)$ has the same first fundamental form as $\sigma$.

1. Prove that a local diffeomorphism, $f : S_1 \to S_2$, is a local isometry if and only given *any* surface patch $\sigma_1$ of $S_1$, its fundamental form is equal to the fundamental form of the surface patch $f \circ \sigma$ of $S_2$ by proving the following parts:
	a) $(f \circ \sigma)_x = D_p(f)(\sigma_x)$. (Remember that $\sigma_x$ can be interpreted as the derivative of some curve on the surface. That should help you to link it up with the definition of $D_p(f)$.
	b) Use part a) to prove that $\langle (f \circ \sigma)_x, (f \circ \sigma)_x \rangle = f^*\langle \sigma_x, \sigma_x \rangle$
	c) Using the fact that $f$ is a local isometry if and only if $\langle D_p(f)(\mathbf{v}), D_p(f)(\mathbf{w}) \rangle_p= \langle \mathbf{v}, \mathbf{w} \rangle_{f(p)}$, and using the previous parts, prove that the first fundamental forms are the same.
	
