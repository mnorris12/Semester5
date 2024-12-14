### Part 1

#### 5.5.2

We have the prove the Schwarz Inequality for any pair of functions such that,
$$
\begin{gather}
\lvert (f,g) \rvert \leq \lvert \lvert f \rvert \rvert \cdot \lvert \lvert g \rvert \rvert
\end{gather}
$$
We consider from the hint, 
$$
\begin{gather}
\lvert \lvert f+tg \rvert \rvert^{2}
\end{gather}
$$
We can rewrite the last math line,
$$
\begin{gather}
\lvert \lvert f+tg \rvert \rvert^{2} = \int _{a}^b \lvert f(x)+tg(x) \rvert^{2} \, dx  = \int _{a}^b \lvert f(x)+tg(x) \rvert [\langle f(x) \rangle +\langle tg(x) \rangle  ]\, dx 
\end{gather}
$$
where $\langle  \rangle$ will represent the complex conjugate. We are now to differentiate the both sides of the equation with respect to $t$, 

$$
\begin{gather}
\frac{ \partial  }{ \partial t } \lvert \lvert f+tg \rvert \rvert^{2} = \frac{ \partial  }{ \partial t }  \int _{a}^b \lvert f(x)+tg(x) \rvert [\langle f(x) \rangle +\langle tg(x) \rangle  ]\, dx \\ \\ 
\text{we bring the partial derivative inside the integral} \\ \\ 
\int _{a}^b [f(x)+tg(x)]\langle g(x) \rangle \, dx 
\end{gather}
$$
From the hint, we now find the value of $t$ where the quadratic polynomial is zero,
$$
\begin{gather}
\int _{a}^b [f(x)+tg(x)]\langle g(x) \rangle  \, dx= 0 \\ \\ 
\int _{a}^b f(x)\langle g(x) \rangle  \, dx + t\int _{a}^b g(x)\langle g(x) \rangle  \, d = 0 
\end{gather}
$$
We'll notice the last math line is equal to
$$
\begin{gather}
\int _{a}^b f(x)\langle g(x) \rangle  \, dx + t\int _{a}^b g(x)\langle g(x) \rangle  \, d = (f,g)+t(g,g) = 0 \\ \\ 
t = -\frac{f,g}{\lvert \lvert g \rvert \rvert^{2}}
\end{gather}
$$
Now that we have a value for $t$, we can plug it in into the $L^2$ norm,
$$
\begin{gather}
\left\lvert  \left\lvert  f-\frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}  \right\rvert  \right\rvert^{2} = \int _{a}^b \left\lvert  f(x)-\frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}  \right\rvert^{2} \, dx  \\ \\ 

\end{gather}
$$
 Now we continue playing around and expanding then condensing the last math line, 
 $$
