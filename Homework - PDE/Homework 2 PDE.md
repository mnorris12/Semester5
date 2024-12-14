## Part 1
#### 1.2.10
We have the following equation $u_{x}+u_{y}+u= e^{ x+2y }$. Luckily, we can gather particular equality from this PDE to create an ODE, to solve for a solution: 
$$
\begin{gather}
u_{x}+u_{y} = \frac{du}{dx}= u-e^{ x+2y } \\ \\ 

\frac{du}{dx} - u = e^{ x +2y} \\ \\ 

y = (\zeta,0), \hspace{.2cm} y = x +\zeta
\end{gather}
$$
We'll realize that the middle equation is a first order linear ODE which can be solved by the following method; 
$$
\begin{gather}
I = e^{ \int p(x) \, dx  } \\ \\ 
\text{where} \hspace{.2cm} p(x) = 1 \hspace{.2cm} \text{so}\hspace{.2cm}I = e^x
\end{gather}
$$
We'll now multiply the value of $I$ times the entire ODE:
$$
\begin{gather}
\frac{du}{dx}e^{ x }+ u e^{ x } = e^{ x+2y }e^{ x } \\ \\

(ue^{ x })' = e^{ 2x+2y } \\ \\ 
\end{gather}
$$
We now integrate both sides of the equation, using $y = x+ \zeta$:
$$
\begin{gather}
\zeta = y - x \\ \\ 

\int (ue^{ x })' \, d = \int e^{ 2x+2y } \, dx \\ \\ 

ue^{ x } = \int e^{ 2(x+x+\zeta) } \, dx \\ \\ 

ue^{ x } = \int e^{ 4x+2\zeta } \, dx \\ \\ 

ue^{ x }= \frac{1e^{ 4x+2\zeta }}{4} + f(\zeta)
\end{gather}
$$
Thus we have: 
$$
\begin{gather}
u(x,\zeta) = \frac{ \frac{e^{ 4x+2\zeta }}{4} + f(\zeta)}{e^{ x }} \\ \\ 

u(x,y) = \frac{ \frac{e^{ 2x+2y }}{4} + f(y-x)}{e^{ x }} \\ \\ 

u(x,y) = e^{ x+2y } + \frac{f(y-x)}{e^{ x }}

\end{gather}
$$
Now we'll make use of our initial condition that $u(x,0) = 0$
$$
\begin{gather}
u(x,0) = e^{ x }+ \frac{f(-x)}{e^{ x }} \\ \\ 

f(-x) = -\frac{e^{ 2x }}{4} \hspace{.5cm} \text{or} \hspace{.5cm}f(w) = -\frac{e^{ -2w }}{4}
\end{gather}
$$
Thus we've arrived at
$$
\begin{gather}
u(x,y) = e^{ x+2y } + e^{ -x }\left( -\frac{e^{ -2(y-x) }}{4} \right)
\end{gather}
$$
#### 1.3.6

We know from example 5, heat flow that the three dimensional heat equation is modeled by: 
$$
\begin{gather}
\rho cu_{t} = \nabla \cdot (\kappa \nabla u)
\end{gather}
$$
We'll assume that $\kappa$ does not depend on spatial coordinates, we can rearrange the previous equation to: 
$$
\begin{gather}
\rho cu_{t}= k (\nabla \cdot \nabla u) = k (\nabla^{2}u)
\end{gather}
$$
We'll solve for $u_{t}$:
$$
\begin{gather}
u_{t}=d \nabla^{2}u
\end{gather}
$$
where $d= \frac{\kappa}{\rho}$. Now, we'll need to consider the laplacian operator $\mathscr{L}$ can be expressed as 
$$
\begin{gather}
\nabla^{2}u = \frac{1}{r} \frac{ \partial  }{ \partial r }\left( r \frac{ \partial u }{ \partial r }  \right) + \frac{1}{r^{2}} \frac{ \partial^{2}u }{ \partial \theta^{2} } + \frac{ \partial^{2}u }{ \partial z^{2} } 
\end{gather}
$$
we can continue our symmetry argument by realizing that, in our cylindrical coordinates, our equation is dependent on $r$ solely. So we rewrite it: 
$$
\begin{gather}
\nabla^{2} u = \frac{1}{r} \frac{ \partial  }{ \partial r }  \left( r \frac{ \partial u }{ \partial r }  \right)
\end{gather}
$$
We now return to the differential equation $u_{t}$ and replace the $\nabla^{2}u$:
$$
\begin{gather}
u_{t} = k\left[ \frac{1}{r} \frac{ \partial  }{ \partial r } \left( r \frac{ \partial u }{ \partial r }  \right) \right] \\ \\ 

