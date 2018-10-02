% MTH 201, Curves and surfaces
% Practice problem set 5

1. Consider a (plane) curve parametrized by $\gamma : (a, b) \to \mathbf{R}^2$ and a point on that curve $p = \gamma(t_0)$. We will find a circle which best approximates the curve at $p$, in the sense defined below: 

	a) Prove that if a circle is tangent to the curve defined by $\gamma$ at $p$ ("tangent" means that the circle touches the curve and the circle's tangent line and the curve's tangent line are the same at p), then its center must lie on the line containing the vector $\mathbf{N}_s(t)$. For this and the part below you may assume that a normal line of a circle contains its center.

	b) For some real number $r$, let  $C_r$ denote the circle of radius $|r|$, with its center at the point $p + r\mathbf{N}_s(t)$. Why is it tangent to the curve at $p$? Note that $C_r$ divides the plane into an interior and exterior component and $r$ may be negative, in which case the center is in a direction opposite to $\mathbf{N}_s(t)$.

	
	c) Prove that a point $\gamma(t)$ avoids the interior component of $C_r$ if and only if $d(t) := \|\gamma(t) - (p + r\mathbf{N}(t))\|^2 \geq r^2$ and avoids the exterior component if and only if $d(t) \leq r^2$ (it always intersects the circle at $p$, so at $t_0$ you get $r^2$). The square is only to allow us to express it as a dot product. Since $d(t)$ always positive, taking the square is harmless.
	
	d) We say that $C_r$ is too small if, at least in the vicinity of $p$, every point on the curve defined by $\gamma$ avoids the interior of $C_r$, i.e. there is an $\epsilon$ so that for any $t$ inside the interval $(t_0 - \epsilon, t_0 + \epsilon)$, $\gamma(t)$ avoids the interior of $C_r$. Use the previous part to rewrite this in terms of the function $d(t)$, which is defined above. Why does that mean that $d$ has a local minimum at $t_0$? Remember that a function has a local minimum at $t_0$ if for $t$ *in the vicinity* of $t_0$, $f(t) \geq f(t_0)$

	e) We say that $C_r$ is too big if, at least in the vicinity of $p$, every point on the curve defined by $\gamma$ avoids the exterior of $C_r$, i.e. there is an $\epsilon$ so that for any $t$ inside the interval $(t_0 - \epsilon, t_0 + \epsilon)$, $\gamma(t)$ avoids the exterior of $C_r$. Use the previous part to rewrite this in terms of the function $d(t)$, which is defined above. Why does that mean that $d$ has a local maximum at $t_0$?
	
	f) Prove that no matter what $r$ is, $d'(t_0) = 0$. (By now you should be in the habit of expressing such derivatives in terms of that orthonormal basis $\mathbf{N}_s(t)$ and $\mathbf{T}(t)$ so that you can easily identify which coefficients cancel).
	
	g) Remember that a function $f$ has a local maximum at $t_0$ if $f'(t_0)=0$ and $f''(t_0)<0$; it has a local minimum at $t_0$ if $f'(t_0)=0$ and $f''(t_0)>0$. Compute $d''(t)$ and use parts d) and e) above to show that $C_r$ would be too big if $r>1/\kappa(t_0)$ and too small if $r < 1/\kappa(t_0)$. Therefore, a circle of radius $1/\kappa(t_0)$ may be thought of as best approximating the curve at $p$. Such a circle is called an *osculating circle* and its radius is $1/\kappa(t_0)$ is called the radius of curvature.

### Space curves	

2. Prove that if $f : (a, b) \to \mathbb{R}^3$  and $g : (a, b) \to \mathbb{R}^3$ are two vector valued functions and $h(t) = f(t) \times g(t)$ then $\dot{h}(t) = \dot{f}(t) \times g(t) + f(t) \times \dot{g}(t)$.

2. Prove that for a space curve parametrized by a *unit-speed parametrization*, $\gamma : (a, b) \to \mathbb{R}^3$, $\mathbf{N}(t) := \frac{\ddot{\gamma}(t)}{\kappa(t)}=\frac{\dot{T}(t)}{\|T(t)\|}$ is a unit vector which is orthogonal to the unit tangent vector $\mathbf{T}(t)= \frac{\dot{\gamma}(t)}{\|\dot{\gamma}(t)\|}$. Note, here $\kappa$ is the curvature and *not* the signed curvature, which only makes sense for plane curves. Note also that all this makes sense only if $\gamma$ is regular and $\kappa(t) \neq 0$ (it appears in the denominator!)