\begin{gather}
\left\lvert  \left\lvert  f-\frac{(f,g)}{\lvert \lvert  g\rvert \rvert^{2}}  \right\rvert  \right\rvert^{2} = \int _{a}^b \left[ f(x)-\frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}} \right]\left[ \langle f(x) \rangle -\left\langle  \frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}  \right\rangle \langle g(x) \rangle  \right]\, dx \\ \\ 
= \int _{a}^b f(x)\langle f(x) \rangle  \, d - \left\langle  \frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}  \right\rangle  \int _{a}^b f(x)\langle g(x) \rangle  \, d - \frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}\int _{a}^b g(x)\langle f(x) \rangle  \, dx+ \\ \\ \frac{(f,g)\langle f,g \rangle }{\lvert \lvert g \rvert \rvert^{4}}\int _{a}^b g(x)\langle g(x) \rangle \, dx  \\ \\
= \lvert \lvert f \rvert \rvert^{2}  - \left\langle  \frac{(f,g)}{\lvert \lvert g \rvert \rvert^{2}}  \right\rangle (f,g) - \frac{(f,g)}{\lvert \lvert g^{2} \rvert \rvert}(g,f)+\frac{(f,g)(f,g)(g,g)}{\lvert \lvert g \rvert \rvert^4} \\ \\ 
=\lvert \lvert f \rvert \rvert^{2} - \frac{\lvert (f,g) \rvert^{2}}{\lvert \lvert g \rvert \rvert^{2}} +\frac{\lvert (f,g) \rvert^{2}}{\lvert \lvert g \rvert \rvert^{2}} \\ \\ 
=\lvert \lvert f \rvert \rvert^{2}- \frac{\lvert (f,g) \rvert^{2}}{\lvert \lvert g \rvert \rvert^{2}}
\end{gather}
$$
We know that the $L^2$ norm is non negative, so we must have 
$$
\begin{gather}
\left\lvert  \left\lvert  f-\frac{f,g}{\lvert \lvert g \rvert \rvert^{2}}  \right\rvert  \right\rvert^{2} = \lvert \lvert f \rvert \rvert^{2}-\frac{\lvert (f,g) \rvert^{2}}{\lvert \lvert g \rvert \rvert^{2}} \geq 0 \\ \\ 
\text{multiply both sides by} \hspace{.2cm} \lvert \lvert g \rvert \rvert^{2} \\ \\ 
\lvert \lvert f \rvert \rvert^{2}\lvert \lvert g \rvert \rvert^{2}  -\cancel{ \lvert \lvert g^{2} \rvert \rvert } \frac{\lvert (f,g) \rvert^{2}}{\cancel{ \lvert \lvert g \rvert \rvert^{2} }}\geq 0 \\ \\\lvert \lvert f \rvert \rvert^{2}\lvert \lvert g \rvert \rvert^{2} - (\lvert (f,g) \rvert^{2}) \geq 0 \\ \\ \lvert \lvert f \rvert \rvert^{2}\lvert \lvert g \rvert \rvert^{2} \geq  \lvert (f,g) \rvert^{2}
\\ \\ 
\text{we take the square root of both sides to find} \\ \\
\lvert \lvert f \rvert \rvert \lvert \lvert g \rvert \rvert \geq \lvert (f,g) \rvert \\ \\ 
\text{thus}
\lvert (f,g) \rvert \leq \lvert \lvert f \rvert \rvert \cdot \lvert \lvert g \rvert \rvert
\end{gather}
$$
And we've proven the inequality.

#### 6.1.6

We solve 
$$
\begin{gather}
u_{xx}+u_{yy} = 1 
\end{gather}
$$
in the annulus $a<r<b$ with $u(x,y)$ vanishing on both parts of the boundary $r=a$ and $r=b$

We'll recognize that the above equations is Poisson's formula such that
$$
\begin{gather}
\nabla^{2}u=1
\end{gather}
$$
Due to the fact that we're working with an annulus, we want to use polar coordinates, 
$$
\begin{gather}
\frac{ \partial^{2}u }{ \partial r^{2} } +\frac{1}{r}\frac{ \partial u }{ \partial r } + \frac{1}{r^{2}}\frac{ \partial^{2}u }{ \partial \theta^{2} } = 1 
\end{gather}
$$
the last term on the left side vanishes as $u$ is only a function of $r$, 
$$
\begin{gather}
\frac{d^{2}u}{d^{2}r}+\frac{1}{r} \frac{du}{dr} =1
\end{gather}
$$
which is a first order differential equation. Similar to the method used by Strauss, we can multiply the entire equation by $r$ 
$$
\begin{gather}
r\frac{d^{2}u}{d^{2}r}+ \frac{du}{dr} =r \\ \\ 
\left( r \frac{du}{dr} \right)' = r \\ \\ 
r \frac{du}{dr} = \frac{r^{2}}{2} + c_{1} \\ \\ 
\frac{du}{dr} = \frac{r^{2}}{2}+c_{1}(r^{-1}) \\ \\ 
u(r) = \frac{r^{2}}{4}+c_{1}\ln r+c_{2}
\end{gather}
$$
Now we must apply the boundary conditions. That is $u(r)\rightarrow u(a)=u(b)=0$. This gives us a system of two equations, 
$$
\begin{gather}
u(a) = \frac{a^{2}}{4}+c_{1}\ln a+c_{2} = 0 \\ \\ 

