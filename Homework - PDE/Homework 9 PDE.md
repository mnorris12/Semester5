### Part 1

#### 9.2.12
We solve the three dimensional wave equation with zero initial conditions and the limiting condition 
$$
\begin{gather}
\lim_{ r \to 0 } 4\pi r^{2}u_{r}(r,t)= g(t) \\ \\ 
g(0)=g'(0) = g''(0)=0
\end{gather}
$$

We'll start off by expressing the wave equation in spherical coordinates 
$$
\begin{gather}
u_{tt} = c^{2}\left(  u_{rr}+\frac{2}{r}u_{r} \right)
\end{gather}
$$
as before, there are angular derivatives that we don't need, so we can get rid of them to produce the spherical coordinates wave equation above. Similar to 9.2.11 from last week, we'll make the substitution, 
$$
\begin{gather}
h(r,t) = ru(r,t)
\end{gather}
$$
we find the derivative of $h(r,t)$, 
$$
\begin{gather}
h_{t} = ru_{t} \hspace{.5cm}h_{tt} =ru_{tt} \hspace{.2cm}u_{tt}=\frac{h_{tt}}{r} \\ \ \
h_{r} = u+ru_{r} \hspace{.5cm} h_{rr} = 2u_{r}+ru_{rr} \rightarrow u_{rr}+\frac{2}{r}u_{r}= \frac{h_{rr}}{r}
\end{gather}
$$
we immediately see that $h$ satisfies the one dimensional wave equation on the half line that we are familiar with! Thus we can rewrite the problem, 
$$
\begin{gather}
h_{tt} -c^{2}h_{rr}= 0 \\ \\ 
h(r,0) = ru(r,0) = 0 \\ \\ 
h_{t}(r,0) = ru_{t}(r,0)= 0
\end{gather}
$$
Now we plug in the $h$ into the boundary condition such that, 
$$
\begin{gather}
\lim_{ r \to 0 } 4\pi r^{2} \frac{ \partial  }{ \partial r } \left( \frac{h(r,t)}{r} \right) = g(t) \\ \\
\lim_{ r \to 0 } 4\pi r^{2} \frac{rh_{r}-h}{r^{2}} = g(t) \\ \\ 
\lim_{ r \to 0 } 4\pi rh_{r}-4\pi h = g(t) \\ \\ 
-4\pi h(0,t) = g(t) \\ \\ 
v(0,t) = -\frac{g(t)}{4\pi}
\end{gather}
$$
Now, we'll compare our wave equation to the general form of a partial differential equation such that 
$$
\begin{gather}
Au_{tt} +Bu_{rt}+Cu_{rr}+Du_{t}+Eu_{r}+Fu = G \\ \\ 
A= 1 \hspace{.5cm}B=D=E=F=G=0 \hspace{.5cm} C = -c^{2} \hspace{.5cm}
\end{gather}
$$
Thus we can use this formula to find the characteristic equations for the PDE, 
$$
\begin{gather}
\frac{dr}{dt} = \frac{1}{2A}(B \pm \sqrt{ B^{2}-4AC }) \\ \\
\frac{dr}{dt} = \frac{1}{2(1)}(0 \pm \sqrt{ 0^{2}-4(1\cdot-c^{2}) }) \\ \\ 
\frac{dr}{dt} = \frac{1}{2}(\pm\sqrt{ 4c^{2} }) = \pm c
\end{gather}
$$
Since the argument inside the square root of the first $\frac{dr}{dt}$ expression is positive, the characteristic curves are real and distinct. They are
$$
\begin{gather}
\frac{dr}{dt} = c \rightarrow r= ct+ \xi \\ \\ 
\frac{dr}{dt} =-c \rightarrow r=-ct+\eta
\end{gather}
$$
with this said, we must consider the solution to wave equation on two separate occasions
$$
\begin{gather}
r-ct<0 \\ \\ 
r-ct<0
\end{gather}
$$
![[Drawing 2024-04-15 06.35.56.excalidraw.svg|center|300]]

We realize for the second case that the solution $h$ is around a closed triangle with no reflection occurring on the boundary, this $h$ must equal zero, 

