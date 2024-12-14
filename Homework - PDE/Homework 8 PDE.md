#### 9.1.1

We find all the three-dimensional plane waves or the solutions to the wave equation of the form $u(\mathbf{x},t) = f(\mathbf{k}\cdot \mathbf{x}-ct)$. We begin with the three-dimensional wave equation, 
$$
\begin{gather}
u_{tt} = c^{2}(u_{xx}+u_{yy}+u_{zz})
\end{gather}
$$
If we have $\mathbf{k} = k_{x}\hat{\mathbf{x}}+k_{y}\hat{\mathbf{y}}+k_{z}\hat{\mathbf{z}}$ and $\mathbf{x} = x \vec{\mathbf{x}}+y\vec{\mathbf{y}}+ z\vec{\mathbf{z}}$ a three dimensional vector, we can plug this into the given solutions such that, 
$$
\begin{gather}
u(\mathbf{x},t) = f(k_{x} \cdot x \underbrace{ (\vec{\mathbf{x}} \cdot\vec{\mathbf{x}}) }_{ 1 }, k_{y}y,k_{z}z-ct)
\end{gather}
$$
We now plug this into the wave equation to determine, 
$$
\begin{gather}
(-c)^{2}f'' = c^{2}[(k_{x})^{2}f''+(k_{y})^{2}f''+(k_{z})^{2}f''] \\ \\ 
c^{2}f'' = c^{2}(k_{x}^{2}+k_{y}^{2}+k_{z^{2}})
\end{gather}
$$
Now, the solutions of the wave equation should depend on $k$, so we have the following possibilities
$$
\begin{gather}
1. \hspace{.2cm}\mathbf{K}= 1 \rightarrow f(k_{x}x+k_{y}y+k_{z}z) = C_{1}(k_{x}x+k_{y}y+k_{z}z-ct)+C_{2} \\ \\ 
\rightarrow f(\mathbf{k}\cdot \mathbf{x}-ct) = C_{1}(\mathbf{k}\cdot \mathbf{x}-ct)+C_{2} \\ \\ 
2. \hspace{.2cm}k_{x}^{2}+k_{y}^{2}+k_{z}^{2} = 1 \rightarrow f(k_{x}x+k_{y}y+k_{z}z) = 0
\end{gather}
$$
Thus, we have the 3-D plane waves, 
$$
\begin{gather}
u(\mathbf{x},t)= C_{1}(\mathbf{k}\cdot \mathbf{x} -ct)= C_{2}
\end{gather}
$$
and specifically in the case when $\mathbf{k}=1$ we have our desired solutions
$$
\begin{gather}
u(\mathbf{x},t)= f(\mathbf{k}\cdot \mathbf{x}-ct)
\end{gather}
$$
#### 9.1.2