u(b) = \frac{b^{2}}{4}+c_{1}\ln b+c_{2}= 0 \\ \\ 
u(a)-u(b) = \frac{a^{2}-b^{2}}{4} +c_{1} = 0 \\ \\ 
c_{1} = \frac{b^{2}-a^{2}}{4\ln\left( \frac{a}{b} \right)} \\ \\ 
c_{2} = \frac{\left( -a^{2}\ln\left( \frac{a}{b} \right)+\ln(a)(-b^{2}+a^{2}) \right)}{4\ln\left( \frac{a}{b} \right)} = \frac{a^{2}\ln(b)-b^{2}\ln(a)}{4\ln \frac{a}{b}}
\end{gather}
$$
Thus we have the final equation for $u$
$$
\begin{gather}
u(r) = \frac{r^{2}}{4}+ \frac{b^{2}-a^{2}}{4\ln\left( \frac{a}{b} \right)}\ln(r) +  \frac{a^{2}\ln(b)-b^{2}\ln(a)}{4\ln \frac{a}{b}}
\end{gather} \\ \\ 
$$
using Wolframe alpha to simplify, we have
$$
\begin{gather}
u(r)= \frac{(a^{2}(\ln(b)-\ln(r)))+b^{2}(\ln(r))-\ln(a)))+r^{2}\ln\left( \frac{a}{b} \right))}{4\ln\left( \frac{a}{b} \right)} =\\ \\
\frac{a^{2}\ln\left( \frac{b}{r} \right) - b^{2}\ln\left( \frac{r}{a} \right)+r^{2}\ln\left( \frac{a}{b} \right)}{4\ln\left( \frac{a}{b} \right)}
\end{gather}
$$
Replacing $r= \sqrt{ x^{2}+y^{2} }$, 
$$
\begin{gather}
u(x,y) = \frac{a^{2}\ln\left( \frac{b}{\sqrt{ x^{2}+y^{2} }} \right) - b^{2}\ln\left( \frac{\sqrt{ x^{2}+y^{2} }}{a} \right)+\sqrt{ x^{2}+y^{2} }\ln\left( \frac{a}{b} \right)}{4\ln\left( \frac{a}{b} \right)}
\end{gather}
$$

#### 6.1.7

We solve the three dimensional Poisson's equation such that,
$$
\begin{gather}
u_{x x}+u_{yy}+u_{zz} = 1 \hspace{.5cm} a<r<b
\end{gather}
$$
with $u(x,y,z)$ vanishing on both the inner and outer boundaries of the spherical shell. Again, we have
$$
\begin{gather}
\nabla^{2}u =1 \\ \\ 
u_{rr} +\frac{2}{r}u_{r}+\frac{1}{r^{2}}\left[ u_{\theta\theta}+\cot(\theta)u_{\theta}+\frac{1}{\sin ^{2}\theta} u_{\phi \phi} \right] =1 
\end{gather}
$$
Similar to the last example, we only care for $u(r)$. Thus, 
$$
\begin{gather}
\frac{d^{2}u}{dr^{2}}+\frac{2}{r} \frac{du}{dr}= 1
\end{gather}
$$
our integrating factor is $e^{\int \frac{2}{r}}=e^{2\ln(r)}=r^{2}$. So,
$$
\begin{gather}
\frac{r^{2}d^{2}u}{dr^{2}} +2r \frac{du}{dr} = r^{2}
\end{gather}
$$
$$
\begin{gather}
\left( \frac{r^{2}du}{dr} \right)' = r^{2}
\end{gather}
$$
Again, the steps are the same as last question to find $u$, 
$$
\begin{gather}
u(r) = \frac{r^{2}}{6}-\frac{c_{1}}{r}+c_{2}
\end{gather}
$$
After creating a system of equations to find the coefficients, we have 
$$
\begin{gather}
c_{1} = -\frac{1}{6}(a^{2}b+a b^{2}) \hspace{.5cm}c_{2}=-\frac{1}{6}(a^{2}+ab+b^{2})
\end{gather}
$$
so we have 
$$
\begin{gather}
u(r) = \frac{r^{2}}{6} +\frac{1}{6r}(a^{2}b+a b^{2})-\frac{1}{6}(a^{2}+ab+b^{2})
\end{gather}
$$
now we plug in for when $r=\sqrt{ x^{2}+y^{2}+z^{2} }$
$$
\begin{gather}
u(x,y,z) = \frac{ x^{2}+y^{2}+z^{2} }{6} +\frac{1}{6\sqrt{  x^{2}+y^{2}+z^{2}  }}(a^{2}b+a b^{2})-\frac{1}{6}(a^{2}+ab+b^{2})
\end{gather}
$$
and we're all set!

