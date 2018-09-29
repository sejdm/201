% MTH 201, Curves and surfaces
% Practice problem set 7

1. Let $f(x, y) = x\mathrm{sin}(x+2y)$. Find $f_x$, $f_y$, $f_{xy}$, and $f_{yx}$.

1. Use the chain rule of partial derivatives to show that if $f :\mathbb{R} \to \mathbb{R}$ is a smooth function such that $y= f(x)$ satisfies $F(x, y) = 0$, where $F:\mathbb{R}^2 \to \mathbb{R}$ is also a smooth function, then $\frac{\mathrm{d}y}{\mathrm{d}x}= -\frac{F_x}{F_y}$. This is called implicit differentiation.

1. Let $f : \mathbb{R}^2 \to \mathbb{R}$ be a smooth function and let $(x_0, y_0)$ be a point in $\mathbb{R}^2$ and $\mathbf{v} = (v_1, v_2)$ a vector. Define $F = f(x_0+v_1t, y_0+v_2t)$. Use the chain rule for partial derivatives to show that $F'(0)= f_x(x_0,y_0)v_1 + f_y(x_0, y_0)v_2 = (f_x(x_0,y_0), f_y(x_0, y_0)) \cdot \mathbf{v}$. Note that $F'(0)= \displaystyle\lim_{t \to 0}\frac{f(x_0 + tv_1, y_0 + tv_2) -f(x_0, y_0)}{t}$; it is called the directional derivative of $f$ in the direction of $\mathbf{v}$ and is denoted by $f_\mathbf{v}$. This exercise shows that one can compute the directional derivative of $f$ in the direction of any vector $\mathbf{v}$ if one knows the partial derivatives of $f$.

1. Which of the following surface patches are regular?
	a) $\sigma: \mathbb{R}^2 \to \mathbb{R}^3$, $\sigma(x,y) = (x, y, x+y)$
	a) $\sigma: \mathbb{R}^2 \to \mathbb{R}^3$, $\sigma(x,y) = (x, x^2, y^3)$

1. Show that each of the following subsets of $\mathbb{R}^3$ are smooth surfaces by finding enough regular surface patches to cover each surface.
	a) The cylinder, defined as $S := \{(x, y, z) \ |\ x^2 + y^2 = 1\}$
	b) The sphere, defined as $S := \{(x, y, z) \ |\ x^2 + y^2 + z^2 = 1\}$

1. Show that the surface patch, 
$\sigma(s,t) = ((a+b\mathrm{cos}(s)) \mathrm{cos}(t), (a+b\mathrm{cos}(s)) \mathrm{sin}(t), b \mathrm{sin}(s))$, where $b < a$, is regular. Can you imagine the surface that it is a surface patch of?
   
2. For an open subset $U$ of $\mathbb{R}^2$, and a smooth map $f: U \to \mathbb{R}^3$, show that the set $S:=\{(x, y, f(x, y)) \ |\ (x, y) \in \mathbb{R}^2\}$ is a smooth surface.

4. If $U$ is an open subset of $\mathbb{R}^2$, then prove that the determinant of the Jacobian of a map $f : U \to \mathbb{R}^3$ is non-zero if and only if $\frac{\partial f}{\partial x} \times \frac{\partial f}{\partial y} \neq 0$

4. If $F : U \to \mathbb{R}$, where $U$ an open subset of $\mathbb{R}^3$, is smooth, what condition do you need to impose on it so that the Jacobian of the map $f : U \to \mathbb{R}^3$, defined by $f(x, y, z) = (x, y, F(x, y, z))$, has non-zero determinant?