![[Drawing 2024-04-15 06.39.37.excalidraw.svg|center|300]]

For the case of $r-ct<0$, it gets more complicated as there are some reflections we must consider!
![[Drawing 2024-04-15 06.42.18.excalidraw.svg|center|300]]

Now we are to integrate the wave equation over the boundary of the above shape, 
$$
\begin{gather}
\iint _{D_{2}} (h_{tt}-c^{2}hu_{rr}) \, dA  = \iint _{D_{2}}\left( \frac{ \partial  }{ \partial r } c^{2}v_{r}-\frac{ \partial  }{ \partial t } v_{t} \right) \, dA \\ \\ 
\end{gather}
$$
We apply Green's Theorem
$$
\begin{gather}
\oint _{\partial D} (h_{r}dr+c^{2}h_{r}dt)
\end{gather}
$$
We'll have to integrate over the four sides of the shape above. If the top leg is $L_{1}$, then in numerical order counterclockwise, 
$$
\begin{gather}
\int _{L_{1}+L_{2}+L_{3}+L_{4}}h_{t}dt+c^{2}h_{r}dr
\end{gather}
$$
in order to aid in find the value of the integrals, we'll states some information about each leg,
$$
\begin{gather}
L_{1}: r-r_{0}=c(t-t_{0}) \hspace{.5cm}dr=c dt \\ \\ 
L_{2}: r = -r_{0}-c(t-t_{0}) \hspace{.5cm} dr=-c dt \\ \\ 
L_{3}: t=0 \hspace{.5cm}dt=0  \\ \\ 
L_{4}: r-r_{0} = -c(t-t_{0})
\end{gather}
$$
So immediately $L_{3}$ vanishes and we only have to worry about three integrals where $h_{t}(r,0)=0$
$$
\begin{gather}
c\int _{L_{1}} (h_{t}dt+h_{r}dr) \, dx -c\int_{L_{2}} (h_{t}dt+h_{r}dr) - c\int_{L_{4}} (h_{t}dt+h_{r}dr) \\ \\ 
c\int _{L_{1}}dh -c\int _{L_{2}}dh -c\int _{L_{4}}dh \\ \\ 
\end{gather}
$$
For the sake of space, $h(r_{0},t_{0})$ has been separately evaluated after taking the integrals above, 
$$
\begin{gather}
h(r_{0},t_{0}) = -\frac{1}{4\pi}g\left( t_{0}-\frac{r_{0}}{c} \right) \\ \\ 
h(r,t) = -\frac{1}{4\pi}g\left( t-\frac{r}{c} \right)
\end{gather}
$$
now we replace $\frac{h}{r}=u$, 
$$
\begin{gather}
u(r,t) = -\frac{1}{4\pi r}g\left( t-\frac{r}{c} \right)
\end{gather}
$$
Thus our final solution to this wave equation is 
$$
\begin{gather}
u(r,t) = -\frac{1}{4\pi r}g\left( t-\frac{r}{c} \right) \hspace{.5cm}r-ct<0 \\ \\ 
u(r,t) = 0 \hspace{.5cm}r-ct>0
\end{gather}
$$
and we're done! Phew

#### 10.1.2