#### 6.1.10

We prove the uniqueness on the Dirichlet problem $\triangle u =f$ in $D$ where $u=g$ on bdy$D$ by the energy method

We first we'll create another function under the same conditions such that, 
$$
\begin{gather}
\triangle u =f \hspace{.5cm}u=g \hspace{.2cm}\text{on bdy}\hspace{.1cm}D \\ \\
\triangle v = f \hspace{.5cm}v=g \hspace{.2cm}\text{on bdy}\hspace{.1cm}D \\ \\
\end{gather}
$$
now we have that $\triangle w = \triangle (u-v) = f-f = 0$. So inside $D$, $w$ must be zero. Now we have, 
$$
\begin{gather}
u-v = g-g =0\hspace{.2cm}\text{on bdy}\hspace{.1cm}D \\ \\
\end{gather}
$$
We see that $w$ is homogeneous and satisfies the its respective boundary conditions. Now we multiply the Laplace equation for $w$ by itself and use the divergence theorem, 
$$
\begin{gather}
w\triangle w = 0 \\ \\
\iiint_{D}w\triangle w \, dvol = 0 \\ \\ 
\text{apply divergence theorem} \\ \\ 
\underbrace{ \iint _{bdy D}w\frac{ \partial w }{ \partial n } dS }_{ w = 0 \hspace{.1cm}\text{on bdy} } - \iiint_{D}\nabla w \cdot \nabla w \,dvol=0 \, \\ \\ 
\iiint_{D}\nabla w \cdot \nabla w \,dvol = \iiint_{D}\lvert \nabla w \rvert^{2} \,dvol =0
\end{gather}
$$

Thus $\nabla w = 0$. Thus if $w,\nabla w,\triangle w =0$ then $u=v$. 

####  6.1.11 (Extra Credit)
We show that there is no solutio to the following equation
$$
\begin{gather}
\triangle u = f \hspace{.5cm} \frac{ \partial u }{ \partial n } =g \hspace{.2cm}\text{on bdy}\hspace{.2cm}D
\end{gather}
$$
unless the following is true
$$
\begin{gather}
\iiint_{D}f dxdydz = \iint_{\text{bdy}\hspace{.1cm}D}g \, ds 
\end{gather}
$$
Then we show the analogue in one and two dimensions 

###### 3-D

We can rewrite the left side of the last math line as 
$$
\begin{gather}
\iiint_{D}\triangle u dV = \iiint_{D} \nabla \cdot \nabla u dV
\end{gather}
$$
once we apply the divergence theorem for the "unless" situation from above
$$
\begin{gather}
\iiint_{D} \nabla \cdot \nabla u dV = \oint \oint \nabla au \cdot \hat{n} \,dS 
\end{gather}
$$
That is equal to
$$
\begin{gather}
\oint \oint g \,dS 
\end{gather}
$$
So we've proved that for $\iiint_{D}f dxdydz$ to exist, we must have 
$$
\begin{gather}
\iiint_{D}f dxdydz  = \oint \oint g \,dS 
\end{gather}
$$

###### 2-D
using the same method of rewriting the Laplacian $\triangle=\nabla \cdot \nabla$, we have that 
$$
\begin{gather}
\oint _{\text{bdy} \hspace{.1cm}D} \nabla u\cdot \hat{n} \,ds = \iint_{D}f\, dA
\end{gather}
$$
Where we care for the area instead of the volume. Notice that we've used Green's theorem here which applies for the two dimensional case. Thus we have 
$$
\begin{gather}
\oint \frac{ \partial u }{ \partial n }  \,ds = \oint_{\text{bdy}\hspace{.1cm}D} g \,ds =\iint_{d} f\, dA  
\end{gather}
$$
Finally, we have
$$
\begin{gather}
\iint_{D} f \, dxdy  = \int _{\text{bdy}\hspace{.1cm}D} \, dx 
\end{gather}
$$
###### 1-D
This one is a little bit more interesting. Our Partial differential equation reduces to 
$$
\begin{gather}
\frac{d^{2}u}{dx^{2}} =f(x) \hspace{.5cm}a<x<b \\ \\ 
\end{gather}
$$
From our boundary conditions $\frac{du}{dn} = g$, we have that,

