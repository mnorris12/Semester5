#### 3.2.10

###### a

Here's the relevant information we've been given for solving this problem:

$$
\begin{gather}
u_{tt} = 9u_{x x} \hspace{.5cm} c^{2}= 9 \hspace{.5cm} 0<x< \frac{\pi}{2} \\ \\ \
u(x,0) = \cos(x)=\phi(x) \hspace{.5cm}u_{t}(x,0) = 0= \psi(x) \\ \\ 
u_{x}(0,t) = 0 \hspace{.5cm}u\left( \frac{\pi}{2},t \right) = 0
\end{gather}
$$

We're going to first extend this problem to the whole line, that is $-\infty<x<\infty$, and then restrict it to $0<x< \frac{\pi}{2}$. The general solution for the whole is provided in 3.1: 
$$
\begin{gather}
u(x,t) = \frac{1}{2}[\phi(ct+x)-\phi(3t-x)] + \frac{1}{2c}\int _{ct-x}^{ct+x} \psi(y) \, dy 
\end{gather}
$$
We easily see that $c=3$ and the integral on the right vanishes because of our initial condition of $\phi(x) = 0$. Thus we have: 
$$
\begin{gather}
u(x,t) = \frac{1}{2}[\phi(3t+x)-\phi(3t-x)]
\end{gather}
$$
using our other initial condition that $\phi(x)= \sin(x)$, we have that
$$
\begin{gather}
u(x,t) = \frac{1}{2}[\cos(3t+x)- \cos(3t-x)]
\end{gather}
$$
Now the answer we're looking for is simply restricted to $0<x< \frac{\pi}{2}$!:
$$
\begin{gather}
u(x,t) = \boxed{\frac{1}{2}[\cos(3t+x)- \cos(3t-x)] \hspace{.5cm}0<x< \frac{\pi}{2}}
\end{gather}
$$
This completes the Strauss method!

###### b

Now we'll think about using the method of separation of variables and Fourier series expansion!

We have that
$$
\begin{gather}
XT'' = c^{2}X''T \\ \\ 
\frac{T''}{9T} = \frac{X''}{X} = \gamma
\end{gather}
$$
when $X'(0)=X\left(0 \right) = 0$ is an eigenvalue

**Positive Eigenvalue** $\gamma =\sigma^{2}$
We already know the general solution to $X(x)$ which is 
$$
\begin{gather}
X(x) = C\cosh(\sigma x)+D\sinh(\sigma x) \\ \\ 
X'(x) = -\sigma C\sinh(\sigma x)+D\gamma \cosh(\sigma x) = 0 \\ \\
X'(0) = -C\sin(\sigma(0))+\sigma D\cos(0) = \sigma D =0
\end{gather}
$$
Thus $D$ equals 0 and so does $C$. The same result applies when $x= \frac{\pi}{2}$. Thus there are no positive eigenvalues 

**Zero Eigenvalues** $\gamma = 0$
There will be no zero eigenvalues, as we'll a few times later in the PDF (for time purposes)

**Negative Eigenvalues** $\gamma = -\sigma^{2}$

We have that 
$$
\begin{gather}
\frac{X''}{X} = -\sigma^{2}
\end{gather}
$$

The same conclusion from the positive eigenvalues, except this time, we don't want the trivial solution of $C=D =0$, so let's assume that they are not! Thus

$$
\begin{gather}
C_{6}\sin\left( \frac{\pi}{2}\sigma \right) = 0
\end{gather}
$$
Now for $T$ we have: 
$$
\begin{gather}
\frac{T''}{9T} = 0 \\ \\ 
T''-(3\sigma)^{2}T = 0
\end{gather}
$$
We'll guess a solution that $T = \sin(3\sigma t) = \sin(3(n\pi)t)$ which checks out because then the last equation becomes the same value subtracted which equal 0!
Thus we have that 
$$
\begin{gather}
T(t) = A_{n}\cos \frac{3n\pi t}{l}+B_{n}\sin\left( \frac{3n\pi t}{l} \right)
\end{gather}
$$
Thus $u$ being a sum of solutions is 
$$
\begin{gather}
u(x,t) = \sum_{n=0}^{\infty}[A_{n}\cos \frac{3n\pi t}{l}+B_{n}\sin\left( \frac{3n\pi t}{l} \right)]\sin((2n+2)x)
\end{gather}
$$
with our initial conditions, we can determine $A_{n},B_{n}$
#### 3.3.2

This will be a long solution so buckle up! I'm going to skip some algebraic steps, the ones without subtitles. 

We're to solve the completely inhomogeneous diffusion equation on the half line with the following conditions
$$
\begin{gather}
v_{t}-kv_{x x} = f(x,t)\hspace{.5cm} 0<x<\infty \hspace{.5cm}0<t<\infty\\ \\
\text{BC:} \hspace{.5cm}v(0,t) = h(t) \hspace{.5cm} v(x,0) = \phi(x)
\end{gather}
$$
using the subtraction method.

The subtraction method entails: 
$$
\begin{gather}
V(x,t) = v(x,t)-h(t)\\ \\ 
V_{t} = v_{t}-h'(t) \hspace{.5cm}v_{t} = V_{t}+h'(t)  \\ \\ 
V_{x} = v_{x} \\ \\ 
V_{x x} = v_{x x}
\end{gather}
$$