We verify that $h=(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-1}$ satisfies the wave equation except on the light cone. As usual, we begin with the wave equation,
$$
\begin{gather}
u_{tt}=c^{2}(u_{x x}+u_{yy}+u_{zz})
\end{gather}
$$
Now the process can easily become convoluted with taking derivatives of $h$ with respect to $x,y,z,t$, so we'll reduce the steps. Essentially that's, all we have to do, find the really long derivatives for for each variable, 
$$
\begin{gather}
u_{tt} = 2(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-3}(2c^{2}t)^{2}-(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-2}(2c^{2}) \\ \\ 
=\frac{ 6c^4 t^{2}-2c^{2}(c^{2}t^{2}-x^{2}-y^{2}-z^{2})}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^3}
\end{gather}
$$
Now, we'll find $u_{xx}$, 
$$
\begin{gather}
u_{xx}= 2(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-3}(-2x)^{2}-x(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-2}(-2) \\ \\ 
= \frac{8x^{2}}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}}+\frac{2}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{2}} \\ \\ 
=\frac{8x^{2}+{2(c^{2}t^{2}-x^{2}-y^{2}-z^{2})}}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}}= \frac{6x^{2}+2(c^{2}t^{2}-y^{2}-z^{2})}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}}
\end{gather}
$$
We'll notice that the final expression for $y,z$ are very similar to the ones for $x$. That is 
$$
\begin{gather}
u_{yy} = \frac{6y^{2}+2(c^{2}t^{2}-x^{2}-z^{2})}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}} \\ \\
u_{zz} = \frac{6z^{2}+2(c^{2}t^{2}-y^{2}-x^{2})}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}}
\end{gather}
$$
once we add $u_{x x},u_{yy},u_{zz}$ we have 
$$
\begin{gather}
= c^{2}\frac{6c^{2}t^{2}+6z^{2}+6x^{2}+6y^{2}-2y^{2}-2y^{2}-2x^{2}-2x^{2}-2z^{2}-2z^{2}}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})} \\ \\ 
c^{2} \frac{2x^{2}+2y^{2}+2x^{2}+6c^{2}t^{2}}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}} \\ \\ 
=\frac{6c^4t^{2}+2c^{2}(x^{2}+y^{2}+z^{2})}{(c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{3}}
\end{gather}
$$
Thus $h$ satisfies our wave equation! We notice that on the light cone 
$$
\begin{gather}
c^{2}t^{2}=x^{2}+y^{2}+z^{2} \\ \ \
h= (c^{2}t^{2}-x^{2}-y^{2}-z^{2})^{-1} = \text{undefined}
\end{gather}
$$

#### 9.1.3

We verify that $(c^{2}t^{2}-x^{2}-z^{2})^{-1/2}$ satisfies the 2-D wave equation on the light cone $x^{2}+y^{2}= c^{2}t^{2}$. We begin with the wave equation
$$
\begin{gather}
u_{tt}= c^{2}(u_{x x}+u_{y y}) 
\end{gather}
$$
Since this the same process as the previous question, we'll list the derivatives for $u_{tt},u_{x x},u_{yy},u_{zz}$ that we've already calculated on paper,
$$
\begin{gather}
u_{tt}= 2c^4t^{2}+\frac{c^{2}(x^{2}+y^{2})}{(c^{2}t^{2}-x^{2}-y^{2})^{3/4}} \\ \\ 
u_{xx} = \frac{2x^{2}+c^{2}t^{2}-y^{2}}{(c^{2}t^{2}-x^{2}-y^{2})^{5/2}} \\ \\ 
u_{yy} = \frac{2y^{2}+c^{2}t^{2}-x^{2}}{(c^{2}t^{2}-x^{2}-y^{2})^{5/2}} \\ \\
\end{gather}
$$
Now we plug $u_{xx},u_{yy}$ into the wave equation and they indeed equal $u_{tt}$, 
$$
\begin{gather}
\frac{c^{2}(2x^{2}+c^{2}t^{2}-y^{2}+2y^{2}+c^{2}t^{2}-x^{2})}{(c^{2}t^{2}-x^{2}-y^{2})^{5/2}} \\ \\ 
\frac{c^{2}(x^{2}+2c^{2}t^{2}+y^{2})}{(c^{2}t^{2}-x^{2}-y^{2})^{5/2}} \\ \\ 
\frac{2c^4t^{2}+c^{2}(x^{2}+y^{2})}{(c^{2}t^{2}-x^{2}-y^{2})^{5/2}}
\end{gather}
$$
Thus the solutions are equal. Similar to the last equation, on the cone, the solution is undefined.

#### 9.2.5

We are asked to find where a three dimensional wave equation vanishes given that $\phi,\psi$ vanish outside the sphere. We begin with the three dimensional wave equation
$$
\begin{gather}
u_{tt} = c^{2} (u_{x x}+u_{yy}+u_{zz}) \hspace{.5cm} -\infty<x,y,z<\infty \hspace{.5cm}t>0\\ \\
u(x,y,z,0)= \phi(x,y,z) \hspace{.5cm}u_{t}(x,y,z) = \psi(x,y,z)
\end{gather}
$$
We know the general solution says 
$$
\begin{gather}
u(x,y,z,t) = \frac{1}{4\pi c^{2}t_{0}} \iint _{S} \phi \, dS+ \frac{ \partial  }{ \partial t_{0} }\left[ \frac{1}{4\pi c^{2}t_{0}} \iint_{S} \phi(x,y,z) \, dS  \right] 
\end{gather}
$$
This equation represents the solutions of the wave equation in three dimensions. We have the solutions to the wave equation $u$ is non-zero wherever  $\phi,\psi$ are non-zero inside. We know this is inside and on the sphere.  This can be described geometrically by a cone that has an apex of cone of apex $x_{a},y_{a},z_{a}$

![[Pasted image 20240408170812.png|center|300]]
That is, what lies inside of the shaded region and the green cone, and everything inside, constitutes a non-zero solution for $u$. Now let's consider two different cones, one that lies outside the radius of $ct$, and another that has an volume intersecting Cone a. Trivially, any cones that do not have intersection with the cone we've described above (not in the radius of $ct$), does not have a non-zero solution, because we know $\phi,\psi$ are zero. Let's consider a different cone, one that doesn't entirely intersect with the cone, 

![[Drawing 2024-04-08 16.18.27.excalidraw.svg|center|300]]

Thus the solution for the wave equation exists by the enclosure of the dashed lines (not including them). We can take this specific example, and rotate it about the t axis to account for any angle and overlap. It looks like the following image

![[Drawing 2024-04-08 17.16.07.excalidraw|center|300]]
Where any volume enclosed by the shape produces a non-zero solution.

#### 9.2.11

We find all the spherical solutions of the three-dimensional wave equation that depend only on $r,t$. We begin with the 3-D wave equation in spherical coordinates given by
$$
\begin{gather}
u_{tt}= c^{2}\nabla^{2}u \\ \\ 
\nabla^{2}u = u_{rr}+ \frac{2}{r}u_{r}+\underbrace{  \frac{1}{r^{2}\sin\theta}\frac{ \partial  }{ \partial \theta } (\sin\theta)+ \frac{1}{r^{2}\sin ^{2}\theta}u_{\phi \phi} }_{ \text{tangential } } \\ \\
\end{gather} 
$$
Since our solution doesn't depend on $\theta$, we don't have to worry about the tangential component of $\nabla^{2}u$. Thus, our wave equation expanded becomes
$$
\begin{gather}
u_{tt} = c^{2} \left( u_{rr}+ \frac{2}{r}u_{r} \right)
\end{gather}
$$
We can multiply both sides by $r$ such that 
$$
\begin{gather}
ru_{tt}= c^{2}(ru_{rr}+2u_{r})
\end{gather}
$$
Now, we'll make the following change of variable such that 
$$
\begin{gather}
h(r,t) = ru(r,t) \\ \\ 
h_{tt}=ru_{tt} \\ \\ 
h_{r} = 1\cdot u+ru_{r}  = u+ru_{r}\\ \\ 
h_{rr}  = u_{r}+(u_{r}+ru_{rr}) = 2u_{r}+ru_{rr} \\ \\ 
\end{gather}
$$

With our substitution, we've reached the one-dimensional wave equation for which we already know it's solutions from page 33: 
$$
\begin{gather}
h_{tt} = c^{2}h_{rr} \\ \\ 
h(r,t) = f(r+ct)+g(r-ct) 
\end{gather}
$$
Thus, our solution $u$ is 
$$
\begin{gather}
u(r,t) = \frac{f(r+ct)+g(r-ct) }{r}
\end{gather}
$$

### Part 2

#### 1a)

We have a symmetric positive definite $n\times n$ real matrix  $A$ for all nonzero elements $x,b \in \mathbb{R}^n$. We consider the quadratic polynomial 
$$
\begin{gather}
Q(x) = \frac{1}{2}(\mathbf{x}|A\mathbf{x})- (\mathbf{b}|\mathbf{x})
\end{gather}
$$
We wanted to show that $Q$ is bounded below such that $Q(x) \geq m$ for all $x\in\mathbb{R}^n$. Firstly, what ever $Q(x)$ should be, it should be a constant for any value of x. That is, the matrix multiplication $A \mathbf{x}$ is a $n\times 1$ matrix and it's inner product with $\mathbf{x}$ produces a constant. This constant must be positive as given by the question. That is 
$$
\begin{gather}
\frac{1}{2}(\mathbf{x}|A\mathbf{x}) = \\ \\ 
\frac{1}{2}x_{1}(a_{11}x_{1}+a_{12}x_{2}+\dots+a_{1n}x_{n})+\dots+\frac{1}{2}x_{n}(a_{n_{1}}x_{n}+a_{n_{2}}x_{2}+\dots+a_{nn}x_{n})
\end{gather}
$$
if $H_{i}$ is the inside of the parenthesis of the last math line, and $i$ corresponds to the $1,2,3\dots n$th term, then it can be rewritten as 
$$
\begin{gather}
\frac{1}{2}(\mathbf{x}|a \mathbf{x}) = \frac{1}{2}x_{1}(H_{1})+\frac{1}{2}x_{2}(H_{2})+\dots+\frac{1}{2}x_{n}(H_{n}) = C_{1}
\end{gather}
$$
we have that $(b|x)$ looks like
$$
\begin{gather}
(b|x) = b_{1}x_{1}+b_{2}x_{2}+\dots+b_{n}x_{n} = C_{2}
\end{gather}
$$
where $C_{1},C_{2}$ are constants whose values depends on how large $n$ is. thus for any $\mathbf{x}$. we have, 
$$
\begin{gather}
Q(x) = C_{1}-C_{2}= C_{3}
\end{gather}
$$
a finite constant. A finite constant must have a constant smaller or equal to it, which we denote $m$. 

#### 1b)

We suppose that $x_{0} \in \mathbb{R}^n$ minimizes Q. We show that $Ax_{0}=b$. We take the approach that for any $y \in \mathbb{R}^n$, we consider a function $Q(x_{0}+ \epsilon y)$ in $\epsilon$ which has a minimum at $\epsilon=0$. So the derivative with respect to $\epsilon$ vanishes at $\epsilon=0$. Let's expand $Q(x_{0}+ \epsilon y)$, 
$$
\begin{gather}
Q(x_{0}+\epsilon y) = \frac{1}{2}(x_{0}+\epsilon y|A(x_{0}+\epsilon y))- (b|x_{0}+\epsilon y)
\end{gather}
$$
at $\epsilon=0$ we have the following 
$$
\begin{gather}
Q(x_{0}) =\frac{1}{2}(x_{0}|Ax_{0})- (b|x_{0})
\end{gather}
$$
which we know minimizes $Q$. We can rewrite $Q(x_{0})$ taking the inner products
$$
\begin{gather}
Q(x_{0}) = \frac{1}{2}x_{0}(Ax_{0}-b)
\end{gather}
$$
Since $(x|Ax)$ is always greater than zero and non-zero, $Ax_{0}\geq 0$. Thus we have the following cases 
$$
\begin{gather}
b=0 \hspace{.5cm}Q(x_{0})= \frac{1}{2}Ax_{0}^{2}>0\\ \\ 
b<0 \hspace{.5cm}Q(x_{0})= \frac{1}{2}Ax_{0}^{2}>0 \\ \\ 
\end{gather}
$$
The last case is when $b>0$, which depending on what positive value that is, can make $Q(x_{0})<0$ or positive. Since $Q(x_{0})$ is bounded, we have to have that $b=Ax_{0}$, the minimum value that $Q(x)$ can be. 


#### 2
Given the conditions we've stated in the problem, we have the following function $J$ on $S$, 
$$
\begin{gather}
J(u) = \int _{\Omega}\left[ \frac{1}{2}|\nabla u|^{2}+F(x)u \right] \, d^{3}x 
\end{gather}
$$
we consider a smooth function $v$ on an open subset $\mathbb{R}^{3}$ which contain the closure of $\Omega$ such that $v$ vanishes on the boundary. Thus we have for some real number $\epsilon$, 
$$
\begin{gather}
\int_{\Omega} \left[ \frac{1}{2}|\nabla u+\epsilon \nabla v|^{2}+F(x)(u+\epsilon v) \right] \, d^{3}x 
\end{gather}
$$
we can expand this integral to be 
$$
\begin{gather}
\int _{\Omega} \frac{1}{2}\nabla^{2}u+\epsilon \nabla u\nabla v+\frac{1}{2}\epsilon^{2}\nabla^{2}v+F(x)u+F(x)\epsilon v \, dx 
\end{gather}
$$
We take the derivative with respect to $\epsilon$, to find 
$$
\begin{gather}
\int _{\Omega}\nabla(uv)+\epsilon \nabla^{2}v +F(x)v \, dx 
\end{gather}
$$