$$
\begin{gather}
\frac{du}{dx}(a) =A  \\ \\ 
\frac{du}{du}(b) = B
\end{gather}
$$
since the derivative of $u$ evaluated at the endpoints is equal to our original integral $\int _{a}^b f(x) \, dx$. We have that 
$$
\begin{gather}
B-A = \int _{a}^b f(x) \, dx 
\end{gather}
$$
since the boundary of a one dimensional function consists of two points, rather than a function, this makes sense!
#### 6.2.3

We find the harmonic function $u(x,y)$ in the square $D = {0<x<\pi, 0<y<\pi}$ for the following boundary conditions,
$$
\begin{gather}
u_{y} = 0 \hspace{.2cm}y=0,\pi \hspace{.5cm}u=0 \hspace{.2cm}x=0 \\ \\ 
u=\cos ^{2}y=\frac{1}{2}(1+\cos_{2}y)\hspace{.2cm}x=\pi
\end{gather}
$$
We have the following drawing, 

![[Pasted image 20240325111228.png|center|300]]

We can rewrite our conditions: 
$$
\begin{gather}
\triangle u =0 \hspace{.5cm}0<x<\pi \hspace{.2cm}0<y<\pi \\ \\ 
u_{y}(x,0) = 0 \hspace{.5cm}u(0,y) = 0 \\ \\ 
u_{y}(x,\pi) = 0 \hspace{.5cm}u(\pi,y) = \frac{1}{2}(1+\cos(2y))
\end{gather}
$$
We realize that nearly all our boundary conditions are homogenous aside from $u(\pi,y)$ thus we can use the separation of variable technique as follows: 

We assume that our solution $u$ is of the form
$$
\begin{gather}
u=X(x)Y(y) \\ \\ 
X''Y+XY'' =0
\end{gather}
$$
a homogenous ordinary differential equation. Thus, 
$$
\begin{gather}
\frac{X''}{X} = -\frac{Y''}{Y} \\ \\ 
\frac{X''}{X} = -\frac{Y''}{Y} = \lambda
\end{gather}
$$
We know the last math line is true, because, $X,Y$ are in terms of different variables, so the equality must equal a constant. We now classify the Eigenvalues: 

**Positive Eigenvalues $\lambda=\mu^{2}$**
If $\lambda$ is a positive eigenvalue, we have 
$$
\begin{gather}
-\frac{Y''}{Y}= \mu^{2} = \lambda \\ \\ 
Y'' = -\mu^{2}Y \\ \\ 
\end{gather}
$$
From equation 6 on page 85, we see that $Y$ has general solution
$$
\begin{gather}
Y(y) = C\cos\mu y +D\sin\mu y
\end{gather}
$$
where
$$
\begin{gather}
Y'(y) = \mu(-C\sin\mu y+D\cos\mu y)
\end{gather}
$$
We now apply the boundary conditions,
$$
\begin{gather}
Y'(0)=\mu(D) = 0 \\ \\ 
Y'(\pi) = \mu(-C\sin\mu \pi+D\cos\mu \pi)
\end{gather}
$$
since $\mu \neq 0$, $D$ =0, so we have
$$
\begin{gather}
Y'(\pi) = \mu(-C\sin\mu \pi) = 0 \hspace{.2cm}\text{where} \hspace{.2cm}C\neq 0
\end{gather}
$$
Thus we have
$$
\begin{gather}
\sin\mu \pi =0 \hspace{.5cm}\mu_{n} = n
\end{gather}
$$
where $n$ is an integer. Thus we have
$$
\begin{gather}
Y_{n}(y) =\cos ny
\end{gather}
$$
Which is our eigenfunction. We do a similar process for $X$, 
$$
\begin{gather}
\frac{X''}{X} = \mu^{2} \\ \\ 
X''=\mu^{2}X  \\ \\ 
X(x) = C_{1}\cosh\mu x = D_{1}\sinh\mu x
\end{gather}
$$
applying the boundary conditions, we have 
$$
\begin{gather}
X(0) = C_{1} = 0
\end{gather}
$$
so we can immediately conclude that the eigenfunction is
$$
\begin{gather}
X(x)= D_{1}\sinh\mu x \rightarrow X_{n}x = \sinh nx
\end{gather}
$$