As stated in equation (10): 
$$
\begin{gather}
V_{t}-kV_{x x} = f(x,t) -h'(t) \hspace{.5cm}0<x<\infty, t>0 \\ \\ 
V(0,t) = 0 \hspace{.5cm}V(x,0) = \phi(x) - h(0)
\end{gather}
$$
We want to us $V$ as then, we deal with a homogeneous Dirichlet boundary condition $V(0,t) = 0$. We can now use the **method of reflection using our new $V$ subtraction strategy**! The motivation behind this, is that now we can solve the problem over the whole line, restrict it to positive values of $x$ and then once we've found $V$, we've essentially found $v(x,t)$ from their relationship stated above. 

Now that we're dealing with a homogeneous boundary condition situation, we want to solve $V$, that is suppose $Q$ is a solution under the same conditions that apply to $V$. Then we'll assume: 
$$
\begin{gather}
Q_{t} -kQ_{x x} = F_{odd}(x,t), \hspace{.5cm}-\infty<x<\infty, t>0 \\ \\
W(x,0) = \phi_{Qodd}(x)
\end{gather}
$$
Where:
$$
\begin{gather}
F_{odd}(x,t) = \begin{cases}
f(x,t)-h'(t) \hspace{.5cm}x>0 \\
-f(-x,t)+h'(t) \hspace{.5cm} x<0  \\
\end{cases} \hspace{.5cm} \\ \\ 
\phi_{Qodd}(x) = \begin{cases}
\phi(x) - h(0) \hspace{.5cm} x>0 \\
-\phi(-x)+h(0) \hspace{.5cm} x<0 \\
\end{cases}
\end{gather}
$$
We've reached a point where clever tricks can produce equations we already know the solutions to. We'll utilize the fact $Q$ can be split in a manner where the combination of its constituents equal $Q$ (as $Q$ is linear): 
$$
\begin{gather}
Q = g(x,t) + p(x,t) \\ \\ 
g_{t} - kg_{x x} = 0 \hspace{.5cm} -\infty<x<\infty,t>0 \hspace{.5cm}g(x,0) =\phi_{Q_{odd}}(x) \\ \\
p_{t} - kp_{x x} = F_{odd}(x,t) \hspace{.5cm} -\infty<x<\infty,t>0 \hspace{.5cm}p(x,0) =0
\end{gather}
$$
Notice that their addition is: 
$$
\begin{gather}
(g_{t}+p_{t}) - k(g_{x x}+p_{x x}) = F_{odd}(x,t) \\ \\
g(x,0)+p(x,0) = \phi_{Qodd}(x)
\end{gather}
$$
This looks familiar! Okay, now that this is the case, we'll notice that $g$ is the diffusion equation on the whole line, which we've found to
$$
\begin{gather}
g(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -\frac{(x-r)^{2}}{4kt} }\phi_{Qodd}(y) \, dy 
\end{gather}
$$
$p$ is just the diffusion equation of the whole line with a source, which we deduced to equation (8) on page 69: 
$$
\begin{gather}
p(x,t) = \int _{o}^t \int_{-\infty}^{\infty}\frac{1}{\sqrt{ 4\pi k(t-s) }}  \, e^{ -\frac{(x-r)^{2}}{4k(t-s)} }  F_{odd}(r,s)\, dr ds
\end{gather}
$$
Thus the solution to V is then the addition of the solutions $g,p$ restricted on the half line: 
$$
\begin{gather}
V = W (x>0)  = \\ \\ 
\frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -\frac{(x-r)^{2}}{4kt} }\phi_{Qodd}(y) \, dy  \hspace{.5cm} + \int _{o}^t \int_{-\infty}^{\infty}\frac{1}{\sqrt{ 4\pi k(t-s) }}  \, e^{ -\frac{(x-r)^{2}}{4k(t-s)} }  F_{odd}(r,s)\, dr ds
\end{gather}
$$