3. Consider the vector $\mathbf{B}(t) := \mathbf{T}(t) \times \mathbf{N}(t)$. What is $\|\mathbf{B}(t)\|$? Why does the set $\{\mathbf{T}(t), \mathbf{N}(t), \mathbf{B}(t)\}$ form an orthonormal basis of $\mathbb{R}^3$?

4. You know the cross product of two vectors written in terms of a basis if you know the cross products of the respective basis elements. Therefore, it will be useful to know $\mathbf{B}(t) \times \mathbf{T}(t)$ and $\mathbf{N}(t) \times \mathbf{B}(t)$ (by the previous part, you already know $\mathbf{T}(t) \times \mathbf{N}(t) = \mathbf{B}(t)$ by the definition of $\mathbf{B}$). What are they? Be careful of the order and the resulting sign!

5. Show that if $\mathbf{v}_1$, $\mathbf{v}_2$, and $\mathbf{v}_3$ form an orthonormal basis in $\mathbb{R}^3$ and if a vector $\mathbf{w}$ is orthogonal to both $\mathbf{v}_1$ and $\mathbf{v}_2$, it must be a scalar multiple of $\mathbf{v}_3$.

5. Show that $\dot{\mathbf{B}}(t)$ is a scalar multiple of $\mathbf{N}(t)$.

5.  Since any vector valued function can be written as a linear combination of $\mathbf{T}(t)$, $\mathbf{N}(t)$, and $\mathbf{B}(t)$, we can know its derivative if we know $\dot{\mathbf{T}}(t)$, $\dot{\mathbf{N}}(t)$, and $\dot{\mathbf{B}}(t)$. Express the following vector valued functions in terms of the basis elements $\mathbf{T}(t)$, $\mathbf{N}(t)$, and $\mathbf{B}(t)$ so that your coefficients involve either $\kappa(t)$ or $\tau(t)$ (Try to use 2. and 5. You will need to use 5. more than once.)
	a) $\dot{\mathbf{T}}(t)$

	b) $\dot{\mathbf{N}}(t)$

	c) $\dot{\mathbf{B}}(t)$


6. Prove that the torsion of a curve is the constant function 0 if and only if the curve lies on a plane.

6. Prove that if the torsion of a curve is always 0 and the curvature is constant, then the curve must lie on a circle (Prove that the curve is at a fixed distance from a particular point, and that therefore it lies on a sphere. Let the osculating circle help you guess what the point should be! By the previous exercise you know that it also lies on a plane so it lies on the intersection of a sphere and plane which is a circle).

6. We define the torsion by choosing some unit speed parametrization. Prove that we get the same answer even if we choose a reparametrization that is also a unit speed parametrization (Remember how two unit speed parametrizations relate with each other. First find out how their respective unit tangents, unit normals, and unit binormals relate).

6. The following parts will help you to prove that if you are given two functions, $t$ and $k$, so that $k(s)>0$, then you will be be able to find a curve parametrized by some unit-speed parametrization $\gamma$ so that the curvature $\kappa(s) = k(s)$ and the torsion $\tau(s) = t(s)$.

	a) Prove that for for any *unit* vector valued function $T(s)$, you can always find a parametrization $\gamma$ so that $\dot{\gamma}(s)=T(s)$. (Therefore, we try to find a $T(s)$ so that the resulting curve has the given curvature and torsion. To find $T$ we try and characterize $\dot{T}$, which is where the $k$ and $t$ would be useful if they are to be the curvature and torsion functions.)
	b) Prove that if, in addition to $T$, there are vector valued functions $N$ and $B$, that relate with $T$ as follows:
	(@) $$\dot{T}(s) = k(s)N(s)$$
	(@) $$\dot{N}(s) = -k(s)T(s)+t(s)B(s)$$
	(@) $$\dot{B}(s) = -T(s)N(s)$$
	then for any $\gamma$ so that $\dot{\gamma}(s)=T(s)$, $N(s)$ will be the principal normal and $B(s)$ will be the binormal of $\gamma$ *as long as* $T(s)$, $N(s)$, $B(s)$ are each unit vectors that are othogonal to each other. 
	c) The theory of differential equations guarantees that there will be a $T(s)$, $N(s)$, and $B(s)$ satisfying equations (1) to (3) but part b) also requires that these solutions be unit vectors and orthonormal for each s. Let us assume that for some initial value $s_0$, $T(s_0)=v_1$, $N(s_0)=v_2$, and $B(s_0)=v_3$ where $v_1$, $v_2$, and $v_3$ are unit vectors that are orthogonal to each other. Let us denote 
	$$f_1(s) = N(s) \cdot N(s)$$
	$$f_2(s) = T(s) \cdot B(s)$$
	$$f_3(s) = T(s) \cdot N(s)$$
	$$f_4(s) = T(s) \cdot T(s)$$
	$$f_5(s) = N(s) \cdot N(s)$$
	$$f_6(s) = B(s) \cdot B(s)$$