**Zero Eigenvalue $\lambda =0$**
For the eigenfunction $Y$ we thus have 
$$
\begin{gather}
-\frac{Y''}{Y}=0 \\ \\ 
Y''(y) = 0 \\ \\ 
Y'(y) = A
\end{gather}
$$
we apply the boundary conditions
$$
\begin{gather}
Y'(0) = 0 \hspace{.5cm}Y'(\pi) = 0
\end{gather}
$$
so $A = 0 = Y'(a)$. Now, 
$$
\begin{gather}
Y(y) = B
\end{gather}
$$
where $B$ is some arbitrary constant. Now we solve for $X$. Notice here that we'll evaluate the eigenfunction with its boundary conditions for the original function $X$ as opposed to $X'$ like we did for $Y$. 
$$
\begin{gather}
X(x) = A_{1}x+B_{1} \\ \\ 
X(0) = B_{1} =0\\ \\ 
X(x) = A_{1}x
\end{gather}
$$
where we insist $A_{1}\neq 0$. 

**Negative Eigenvalues $\lambda=-\gamma^{2}$**
The same process: 
$$
\begin{gather}
-\frac{Y''}{Y}= -\gamma^{2} \\ \\ 
Y'' = \gamma^{2}Y \\ \\
Y(y) = A_{2}\cosh\gamma y+B_{2}\sinh\gamma h \\ \\ 
Y'(y) = \gamma (A_{2}\sinh\gamma y+B_{2}\cosh\gamma y)
\end{gather}
$$
After applying the boundary conditions, there are no negative Eigenvalues by the same process we've done twice. 

 **Solution** 
We know that the general solution for $u$ is a linear combination of all $X(x)Y(y)$ for each determination of eigenvalues. 
So
$$
\begin{gather}
u(x,y) = B\cdot A_{1}x +\sum_{n=1}^\infty A_{n}\sin n x\cos ny \\ \\ 
\end{gather}
$$
Now, to determine our coefficients where $B\cdot A_{1}=A_{0}$, we'll finally use our inhomogeneous boundary condition $x=\pi$
$$
\begin{gather}
u(\pi,y) = A_{0}\pi+\sum_{n=1}^\infty A_{n}\sinh(n\pi)\cos(n\pi) = \frac{1}{2}(1+\cos(2y))
\end{gather}
$$
thus we have that, 
$$
\begin{gather}
A_{0}\pi = \frac{1}{2} \\ \\ 
A_{0} = \frac{1}{2\pi} \\ \\
\sum_{n=1}^\infty A_{n}\sinh(n\pi)\cos(n\pi) = \frac{1}{2} \cos(2y)
\end{gather}
$$
we notice that the 2 on the right side of the equation suggests that $n=2$, thus
$$
\begin{gather}
A_{2}\sinh(2\pi)\cos(2\pi) =\frac{1}{2}\cos(2y) \\ \\ 
A_{2}\sinh(2\pi) = \frac{1}{2} \\ \\ 
A_{2}=\frac{1}{2\sinh(2\pi)}
\end{gather}
$$
Thus our solution is 
$$
\begin{gather}
u(x,y) = \frac{1}{2\pi x}+ \frac{1}{2\sinh_{2}\pi}\sinh_{2}x
\end{gather}
$$
#### 6.3.3

We solve the Laplace's equation with the following boundary conditions,
$$
\begin{gather}
u_{x x}+u_{ y y}= 0 \\ \\
u=\sin ^{3}(\theta), \hspace{.2cm}r=a
\end{gather}
$$
that is the solution inside the boundary. We're also given the following hint