u_{t} = k \left( \frac{1}{r} \frac{ \partial u }{ \partial r } +\frac{ \partial^{2}u }{ \partial r^{2} }  \right)
\end{gather}
$$
This is of the same form as: 
$$
\begin{gather}
u_{t} = k \left( u_{rr}+\frac{1}{r}u_{r} \right)
\end{gather}
$$
So our proof is complete. 

#### 1.5.3

We note that $u'' = 0$ suggest that $u= mx + n$. From here, we'll make note of the boundary conditions that $u'(0) + ku(0) = 0$. Thus $m+kn = 0$. 

**We'll first begin with the + case:** 

For the + case, we'll utilize $u'(1) \pm ku(1) = 0$. This would suggest that $m+k(m+n) = 0$.  From here, we'll use that information and apply it to the equation $m+kn = 0$ such that $m = -kn$, and also to the second equation 
$$
\begin{gather}
-kn +k(-kn+n) = -k^{2}n = 0
\end{gather}
$$
Now, in order for these equation to make sense, we'll start by looking at the second one, and seeing what we can generalize from that. If $k\neq 0$ then $n=0$. If $n$ is some number, then $k=0$. Using either of those conditions, we know from equation $m=-kn$ that $m=0$. Let's mathematically state that: 
$$
\begin{gather} u(x) = 
\begin{cases}
0 \hspace{.2cm}\text{when} \hspace{.2cm} k\neq 0  \\
n \hspace{.2cm}\text{when} \hspace{.2cm} k = 0
\end{cases}
\end{gather}
$$

**Now let's move on the $-$ case, and we'll use the similar strategies for that one:** 

The $-$ case tells us that 
$$
\begin{gather}
u'(1) - ku(1) = 0 \hspace{.5cm} \\ \\ 
m - k (m+n) = 0
\end{gather}
$$
So similarly to above, we see that 
$$
\begin{gather}
m = -kn \\ \\ 

n(k^{2} - 2k) = 0
\end{gather}
$$
In the conditions that $n=0$, we thus have that $m=0$, and k as some number. When $n\neq 0$ this must mean $k=0\hspace{.2cm}\text{or}\hspace{.2cm}2$. With this said, the following gives us the value $u(x)$ for every $k$
$$
\begin{gather} u(x)
\begin{cases}
0 \hspace{.5cm}\text{when} \hspace{.2cm} k\neq 0 \hspace{.2cm}\text{and} \hspace{.2cm} k\neq 2  \\
n \hspace{.5cm}\text{when} \hspace{.2cm} k = 0 \\
n(1-2x) \hspace{.5cm} \text{when} \hspace{.2cm} k=2
\end{cases}
\end{gather}
$$
Thus we've provided both the $\pm$ cases

#### 2.1.2

