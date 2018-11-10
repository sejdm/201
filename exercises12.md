% MTH 201, Curves and surfaces
% Practice problem set 12

1. Consider a plane intersecting a surface $S$. If the plane is perpendicular to the tangent space of $S$ at a point lying on the plane, then the intersection is a curve that is called a normal section of the surface. Prove that such a curve has zero geodesic curvature.

1. Generalize the previous exercise as follows: assume that the plane is not perpendicular, but makes an angle $\theta$ wih the tangent plane at $S$. Prove that curvature of the curve of intersection is $\kappa_n/\mathrm{sin}(\theta)$. What about the geodesic curvature?

1. Compute the normal curvature of any curve on the sphere. Can you interpret the answer physically? Using this, prove that curves on the sphere that have constant geodesic curvature are circles.

1. Compute the geodesic curvature of any circle on a sphere. (A circle on the sphere can always be obtained by intersecting it with a plane.)

1. Prove that the geodesic curvature of a curve in a plane (treated as a surface in $\mathbb{R}^3$) is equal to the plane curvature.

1. Compute the second fundamental form, principle curvatures, mean curvature, and the Gaussian curvature of a surface of revolution. Remember that its surface patch is $\sigma(x, y) = (f(x)\mathrm{cos}(y), f(x) \mathrm{sin}(y), g(y))$. Use this to compute these quantities for the cylinder and the sphere. (Rememeber that the eigenvalues of a matrix $A$ can be computed by computing the roots of the polynomial, $\mathrm{det}(xI - A)$. This will help you to compute the principle curvatures. This will help you to compute the principle curvatures which can also be used to compute the mean and Gaussian curvatures.)

1. Prove that the Gussian and mean curvatures are smooth functions. This will need you to recall the way we defined smooth functions on a surface.

1. Remember that $\kappa_n=\langle \dot{\gamma}, \rangle \dot{\gamma}\rangle'$. Rather than using the usual basis for the tangent space, let us use an orthogonal basis of eigenvectors of $\mathcal{W}_{p,S}$. Why does such a basis always exist, even if the principle curvatures are not distinct? Prove that
	a) If $\dot{\gamma}=\alpha \mathbf{t}_1 + \beta \mathbf{t}_2$, then $\kappa_n = \kappa_1 \alpha^2 + \kappa_2 \beta^2$.
	b) If $\gamma$ is a unit speed parametrization then $\alpha = \mathrm{cos}(\theta)$ and $\beta = \mathrm{sin}(\theta)$, for some $\theta$. Use part a) to prove that the principle curvatures are the maximum and minimum normal curvatures of all curves passing through the point.

1. The following parts will prove that if every point on a surface is umbilic, then must be a part of a plane or a sphere. Let $\sigma : U \to S$ be a surface patch of a surface $S$.
	a) Prove that if the two principle curvatures are equal for every point in $U$, then the curvature is constant. Denote $\kappa := \kappa_1 = \kappa_2$ (If the principle curvatures are the same, then $\mathcal{W}_{p,S}\mathbf{v}=\kappa_1\mathbf{v}$ for *every* vector $\mathbf{v}$.)
	a) Prove that if $\mathbf{n}(x,y)$ is constant, then $\sigma(x, y)$ lies on a plane (Of course, the normal to the plane ought to be $\mathbf{n}(x_0, y_0)$ for some $(x_0, y_0)$ so you just need to show that $\mathbf{n}(x, y) \cdot (\sigma(x, y) -\sigma(x_0, y_0))$. We tackled a similar problem for curves, and here too you have an opportunity of proving that equality by examining the derivative of the expression, and its value at one point.)
	b) Prove that if $\kappa = 0$, then $\sigma(x, y)$ lies on a plane. 
	c) Prove that if $\kappa \neq 0$, then $\sigma(x, y)$ lies on a sphere. (Apart from the method during the lecture, you can also derive this by making a reasonable guess of the center of the sphere. It should be $c = \sigma(x_0, y_0) + \frac{1}{\kappa}\mathbf{n}$ (because the curvature of a sphere is the reciprocal of the radius). Therefore, you merely have to prove that the $\|\sigma(x, y) - c\|$ is constant. Once again, differentiate!)

1. The following parts will provide a geometric interpretation for the Gaussian curvature. $\sigma : U \to S$ is a regular surface patch of a surface $S$ of Gaussian curvature $K$.
	a) Show that $\mathbf{n}_x\times\mathbf{n}_y=K \sigma_x \times \sigma_y$, thereby expressing the cross product in terms of the standard basis of $\sigma_x$ and $\sigma_y$.
	b) Prove that as long as $K$ is non-zero, $\mathbf{n}$ is a regular surface patch for the sphere of radius 1.
	b) Let $f : U \to \mathbb{R}$ and $g : U \to \mathbb{R}$, where $U$ is an open subset of $\mathbb{R}^2$, be continuous functions. If $B_\delta$ is an open ball of radius $\delta$ in $U$, centred around $(_0, y_0)$, then prove that $\displaystyle\lim_{\delta \to 0} \frac{\int_{B_\delta}f(x, y)g(x, y) \mathrm{d}x\mathrm{d}y}{\int_{B_\delta}g(x, y) \mathrm{d}x\mathrm{d}y}= f(x_0, y_0)$
	c) Use the fact that $K$ is continuous and the observations in the previous parts to prove that $\displaystyle\lim_{\delta \to 0} \frac{\int_{B_\delta}\mathbf{n}_x \times \mathbf{n}_y\mathrm{d}x\mathrm{d}y}{\int_{B_\delta}\sigma_x \times \sigma_y\mathrm{d}x\mathrm{d}y} = K(x_0, y_0)$. Note that the integral in the denominator is simply the area of the region $\sigma(B_\delta)$ on the surface. Why is the integral in the numerator the area of that image of that region, but on the sphere, under the Gauss map?
	d) Use this interpretation to compute the Gaussian curvature of the plane, cylinder, and sphere.

1. Since a surface patch, $\sigma$, is smooth, $\sigma_{xxy}=\sigma_{xyx}$. However, each of the vectors $\sigma_{xxy}$ and $\sigma_{xyx}$ can be written in terms of the standard basis $\sigma_x$, $\sigma_y$, $\mathbf{n}$, and, therefore, by comparing coefficients you should discover some relations between $L$, $M$, $N$, and $\Gamma_{ij}^k$. From one of them you will be able to extract an expression of the Gaussian curvature in terms of only $E$, $F$, and $G$ (remember that the Christoffel symbols $\Gamma_{ij}^k$ are only in terms of $E$, $F$, and $G$).