$$
\begin{gather}
\sin(3\theta) = 3\sin\theta-4\sin ^{3}\theta
\end{gather}
$$
Since we're dealing with a disk, we opt to use polar coordinates. Thus the Laplacian in polar coordinates can be expressed as the following,
$$
\begin{gather}
u_{rr} +\frac{1}{r}u_{r}+\frac{1}{r^{2}}u_{\theta\theta} = 0
\end{gather}
$$
Based on information $u=\sin ^{3}\theta$, we can guess a solution of the form, 
$$
\begin{gather}
u(r,\theta) =f(r)\sin\theta+g(r)\sin 3\theta
\end{gather}
$$
Now, we must take our guess and plug it into the original equation for $u$ in polar coordinates,
$$
\begin{gather}
[f(r)\sin\theta+g(r)\sin 3\theta]_{rr}+\frac{1}{r}[f(r)\sin\theta+g(r)\sin 3\theta]_{r}+\\ \\ \frac{1}{r^{2}}[f(r)\sin\theta+g(r)\sin 3\theta]_{\theta\theta} = 0
\end{gather}
$$
Thus we have
$$
\begin{gather}
f''(r)\sin\theta+g''(r)\sin_{3}\theta+\frac{1}{r}f'(r)\sin\theta+\frac{1}{r}g'(r)\sin_{3}\theta+ \\ \\ 
-\frac{1}{r^{2}}f(r)\sin\theta-\frac{9}{r^{2}}g(r)\sin_{3}\theta \\ \\ 
\end{gather}
$$
we'll take each of the functions $f,g$ and set them equal to zero such that
$$
\begin{gather}
f''(r)\sin\theta+g''(r)\sin_{3}\theta+\frac{1}{r}f'(r)\sin\theta = 0 \\ \\ 
\frac{1}{r}g'(r)\sin_{3}\theta+ 
-\frac{1}{r^{2}}f(r)\sin\theta-\frac{9}{r^{2}}g(r)\sin_{3}\theta = 0
\end{gather}
$$
we'll simplify the equations so the look nicer,
$$
\begin{gather}
r^{2}f''+rf'-f = 0 \\ \\ 
r^{2}g''+rg'-9g = 0 \\ \\ 
\end{gather}
$$
thus, we can use the Cauchy-Euler Equation where the general solutions are as follows, 
$$
\begin{gather}
f = r^m \hspace{.5cm}f' = mr^{m-1} \hspace{.5cm}y''=m(m-1)r^{m-2}
\end{gather}
$$
which is the same for $g$, but we'll replace the $m$'s with $n$'s. We'll start of with $f$ by plugging it in to it's equidimensional equation: 
$$
\begin{gather}
r^m[m(m-1)+m-1] = 0 \\ \\ 
(m^{2}-1) = 0 \\ \\ 
(m^{2}-1) = 0 \\ \\ 
m= \pm1
\end{gather}
$$
Using a similar process for $g$ we have,
$$
\begin{gather}
n=\pm 3
\end{gather}
$$
Thus $f,g$ are a linear combination of both values of $m,n$,
$$
\begin{gather}
f(r) = Ar+Br^{-1} \\ \\ 
g(r) = A_{1}r^{3}+B_{1}r^{-3} \\ 
\end{gather}
$$
where the last $B,B_{1}$ terms are zero to satisfy the condition at $r=0$. We use $u(a,\theta)$ from earlier to find
$$
\begin{gather}
u(a,\theta) = \sin ^{3}(\theta) = \frac{3}{4}\sin\theta-\frac{1}{4}\sin(3\theta) \\ \ \
Aa = \frac{3r}{4} \rightarrow A = \frac{3r}{4a}\\ \\ 
A_{1}a^{3} = \frac{r^{3}}{4} \rightarrow A_{1} = \frac{r^{3}}{4a^{3}}
\end{gather}
$$
Thus our solution is then
$$
\begin{gather}
u(r,\theta) = \frac{3r}{4 a}\sin\theta-\frac{r^{3}}{4 a^{3}}\sin_{3}\theta
\end{gather}
$$

#### Part 2

#### 2

###### a

