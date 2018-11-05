% MTH 201, Curves and surfaces
% Practice problem set 11

Recall that $\mathbf{n}(x, y)$ is the standard unit normal at $\sigma(x, y)$ with respect to some surface patch $\sigma(x,y)$. With respect to this same surface patch, $\sigma_x(x, y)$ and $\sigma_y(x, y)$ form a basis for the tangent space at $\sigma(x, y)$. Together, the three vectors form a basis for the all vectors at $\sigma(x, y)$ (not necessarily only the ones tangent to the surface). Be careful, only $\mathbf{n}$ is a unit vector and is orthogonal to the other two vectors.

Recall the following definitions: 
$E(x, y) := \sigma_x(x, y) \cdot \sigma_x(x, y)$,
$F(x, y) := \sigma_x(x, y) \cdot \sigma_y(x, y)$,
$G(x, y) := \sigma_y(x, y) \cdot \sigma_y(x, y)$, and that,

$L(x, y) := \sigma_{xx}(x, y) \cdot \mathbf{n}(x, y)$,
$M(x, y) := \sigma_{xy}(x, y) \cdot \mathbf{n}$,
$N(x, y) := \sigma_{yy}(x, y) \cdot \mathbf{n}$,

1. The following parts will attempt to find the derivatives of the above basis vector valued functions, i.e. $\mathbf{n}_x$, $\mathbf{n}_y$, $\sigma_{xx}$, $\sigma_{xy}$, and $\sigma_{yy}$, as linear combinations of the basis vectors $\mathbf{n}$, $\sigma_x$, and $\sigma_y$. Observe that all the coefficients will be in terms of $E, F, G, L, M$, and $N$.
	a) Why are $\mathbf{n}_x$ and $\mathbf{n}_y$ linear combinations of merely $\sigma_x$ and $\sigma_y$? Therefore, $\mathbf{n}_x = \alpha\sigma_x + \beta\sigma_y$ and $\mathbf{n}_y = \gamma\sigma_x + \delta\sigma_y$. Prove that the coefficients, $\alpha, \beta, \gamma, \delta$, can be computed in terms of $E, F, G, L, M$, and $N$. (Take the dot product of each equation with $\sigma_x$ and then with $\sigma_y$ to get four linear equations involving $E, F, G, L, M$, and $N$. You now have four equations and four unknowns. You will need to use the fact that $\mathbf{n}$ is orthogonal to $\sigma_x$)
	b) Show that the respective coefficients of $\mathbf{n}$, when writing $\sigma_{xx}$, $\sigma_{xy}$, and $\sigma_{yy}$, as a linear combination of $\sigma_x$, $\sigma_y$, and $\mathbf{n}$, are $L$, $M$, and $N$, respectively. Thefore, 
	$$\sigma_{xx} = \Gamma_{11}^1 \sigma_x + \Gamma_{11}^2 \sigma_y + L \mathbf{n}$$
	$$\sigma_{xy} = \Gamma_{12}^1 \sigma_x + \Gamma_{12}^2 \sigma_y + M \mathbf{n}$$
	$$\sigma_{yy} = \Gamma_{22}^1 \sigma_x + \Gamma_{22}^2 \sigma_y + N \mathbf{n}$$
	Prove that each $\Gamma_{ij}^k$ can be expressed entirely in terms of $E$, $F$, and $G$. (To find enough linear relations, take the dot product with $\sigma_x$, and then with $\sigma_y$. Play with the derivatives of $\sigma_x\cdot \sigma_y, \sigma_x\cdot \sigma_y$, and  $\sigma_x\cdot \sigma_y$, which are just $E$, $F$, and $G$, to rewrite terms such as $\sigma_{xy} \cdot \sigma_x$ in terms of $E$, $F$, and $G$.)
	