We solve the wave equation in the rectangle $R = (0<x<a, 0<y<b)$ with homogeneous Dirichlet boundary conditions, and the initial conditions $u(x,y,0)=(x,y)(b-y)(a-x)$, $u_{t}(x,y,0)\equiv0$. We are to solve the following wave equation, 
$$
\begin{gather}
u_{tt} = c^{2}(u_{xx}+u_{yy}) \hspace{.5cm} t>0 \\ \\ 
u(0,y,t) = 0 \hspace{.5cm}u(x,0,t) = 0 \\ \\ 
u(a,y,t) =0 \hspace{.5cm} u(x,b,t) = 0 \\ \\ 
u(x,y,0) = (x,y)(b-y)(a-x) \hspace{.5cm}u_{t}(x,y,0) = 0
\end{gather}
$$
We can use the method of separation of variables since we have a linear and homogenous solutions (boundaries) where $u(x,y,t)=X(x)Y(y)T(t)$. Thus the wave equation becomes
$$
\begin{gather}
XYT'' = c^{2}(X''YT +XY''T)
\end{gather}
$$
and the boundary conditions are, 
$$
\begin{gather}
X(0)Y(y)T(t) = 0 \rightarrow X(0) = 0 \\ \\ 
X(a)Y(y)T(t) = 0 \rightarrow X(a) = 0 \\ \\ 
X(x)Y(0)T(t) = 0 \rightarrow Y(0) = 0 \\ \\ 
X(x)Y(b)T(t) = 0 \rightarrow Y(b) = 0 \\ \\ 
\end{gather}
$$
Now we separate the variables as usual to find, 
$$
\begin{gather}
\frac{T''}{c^{2}T} = \frac{X''}{X}+\frac{Y''}{Y} = \lambda
\end{gather}
$$
Thus we have, 
$$
\begin{gather}
\frac{X''}{X} = \lambda-\frac{Y''}{Y} = \upsilon
\end{gather}
$$
where $\alpha$ is an additional constant we'll use. Thus we have the following three ODEs, 
$$
\begin{gather}
\frac{T''}{c^{2}T} =\lambda \hspace{.5cm} \frac{X''}{X}=\alpha \hspace{.5cm}\lambda-\frac{Y''}{Y}=\alpha
\end{gather}
$$
We know well the solution to $X$, and if $\alpha=\upsilon^{2}$
$$
\begin{gather}
X(x) = C\cosh\upsilon x+D\sinh\upsilon x \\ \\ 
X(0) = C = 0 \\ \\ 
X(a) = C\cosh\upsilon a+D\sinh\upsilon a = 0
\end{gather}
$$
Since it's possible for $\upsilon a\neq 0$, we must have that $D$ is zero, so $X(x)=0$ so no positive eigenvalues. Let's check for eigenvalues $\alpha = 0$
$$
\begin{gather}
X''(0) = 0 \\ \\ 
X(x) = C_{1}x+D_{1}  \\ \\ 
X(0) = C_{1} = 0 \\ \\ 
X(a) = C_{1}a+D_{1} = 0
\end{gather}
$$
So we have another trivial solutions. Now, let's check for negative eigenvalues such that 
$$
\begin{gather}
X'' = -\upsilon^{2}X
\end{gather}
$$
we have the general solutions
$$
\begin{gather}
X(x) = C_{2}\cos(\upsilon x)+D_{2}\sin(\upsilon x)
\end{gather}
$$
using boundary conditions, we determine $C_{2},D_{2}$
$$
\begin{gather}
X(0) = C_{2} = 0 \\ \\ 
X(a) = D_{2}\sin(\upsilon a) = 0 \\ \\ 
\upsilon_{n} = \frac{n\pi}{a}
\end{gather}
$$
Thus the negative eigenvalues are $\alpha = -\frac{n^{2}\pi^{2}}{a^{2}}$, which corresponds to the following eigenfunctions, 
$$
\begin{gather}
X(x) = C_{2}\cos\upsilon x+D_{2}\sin\upsilon x \\ \\ 
X_{n}(x) = \sin\left( \frac{n\pi x}{a} \right)
\end{gather}
$$
Now we can substitute this value in, in order to find $Y$, 
$$
\begin{gather}
\lambda- \frac{Y''}{Y} = -\frac{n^{2}\pi^{2}}{a^{2}} \\ \\ 
Y'' = \left( \lambda+\frac{n^{2}\pi^{2}}{a^{2}} \right)Y
\end{gather}
$$
Similar to the $X$ case, only negative eigenvalues work for $Y$. So we'll suppose $\lambda = -\omega^{2}$. Then we have the following ODE, 
$$
\begin{gather}
Y'' = -\left( \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} \right)Y
\end{gather}
$$
Thus the general solution of $Y(y)$ is,
$$
\begin{gather}
Y(y) = C_{3}\cos \sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} }y+ D_{3}\sin \sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} }y
\end{gather}
$$
applying the boundary conditions, 
$$
\begin{gather}
Y(0) = C_{3} = 0
Y(b) = D_{3}\sin \sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} }b
\end{gather}
$$
to avoid the trivial solutions we'll insist that $D_{3}\neq 0$
$$
\begin{gather}
\sin \sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} }b = 0 \\ \\ 
\sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} } = \frac{m\pi}{b} \\ \\ 
\omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} = \frac{m^{2}\pi^{2}}{b^{2}} \\ \\ 
\omega = \pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }
\end{gather}
$$
Thus we have the negative eigenvalues 
$$
\begin{gather}
\lambda= -\pi^{2}\left( \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} \right)
\end{gather}
$$
with the following eigenfunctions, 
$$
\begin{gather}
Y(y) = D_{3}\sin \sqrt{ \omega^{2}-\frac{n^{2}\pi^{2}}{a^{2}} }y \\ \\ 
Y_{m}(y) = \sin\left( \frac{m\pi y}{b} \right)
\end{gather}
$$
Finally, we can find a solution to the ODE $T$. The equation for $T$ is thus
$$
\begin{gather}
\frac{T''}{c^{2}T}  = \frac{X''}{X}+\frac{Y''}{Y} \\ \\ 
T'' = -c^{2}\pi^{2}\left( \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} \right)T
\end{gather}
$$
with general solution
$$
\begin{gather}
T(t) = C_{4}\cos c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }t+ D_{4}\sin c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }t
\end{gather}
$$


