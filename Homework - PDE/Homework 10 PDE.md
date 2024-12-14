### Part 1

#### 10.2.1

We show that the intial conditions of (26), all the $\cos \sqrt{ \lambda}ct$ terms in the series (18) are missing. We also show that $D_{nm}=C_{nm}=0$ for $n\neq 0$. 

We solve the wave equation with Dirichlet boundary conditions as the vibrations of a membrane with fixed boundaries can be modeled as a two dimensional wave equation using polar coordinates. Our equation is 
$$
\begin{gather}
u_{tt} = c^{2}(u_{rr}+\frac{1}{r}u_{r}+\frac{1}{r^{2}}u_{\alpha\alpha}) \hspace{.5cm}0\leq r\leq a \hspace{.4cm} 0\leq\alpha \leq 2\pi \\ \\ 
u(a,\theta,t) =0 \\ \\ 
u(r,\theta,0) =\phi(r) = 0 \\ \\ 
u_{t}(r,\theta,0)=\psi(r)

\end{gather}
$$
The general solution to the wave equation is given by equation 18, 
$$
\begin{gather}
u(r,\theta,t) = \sum_{m+1}^\infty J_{0}(\sqrt{ \lambda_{0m}r })(A_{0m}\cos \sqrt{ \lambda_{0m}ct}+C_{0m}\sin \sqrt{ \lambda_{0m}ct }) \\ \\ 
\hspace{.5cm}+\sum_{m,n=1}^\infty J_{n}(\sqrt{ \lambda_{nm}r })[(A_{nm}\cos n\theta+B_{nm}\sin n\theta)\cos \sqrt{ \lambda_{nm}ct } \\ \\ \hspace{.5cm}\hspace{.5cm}+(C_{nm}\cos n\theta+D_{nm}\sin n\theta)\sin \sqrt{ \lambda_{nm}ct }]
\end{gather}
$$
Now we take the derivative with respect to time to find, 
$$
\begin{gather}
u_{t}(r,\theta,t) = \sum_{m+1}^\infty J_{0}(\sqrt{ \lambda_{0m}r })\sqrt{ \lambda_{0m} }c(-A_{0m}\sin \sqrt{ \lambda_{0m}ct}+C_{0m}\cos \sqrt{ \lambda_{0m}ct }) \\ \\ 
\hspace{.5cm}+\sum_{m,n=1}^\infty J_{n}(\sqrt{ \lambda_{nm}r })[-\sqrt{ \lambda_{nm} }c(A_{nm}\cos n\theta+B_{nm}\sin n\theta)\sin \sqrt{ \lambda_{nm}ct } \\ \\ \hspace{.5cm}\hspace{.5cm}+\sqrt{ \lambda_{nm} }c(C_{nm}\cos n\theta+D_{nm}\sin n\theta)\cos \sqrt{ \lambda_{nm}}ct]
\end{gather}
$$
Now we utilize our initial conditions 
$$
\begin{gather}
u(r,\theta,0) = \sum_{m=1}^\infty A_{0m}J_{0}(\sqrt{ \lambda_{0m} }r)+\sum_{m=1} ^\infty \sum_{n=1}^\infty J_{n}(\sqrt{ \lambda_{nm} }r) \\ \\ \cdot (A_{nm}\cos n\theta+B_{nm}\sin n\theta) = 0 \\ \\ 
u_{t}(r,\theta,0) = \psi(r) = \sum_{m=1}^\infty J_{0}(\sqrt{ \lambda_{0m} }r)\sqrt{ \lambda_{0m} }cC_{0m}+ \\ \\ 
\sum_{m=1}^\infty \sum_{n=1}^\infty J_{n}(\sqrt{ \lambda_{nm} }r)\sqrt{ \lambda_{nm} }c(C_{nm}\cos n\theta+D_{nm}\sin n\theta)
\end{gather}
$$
Next, we find all the coefficients and show that
$$
\begin{gather}
A_{0m} = A_{nm} = B_{nm} = C_{nm} = D_{nm} = 0
\end{gather}
$$
This can get pretty lengthy, so for some of the mathematical steps, we'll just state some of the steps we skipped. For finding $A_{0m}$, we integrated equation 1 w/r/t/$\theta$ from 0 to $2\pi$. We then have two integrals equal to zero that make the $\sum_{n,m=1}^\infty$ term vanish. We are left with, 
$$
\begin{gather}
\sum_{n=1}^\infty A_{0m}J_{0}(\sqrt{ \lambda_{0m} }r)(2\pi) = 0
\end{gather}
$$
we multiply both sides of the equation by $J_{0}(\sqrt{ \lambda_{0q} }r)r$ for reasons that will shortly become clear. After that we integrate w/r/t/$r$, 
$$
\begin{gather}
\int _{0}^a 2\pi \sum_{m=1}^\infty A_{0m}J_{0}(\sqrt{ \lambda_{0m} }r)J_{0}(\sqrt{ \lambda_{0q} }r)r \, dr = 0 \\ \\ 
= 2\pi \sum_{m=1}^\infty A_{0m}\int _{0}^a J_{0}(\sqrt{ \lambda_{0m} }r)J_{0}(\sqrt{ \lambda_{0q} }r)r \, dr = 0
\end{gather}
$$
because $J_{0}$ is an odd function, similar to the nature of a $\sin$ function, the integral equals zero unless $m=n$. Thus we'll consider, 
$$
\begin{gather}
2\pi A_{0m}\int _{0}^a J_{0}^{2}(\sqrt{ \lambda_{0m} }r)r \, dr = 0 \\ \\
2\pi A_{0m}\left[ \frac{a^{2}}{2}J_{1}^{2}(\lambda_{0m}a) \right] = 0
\end{gather}
$$
Where we have used an WolframAlpha for the integral. Dividing everything to isolate $A_{0m}$, we have, 