Write each $f_i'$ in terms of the $f_i$ to get a system of differential equations characterizing $f_i$. Note that in addtion, these functions also satisfy the intitial conditions $f_1(s_0) = f_2(s_0) = f_3(s_0)=0$ and $f_4(s_0) = f_5(s_0) = f_6(s_0) = 1$. Now prove that if instead we took $f_1'(s) = f_2'(s) = f_3'(s)=0$ and $f_4'(s) = f_5'(s) = f_6'(s) = 1$ (all constant functions), they would also satisfy the same system of differerntial equations $f_i$ and the same initial conditions (the latter is very obvious but the former is where you should see terms cancelling out if you do everything correctly). How does the uniqueness of a the solution of a diffferntial equations, given the intial value, help to conclude that if $v_i$ are orthonormal, then $T(s)$, $N(s)$, and $B(s)$ are orthonormal for all $s$? Combined with the earlier parts, you should see how to get a curve with the given $k$ and $t$ as curvature and torsion.

12. The following parts will help you to prove that if a two curves, paramatrized by unit speed parametrizations $\gamma_1(t)$ and $\gamma_2(t)$, respectively, have the same curvature and torsion functions, say, $\kappa(t)$ and $\tau(t)$, then they will differ by a rigid transformation.
	a) Prove that if $\mathbf{T}_1(t) = \mathbf{T}_2(t)$, where $\mathbf{T}_1(t)$ and $\mathbf{T}_2(t)$ are the unit tangents of $\gamma_1$ and $\gamma_2$, respectively, then $\gamma_2(t)$ is a translate of $\gamma_1(t)$. 
	b) Let $\mathbf{v}$ and $\mathbf{w}$ be unit vectors. Prove the inequality $\mathbf{v}\cdot \mathbf{w}\leq 1$ and also show that it is an equality if and only if $\mathbf{v}$ = $\mathbf{w}$.
	a) Let $\mathbf{N}_1(t)$ and $\mathbf{N}_2(t)$ denote the principal normals of $\gamma_1$ and $\gamma_2$, respecitively. Let $\mathbf{B}_1(t)$ and $\mathbf{B}_2(t)$ denote the binormals of $\gamma_1$ and $\gamma_2$, respecitively. Prove that if $\mathbf{T}_1(t_0)= \mathbf{T}_2(t_0)$, $\mathbf{N}_1(t_0)= \mathbf{N}_2(t_0)$, and $\mathbf{B}_1(t_0)= \mathbf{B}_2(t_0)$, then $\mathbf{T}_1(t)= \mathbf{T}_2(t)$, $\mathbf{N}_1(t)= \mathbf{N}_2(t)$, and $\mathbf{B}_1(t)= \mathbf{B}_2(t)$ for all $t$. (Hint: use the previous part to show that this happens if and only if the $\mathbf{T}_1(t)\cdot\mathbf{T}_2(t) + \mathbf{N}_1(t)\cdot\mathbf{N}_2(t) + \mathbf{B}_1(t)\cdot\mathbf{B}_2(t) = 3$. You know that this is satisfied for $t=t_0$ so all that remains is to show that the derivative is 0. This is where you will use that the curvatures and torsion are the same.)
	a) The previous part is saying that if you align the tangent, normal, and binormal of one curve with the tangent, normal, and binormal of the other curve at one point, then they also align for all other points $t$. Why can you use only two rotations to make them match for the point $\gamma(t_0)$?