We have $u(x)$ a twice differentiable solution which satisfies the following ODE, 
$$
\begin{gather}
u''+b(x)u'-c(x)u = 0
\end{gather}
$$
We show that $u$ cannot have a positive local maximum on the open interval $(0,1)$.

In our search for a local maximum or minimum, we set the derivative of our solution equal to zero, thus we have
$$
\begin{gather}
u''-c(x)u = 0
\end{gather}
$$
If there's a local maximum, by the second derivative test, we would expect 
$$
\begin{gather}
u'(p)=0 \\ \\ \
u''(p) <0
\end{gather}
$$
Thus our third to the last math line suggests
$$
\begin{gather}
\underbrace{ u'' }_{ neg }-c(x)\underbrace{ u }_{ pos } = 0
\end{gather}
$$
If $c(x)>0$ then the left side of the equation must be negative, which cannot equal zero. Thus at a point $u(p)$ when $p>0$, there can be no positive local maximum. For the minimum case we assume
$$
\begin{gather}
\underbrace{ u }_{ pos }''-c(x)\underbrace{ u }_{ neg }=0
\end{gather}
$$
so the left side of the equation must be a positive value which is not equal zero. Thus there can be no negative local minimum. 

###### b
Since $u$ is a harmonic function thats continuous on $\bar{D}$, we have from the maximum principle that the maximum and the minimum occur on the bdy $D$ and nowhere inside, unless $u$ is a constant. If $u$ is a constant, then we have 
$$
\begin{gather}
-c(x)u = 0
\end{gather}
$$
which would only be true if $c(x)=0$ but we know it's positive so $u \neq \text{constant}$. Thus if the maximum or minimum must occur on the boundaries $u(0)=u(1)=0$, then it must be that $u=0$

###### c 
(not included:/) wasn't for sure


#### 3 

We show that if $u$ satisfies
$$
\begin{gather}
4u_{x x}+3u_{yy}-5u= 0
\end{gather}
$$
in a region $D \in\mathbb{R}^{2}$, then $u$ cannot have a local positive maximum at a point $D$ (a local maximum $p \in D$ with $u(p)>0$. 

for this differential equation, we can utilize the Hessian matrix which entails for our two dimensional case,
$$
\begin{gather}
H(x,y) = \begin{pmatrix}
u_{x x} &u_{xy} \\
u_{yx}&u_{yy}
\end{pmatrix}
\end{gather}
$$
The useful information about the Hessian matrix, is that its determinant provides us some useful information about the max and min case for partial differential equations. That is, for our local maximum case, we want when determinant $\det H(p)>0$ and when $u_{x x}(p)<0$. Thus our determinant is 
$$
\begin{gather}
u_{xx}u_{yy}-(u_{xy})^{2}>0
\end{gather}
$$
Since $u_{x x}<0$ for our maximum case, $u_{yy}$ has to be less than zero other wise the left side of the equation would be a negative number, contradicting the inequality. Thus we have 
$$
\begin{gather}
\underbrace{ 4u_{x x} }_{ <0 }+\underbrace{ 3u_{yy} }_{ <0 }-\underbrace{ 5u }_{ >0 }= 0
\end{gather}
$$
which cannot happen! So, there can be no local positive Maximum. In the case of the minimum, we want the determinant greater than zero but $u_{x x}(p)>0$. Thus $u_{yy}$ must be positive and 
$$
\begin{gather}
u_{x x}u_{yy}>(u_{xy})^{2}
\end{gather}
$$
We also want when our solution $u$ is negative. Thus we have 
$$
\begin{gather}
\underbrace{ 4u_{x x} }_{ >0 }+\underbrace{ 3u_{yy} }_{ >0 }-\underbrace{ 5u }_{ <0 }= 0
\end{gather}
$$
which would suggest that the left side of the equation has a positive value which does not equal zero! Thus $u$ cannot have a local negative minimum at a point of $D$

#### 4
###### b

Because $u(x,y)$ is a twice differential function extended to a continuous function on the closure of $D$ and $u$ vanishes on the boundary $\partial D$ of D, then it's maximum and minimums are 0.  We know this by the maximum principle that the maximum and minimum of $u$ occurs on the boundary. Since it vanishes on the boundaries. $u$ must be 0 throughout the\
domain $D$. 