$$
\begin{gather}
\boxed{A_{0m} = 0} 
\end{gather}
$$
To find $A_{nm}$ we first start by multiplying the equation by $\cos w\theta$ where $w$ i some positive integer. The we integrate w/r/t/$\theta$ from 0 to $2\pi$. We notice that in both of the sum terms, there is one integral equal to zero. Thus reduces our equation to 
$$
\begin{gather}
\sum_{m,n=1}^\infty A_{nm}J_{n}(\sqrt{ \lambda_{nm} }r)\int _{0}^{2\pi}\cos n\theta \cos p\theta \, d\theta=0 
\end{gather}
$$
similar to the reasoning we've stated above and on page 106 from Strauss, the integral is 0 unless $n=p$. We have, 
$$
\begin{gather}
\sum_{m,n=1}^\infty A_{nm}J_{n}(\sqrt{ \lambda_{nm} }r)\int _{0}^{2\pi}\cos ^{2} n\, d\theta=0 \\ \\
\sum_{m,n=1}^\infty A_{nm}J_{n}(\sqrt{ \lambda_{nm} }r)\pi \\ \\ 
\end{gather}
$$
We multiply both sides by $J_{n}(\sqrt{ \lambda_{nv}  }r)r$ where $v$ is some positive integer. We take out the sum and integrate w/r/t/$r$ and integrate from 0 to $a$, 
$$
\begin{gather}
\pi A_{nm}\int _{0}^a J_{n}^{2}(\sqrt{ \lambda_{nm} }r)r \, dr = 0 \\ \\ 
\boxed{A_{nm}=0}
\end{gather}
$$
Where similar to above, we know that integral. 
For $B_{nm}$ its the exact same process for $A_{nm}$ but instead of multiplying the expression by a $\cos$, we multiply it by a $\sin hp$ where $h$ is some positive constant. We integrate, some of the integrals equal zero, we want when $n=h$, we multiply both sides by $J_{n}(\sqrt{ \lambda_{nq} }r)r$ where $q$ is some positive integer. We integrate again to get
$$
\begin{gather}
\pi B_{nm}\left[ \frac{a^{2}}{2}J^{2}_{n+1}(\sqrt{ \lambda_{nm} }a) \right] = 0 \\ \\ 
\boxed{B_{nm} = 0}
\end{gather}
$$
So, all the $\cos \sqrt{ \lambda }ct$ terms vanish or are "missing" in equation 18. Luckily, $C_{nm}$ is the exact same process as $A_{nm}$, which steps I've already done once, and explained twice. What's lightly different is that the right hand side of the equation is not zero, but instead $\phi(r)$. It's no issue however, because when we multiply it by $\cos lp$, where $l$ is some positive integer, we integrate a $\cos$ function from 0 to $2\pi$ which equals zero anyway. We are left with, 
$$
\begin{gather}
c\pi \sqrt{ \lambda_{nm} }C_{nm}\left[ \frac{a^{2}}{2}J^{2}_{n+1}(\sqrt{ \lambda_{nm} }a) \right] = 0 \\ \\ 
\boxed{C_{nm}= 0}
\end{gather}
$$
For $D_{nm}$ its the same process as $C_{nm}$, and sort of an analog of $B_{nm}$ as $C_{nm}$ is to $A_{nm}$. We get, 
$$
\begin{gather}
c\pi \sqrt{ \lambda_{nm} }D_{nm}\left[ \frac{a^{2}}{2}J_{n+1}^{2}(\sqrt{ \lambda_{nm} }a)= 0 \right] \\ \\ 
D_{nm}= 0
\end{gather}
$$
I hope it's okay that I skipped some steps for the coefficients! The process to find them are identical, but as you may have noticed, this solution is really long, even still!