1. Consider a regular curve on a surface parametrized by a unit speed parametrization, $\gamma(t) = \sigma(x(t), y(t))$, where $\sigma$ is a surface patch  of the surface.
	a) Compute the vector $\dot{\gamma}(t)$ as a linear combination of $\sigma_x$ and $\sigma_y$ (You have done this in a previous problem set!).
	b) Compute the vector $\ddot{\gamma}(t)$ as a linear combination of $\sigma_x$, $\sigma_y$, and $\mathbf{n}$ (The previous exercise should help you to replace the $\sigma_{xx}$ etc in your calculations.).
	c) An alternative basis, instead of $\{\sigma_x, \sigma_y, \mathbf{n}\}$, is the set (taking $\mathbf{T} := \dot{\gamma}$), $\{\mathbf{T}, \mathbf{n}, \mathbf{n}\times \mathbf{T}\}$. Why is $\ddot{\gamma}$ a linear combination of only $\mathbf{n}$ and $\mathbf{n}\times \mathbf{T}$? Therefore $\ddot{\gamma} = \kappa_n \mathbf{n} + \kappa_g \mathbf{n}\times \mathbf{T}$, for some $\kappa_n= \ddot{\gamma}\cdot \mathbf{n}$ and $\kappa_g= \ddot{\gamma}\cdot (\mathbf{n} \times \mathbf{T})$. Show that $k_n$ depends only on $L$, $M$, and $N$, and that $k_g$ depends only on $E$, $F$, and $G$. (Use the previous parts and the linearity of the dot and cross products, wherever applicable, to write everything in terms of $\sigma_x$, $\sigma_y$, and $\mathbf{n}$. Somewhere, you will get a term like $\mathbf{n}\cdot (\sigma_x\times\sigma_y)$, but that can be written in terms of $E$, $F$, and $G$. Do you see why?)
	
1. Recall the definition of $\mathcal{W}_{p, S}$, which can be interpreted as a linear map from $T_p(S)$ to itself.
	a) Prove that $\mathcal{W}_{p, S}(\sigma_x) = -\mathbf{n}_x$ and $\mathcal{W}_{p, S}(\sigma_y) = -\mathbf{n}_y$. (Recall the definition of $D_p(f)$. What curve represents $\sigma_x$? Why is the derivative of the image of that curve under the Gauss map $\mathcal{G}_S$ equal to $\mathbf{n}_x$?)
	a) $\mathcal{W}_{p, S}(\sigma_x)$ and $\mathcal{W}_{p, S}(\sigma_y)$ are both tangent vectors of the surface (why?) and therefore is some linear combination of only $\sigma_x$ and $\sigma_y$, i.e. $-\mathbf{n}_x = \alpha\sigma_x + \beta\sigma_y$ and $-\mathbf{n}_y = \gamma\sigma_x + \delta\sigma_y$. This is another way of seeing that $\mathbf{n}_x$ and $\mathbf{n}_y$ can be written as linear combinations of only $\sigma_x$ and $\sigma_y$ (proved in 1 (a)). Use part a) of the first question to find a matrix representation for $\mathcal{W}_{p,S}$.

2. Recall the definition $\langle v, w\rangle'_p:= \langle \mathcal{W}_{p, S} v , w \rangle$
	a) $\langle \sigma_x, \sigma_x \rangle' = L$, $\langle \sigma_x, \sigma_y \rangle' = M$, $\langle \sigma_y, \sigma_y \rangle' = N$ (Relate, for example, $\mathbf{n}_x \cdot \sigma_x$ with $L$ by using the fact that $\mathbf{n} \cdot \sigma_x$ is orthogonal.)
	a) $\langle v, w\rangle'$ is symmetric.
	a) Show that if we express any vector tangent to the surface in terms of the basis $\sigma_x$ and $\sigma_y$ as  $v = \alpha \sigma_x + \beta \sigma_y$, then $\langle v, v\rangle' = L\alpha^2 + 2M\alpha\beta + N\beta^2$.
	c) Show that for a unit speed parametrization $\gamma$ of a regular curve on the surface, $\kappa_n$ (defined in question 2) is $\langle \dot{\gamma}, \dot{\gamma}\rangle'$. (You can use part (a) of the previous question to relate it with $\mathcal{W}_{p,S}$). This will be an alternative proof for why $\kappa_n$ depends only on $L$, $M$, and $N$.

