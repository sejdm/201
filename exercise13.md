% MTH 201, Curves and surfaces
% Practice problem set 13

1. Let $\mathbf{v}(t)$ be a vector field along a curve parametrized by $\gamma(t)$ on a surface $S$. In terms of a surface patch $\sigma: U \to S$, we may write $\gamma(t)=\sigma(x(t), y(t)$, and $\mathbf{v}(t) = \alpha(t)\sigma_x(x(t), y(t)) +  \beta\sigma_y(x(t), y(t)$. Prove that $\mathbf{v}$ is parallel along $\gamma$ if and only if $\alpha$, $\beta$, $x$, and $y$ satisfy a pair of differential equations. Does parallelism along $\gamma$ depend only on the first fundamental form? Why is that expected? (This exercise is a straightforward calculation: express $\dot{\mathbf{v}}$ in terms of $\sigma_x$, $\sigma_y$, and $\mathbf{n}$. Remember that the covariant derivative ignores the component that is along $\mathbf{n}$).

1. Prove that a curve parametrized by $\gamma$ is a geodesic if and only if the vector field $\dot{\gamma}$ is parallel along $\gamma$.

1. Prove that the parallel transport map is an invertible linear map that preserves dot products.

1. Prove that a local isometry takes geodesics to geodesics.

1. What are all the geodesics on the cylinder? (Hint: No calculations are needed for this question)


1. If $\mathbf{v}(t)$ is a vector field parallel along a curve parametrized by $\gamma(t)$, and $\tilde{\gamma}(t)$ is a reparametrization of $\gamma$ by the function $\phi(t)$, then prove that $\mathbf{v}(\phi(t))$ is also parallel. Owing to question 2., does this imply that a reparametrization of a geodesic is a geodesic? Be careful; see the next question.

1. Prove that the geodesics are of constant speed.

1. Use questions 1. and 2. to prove that $\gamma(t)=\sigma(x(t), y(t))$ is a geodesic if and only if $x(t)$ and $y(t)$ satisfy a system of differential equations.

1. We can also find an alternative system of differential equations using the following procedure: $\ddot{\gamma}$ must be tangent to both $\sigma_x$ and $\sigma_y$, which is equivalent to $\frac{\mathrm{d}}{\mathrm{d}t}(\dot{x}(t)\sigma_x(x(t), y(t)) + \dot{y}(t)\sigma_y(x(t), y(t))) \cdot \sigma_x(x(t), y(t))) = 0$ and $\frac{\mathrm{d}}{\mathrm{d}t}(\dot{x}(t)\sigma_x(x(t), y(t)) + \dot{y}(t)\sigma_y(x(t), y(t))) \cdot \sigma_y(x(t), y(t))) = 0$. Observe that they are each one of the terms of the following derivatives: $(\frac{\mathrm{d}}{\mathrm{d}t}(\dot{x}(t)\sigma_x(x(t), y(t)) + \dot{y}(t)\sigma_y(x(t), y(t)) \cdot \sigma_x(x(t), y(t))))$ and $(\frac{\mathrm{d}}{\mathrm{d}t}(\dot{x}(t)\sigma_x(x(t), y(t)) + \dot{y}(t)\sigma_y(x(t), y(t)) \cdot \sigma_y(x(t), y(t))))$. Use this observation to derive the differential equations in terms of $E$, $F$, $G$ and their derivatives.


1. Find as many geodesics on a surface of revolution as you can.