#### 10.2.2

Again, this solution will be quite long, so we'll explain a lot of the steps rather than write it out. 

We determine the vibrations of a circular drumhead (held fixed on the boundary) with the initial conditions $u=1-\frac{r^{2}}{a^{2}}$ and $u_{t}\equiv_{0}$ when $t=0$.

We have the wave equation
$$
\begin{gather}
u_{tt} =c^{2} \triangle u = c^{2}\left( u_{rr}+\frac{1}{r}u_{r}+\frac{1}{r^{2}}u_{\theta\theta} \right) \hspace{.5cm} 0\leq r\leq a, 0\leq\theta \leq 2\pi \\ \\ \
u(a,\theta,t) = 0
u(r,\theta,0) = f(r,\theta)
u_{t}(r,\theta,0) = g(r,\theta) = 0 \\ \\ 
R(a) = 0
\end{gather}
$$
We use the method of separation of variables such that 
$$
\begin{gather}
R\Theta T'' = c^{2}\left( R''\Theta T+\frac{1}{r}R'\Theta T+ \frac{1}{r^{2}}R\Theta''T \right)
\end{gather}
$$
We now proceed to separation of variables, 
$$
\begin{gather}
\frac{T''}{c^{2}T} = \frac{R''}{R}+\frac{1}{r} \frac{R'}{R}+\frac{1}{r^{2}} \frac{\Theta''}{\Theta} = \lambda \\ \\ 
\frac{r^{2}R''}{R}+r \frac{R'}{R}-r^{2}\lambda = - \frac{\Theta''}{\Theta} = \mu
\end{gather}
$$
We solve the ODE for $\Theta$, with which its boundary conditions are periodic. We'll first start by determining the positive eigenvalues such that $\mu=m^{2}$. We have the resulting Eigenfunction, 
$$
\begin{gather}
\Theta_{m}(\theta) =C\cos m\theta+D\sin m\theta
\end{gather}
$$
We now have the following equation for $R$,
 $$
\begin{gather}
r^{2}R''+rR'+(-r^{2}\lambda-m^{2})R = 0
\end{gather}
$$
It has solutions when we consider the negative eigenvalue $-\lambda$, 
$$
\begin{gather}
R(r) =C_{1}J_{m}(\sqrt{ -\lambda r })+DY_{m}(\sqrt{ -\lambda r })
\end{gather}
$$
which reduces to 
$$
\begin{gather}
R(r) = C_{1}J_{m}(\sqrt{ -\lambda r })
\end{gather}
$$
We now apply the boundary conditions such that, 

$$
\begin{gather}
R(a) = C_{1}J_{m}(\sqrt{ -\lambda a }) = 0 \\ \\ 
\lambda_{mn} = -\frac{\alpha^{2}_{mn}}{a^{2}}
\end{gather}
$$
Thus we can rexpress our eigenfunctions $R$, 
$$
\begin{gather}
R_{mn} =J_{m}\left( \frac{\alpha_{mn}}{a}r \right)
\end{gather}
$$
We now use the information we've gathered to solve for $T$, 
$$
\begin{gather}
T'' = -\frac{c^{2}\alpha^{2}_{mn}}{a^{2}}T
\end{gather}
$$
We have the following general solution, 
$$
\begin{gather}
T(t) = C_{2}\cos\left( \frac{c\alpha_{mn}t}{a} \right)+D_{2}\sin\left( \frac{c\alpha_{mn}t}{a} \right)
\end{gather}
$$
We consider the circumstance when $\mu=0$
$$
\begin{gather}
\Theta'' = 0 \\ \\ 
\Theta' = C_{3}
\end{gather}
$$
We now apply the second periodic boundary conditions to determine $C_{3}$, 
$$
\begin{gather}
\Theta'(0) =C_{3}=\Theta'(2\pi)
\end{gather}
$$
We have the general eigenfunction, 
$$
\begin{gather}
\Theta(\theta) = C_{3}\theta+D_{3}
\end{gather}
$$
We now apply the boundary conditions to the original function to obtain, 
$$
\begin{gather}
\Theta(0) = C_{4} = 2\pi C_{3}+D_{3}=\Theta(2\pi)
\end{gather}
$$
thus $C_{3}=0$. We now discuss the eigenfunction $R$ when $\mu=0$, 
$$
\begin{gather}
r^{2}R''+rR'-r^{2}\lambda R = 0
\end{gather}
$$
It has general solution, 
$$
\begin{gather}
R(r) = C_{5}J_{0}(\sqrt{ -\lambda }r)+D_{4}Y_{0}(\sqrt{ -\lambda }r)  \\ \\ 
R(r) = C_{5}J_{0}(\sqrt{ -\lambda  }r)
\end{gather}
$$
We now apply the boundary conditions such that, 
$$
\begin{gather}
R(a) = C_{5}J_{0}(\sqrt{ -\lambda a }) =0 \\ \\ 
\lambda_{0n} = -\frac{\alpha^{2}_{0n}}{a^{2}}
\end{gather}
$$
Thus we have the following Eigenfunction, 
$$
\begin{gather}
R_{0n}(r) = J_{0}\left( \frac{\alpha_{0n}}{a}r \right)
\end{gather}
$$
We now use this formula we arrived at $\lambda_{0n}$, 
$$
\begin{gather}
T'' = -\frac{c^{2}\alpha^{2}_{0n}}{a^{2}}T
\end{gather}
$$
which has general solution, 
$$
\begin{gather}
T(t) = C_{6}\cos\left( \frac{c\alpha_{0n}t}{a} \right)+D_{5}\sin\left( \frac{c\alpha_{0n}t}{a} \right)
\end{gather}
$$
There are no negative values of $\mu$ as it results in the trivial solution of $\Theta$. We finally meet the solutions $u$ which is the product of our $R,\Theta,T$ eigenfunctions, 
$$
\begin{gather}
u(r,\theta,t) = \sum_{n=1}^\infty \left( A_{0n}\cos\left( \frac{c\alpha_{0n}t}{a} \right)+B_{0n}\sin\left( \frac{c\alpha_{_{0n}}t}{a} \right) \right)J_{0}\left( \frac{\alpha_{0n}}{a}r \right) \\ \\ 
\hspace{.5cm} + \sum_{m,n=1}^\infty \left( A_{mn}\cos \left( \frac{c\alpha_{mn}t}{a} \right)+B_{mn}\sin\left( \frac{c\alpha_{mn}t}{a} \right) \right)J_{m}\left( \frac{\alpha_{mn}}{a}r \right)\cos m\theta \\ \\ 
+\sum_{m,n=1}^\infty \left( D_{mn}\cos\left( \frac{c\alpha_{mn}t}{a} \right)+E_{mn}\sin\left( \frac{c\alpha_{mn}t}{a} \right) \right)J_{m}\left( \frac{\alpha_{mn}}{a}r \right)\sin m\theta
\end{gather}
$$

Lastly, we need to determine the coefficients 
$$
\begin{gather}
A_{0n}, B_{0n}, A_{mn},B_{mn},D_{mn},E_{mn}
\end{gather}
$$
This could actually take forever. Like a seriously long right up, and since this is my last question, I realize the document is becoming extremely long. Luckily $u_{t} = g = 0$, which takes care of of all of the coefficients aside from $A_{0n}$. This is because many of the integrals we'll need to evaluate end up having $\sin$ or $\cos$ integrated from 0 to $2\pi$ which gives zero. So we evaluate $A_{0n}$.
$$
\begin{gather}
A_{0n} = \frac{1}{\pi a^{2}J_{1}^{2}(\alpha_{0n})}\int _{0}^{2\pi}\int _{0}^a \left( 1-\frac{r^{2}}{a^{2}} \right)J_{0}\left( \frac{\alpha_{0n}}{a}r \right)r\, dr  \, d\theta \\ \\
=\frac{2}{a^{2}J_{1}^{2}(\alpha_{0n})}\int _{0}^a \left( 1-\frac{r^{2}}{a^{2}} \right)J_{0}\left( \frac{\alpha_{0n}}{a}r \right)r \, dr 
\end{gather}
$$
With the help of WolframeAlpha, we find, 
$$
\begin{gather}
A_{0n} = \frac{2}{a^{2}J_{1}^{2}(\alpha_{0n})}\int _{0}^{\alpha_0n}\left( 1-\frac{^{2}}{\alpha^{2}_{0n}} \right)J_{0}(s)\left( \frac{as}{\alpha_{0n}} \right) \frac{a}{\alpha_{0n}} \, ds \\ \\ 
 \frac{2}{a^{2}J_{1}^{2}(\alpha_{0n})} [2J_{2}(\alpha_{0n})\alpha^{2}_{0n}] \\ \\ 
 \frac{4}{\alpha^{2}_{0n}J_{1}^{2}(\alpha_{0n})}J_{2}(\alpha_{0n})
\end{gather}
$$
We can simplify this further with known properties of Bessel functions, 
$$
\begin{gather}
A_{0n} = \frac{8}{\alpha^{3}_{0n}J_{1}(\alpha_{0n})}
\end{gather}
$$
Thus we have our final solution
$$
\begin{gather}
u(r,\theta,t) = \sum_{n=1}^\infty \frac{8}{\alpha_{0n}^{3}J_{1}(\alpha_{0n})}\cos\left( \frac{c\alpha_{0n}t}{a} \right)J_{0}\left( \frac{\alpha_{0n}}{a}r \right)
\end{gather}
$$
#### 10.2.5
We solve the diffusion equation in the disk of radius a, with $u=B$ on the boundary and $u=0$ when $t=0$, where $B$ is some constant. We first begin with our usual two dimensional but polar Initial boundary value problem, 
$$
\begin{gather}
u_{t} = k \triangle u = k \left( u_{rr}+\frac{1}{r}u_{r}+\frac{1}{r^{2}}u_{\theta\theta} \right) \hspace{.5cm} 0\leq r\leq a, \hspace{.3cm} 0\leq\theta \leq 2\pi \\ \\ 
u(a,\theta,t) =a \\ \\ 
u(r,\theta,0)= 0
\end{gather}
$$

Sine the solution is radial per the hint, meaning that $u=u(r,t)$, we can drop the angular derivative components such that the diffusion equation becomes, 
$$
\begin{gather}
u_{t} =k\left( u_{rr}+\frac{1}{r}u_{r} \right)
\end{gather}
$$
We'll make the following substitution $h(r,t) = u(r,t)-B$ such that 
$$
\begin{gather}
u_{t} = h_{t} \\ \\
u_{r} = h_{r} \\ \\ 
u_{rr} = h_{rr}
\end{gather}
$$
Thus we have the following diffusion equation in term so of $h$, 
$$
\begin{gather}
h_{t} = k\left( h_{rr}+\frac{1}{r}h_{r} \right)
\end{gather}
$$
We now evaluate $h$ for new initial conditions, 
$$
\begin{gather}
h(a,t) = B-B = 0
h(r,0) = 0-B = -B
\end{gather} 
$$
We can now use the method of separation of variables to solve this problem such that our solution $h(r,t)=R(t)T(t)$. Now our diffusion equation becomes, 
$$
\begin{gather}
R(r)T'(t) = k\left[ R''(r)T(t)+\frac{1}{r}R'(r)T(t) \right] \\ \\ 
h(a,t) =R(a)T(t)=0 \hspace{.5cm}R(a) = 0
\end{gather}
$$
We can separate the $T,R$s as usual to find
$$
\begin{gather}
\frac{1}{kT}T' =\frac{1}{R}\left( R''+\frac{1}{r}R' \right) = \lambda \\ \\ 
\begin{cases}
\frac{1}{kT}T' = \lambda   \\
\frac{1}{R}\left( R''+\frac{1}{r}R' \right)=\lambda
\end{cases}
\end{gather}
$$
We'll first begin by solving for a solution to $R$. We'll take both sides of the $R$ equation and multiply them by $r^{2}R$, 
$$
\begin{gather}
r^{2}R''+rR'-\beta^{2} r^{2}R = 0
\end{gather}
$$
where $\beta^{2}=\lambda$. We suppose $\lambda=-\gamma^{2}$ is a negative eigenvalue (again for space, I showed that the trivial solution comes about when $\lambda$ is positive and zero). Thus the general solution to the ODE is in terms of the Bessel Functions $J_{0},Y_{0}$ such that, 
$$
\begin{gather}
R(r)=CJ_{0}(\gamma r) + DY_{0}(\gamma r)
\end{gather}
$$
As $r$ gets smaller and smaller, $Y_{0}$ diverges so we have the following equation, 
$$
\begin{gather}
R(r) = CJ_{0}(\gamma r)
\end{gather}
$$
Now we'll use the boundary conditions, 
$$
\begin{gather}
R(a) = CJ_{0}(\gamma a)=0
\end{gather}
$$
we avoid the trivial solution and insist that $C\neq 0$. So we have, 
$$
\begin{gather}
J_{0}(\gamma a) =0 \\ \\ 
\gamma_{a} = \alpha_{0n} \hspace{.5cm} \gamma_{n}=\frac{\alpha_{0n}}{a} 
\end{gather}
$$
Thus we've figured out the Eigenfunction $R(r)$,
$$
\begin{gather}
R_{n}(r) = J_{0}\left( \frac{\alpha_{0n}}{a}r  \right)
\end{gather}
$$
We move on to the time component of $h$, the ODE $T$. We can now say
$$
\begin{gather}
\frac{dT}{dt} = -\frac{k\alpha^{2}_{0n}}{a^{2}}T \\ \\ 
T(t) = C_{1}e^{t (-k\alpha^{2}_{0n}/a^{2} )}
\end{gather}
$$
Thus, we now have a solution for $h(r,t)$ which is
$$
\begin{gather}
h(r,t) = \sum_{n=1}^\infty A_{n}e^{t (-k\alpha^{2}_{0n}/a^{2} )}J_{0}\left( \frac{\alpha_{0n}}{a}r \right)
\end{gather}
$$
determined by multiplying the eigenfunctions that compose $h$. We now use the initial conditions for $h$ such that, 
$$
\begin{gather}
h(r,0) = -B \\ \\ 
h(r,0) = \sum_{n=1}^\infty A_{n}J_{0}\left( \frac{\alpha_{0n}}{a}r \right)=-B \\ \\ 
\end{gather}
$$
We can multiply both sides by $J_{0}\left( \frac{\alpha_{0m}r}{a} \right)r$, similar to what we did when finding the value of the coefficients in 10.2.1. We arrive at, 
$$
\begin{gather}
\sum_{n=1}^\infty A_{n}J_{0}\left( \frac{\alpha_{0n}}{a}r \right)J_{0}\left( \frac{\alpha_{0m}r}{a} \right)r=-BJ_{0}\left( \frac{\alpha_{0m}r}{a} \right)r
\end{gather}
$$
We pull out constants and integrate with respect to $r$, 
$$
\begin{gather}
\int_{0}^r \sum_{n=1}^\infty A_{n}J_{0}\left( \frac{\alpha_{0n}}{a}r \right) J_{0}\left( \frac{\alpha_{0m}}{a}r \right)  \, dr =\int _{0}^a (-B)J_{0}\left( \frac{\alpha_{0m}}{a}r \right)r \, dr
\end{gather}
$$
The left hand side of the integral is zero unless $m=n$, so we have 
$$
\begin{gather}
A_{n}\int _{0}^a J_{0}^{2}\left( \frac{\alpha_{0n}}{a}r \right)r\, dr = -B\int _{0}^a J_{0}\left( \frac{\alpha_{0n}}{a}r \right)r \, dr  
\end{gather}
$$
We evaluate the integrals such that $A_{n}$ is, 
$$
\begin{gather}
A_{n} = - \frac{2B}{\alpha_{0n}J_{1}(\alpha_{0n})}
\end{gather}
$$
Now we can finally write out our solution in terms of $u(r,t)$, 
$$
\begin{gather}
u(r,t) = B-2B\sum_{n=1}^\infty \frac{1}{\alpha_{0n}J_{1}(\alpha_{0n})}e^{t (-k\alpha^{2}_{0n}/a^{2} )}J_{0}\left( \frac{\alpha_{0n}}{a}r \right)
\end{gather}
$$
The solution is checked and works!
### Part 2
We show that 
$$
\begin{gather}
\int x^{2}J_{0}(x) \, dx  = x^{2}J_{1}(x)+xJ_{0}(x)-\int J_{0}(x) \, dx 
\end{gather}
$$
We'll prove this by taking the derivative of the right hand side of the equation. It is, 
$$
\begin{gather}
\frac{d}{dx}\left( x^{2}J_{1}(x)+xJ_{0}(x)-\int J_{0}(x) \, dx  \right) \\ \\ 
= \left( 2xJ_{1}(x)+x^{2}\left( J_{0}(x)-\frac{J_{1}(x)}{x} \right) \right)+(J_{0}(x)-xJ_{1}(x))-J_{0}(x) \\ \\ 
2xJ_{1}(x)+x^{2}J_{0}(x)-xJ_{1}(x)\cancel{ +J_{0}(x) }-xJ_{1}(x)\cancel{ -J_{0}(x) } \\ \\ 
x^{2}J_{0}(x)-2xJ_{1}(x)+2xJ_{1}(x) = x^{2}J_{0}(x)
\end{gather}
$$
Thus we've shown that 
$$
\begin{gather}
\frac{d}{dx}\left( x^{2}J_{1}(x)+xJ_{0}(x)-\int J_{0}(x) \, dx  \right)  = x^{2}J_{0}(x)
\end{gather}
$$
or
$$
\begin{gather}
\int \frac{d}{dx} \,  \left( x^{2}J_{1}(x)+xJ_{0}(x)-\int J_{0}(x) \, dx  \right) =\int x^{2}J_{0}(x) \, dx  \\ \\ \boxed{\left( x^{2}J_{1}(x)+xJ_{0}(x)-\int J_{0}(x) \, dx  \right) = \int x^{2}J_{0}(x) \, dx}   
\end{gather}
$$
We also show that 
$$
\begin{gather}
\int _{0}^1 xJ_{0}(\alpha x) \, dx = \frac{1}{\alpha}J_{1}(x)
\end{gather}
$$
We'll first start off by expanding the sum inside the integral on the left. Normally, we have 
$$
\begin{gather}
xJ_{0}(\alpha x)= x\sum_{k=0}^\infty (-1)^k \frac{\left( \frac{\alpha x}{2} \right)^{2k}}{(k!)^{2}} \\ \\ 
\begin{cases}
k=0  \rightarrow x\\
k=1 \rightarrow - \frac{\alpha^{2}x^{3}}{4}\\
k=2 \rightarrow \frac{\alpha^4x^5}{64}\\
k=3 \rightarrow - \frac{\alpha^6x^7}{2304}
\end{cases}
\end{gather}
$$
now we integrate the test value entries for $k$, 
$$
\begin{gather}
\begin{cases}
k=0 \rightarrow \frac{x}{2} |_{0}^1 = \frac{1}{2} \\
k=1 \rightarrow \frac{\alpha^{2}x^4}{16}|_{0}^1 =- \frac{\alpha^{2}}{16} \\ 
k=2 \rightarrow\frac{\alpha^4x^6}{384}|_{0}^1 = \frac{\alpha ^4}{384}  \\
k=3 \rightarrow \frac{\alpha^6x^8}{18432} |_{0}^1 = \frac{\alpha^6}{18432}
\end{cases}
\end{gather}
$$
Now that we have the a few terms of the left hand side of the equality that we want to prove, let's take a look at the right hand side

$$
\begin{gather}
\frac{1}{\alpha}J_{1}(\alpha) = \frac{1}{\alpha}\sum_{k=0}^\infty (-1)^k \frac{\left( \frac{\alpha}{2} \right)^{1+2k}}{(1+k)!(k)!}
\end{gather}
$$
We'll list the first four terms
$$
\begin{gather}
\begin{cases}
k=0 \rightarrow \frac{1}{\alpha} \cdot \frac{\alpha}{2} = \frac{1}{2}\\
k=1 \rightarrow \frac{1}{\alpha} \cdot \frac{\left( -\frac{\alpha^3}{8} \right)}{2} = -\frac{\alpha^{2}}{16}\\
k=2 \rightarrow \frac{1}{\alpha} \cdot \frac{\left( \frac{\alpha^5}{32} \right)}{12} =\frac{\alpha^4}{384}\\
k=3 \rightarrow \frac{1}{\alpha} \cdot \frac{\left( -\frac{\alpha^7}{128} \right)}{144} = -\frac{\alpha^6}{18432}
\end{cases}
\end{gather}
$$
As we can see, the first four terms are equal. If we continue to expand them, we would find that all their terms would be equal, thus we've proven the equality. 
#### 2
We prove that if $\alpha$ is a root of the equation 
$$
\begin{gather}
J_{0}(x) = 0 \hspace{.3cm}\text{then} \hspace{.3cm}\int _{0}^\alpha J_{1}(x)\, dx =1 \hspace{.5cm}\text{is true}
\end{gather}
$$
This can be interpreted as when $x=\alpha$ then $J_{0}(x)=0$ or simply $J_{0}(\alpha) = 0$. Our next step will be to evaluate the integral above,
$$
\begin{gather}
\int _{0}^\alpha J_{1}(x) \, dx =-J_{0}(x)|_{0}^\alpha = -(J_{0}(\alpha)-J_{0}(0)) = -(0-1) = 1
\end{gather}
$$
Thus we've proven the equality. 

#### 3

###### i

We prove that if 
$$
\begin{gather}
y = I_{0}(x) = J_{0}(\sqrt{ -1 }x) = J_{0}(ix)
\end{gather}
$$
Then it satisfies the equation
$$
\begin{gather}
\frac{d}{dx}\left( x \frac{dy}{dx} \right) = 0
\end{gather}
$$
We plug $I_{0}(x)$ in for $y$ using the identity that $\frac{d}{dx}J_{1}(x) = J_{0}(x)-\frac{J_{1}(x)}{x}$, 
$$
\begin{gather}
\frac{d}{dx}(-x iJ_{1}(ix))- xJ_{0}(ix) \\ \\ 
= -iJ_{1}(ix)-x i\left( iJ_{0}(ix)-\frac{iJ_{1}(ix)}{ix} \right)-xJ_{0}(ix) \\ \\ 
= -iJ_{1}(ix)-(-xJ_{0}(ix)-iJ_{1}(ix))-xJ_{0}(ix) =0
\end{gather}
$$
Thus we've proven that $I_{0}(x)$ is a solution to the differential equation. 

###### ii

We show that if $u(x)=\sqrt{ x }I_{0}(x) = (x)^{1/2}J_{0}(ix)$, then the following is true
$$
\begin{gather}
\frac{d^{2}u}{dx^{2}} = \left( 1-\frac{1}{4x^{2}} \right)u = (x)^{1/2}J_{0}(ix)-\frac{J_{0}(ix)}{4x^{3/2}}
\end{gather}
$$
We'll just have to use the product rule twice to find the second derivative. Things cancel out nicely, but the process is kinda of a mess:/

$$
$$
Thus, we've proved that $u$ satisfies the differential equation!

#### iii (extra credit)

We show, 

$$
\begin{gather}
\lim_{ x \to \infty } I_{0}(x) = \infty
\end{gather}
$$
given that $u(x) \approx Ae^{ x }$ for some positive constant $A$. 

We know from earlier that
$$
\begin{gather}
u(x)\approx Ae^{ x } \approx \sqrt{ x }I_{0}(x) \\ \\ 
I_{0}(x_{0}) \approx \frac{Ae^{ x }}{\sqrt{ x }}
\end{gather}
$$
When we take the limit
$$
\begin{gather}
\lim_{ x \to \infty } I_{0}(x) =\lim_{ x \to \infty } \frac{Ae^{ x }}{\sqrt{ x }}
\end{gather}
$$
We notice that as $x\rightarrow\infty$, that the exponential function increases faster than the rational function on the bottom, so it must go to infinity. 