This is going to be a long process, so buckle up! We are going to solve: 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x}, u(x,0) = \log(1+x^{2}), u_{t}(x,0) = 4 + x
\end{gather}
$$
We'll solve this by Method of Characteristics! We'll start off with
$$
\begin{gather}
u_{tt} - c^{2}u_{x x} = 0
\end{gather}
$$
The characteristic equations of the PDE is given as follows: 
$$
\begin{gather}
\frac{dx}{dt} = \frac{1}{2a}(b \pm \sqrt{ b^{2}-4 ac }) \\ \\ 
\frac{dx}{dt} = \pm c
\end{gather}
$$
We note that the solutions to the ODEs are real and curves in the $tx$ plane: 
$$
\begin{gather}
x = ct + C_{1}, \hspace{.2cm}x = -ct + C_{2}
\end{gather}
$$
If we solve for $C_{1,2}$ we have that 
$$
\begin{gather}
C_{1} = x - ct \\ \\
C_{2} = x+ ct
\end{gather}
$$
Okay, let's make a change of variables! We'll start by assigning some of the new variables values in term so of the former ones: 
$$
\begin{gather}
\beta = x + ct\\ \\ 
\zeta = x - ct \\ \\ 
\end{gather}
$$
Now with the use of those conventions we can do the chain rule in terms of our new variables: 
$$
\begin{gather}
\frac{ \partial u }{ \partial t } = \frac{ \partial u }{ \partial \zeta } \frac{ \partial \zeta }{ \partial t } + \frac{ \partial u }{ \partial \beta } \frac{ \partial \beta }{ \partial t } = u_{\zeta}(-c) + u_{\beta}(c) = c(u_{\beta}-u\zeta) \\ \\ 

u_{tt} = \frac{ \partial^{2}u }{ \partial t^{2} } = c^{2} (u_{\beta\beta}-2u_{\zeta\beta}+ u_{\zeta\zeta})
\end{gather}
$$
also 
$$
\begin{gather}
\frac{ \partial u }{ \partial x }  = u_{\beta}+ u_{\zeta} \\ \\ 

u_{x x} = \frac{ \partial^{2}u }{ \partial x^{2} } = u_{\beta\beta} + 2u_{\zeta\beta} + u_{\zeta\zeta} 
\end{gather}
$$
Now that we have $u_{tt}$ and $u_{x x}$, we plug them in back into the original PDE: 
$$
\begin{gather}
c^{2} (u_{\beta\beta}-2u_{\zeta\beta}+ u_{\zeta\zeta}) -  u_{\beta\beta} + 2u_{\zeta\beta} + u_{\zeta\zeta} = 0 \\ \\ 
u_{\zeta\beta} = 0
\end{gather}
$$
We'll now realize that we can integrate both sides of the last math equation to obtain $u_{\zeta}$

$$
\begin{gather}
\int u_{\zeta\beta} \, = \int 0 \, dx \\ \\ 
u_{\zeta} = f(\zeta)
\end{gather}
$$
Lastly, we can integrate both sides with respect $\zeta$ so that we'll have $u(\zeta,\beta)$:
$$
\begin{gather}
\int u_{\zeta} \, = \int f( \zeta) \\ \\ 

u(\zeta,\beta) = F(\zeta) + g(\beta)
\end{gather}
$$
Now that we've found the function of $u$, we can switch back to the $tx$ plane. 
$$
\begin{gather}
u(x,t) = F(x-ct) + g(x+ct)
\end{gather}
$$
We'll also use the initial conditions such that 
$$
\begin{gather}
F(x) + g(x) = \log(1+ x^{2}) \\ \\ 
-cF'(x) + cg'(x) = 4 + x
\end{gather}
$$

We'll now multiply each sides of both of those equations by $c$ and then differentiate with respect to $x$:
$$
\begin{gather}
cf(x) + cg'(x) = c \frac{2x}{1+x^{2}} \\ \\ 

-cf(x) + cg'(x) = 4+x
\end{gather}
$$
We can treat this like a system of equalities and add the respective equations: 
$$
\begin{gather}
0 + 2cg'(x)
\end{gather} = c \frac{2x}{1+x^{2}}+ 4+x
$$
If we were to subtract the sides we'd find: 
$$
\begin{gather}
2cf(x) = c \frac{2x}{1+x^{2}} - 4 - x \\ \\
\end{gather}
$$
we can solve both of these equations to find that $f(x) \hspace{.2cm}\text{and} \hspace{.2cm}g'(x) =$
$$
\begin{gather}
f(x) = \frac{1}{2} \frac{2x}{1+x^{2}} - \frac{1}{2c}(4+x) \\ \\ 