Now we're finally in a position to solve for $u(x,y,)$ which has the general form for separation of variables, 
$$
\begin{gather}
u(x,y,t) = \sum_{m=1}^\infty \sum_{n=1}^\infty  (A_{mn}\cos c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} } t+\\ \\B_{mn}\sin c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }t\sin\left( \frac{n\pi x}{a} \right)\sin\left( \frac{m\pi y}{b} \right))
\end{gather}
$$
now we use the initial conditions $u(x,y,0)=(x,y)(b-y)(a-x)$ and $u_{t}(x,y,0)=0$, to determine the coefficients. We start by taking the derivative of the solution.  
$$
\begin{gather}
u_{t}(x,y,y) = \sum_{m=1}^\infty \sum_{n=1}^\infty \left( c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }\right) \cdot \\ \\ 
\left( -A_{mn}\sin c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }t+B_{mn}\cos c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }t \right)\cdot \\ \\ 
\sin\left( \frac{n\pi x}{a} \right)\sin \frac{m\pi y}{a}
\end{gather}
$$
we finally apply the initial conditions such that
$$
\begin{gather}
u(x,y,0) = \sum_{m=1}^\infty \sum_{n=1}^\infty A_{mn}\sin\left( \frac{n\pi x}{a} \right)\sin\left( \frac{m\pi y}{a} \right)=(x,y)(b-y)(a-x) \\ \\ 
u_{t}(x,y,0) = \sum_{m=1}^\infty \sum_{n=1}^\infty c\pi \sqrt{ \frac{m^{2}}{b^{2}}+\frac{n^{2}}{a^{2}} }B_{mn}\sin\left( \frac{n\pi x}{a} \right)\sin\left( \frac{m\pi y}{b} \right)=0
\end{gather}
$$
in order for the second equation to be $0$ for all $x$, then $B_{mn}=0$. For the first equation we have, 
$$
\begin{gather}
\sum_{m=1}^\infty \sum_{n=1}^\infty A_{mn}\sin\left( \frac{n\pi x}{a} \right)\sin\left( \frac{m\pi y}{b} \right)\sin\left( \frac{g\pi y}{b} \right) =(x,y)(b-y)(a-x)\sin \frac{g\pi y}{b}
\end{gather}
$$
where we've multiplied the equation by $\sin\left( \frac{g\pi y}{b} \right)$ for reasons that will shortly become clear. We integrate both sides w/r/t/y 
$$
\begin{gather}
\int _{0}^b \sum_{m=1}^\infty\sum_{n=1}^\infty A_{mn}\sin \frac{\pi nx}{a}\sin \frac{m\pi y}{b}\sin \frac{g\pi y}{b}\, dy  \\ \\ 
=\int _{0}^b (x,y)(b-y)(a-x)\sin \frac{g\pi y}{b} \, dy \\ \\ 
\sum_{m=1}^\infty\sum_{n=1}^\infty A_{mn}\sin \frac{\pi nx}{a} \int _{0}^b \sin \frac{m\pi y}{b}\sin \frac{g\pi y}{b} \, dy  = x(a-x)\int _{0}^b y(b-y)\sin \frac{g\pi y}{b}\, dy 
\end{gather}
$$
From before, the integral on the left equals zero on every value of $m,n$ except when $m=g$. so we can rewrite the integrals, 
$$
\begin{gather}
\sum_{n=1}^\infty A_{mn}\sin \frac{n\pi x}{a}\int _{0}^b \sin \frac{^{2}m\pi y}{b} \, dy = x(a-x)\int _{0}^b y(b-y)\sin \frac{m\pi y}{b} \, dy
\end{gather}
$$
now we calculate the integrals, 
$$
\begin{gather}
\sum_{n=1}^\infty A_{mn}\sin \frac{n\pi x}{a}\left( \frac{b}{2} \right) = x(a-x)\left[ -\frac{2b^{3}[-1+(-1)^m]}{m^{3}\pi^{3}} \right]
\end{gather}
$$
Because this problem is being increasingly long, we'll continue the solution with the expression with the value of the constant $A_{mn}$
$$
\begin{gather}
A_{mn} = \frac{16a^{2}b^{2}}{m^{3}n^{3}\pi^6}[-1+(-1)^m][-1+(-1)^n]
\end{gather}
$$
Therefore we have
$$
\begin{gather}
u(x,y,t) = \frac{6a^{2}b^{2}}{\pi^6} \sum_{s=1}^\infty \sum_{z=1 } ^\infty \frac{1}{(2s-1)^{3}`(2z-1)^{3}} \\ \\ 
\cdot \cos\left[ c\pi \sqrt{ \frac{(2s-1)^{2}}{b^{2}} +\frac{(2z-1)^{2}}{a^{2}}t} \right] \sin \frac{(2z-1)\pi x}{a} \sin \frac{(2s-1)\pi y}{b}
\end{gather}
$$
which is the solution when $m=2s-1$ and $n=2z-1$, as when $m,n$ the sum vanishes. 
#### 10.1.3

We find the condition on $\gamma$ so that the concentration does not grow without bound. In order to do this, we'll evaluate the wave equation given with boundary conditions $u=0$ on all sides. Our wave equation is thus
$$
\begin{gather}
u_{t} = k \triangle u +\gamma u \hspace{.5cm} 0<x,y,z<a \hspace{.5cm}t>0 \\ \\
u(0,y,z,t) = 0 \hspace{.5cm} u(x,0,z,t) = 0 \hspace{.5cm}u(x,y,0,t) = 0 \\ \\ 
u(a,y,z,t) = 0 \hspace{.5cm} u(x,a,z,t) = 0 \hspace{.5cm} u(x,y,a,t) = 0 \\ \\ 
u(x,y,z,0)= 0
\end{gather}
$$
we can use the method of separation of variables such that our solution becomes a product of ODEs
$$
\begin{gather}
u(x,y,z,t) = X(x)Y(y)Z(z)T(t) \\ \\ 
XYZT' = K(X''YZT+XY''ZT+XYZ''T)+\gamma XYZT
\end{gather}
$$
where the boundary at $x,y,z,=0$ and $x,y,z=a$ (only one variable needs to satisfy) gives a $u=0$. We separate the the last equation as usual to find
$$
\begin{gather}
\frac{T'}{kT} = \frac{X''}{X} +\frac{Y''}{Y}+\frac{Z''}{Z}+\frac{\gamma}{k} \\ \\ 
\frac{T'}{kT}-\frac{\gamma}{k} = \frac{X''}{X}+\frac{Y''}{Y}+\frac{Z''}{Z} = \lambda
\end{gather}
$$
We can subtract $\frac{Z''}{Z}$ on both sides of the equation to get
$$
\begin{gather}
\frac{X''}{X}+\frac{Y''}{Y}= \lambda-\frac{Z''}{Z} = \upsilon \\ \\ 
\frac{X''}{X} = \upsilon-\frac{Y''}{Y} = \alpha
\end{gather}
$$
thus we have the following ODEs
$$
\begin{gather}
\frac{T'}{kT}-\frac{\gamma}{k}=\lambda \\ \\ 
\frac{X''}{X} = \alpha \\ \\ 
\upsilon-\frac{Y''}{Y}=\alpha \\ \\ 
\lambda-\frac{Z''}{Z} = \upsilon
\end{gather}
$$
Since this is similar to the last problem, and just as long, we'll save some time on the computation. We have the Eigenfunction of $X$, given $\alpha=j^{2}$, 
$$
\begin{gather}
X(x)=C\cosh(jx)+D\sinh(jx) \\ \\ 
X_{n}(x) = \sin\left( \frac{\pi nx}{a} \right) \hspace{.5cm}n>0
\end{gather}
$$
We can skip to such value of $X_{n}(x)$ because we already showed how to get there in the last question. The same process we also already showed for $Y(y)$ as it also happens to be equivalent. Thus we have 
$$
\begin{gather}
Y_{m}(y) = \sin \frac{m\pi y}{a} \hspace{.5cm} m>0
\end{gather}
$$
Now, although we didn't have $Z(z)$ in the last problem, we see a pattern that, after similar calculations to $X,Y$, $Z(z)$ should be 
$$
\begin{gather}
Z_{g}(z) = \sin \frac{g\pi z}{a} \hspace{.5cm}g>0
\end{gather}
$$
Thus, we can rewrite our original ODE such that
$$
\begin{gather}
\frac{T'}{kT} -\frac{\gamma}{k} =\frac{\pi^{2}}{a^{2}}(n^{2}+m^{2}+g^{2}) \\ \\ 
T' = k\left[ \frac{\gamma}{k} - \frac{\pi^{2}}{a^{2}}(n^{2}+m^{2}+g^{2}) \right]
\end{gather}
$$
We can notice that an exponential function will provide a function for $T(t)$ such that
$$
\begin{gather}
T(t) = C_{1}e^{ k\left[ \frac{\gamma}{k} - \frac{\pi^{2}}{a^{2}}(n^{2}+m^{2}+g^{2}) \right]t }
\end{gather}
$$
Now, in order to maintain the boundary conditions where $t>0$, what's inside the brackets in the previous equation must be $\leq 0$. Thus we have 
$$
\begin{gather}
\frac{\gamma}{k} - \frac{\pi^{2}}{a^{2}}(n^{2}+m^{2}+g^{2}) \leq 0 \\ \\ 
\gamma \leq \frac{k\pi^{2}}{a^{2}}(n^{2}+m^{2}+g^{2}) \\ \\ 
\end{gather}
$$
Using the smallest value for our integers, we finally have
$$
\begin{gather}
0<\gamma \leq \frac{3k\pi^{2}}{a^{2}}
\end{gather}
$$


#### Part 2 
#### 2

###### 1

We show that 
$$
\begin{gather}
\frac{d}{dx}J_{0}(x) = -J_{1}(x)
\end{gather}
$$
We have that in general 
$$
\begin{gather}
J_{n}(x) =  \sum_{l=0}^\infty \frac{(-1)^l}{l!(l+n)!} \left( \frac{x}{2} \right)^{2l+n} \hspace{.5cm}n\in\mathbb{Z} \\ \\ 
\end{gather}
$$
Where we've assumed $n\geq 0$Now let's evaluate $J_{0}(x)$, 
$$
\begin{gather}
J_{0}(x)  =\sum_{l=0}^\infty \frac{(-1)^l}{l!(l+0)!} \left( \frac{x}{2} \right)^{2l+0} = \\ \\ 
\sum_{l=0}^\infty \frac{(-1)^l}{(l!)^{2}} \left( \frac{x}{2} \right)^{2j}
\end{gather}
$$
Now we'll expand $J_{0}(x)$ which equals 
$$
\begin{gather}
J_{0}(x) = 1- \frac{x^{2}}{2^{2}}+\frac{x^4}{2^4(2!)^{2}}-\frac{x^6}{2^6(3!)^{2}}\dots \frac{x^{2n}}{2^{2n}(n!)^{2}}
\end{gather}
$$
Now let's evaluate its derivative, 
$$
\begin{gather}
\frac{d}{dx}(J_{0}(x)) = -\frac{x}{2}+\frac{x^{3}}{2^{3}(2!)}-\frac{x^5}{2^5(2!)(3!)} \pm \frac{x^{2n-1}}{2^{2n-1}(n)!(n-1)!}
\end{gather}
$$
Now let's evaluate $-J_{1}(x)$, 
$$
\begin{gather}
-J_{n}(x) = \sum_{l=0}^\infty \frac{(-1)^l}{l!(l+1)!} \left( \frac{x}{2} \right)^{2l+1} \\ \\ 
-J_{1}(x) = \sum_{l=0}^\infty \frac{(-1)^l}{l!(l+1)!}\left( \frac{x}{2} \right)^{2l+1}
\end{gather}
$$
now the sum is 
$$
\begin{gather}
-J_{1}(x) = -\frac{x}{2}+\frac{x^{3}}{2^{3}(2!)}-\frac{x^5}{2^5(2!)(3!)} \pm \frac{x^{2n-1}}{2^{2n-1}(n)!(n-1)!}
\end{gather}
$$
Which we notice is exactly the value of $\frac{d}{dx}(J_{0}(x))$, thus we've proven that they are equal. 

###### 2

We show that 
$$
\begin{gather}
\frac{d}{dx}(x^nJ_{n(x)}) = x^n J_{n-1}(x)
\end{gather}
$$
using WolframeAlpha, we have 
$$
\begin{gather}
\frac{d}{dx}(x^n)\sum_{l=0}^\infty   \frac{(-1)^l}{l!(l+1)!} \left( \frac{x}{2} \right)^{2l+1} = \\ \\ 
\frac{1}{2}x^n (J_{n-1}(x)+\frac{2nJ_{n}(x)}{x}-J_{n+1}(x) \hspace{.5cm} n\geq 0 \\ \\ 
=\frac{1}{2}x^nJ_{n-1}(x) + x^n\left( \underbrace{ J_{n}(x)- \frac{J_{n+1}(x)}{2}  }_{ \frac{1}{2} x^nJ_{n-1}(x)}\right) = \\ \\ 
x^nJ_{n-1}(x) 
\end{gather}
$$
Thus we've proved what we wanted!

### Part 3

#### 1a
We ask ourselves, given the the information in the problem statement is 
$$
\begin{gather}
u_{1}\left( \mathbf{0}, \frac{r_{0}}{c} \right) = u_{2}\left( \mathbf{0}, \frac{r_{0}}{c} \right)
\end{gather}
$$
Since this is a three dimensional wave equation, we can use the information we've derived from the method of spherical means. More specifically, we know that the value of $\Psi,\phi$ influence the values on the surface $\lvert \mathbf{x}-\mathbf{x_{1}} \rvert=ct$. In our case, we that $\mathbf{x_{1}=0}$ and that $ct=r_{0}$. Given equation 13 on page 237, we have that 
$$
\begin{gather}
u_{i}\left( 0, \frac{r_{0}}{c} \right)= \frac{1}{4\pi cr_{0}}\iint _{\lvert \mathbf{x} \rvert=r_{0}}\Psi(\mathbf{x}) \, ds
\end{gather}
$$
Thus we have
$$
\begin{gather}
u_{1}\left( 0, \frac{r_{0}}{c} \right)= \frac{1}{4\pi cr_{0}}\iint _{\lvert \mathbf{x} \rvert=r_{0}} g_{1}(\lvert x \rvert) \, dx \\ \\ 
u_{2}\left( 0, \frac{r_{0}}{c} \right)= \frac{1}{4\pi cr_{0}}\iint _{\lvert \mathbf{x} \rvert=r_{0}}g_{2}(\lvert x \rvert) \, dx
\end{gather}
$$
We're told that on the boundary of the sphere $g_{1}(r_{0})=g_{2}(r_{0})$ thus, given the bounds of the integral, the two equations are the same. Thus it is necessary that 
$$
\begin{gather}
u_{1}\left( \mathbf{0}, \frac{r_{0}}{c} \right)=u_{2}\left( \mathbf{0}, \frac{r_{0}}{c} \right)
\end{gather}
$$