The steps here are quite tricky and are honestly a pain for both me and you to look at. I think it would be more useful to explain how we solve $V$, rather than see every integral required. We want to take the current integrals we have now and do to things
1. split the last line of integrals into positive and negative values of $x$ 
2. get our solutions in terms of $\phi(x)$ and $f(x,t)$ as our diffusion equation solutions usually are. 
We have: 
$$
\begin{gather}V = \\
\frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{0} e^{ -\frac{(x-r)^{2}}{4kt} }(-\phi(-r)+h(0)) \, dr+\frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{ -\frac{(x-r)^{2}}{4kt} }(\phi(r)-h(0)) \, dr + \\ \\ 
\int _{o}^t [\int_{-\infty}^{0}\frac{1}{\sqrt{ 4\pi k(t-s) }}  \, e^{ -\frac{(x-r)^{2}}{4k(t-s)} }  (-f(-r,s)+h'(s))(r,s)\, dr +\\ \\ 
\int_{0}^{\infty}\frac{1}{\sqrt{ 4\pi k(t-s) }}  \, e^{ -\frac{(x-r)^{2}}{4k(t-s)} }  (f(r,s)-h'(s))(r,s)\, dr]ds
\end{gather}
$$
we'll substitute $n=-r$ for negative values and $n=r$ for positive and combine the integrals: 
$$
\begin{gather}
V = \frac{1}{\sqrt{ 4\pi kt }}\int _{0}^{\infty } e^{ -\frac{(x-n)^{2}}{4kt} } - e^{ -\frac{(x+q)^{2}}{4kt} }\phi(n)\, dn -  \frac{1}{\sqrt{ 4\pi kt }}\int _{0}^{\infty } e^{ -\frac{(x-n)^{2}}{4kt} } - e^{ -\frac{(x+q)^{2}}{4kt} }h(0)\,dn \\ \\ 
\end{gather}
$$

$$\begin{gather}

+ \int _{o}^t (\int_{0}^{\infty}\frac{1}{\sqrt{ 4\pi k(t-s) }}  e^{ -\frac{(x-n)^{2}}{4k(t-s)}- }  - 
+ e^{ -\frac{(x+n)^{2}}{4k(t-s)} }f(n,s)\, dn - \\ \\ 
\int_{0}^{\infty} e^{ -\frac{(x-n)^{2}}{4k(t-s)} }- e^{ -\frac{(x+n)^{2}}{4k(t-s)} }h'(s)  \, dn ) ds
\end{gather}
$$



Thus our final solution is just 
$$
\begin{gather}
v(x,t) = h(t) + \\ \\ 
\frac{1}{\sqrt{ 4\pi kt }}\int _{0}^{\infty } e^{ -\frac{(x-n)^{2}}{4kt} } - e^{ -\frac{(x+q)^{2}}{4kt} }\phi(n)\, dn -  \frac{1}{\sqrt{ 4\pi kt }}\int _{0}^{\infty } e^{ -\frac{(x-n)^{2}}{4kt} } - e^{ -\frac{(x+q)^{2}}{4kt} }h(0)\, dn \\ \\ 
+ \int _{o}^t ( \int_{0}^{\infty}\frac{1}{\sqrt{ 4\pi k(t-s) }}  \, e^{ -\frac{(x-n)^{2}}{4k(t-s)}- }  - e^{ -\frac{(x+n)^{2}}{4k(t-s)} }f(n,s)\, dn - \\ \\ 
\int_{0}^{\infty} \frac{ \partial  }{ \partial x }  \left[ {e^{ -\frac{(x-n)^{2}}{4k(t-s)}- }- e^{ -\frac{(x+n)^{2}}{4k(t-s)}- }}h(s)  \, dn  \right] )ds
\end{gather}
$$


#### 3.4.2

We'll use the operator Factorization method to solve this problem,
$$
\begin{gather}
u_{tt} - c^{2}u_{x x} = e^{ ax } \\ \\
\end{gather}
$$
We'll write the left side of the equation in terms of an operator
$$
\begin{gather}
(\partial^{2}_{t} - c^{2}\partial^{2}_{x})u = e^{ ax } \\ \\
\text{where} \hspace{.2cm} \mathcal{L} = (\partial^{2}_{t} - c^{2}\partial^{2}_{x}) = (\partial_{t} + c\partial_{x})(\partial_{t}-c\partial_{x})
\end{gather}
$$
We can do a clever trick in which $n = (\partial_{t}-c\partial_{x})u$, which makes our problem, 
$$
\begin{gather}
(\partial_{t}+c\partial_{x})n = e^{ ax } \\ \\ 
\end{gather}
$$
The motivation behind this transformation, was to reduce our problem from a second order PDE to a First order PDE. We can now proceed with the method of characteristics,
$$
\begin{gather}
u_{t} - cu_{x} = n\\ \\ 
n_{t} +cn_{x} = e^{ ax }
\end{gather}
$$

We'll solve the second equation for $n$ which will give us the right side of the first equation. That value will motivate our solution $u$. The derivative for a two variable function $\phi(x,t)$ is,
$$
\begin{gather}
d\phi = \frac{\partial \phi}{\partial t}dt+\frac{\partial \phi}{\partial x}dx \\ \\
\text{multiply} \hspace{.2cm} \frac{1}{dt} \hspace{.2cm} \text{on both sides}: \\ \\
\underbrace{ \frac{d\phi}{dt} }_{ e^{ ax } } = \frac{\partial \phi}{\partial t}+\frac{\partial \phi}{\partial x}\underbrace{  \frac{dx}{dt} }_{ c }
\end{gather}
$$

That is, we now have two different ODE which we can solve for by separation of variables where $\phi\rightarrow n$,
$$
\begin{gather}
\frac{dx}{dt} = c\hspace{.25cm}\rightarrow \hspace{.25cm}x=ct + \xi\hspace{.5cm} \\ \\ 
\frac{dn}{dt} = e^{ ax } = e^{ a(ct+\xi) } = e^{ act }e^{ a\xi }
\end{gather}
$$
Now we can integrate both sides with respect to $t$: 
$$
\begin{gather}
n(\xi,t) = \frac{e^{ a\xi }}{ac}e^{ act }+ f(\xi)
\end{gather}
$$
Where the $f(\xi)$ is an integration function of characteristic coordinate $\xi$. Since $\xi = x-ct$, 
$$
\begin{gather}
n(x,t) = \frac{e^{ ax }}{ac}+f(x-ct)
\end{gather}
$$
Thus we've solved for $n$, which we can apply now to our first order partial differential equation $u_{t}-cu_{x} = n$:
$$
\begin{gather}
u_{t} -cu_{x} = \frac{e^{ ax }}{ac}+f(x-ct)
\end{gather}
$$
using the fact that $\frac{dx}{dt} = -c$, we again reduce a PDE to an ODE, 
$$
\begin{gather}
\frac{du}{dt} = \frac{e^{ ax }}{ac}+f(x-ct)
\end{gather}
$$
We use the characteristic coordinate $\eta$ where, 
$$
\begin{gather}
\frac{dx}{dt}= -c \\ \\ 
x=-ct+\eta
\end{gather}
$$
Thus we can resubstitute,
$$
\begin{gather}
\frac{du}{dt} = \frac{e^{ a\eta }}{ac}e^{ -act } +f(\eta-2ct) 
\end{gather}
$$
We integrate,
$$
\begin{gather}
u(\eta,t) = -\frac{e^{ a\eta }}{a^{2}c^{2}}e^{ -act } + F(\eta-2ct) +g(\eta) 
\end{gather}
$$
we rewrite $u(\eta,t)$, solving for $\eta = x+ct$, 
$$
\begin{gather}
u(x,t) = -\frac{e^{ ax }}{a^{2}c^{2}}+F(x-ct)+g(x+ct) 
\end{gather}
$$
And thus we've arrived at the general solution of $u(x,t)$. We'll now try to implement the initial conditions. 
$$
\begin{gather}
u(x,0) = 0 \hspace{.5cm}\rightarrow\hspace{.5cm} -\frac{e^{ ax }}{a^{2}c^{2}}+F(x) +g(x) = 0\\ \\ 
u_{t}(x,0) = 0 \hspace{.5cm}\rightarrow \hspace{.5cm} -cF'(x)+cg'(x) = 0
\end{gather}
$$
where we've differentiated the $u(x,t)$ with respect to $t$ for the second math line. We can use a substitution for $x =v$ such that
$$
\begin{gather}
-\frac{e^{ av }}{a^{2}c^{2}}+F(v) +g(v) = 0 \\ \\
-cF'(v)+cg'(v) = 0
\end{gather}
$$
and now we can differentiate with respect to our new substitution $v$ to get
$$
\begin{gather}
-\frac{e^{ av }}{ac^{2}}+F'(v)+g'(v) = 0 \\ \\
g'(v)= \frac{e^{ av }}{ac^{2}}-F'(v)
\end{gather} 
$$
plugging this value in to $-cF'(v)+cg'(v) = 0$ we arrive at
$$
\begin{gather}
F'(v) =\frac{e^{ av }}{2ac^{2}} \\ \\

\text{we integrate:} \\ \\
F(v) = \frac{e^{ av }}{2a^{2}c^{2}}+C_{1} \rightarrow F(x-ct) = \frac{e^{ a(x-ct) }}{2a^{2}c^{2}}+C_{1}
\end{gather}
$$
plugging this information into $g(v)$ we have: 
$$
\begin{gather}
g(w) = \frac{e^{ av }}{2a^{2}c^{2}}- C_{1} \rightarrow g(x+ct) = \frac{e^{ a(x+ct) }}{2a^{2}c^{2}}-C_{1}
\end{gather}
$$
Finally, the general solution for $u(x,t)$ becomes
$$
\begin{gather}
u(x,t) = -\frac{e^{ ax }}{a^{2}c^{2}}+ \frac{e^{ a(x-ct) }}{2a^{2}c^{2}}+\cancel{ C_{1 }}+ \frac{e^{ a(x+ct) }}{2a^{2}c^{2}}- \cancel{ C_{1} } \\ \\ 
= -\frac{e^{ ax }}{a^{2}c^{2}}+ \frac{e^{ a(x-ct) }}{2a^{2}c^{2}}+ \frac{e^{ a(x+ct) }}{2a^{2}c^{2}}
\end{gather}
$$
We'll notice that there's potential to write the above equation in terms of a hyperbolic function! 
$$
\begin{gather}
u(x,t) = \frac{e^{ ax }}{a^{2}c^{2}}\left( -1+ \frac{e^{ -act }+e^{ act }}{2} \right) \\ \\ 
u(x,t) = \boxed{\frac{e^{ ax }}{a^{2}c^{2}}\left( -1+ \cosh(act) \right)}
\end{gather}
$$
We've arrived at our solution!

#### 3.4.4

We are to show that the solution to the inhomogeneous wave equation,
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} +f \hspace{.5cm}u(x,0)= \phi(x) \hspace{.5cm}u_{t}(x,0) =\psi(x) \\ \\ 
-\infty<x<\infty \hspace{.5cm}t>0
\end{gather}
$$
is the sum of the three terms $f, \phi,\psi$, the source and the two initial conditions. 

We'll use Duhamel's principle. This means we can utilize the linearity of the PDE to split up the problem into useful equations where we already have the solutions. Now let,

$$
\begin{gather}
u(x,t) = g(x,t) + p(x,t)
\end{gather}
$$
Where the following initial value problem are: 
$$
\begin{gather}
g_{tt} -c^{2}g_{x x} = 0 \hspace{.5cm}g(x,0) = \phi(x)\hspace{.5cm}g_{t}(x,0)=\psi(x) \\ \\ 
p_{tt} - c^{2}p_{x x} = f(x,t) \hspace{.5cm}p(x,0) = 0 \hspace{.5cm} p_{t}(x,0)=0 
\end{gather} 
$$
The solution for $g$ is simply the solution to a homogenous wave equation on the whole line give early in chapter 2: 
$$
\begin{gather}
g(x,t) = \frac{1}{2}[\phi(x+ct)+\phi(x-ct)] + \frac{1}{2c} \int _{x-ct}^{x+ct}\phi(x_{0}) \, dx 
\end{gather}
$$
The solution for $p$ is the solution to a inhomogenous wave equation with homogeneous boundary conditions on the whole line which we deduced earlier in problem 3.2.2 and equation 8 on page 69:
$$
\begin{gather}
p(x,t) = \frac{1}{2c}\int _{0}^t \int _{x-c(t-s)}^{x+c(t-s)} S(x-y,t-s)f(y,s) \, dx  \, dx 
\end{gather}
$$
Therefore $u$ is the some of three terms $\phi,\psi,f$: 
$$
\begin{gather}
u(x,t)  = \frac{1}{2}[\phi(x+ct)+\phi(x-ct)] + \frac{1}{2c} \int _{x-ct}^{x+ct}\phi(x_{0}) \, dx \\ \\ 
+ \frac{1}{2c}\int _{0}^t \int _{x-c(t-s)}^{x+c(t-s)} S(x-y,t-s)f(y,s) \, dx  \, dx 
\end{gather}
$$
#### 3.4.11

We need to show that
$$
\begin{gather}
u(x,t) = \begin{cases}
h\left( t-\frac{x}{c} \right) \hspace{.5cm}x<ct \\
0 \hspace{.5cm}x \geq ct
\end{cases}
\end{gather}
$$
solves the wave equation such that, 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x}, \hspace{.5cm}0<x<\infty \\ \\ 
u(x,0) = 0 \hspace{.5cm}u_{t}(x,0) = 0 \hspace{.5cm}u(0,t)
\end{gather}
$$
We'll use the first math line and differentiate twice with respect to $t$ and then with respect to $x$:
$$
\begin{gather}
u_{tt}(x,t) =  \begin{cases}
h''\left( t-\frac{x}{c} \right) \hspace{.5cm}x<ct \\
0 \hspace{.5cm}x \geq ct
\end{cases} \\ \\ 
u_{x x}(x,t) =  \begin{cases}
h''\left( t-\frac{x}{c} \right) \cdot \left( -\frac{1}{c} \right)^{2} \hspace{.5cm}x<ct \\
0 \hspace{.5cm}x \geq ct
\end{cases}
\end{gather}
$$
Let's start with $u_{tt}$ and split it up based on $x$ values. for $x\geq ct$
$$
\begin{gather}
u_{tt} = 0= c^{2}u_{x x}
\end{gather}
$$
Now for $x <ct$ 
$$
\begin{gather}
h''\left( t-\frac{x}{c} \right) = \cancel{ c^{2} }h''\left( t-\frac{x}{c} \right) \cdot \cancel{ \left( -\frac{1}{c} \right)^{2} } \\ \
u_{tt}= h''\left( t-\frac{x}{c} \right) = c^{2}u_{ x x} \\ \\ 
h''\left( t-\frac{x}{c} \right) = u_{t t} = c^{2}u_{x x}
\end{gather}
$$
Thus our solution $u(x,t)$ satisfies the wave equation. Using our conditions, if $x= 0$ then $x<ct$
$$
\begin{gather}
u(0,t) = h(t)
\end{gather}
$$
if $t= 0$ then $x\geq ct$ 
$$
\begin{gather}
u(x,0) = 0 \\ \\ 
u_{t}(x,0) = 0
\end{gather}
$$
#### 4.4.1

##### a

The Fourier solution give on page 85 equation 9 to the wave equation is, 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} \hspace{.5cm} 0<x<l \\ \\ 
u(o,t) = u(l,t) = 0 \\ \\ 
u(x,t) = \sum_{n=1}^\infty \left[ A_{n}\cos\left( \frac{n\pi ct}{l} \right)+B_{n}\cos\left( \frac{n\pi ct}{l} \right) \right]\sin\left( \frac{n\pi x}{l} \right)
\end{gather}
$$
Strauss tells us, as usually referred to in physics, the coefficient of $t$ we will call $\omega$ is,
$$
\begin{gather}
\omega = \frac{n\pi c}{l} 
\end{gather}
$$
where $n$ is a integer. Returning to the violin example on page 87, we have, 
$$
\begin{gather}
\omega =  \frac{n\pi \sqrt{ T }}{l\sqrt{ \rho }} = \frac{n\pi c}{l} \\ \\
\end{gather}
$$
At the midpoint, the string is split in half. With that information we have, 
$$
\begin{gather}
\frac{n\pi}{\left( \frac{l}{2} \right)}\sqrt{ \frac{T}{\rho} }= \frac{2n\pi}{l}\sqrt{ \frac{T}{\rho} }
\end{gather}
$$

Mathematically speaking, an octave is the distance between any given note with a set frequency, and another note with double that frequency which, as the equation suggest, happens when the string is clamped exactly at its midpoint.

#### 4.1.4
We're asked to consider the following,
$$
\begin{gather}
u_{tt} = c^{2}u_{x x}-ru_{t} \hspace{.5cm}0<x<l \\ \\ 
u=0 \hspace{.5cm}\text{at both ends} \\ \\
u(x,0) = \phi(x) \hspace{.5cm} u_{t}(x,0) = \psi(x)
\end{gather}
$$
where $r$ is constant, $0<r<2\pi c /l$. We are to find the series expansion of the solution. 

Immediately, the boundary conditions are homogeneous so we can use the separation of variables method as outlined in chapter 4.1. We first have 
$$
\begin{gather}
u(x,t) = X(x)T(t) \\ \\ 
XT'' = c^{2}X''T - rXT'
\end{gather}
$$
Using the boundary conditions, we have, 
$$
\begin{gather}
u(0,t) = u(l,t) =X(0)=X(l)
\end{gather}
$$
We can now proceed with separation of variables: 
$$
\begin{gather}
\frac{T''+rT'}{c^{2}T} = \frac{X''}{X} = \lambda
\end{gather}
$$
where $\lambda$ is an eigenvalue

We'll now continue with determining different kinds of Eigenvalues; 

**Positive Eigenvalues $\sigma = \beta^{2}$**
Much of this process has actually been outlined by Strauss, so much of this is translating this example to his Fourier Series Transformation. Anyway, he determines that 
$$
\begin{gather}
X(x) = C\cosh(\beta x)+D\sinh(\beta x) \\
0 = X(0) = c
0 = X(l) = D\sinh(\beta x) \hspace{.5cm}D = 0
\end{gather}
$$
Where we'll say $C,D$ are particular to the type of eigenvalue we're discussing (i.e. they're welcome to be something else in the next case). Thus, only the trivial solution exists such that
$$
\begin{gather}
X'' = (0)X
\end{gather}
$$
meaning there are no positive eigenvalues $\lambda$

**Zero Eigenvalue $\sigma= 0$**
$$
\begin{gather}
\frac{X''}{X} = 0 \\ \\ 
X'' =0
\end{gather}
$$
Thus 
$$
\begin{gather}
X(x) = Cx + D \\ \\ 
X(0) = D = 0  \hspace{.5cm}X(l) = Cl + D = 0 \\ \\ 
C=D=0
\end{gather}
$$
This only results from $\sigma = 0$ and zero cannot be eigenvalue. 

**Negative Eigenvalues $\sigma =-\lambda^{2}$**
We have
$$
\begin{gather}
\frac{X''}{X} = -\lambda^{2} \\ \\ 
X'' = -\lambda^{2}X
\end{gather}
$$
Thus
$$
\begin{gather}
X(x) = C\cos\beta x D\sin\lambda x \\ \\
X(0) = C = 0 \\ \\ 
X(l) = \underbrace{ C\cos\lambda }_{ =0 } l+D\sin\lambda l = 0 \\ \\
D\sin\lambda l = 0 
\end{gather} 
$$
We don't want the trivial solution, so we'll say $D=0$
This would suggest
$$
\begin{gather}
\sin\lambda l = 0 \\
\lambda l = n\pi \hspace{.5cm}\lambda_{n} = \frac{n\pi}{l}
\end{gather}
$$
Thus our eigenfunction in terms of n is 
$$
\begin{gather}
X_{n}(x) = \sin\lambda_{n}(x)
\end{gather}
$$
Now we'll work on the differential equation for $T(t)$
$$
\begin{gather}
\frac{T''+rT'}{c^{2}T} = -\lambda^{2} \\ \\
T'' + rT' = -c^{2}\lambda^{2}T \\ \\ 
T'' + rT'+c^{2}\lambda^{2}T = 0
\end{gather}
$$
We recognize that this is a differential equation where $T$ has solution
$$
\begin{gather}
T= e^{ st }
\end{gather}
$$
We sub this in for our ODE to find s
$$
\begin{gather}
s^{2}e^{ st } +rse^{ st }+c^{2}\lambda^{2}e^{ st }=0 \\ \\
s^{2}+rs+c^{2}\lambda^{2} = 0
\end{gather}
$$
using the quadratic formula, we have
$$
\begin{gather}
s= \frac{-r \pm \sqrt{ r^{2}-4c^{2}\lambda^{2} }}{2}
\end{gather}
$$
We can now substitute for $\lambda = \frac{n\pi}{l}$
$$
\begin{gather}
s = \frac{\left( -r\pm \sqrt{ r^{2}-n^{2}\left( \frac{2\pi c}{l} \right)^{2} } \right)}{2}
\end{gather}
$$
Thus the the general solution for $T$ is: 
$$
\begin{gather}
\ce{ We substitute s back into e^{ st } :} \\ \\ 
T(t) = Ce^{ -\frac{r}{t} }\cos\left( \frac{\sqrt{ 2n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l}t \right)+De^{ \frac{-r}{2}t }\sin\left( \frac{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l}t \right)
\end{gather}
$$
Where the information of in parenthesis has been simplified using WolframeAlpha. Our solution $u(x,t)$ is thus a sum of solutions: 
$$
\begin{gather}
u(x,t) =  \\ \\ \sum_{n=1}^{\infty}A_{n}e^{ -\frac{r}{t} }\cos\left( \frac{\sqrt{ 2n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l}t \right) \\ \\ +B_{n}e^{ \frac{-r}{2}t }\sin\left( \frac{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l}t \right)\sin\left( \frac{n\pi x}{l} \right)
\end{gather}
$$

Now we have to use the Fourier's method to express our coefficients $A_{n}, B_{n}$ in terms of our initial conditions such that 
$$
\begin{gather}
u(x,0) = \sum_{n=1}^{\infty}A_{n}\sin\left( \frac{n\pi x}{l} \right)= \phi(x)
\end{gather}
$$
We'll multiply both sides by $v$ a positive integer, 
$$
\begin{gather}
u(x,0) = \sum_{n=1}^{\infty} A_{n}\sin\left( \frac{n\pi x}{l} \right)\sin \left( \frac{m\pi x}{l} \right) = \phi(x)\sin \frac{m\pi x}{l}
\end{gather}
$$
We not integrate over $0<x<l$ such that
$$
\begin{gather}
\int _{0}^l \sum_{n=1}^{\infty} A_{n}\sin\left( \frac{n\pi x}{l} \right)\sin \left( \frac{m\pi x}{l} \right) \, dx= \int _{0}^l \phi(x)\sin \frac{m\pi x}{l}\, dx \\ \\ 
= \sum_{n=1}^{\infty}A_{n}\int _{0}^l  \sin\left( \frac{n\pi x}{l} \right)\sin \left( \frac{m\pi x}{l} \right)\, dx  = \int _{0}^l \phi(x)\sin \frac{m\pi x}{l}\, dx 
\end{gather}
$$
given what we stated $\phi(x)$ is $n=m$ and thus our integral
$$
\begin{gather}
 \sin\left( \frac{n\pi x}{l} \right)\sin \left( \frac{m\pi x}{l} \right)\, = \frac{l}{2}
\end{gather}
$$
Thus we have
$$
\begin{gather}
\boxed{A_{n} =\frac{2}{l}\int _{0}^l \phi(x)\sin\left( \frac{n\pi x}{l} \right) \, dx} 
\end{gather}
$$
We now use the second initial condition $u_{t}(x,t)$ (we used WolframAlpha) and plugged in $t=0$ 
$$
\begin{gather}
u_{t}(x,0) = \sum_{n=1}^{\infty}\left( -\frac{r}{2} \right)A_{n}\sin\left( \frac{n\pi x}{l} \right)+ \sum_{n=1}^{\infty}B_{n} \frac{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l} \sin\left( \frac{n\pi x}{l} \right) = \psi(x)
\end{gather}
$$
We have that the sum of $u(x,0)$ and $u(x,0)$ is also a solution for $\phi(x)$
$$
\begin{gather}
\left( -\frac{r}{2} \right)\phi(x) +  \sum_{n=1}^{\infty}B_{n} \frac{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l} \sin\left( \frac{n\pi x}{l} \right) = \psi(x) \\ \\
 \sum_{n=1}^{\infty}B_{n} \frac{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}{2l} \sin\left( \frac{n\pi x}{l} \right) = \psi(x) +\left( -\frac{r}{2} \right)\phi(x)
\end{gather}
$$
we now multiply both sides by $\sin\lambda_{m}x$ (as we did earlier), where we conducted the same process to find

$$
\begin{gather}
\boxed{B_{n} = \frac{4}{\sqrt{ 4n^{2}\pi^{2}c^{2}-r^{2}l^{2} }}\int _{0}^l \left[ \frac{r}{2}\phi(x)+\psi(x) \right]\sin\left( \frac{n\pi x}{l} \right) \, dx }
\end{gather}
$$

#### 4.2.2

We consider the following 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} \hspace{.5cm} 0<x<l  \\ \\ 
u_{x}(0,t) \hspace{.5cm} u(l,t) = 0 
\end{gather}
$$
###### a 

We are to show that the eigenfunctions are $\cos\left[ \left( n+\frac{1}{2} \right) \frac{\pi x}{l} \right]$

Similar to the last problem, we can apply the method of separation of variables
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} \rightarrow XT''= c^{2}X''T \\ \\ 
\frac{T''}{c^{2}T} = \frac{X''}{X} = \gamma
\end{gather}
$$
as before, since they are different variables on either side, we have that the fractions both must equal a constant. When $X'(0) = X(l) = 0$, we have ourselves an eigenvalue. 

**Positive Eigenvalues** $\sigma = \gamma^{2}$
$$
\begin{gather}
\frac{X''}{X} = \gamma^{2} \\ \\
X'' = \gamma^{2}X
\end{gather}
$$
We already know the general solution to be
$$
\begin{gather}
X(x) = C\cosh(\gamma x)+ D\sinh(\gamma x)
\end{gather}
$$
We'll now use boundary conditions to find our constants
$$
\begin{gather}
X'(0)=D\gamma = 0 \\ \\ 
X(l) = C\cosh(\gamma l)+D\sin(\gamma l) = 0
\end{gather}
$$
The coefficients both equal zero thus as before, there are no positive eigenvalues 

**Zero Eigenvalues** $\sigma = 0$
We have
$$
\begin{gather}
\frac{X''}{X} = 0
\end{gather}
$$
Similar to the negative eigenvalue situation in the previous question, the coefficients will equal 0, thus the only solution $X(x) = 0$ is trivial and zero is not an eigenvalue

**Negative Eigenvalue** $\sigma = -\lambda^{2}$
As before we assume
$$
\begin{gather}
\frac{X''}{X } = -\lambda^{2} \\ \ \
X'' = -\lambda^{2}X
\end{gather}
$$
The general solution is then
$$
\begin{gather}
X(x) = C\cos\lambda x +D\sin\lambda x
\end{gather} 
$$
We now use the boundary conditions to determine
$$
\begin{gather}
X'(0) = D\lambda = 0 \\ \\ 
X(l) = \underbrace{ C\cos\lambda l }_{ =0 } + D\sin\lambda l = 0 \\ \\
\cos\lambda l = 0
\end{gather}
$$
Thus $\lambda$ is
$$
\begin{gather}
\lambda  = \frac{\pi}{2l}(2n+1)
\end{gather}
$$
This produces
$$
\begin{gather}
X(x) = C\cos\lambda x \\ \\ 
X_{n}(x) = \cos\left[ \frac{\pi}{2l}(2n+1)x \right]
\end{gather}
$$
where $n = 0,1,2\dots$
###### b

We are to write a series expansion for the solution $u(x,t)$

We solve the ODE for $T(t)$
$$
\begin{gather}
\frac{T''}{c^{2}T} = \lambda^{2} \\ \\ 
T'' = -c^{2}\lambda^{2}T
\end{gather}
$$
We know the general solution then for $T(t)$ is just
$$
\begin{gather}
T(t) = C\cos c\lambda t + D\sin c\lambda t
\end{gather}
$$
The linearity of $T$ tells us that the solution to the partial differential equation $u(x,t)$ can be composed of a linear combination of the products of $T_{n}(t)X_{n}(x)$ over all the eigenvalues. Thus we have the following some for the solution $u(x,t)$
$$
\begin{gather}
u(x,t) = \sum_{n=0}^{\infty}(A_{n}\cos c\lambda_{n}t+B_{n}\sin c\lambda_{n}t)X_{n}(x)
\end{gather}
$$
where we already determined $\lambda$ and $X_{n}(x)$
$$
\begin{gather}
u(x,t) =  \sum_{n=0}^{\infty}\left( A_{n}\cos\left[ c \frac{\pi}{2l}(2n+1)t \right]+B_{n}\sin c\left[ c \frac{\pi}{2l}(2n+1)t \right] \right) \\ \\ 
\cdot \cos\left[ \frac{\pi}{2l}(2n+1)x \right]
\end{gather}
$$




### Part 2

#### 1

We are to Duhamel's principle (page 78 Strauss) to find a formula for a particular solution of the ODE $u''(x)+a^{2}u(x)=f(x)$, where $a>0$ is a positive real number

In the case in situation where the ODE was homogenous, meaning $f(x) = \phi(x) = 0$, we would have
$$
\begin{gather}
u''(x)+a^{2}u(x) = 0
\end{gather}
$$
We can guess a solution to the above ODE as $u(t) = \psi\frac{1}{a}\sin(ta)$
We'll check that the solution is correct
$$
\begin{gather}
u''(x) = -\phi a\sin(ta) \\ \\
a^{2}u(x) = \phi a\sin(ta) \\ \\
\text{Thus} \hspace{.5cm}u''(x) +a^{2}u(x) =0
\end{gather}
$$
Duhamels principle applied to ODE tells us 
$$
\begin{gather}
u(x) =  S(x)\psi (x) \\ \\ 
u'(x) = S'(x)\psi(x) \\ \\ 
S(x) = \frac{1}{a}\sin(ta)
\end{gather}
$$
where
$$
\begin{gather}
u(x) = S'(x)\phi+S(x)\psi+\int _{0}^x S(x-s)f(s)\, ds \\ \\ 
\text{we plug in:} \hspace{.5cm} \\ \\ 
u(t) = \cos(xa)\phi + \frac{1}{a}\sin(ta)\psi+ \int _{0}^x \frac{1}{a}\sin((x-s)a)f(s) \, ds
\end{gather}
$$

#### 2

We have the following: 
$$
\begin{gather}
u_{t}-ku_{x x}+bt^{2}u = 0
\end{gather}
$$
on the whole line with positive values of $t$ with the initial conditions that $u(x,0) = f(x)$. We'll first start off by using the hint that 
$$
\begin{gather}
u(x,t) = e^{ -bt^{3}/3 }v(x,t)
\end{gather}
$$
We substitute and simplify
$$
\begin{gather}
-\frac{bt^{2}}{6}e^{ -bt^{3}/3 }v-e^{ -bt^{3}/3 }v_{t}-k(e^{ -bt^{3}/3 }v_{xx})+\frac{d}{dt}(-6e^{ -bt^{3}/3 })v = 0 \\ \\ 
-e^{ -bt^{3}/3 }v_{t}-k(e^{ -bt^{3}/3 }v_{xx})+\frac{5bt^{2}}{6}e^{ -bt^{3}/3 }v = 0
\end{gather}
$$
We take the derivative of the last term on the left