g'(x) = \frac{1}{2} \frac{2x}{1+x^{2}} + \frac{1}{2c} (4+c)
\end{gather}
$$
we can now integrate these functions and replace $x \rightarrow x-ct$ such that 
$$
\begin{gather}
F(x-ct)=\frac{1}{2} log[1 + (x − ct)^{2} ] − \frac{1}{4c} [8(x − ct) + (x − ct)^{2} ] \\ \\ 

g(x + ct) = \frac{1}{2} log[1 + (x + ct)^{2}] + \frac{1}{4c} [8(x + ct) + (x + ct)^{2}]
\end{gather}
$$
No we can put together $u(x,y) = F(x-ct) + g(x+ct)$ such that 
$$
\begin{gather}
= \log \sqrt{ [1+(x-ct)^{2}][1+(x+ct)^{2}] } + t(4+x)
\end{gather}
$$
and we're all complete

#### 2.1.7

We have that 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x}, \hspace{.2cm} u(x,0) = \phi(x), \hspace{.2cm} u_{t}(x,0) = \psi(x)
\end{gather}
$$
Equation 8 of chapter 2.1 states that 
$$
\begin{gather}
u(x,t) = \frac{1}{2} [\phi(x+ct)+\phi(x-ct)]+ \frac{1}{2c}\int _{x-ct} ^{x+ct} \psi(s) \, ds 
\end{gather}
$$
now we'll consider the conditions that both $\phi(x)$ and $\psi(x)$ are odd functions. We know this means 
$$
\begin{gather}
\phi(-x) = -\phi(x) \\ \\ 

\psi(-x) = -\psi(x) \\ \\ 
\end{gather}
$$
Now from there, we want to prove that $u(-x,t) = -u(x,t)$. 
So we'll start by replacing the left side of the equation with the second math line we have above to get: 
$$
\begin{gather}
u(-x,t) = \frac{1}{2}[\phi(-x+ct)+\phi(-x-ct)] + \frac{1}{2c} \int _{-x-ct}^{-x+ct} \psi(s)\, ds 
\end{gather}
$$
We'll substitute $w = -s$. The if we $d$ both sides we have that $dw = -ds$ such that
$$
\begin{gather}
u(-x,t) = \frac{1}{2}[\phi(-x+ct)+\phi(-x-ct)] - \frac{1}{2c} \int _{x+ct}^{x-ct} \psi(-w)\, dw 
\end{gather}
$$
Where we've switched the limits of integration. 
Thus we have 
$$
\begin{gather}
u(-x,t) = -\left( \frac{1}{2}[\phi(x+ct)+\phi(x-ct)]+ \frac{1}{2c} \int _{x-ct}^{x+ct} \phi(w) \, dw  \right) \\ \\ 

\end{gather}
$$
but this is the same expression as $-u(x,t)$. Thus we've shown that if $\phi(x)$ and $\psi(x)$  are odd functions, then generally $u(x,t)$ is odd $\forall x,t$

## Part 2


#### 1. 

If we have that 
$$
\begin{gather}
\frac{ \partial^{2}u }{ \partial x^{2} } - \frac{ \partial^{2}u }{ \partial y^{2} } = 0 
\end{gather}
$$
This must mean that $u$ is of the form $ax^{2}\pm by^{2}$ some constant $\in \mathbb{R}$. Thus we'll consider the case: 
$$
\begin{gather}
\frac{ \partial u }{ \partial x } - \frac{ \partial u }{ \partial y } = 2ax - 2by
\end{gather}
$$
Thus we need to show that $2ax \pm 2by$ is a constant

#### 2. 



