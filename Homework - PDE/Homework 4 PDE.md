#### 2.5.4
##### a
We have that 
$$
\begin{gather}
v(x,t) = \frac{c}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -s^{2}c^{2}/4kt }u(x,s) \, dx 
\end{gather}
$$

We'll first start by considering the hint that $H(x,t) = \frac{c}{\sqrt{ 4\pi kt }}e^{ -x^{2}c^{2}/4kt }$ .

We can rewrite the integral:

$$
\begin{gather}
v(x,t) = \int_{-\infty}^{\infty} H(s,t)u(x,s) \, ds 
\end{gather} 
$$
We must now check to see if $H(x,t)$ satisfies the diffusion equation: 

$$
\begin{gather}
H_{x} = \frac{c}{\sqrt{ 4\pi kt }}e^{ \frac{x^{2}c^{2}}{4kt} }\left( -\frac{xc^{2}}{4kt}\right) = -\frac{c^{3}}{\sqrt{ \pi k^{3}t^{3} }}xe^{ -\frac{x^{2}c^{2}}{4kt} }
\\ \\ 
H_{t} = \frac{C}{\sqrt{ 4\pi k }} \left( \left( -\frac{1}{2} t^{-3/2} \right)e^{ -x^{2}c^{2}/4kt }+t^{-\frac{1}{2} }\left( \frac{x^{2}c^{2}}{4kt^{2}} \right)e^{ -\frac{x^{2}c^{2}}{4kt} }\right)  = 
\\ \\ 
-\frac{c}{4\sqrt{ \pi kt^{3} }}e^{ \frac{x^{2}c^{2}}{4kt} }\left( 1-\frac{x^{2}c^{2}}{2kt} \right) \\ \\ 

H_{ xx} = -\frac{c^{3}}{4\sqrt{ \pi k^{3}t^{3} }}\left[ e^{ -\frac{x^{2}c^{2}}{4kt} }+x\left( -\frac{xc^{2}}{2kt} \right)e^{ -\frac{x^{2}c^{2}}{4kt} } \right] = \\ \\ 
-\frac{c^{3}}{4\sqrt{ \pi k^{3}t^{3} }}e^{ -\frac{x^{2}c^{2}}{4kt} }\left( 1-\frac{x^{2}c^{2}}{2kt} \right)
\end{gather}
$$

Upon further inspection of the components of $H$ we see that $H_{t}$ and $\frac{k}{c^{2}}H_{ xx}$. This must mean that $H$ satisfies the conditions with a constant $\frac{k}{c^{2}}$. Now we'll go back to $v$ and show that it satisfies the diffusion equation: 

$$
\begin{gather}
v_{t} = \int_{-\infty}^{\infty} H_{t}(s,t)u(x,s) \, ds = \frac{k}{c^{2}} \int_{-\infty}^{\infty} H_{x x}(s,t)u(x,s) \, ds \\ \\ 

v_{x} = \int_{-\infty}^{\infty} H(s,t)u_{x}(x,s) \, ds \\ \\

v_{ x x} = \int_{-\infty}^{\infty} H(s,t)u_{ x x}(x,s) \, ds 
\end{gather}
$$
Now that we've found $v_{ x x}$ we need to show that $v_{t} = \frac{k}{c^{2}}v_{x x}$:
$$
\begin{gather}
v_{t} = \frac{k}{c^{2}}\left( \underbrace{ H_{x}(s,t) }_{ \rightarrow_{0} }u(x,s)|_{-\infty}^{\infty} -\int_{-\infty}^{\infty} H_{x}(s,t) u_{x}(x,s) \, ds  \right) = \\ \\ 

-\frac{k}{c^{2}} \int_{-\infty}^{\infty} H_{x}(s,t)u_{x}(x,s) \, ds \\ \\ 

\text{We need to integrate by parts once more} \hspace{.2cm} \\ \\ 

v_{t} = -\frac{k}{c^{2}}\left( H(s,t)u_{x}(x,s)|_{-\infty}^{\infty} -\int_{-\infty}^{\infty} H(s,t)u_{x x}(x,s) \, ds  \right) \\ \\ 
v_{t}= \frac{k}{cs} \int_{-\infty}^{\infty} H(s,t)u_{x x}(x,s) \, ds 
\end{gather}
$$
Thus we've proved that $v(x,t)$ solves the diffusion equation!


##### b

From the following hint, we know that $H(x,t)$, the Green's function for the heat equation not only saitisfies the diffusion equation by also entails the initial condition $H(x,0) = \delta(x)$. We can thus say:
$$
\begin{gather}
\lim_{ t \to 0 } v(x,t) = \lim_{ t \to 0 } \int_{-\infty}^{\infty} H(s,t)u(x,s) \, ds \\ \\ 
= \int_{-\infty}^{\infty} (\lim_{ t \to 0 } H(s,t))u(x,s) \, ds \\ \\ 

\int_{-\infty}^{\infty} H(s,0)u(x,s) \, ds  \\ \\ 

\int_{-\infty}^{\infty} \delta(s)u(x,s) \, ds = u(x,0) 
\end{gather}
$$
Thus we've proven that $\lim_{ t \to 0 }v(x,t) = u(x,0)$

#### 3.1

We essentially consider the whole line using the odd extension of the initial condition $u(x,0)$: 
$$
\begin{gather}
v_{t} = kv_{x x}, \hspace{.5cm} -\infty<x<\infty \hspace{.5cm} t>0 \\ \\ 

v(x,0) = \phi_{odd}(x) = \begin{cases}
e^{ -x } \hspace{.5cm} x>0  \\
-e^{ x } \hspace{.5cm} x<0
\end{cases}
\end{gather}
$$
We have that on page 49, equation 8:
$$
\begin{gather}
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\int_{-\infty}^{\infty} e^{ -(x-y)/4kt }\phi(y) \, dy \hspace{.5cm} x>0 
\end{gather} 
$$
We have that $x>0$ as we consider the half line. We now reduce this formula using two different integrals over the half line and $x<0$. We use the odd extension: 
$$
\begin{gather}
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \left[ \int _{-\infty}^0 e^{ -\frac{(x-y)^{2}}{4kt}}(-e^{ y }) \, dy  +\int _{0}^\infty e^{ -\frac{(x-y)^{2}}{4kt} }e^{ -y }\, dy \right] \\ \\ 
\text{ in first integral } \hspace{.2cm} y=-p \hspace{.5cm} \text{in second integral} \hspace{.2cm} y=p: \\ \\ 

u(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\left[ \int _{\infty}^0 e^{ -\frac{(x+p)^{2}}{4kt} }e^{ -p }\, dp  \hspace{.2cm} + \int_{0}^\infty  e^{ -\frac{(x-p)^{2}}{4kt} }e^{ -p }\, dp \right] \\ \\ 

\text{thus} \hspace{.2cm} u(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\left[ \int _{\infty}^0 e^{ -\frac{(x+p)^{2}}{4kt} -p}\, dp  \hspace{.2cm} + \int_{0}^\infty  e^{ -\frac{(x-p)^{2}}{4kt} -p}\, dp \right] \\ \\ 
\end{gather}
$$
After some not so fun algebra:/

$$
\begin{gather}
-\frac{(x+p)^{2}}{4kt} = kt + x - \frac{(x+2kt+p)^{2}}{4kt} \\ \\ 

-\frac{(x-p)^{2}}{4kt} - p = kt-x-\frac{(x-2kt-p)^{2}}{4kt} \\ \\ 
\end{gather}
$$
We now put this into our integrals
$$
\begin{gather}
 u(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\left[e^{ kt+x } \int _{\infty}^0 e^{ -\frac{(x+2kt+p)^{2}}{4kt} -p}\, dp  \hspace{.2cm} +
 e^{ kt-x }\int_{0}^\infty  e^{ -\frac{(x-2kt-p)^{2}}{4kt} -p}\, dp \right] \\ \\ 
\end{gather}
$$
We'll have to use something similar to u-sub, only this time its more like a,b sub:
$$
\begin{gather}
a = \frac{x+2kt+p}{\sqrt{ 4kt }} \hspace{1cm} b = \frac{-x+2kt+p}{\sqrt{ 4kt }} \\ \\ 

da = \frac{dp}{\sqrt{ 4kt }} = db = \frac{dp}{\sqrt{ 4kt }} \\ \\ 
\end{gather}
$$
We now plug in and simplify:

$$
\begin{gather}
u(x,t) = -\frac{e^{ kt+x }}{2} \left( \frac{2}{\pi}\int _{\frac{x+2kt}{\sqrt{ 4kt }}}^\infty e^{ -a^{2} } \, da  \right) + \frac{e^{ kt-x }}{2}\left( \frac{2}{\pi} \int _{\frac{-x+2kt}{\sqrt{ 4kt }}}^\infty e^{ -b^{2} }\, db  \right)
\end{gather}
$$
This matches the error function we use, so we make a further substitution
$$
\begin{gather}
u(x,t) = -\frac{e^{ kt+x }}{2}\text{erfc} \left( \frac{\hspace{.2cm}(x+2kt)}{\sqrt{4kt }} \right)+\frac{e^{ kt-x }}{2}\text{erfc} \frac{\hspace{.2cm}(-x+2kt)}{\sqrt{ 4kt }}
\end{gather}
$$
and that's it!

#### 3.1.4

#### a

From equation 6 on page 59, the integral is simply: 
$$
\begin{gather}
v(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\int _{0}^\infty S(x-y,t)\phi(y)\, dy 
\end{gather}
$$
We'll remember back from chapter 2 (page 49 equation 8) that this satisfies the diffusion equation over the whole line with initial conditions
$$
\begin{gather}
v_{t} = ku_{x x} \\ \\ 
v(x,0) = \phi(x) = \begin{cases}
x \hspace{.5cm} x>0 \\
x+1-e^{ 2x } \hspace{.5cm} x<0 
\end{cases} \\ \\ 
-\infty<x<\infty
\end{gather}
$$
##### b

We'll show the fact that the derivative to a solution is a solutions and linearity to show $w = v_{x} - 2v$:
$$
\begin{gather}
\text{Differentiate w/r/t/x} \hspace{.2cm}(v_{t})_{x} = k(v_{x x})_{x} \\ \\ 

2v_{t} = 2kv_{x x} \\ \\ 
\text{we substract:} \hspace{.2cm} (v_{x})_{t} -2v_{t} = k(v_{x})_{x x} - 2kv_{x x} \\ \\  
(v_{x} - 2v)_{t} = k(v_{x}-2v)_{x x} \\ \\ 

\end{gather}
$$
We see that $w = v_{x} - 2v$ satisfies the diffusion equation $w_{t} = kw_{x x}$. We know focus on the initial conditions:
$$
\begin{gather}
w(x,0) = v_{x}(x,0) - 2v(x,0) \\ \\ 
v(x,0) = \phi(x) = \begin{cases}
x \hspace{.5cm}x>0  \\
x+1-e^{ 2x } \hspace{.5cm} x<0
\end{cases} \\ \\ 
v_{x}(x,0) = \phi'(x) = \begin{cases}
1 \hspace{.5cm}x>0 \\
1-2e^{ 2x } \hspace{.5cm} x<0 \\
\end{cases} \\ \\

w(x,0) = \phi'(x)-2\phi(x) = \begin{cases}
1-2x \hspace{.5cm} x>0 \\
-1-2x \hspace{.5cm} x<0 
\end{cases}
\end{gather}
$$

##### c

if $w(-x,0)= -w(x,0)$ , then $w(x,0) = \phi'(x)-2\phi(x)$ is a odd function. We use $w(x,0)$ that we found earlier, using $x\rightarrow -x$: 

$$
\begin{gather}
w(-x,0) = \begin{cases}
1-2(-x) \hspace{.5cm} -x>0 \rightarrow 1+2x \hspace{.5cm}x<0 \rightarrow -1+2x \hspace{.2cm}x>0 \\
-1-2(-x) \hspace{.5cm} -x<0 \rightarrow-1+2x \hspace{.5cm}x>0 \rightarrow 1+2x \hspace{.5cm} x>0
\end{cases}
\end{gather}
$$
This is equivalent to $-w(x,0)$

##### d
Both in class, and as a result of exercise 2.4.11.a, if the initial condition is an odd function of $x$ then our solution to the equation is also an odd function. Thus $w(-x,t)= -w(x,t)$


##### e

Because $w(x,t)$ is an odd function, $w(0,t)=0$ is already true, thus we can solve the half-line problem simply considering $x>0$. We already know the solution is: 
$$
\begin{gather}
w_{t} = kw_{x x} \hspace{.5cm}w(x,0) = \phi'(x)-2\phi(x) \hspace{.5cm} -\infty<x<\infty \\ \\ 
\text{where} \hspace{.2cm} w(x,t) = \frac{1}{\sqrt{ 4\pi kt }}\int_{-\infty}^{\infty} e^{ \frac{(x-s)^{2}}{4kt} }[\phi'(s) - 2\phi(s)] \, ds \\ \\ 

\end{gather}
$$
We use our earlier substitution $w = v_{x}-2v$
$$
\begin{gather}
v_{x} - 2v = \frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ \frac{(x-s)^{2}}{4kt} }[\phi'(s)-2\phi(s)] \, ds \\ \\ 
\end{gather}
$$
we can break up the integral
$$
\begin{gather}
v_{x} - 2v = \\ \\ 
\frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -\frac{(x-s)^{2}}{4kt} }\phi'(s) \, ds = v_{x}(x,t) \\ \\ 
-2 \frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -\frac{(x-s)^{2}}{4kt} }\phi(s) \, ds = v(x,t) \\  
\end{gather}
$$
If we discount the -2 in the third line, we essentially have, considering $x>0$, a solution to the initial boundary value problem satisfied by $u(x,t)$. Since it's unique for $u(x,t)$: 
$$
\begin{gather}
u(x,t) =  \frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -\frac{(x-s)^{2}}{4kt} }\phi(s) \, ds  \hspace{.5cm}x>0 \\  
\end{gather}
$$
We're all set.

#### 3.2.3

We know that we can model the infinite string with the wave equation. The initial boundary value problem is:
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} \hspace{.5cm} 0<x<\infty \hspace{.2cm} t>0 \\ \\ 

u(x,0) = \phi(x)  \hspace{.5cm} u_{t}(x,0) = c\phi'(x) \\ \\ 
u(0,t) = 0
\end{gather}
$$
Similar to the tricks above, we only want the half line $0<x<\infty$, so we can use the method of reflection to satisfy the Dirichlet boundary conditions: 
$$
\begin{gather}
v_{tt} = c^{2}v_{xx} \hspace{.5cm}-\infty<x<\infty \hspace{.2cm}t>0 \\ \\ 
v(x,0) = \phi_{odd}(x), v_{t}(x,0) = c\phi'_{odd}(x) \\ \\ 

\phi_{odd}(x) = \begin{cases}
\phi(x) \hspace{.5cm}x>0 \\
-\phi(-x) \hspace{.5cm} x<0
\end{cases} \\ \\ 

c\phi'_{odd}(x) = \begin{cases}
c\phi'(x) \hspace{.5cm}x>0 \\
-c\phi'(-x) \hspace{.5cm} x<0
\end{cases}
\end{gather}
$$
using the d'Alembert's formula: 
$$
\begin{gather}
v(x,t) = \frac{1}{2}\left[ \phi_{odd}(x+ct)+\phi_{odd}(x-ct)+ \frac{1}{2c}\int _{x-ct}^{x+ct}c\phi'_{odd}(s) \, ds  \right]
\end{gather}
$$
we realize that if we restrict $v>0$, then it's our solution for $u$ on the half line. 
$$
\begin{gather}
v(x,t) = \frac{1}{2}[\phi_{odd}(x+ct) + \phi_{odd}(x-ct)]+ \frac{1}{2c}\int _{x-ct}^{x+ct}c\phi'_{odd}(s) \, ds 
\end{gather}
$$
We now have two different functions
$$
\begin{gather}
1. 
\hspace{.5cm} \phi_{odd}(x+ct) = \begin{cases} \phi(x+ct) \hspace{.5cm}x+ct>0 \\ 
-\phi(-x-ct) \hspace{.5cm}x+ct<0
\end{cases} \\ \\ 

\phi_{odd}(x-ct) = \begin{cases}
\phi(x-ct) \hspace{.5cm}x-ct>0  \\
-\phi(-x+ct) \hspace{.5cm} x-ct<0
\end{cases}
\end{gather}
$$
For each quadrant of the $xt$ graphs, we have to check $u(x,t)$. For the portion of the quadrant  above the line $x-ct = 0$ (with the help of substitution)
$$
\begin{gather}
u(x,t) = \phi(x+ct) - \phi(-x+ct)
\end{gather}
$$
for the portion of the quadrant below the line $x-ct=0$
$$
\begin{gather}
u(x,t) = \phi(x+ct)
\end{gather}
$$
Thus for all $t>0$
$$
\begin{gather}
u(x,t) = \begin{cases}
\phi(x+ct)-\phi(-x+ct) \hspace{.5cm} x-ct<0 \hspace{.5cm} \\
\phi(x+ct) \hspace{.5cm}x-ct>0
\end{cases}
\end{gather}
$$
Dirichlet is happy now.


#### 3.2.10

We use the lovely method of reflection. Over the whole line, we'll use the even extension when $x=0$ and odd when $x= \frac{\pi}{2}$: 
$$
\begin{gather}
v_{tt}= 9v_{x x} -\infty<x<\infty \hspace{.5cm}t>0\\ \\ 
v(x,0) = \phi_{ext}(x) \\ \\ 
v_{t}(x,0) = \psi_{ext}(x)
\end{gather}
$$
Inspired by the initial conditions, the solution for v using d'Alembert's formula: 
$$
\begin{gather}
v(x,t) = \frac{1}{2}[\phi_{ext}(x+3t)+\phi_{ext}(x-3t)]+ \frac{1}{6}\int _{x-3t}^{x+3t}\psi_{ext}(s) \, ds \\ \\ 
\frac{1}{2}[\cos(x+3t)+\cos(x-3t)] \\ \\ 
u(x,t) = \cos x\cos 3t \hspace{.5cm}0<x< \frac{\pi}{2}
\end{gather}
$$
We're all set!

### Part 2

#### 1

##### a

The heat equation tells us that $u_{t} = u_{\theta\theta}$. We're also given, and just by the nature of trigonometric functions: $u(\theta+2\pi) = u(\theta)$. We have that
$$
\begin{gather}
E(t) = \frac{1}{2} \int _{-\pi}^\pi u^{2}(\theta,t)\, d\theta \\ \\ 
\end{gather}
$$
we found that
$$
\begin{gather}
E'(t) = \int_{-\pi}^\pi uu_{t}\, d\theta =   \int _{\pi}^\pi uu_{\theta\theta} \, d \\ \\ 
\text{we use integration by parts} \hspace{.2cm} \\ \\ 
u = u \hspace{.5cm}dv= u_{\theta\theta} \\ \\ 
du = u_{\theta}d\theta \hspace{.5cm} v = u\theta \\ \\
E'(t) = uu_{\theta}|_{-\pi}^\pi - \int _{-\pi}^\pi (u_{\theta})^{2}\, d\theta 
\end{gather}  
$$
but $u_{\theta}= 0$ as we're periodic. Thus $E'(t)\leq 0$

##### b
we have that our initial condition $u(\theta,0) = 0$. Thus tells us immediately that $E(0)=0$. Now if $E(0)=0$ and $E'(t)\leq 0$ as we've proven in part a, then $E(t)\equiv0$. Thus we have that
$$
\begin{gather}
0 = \int _{-\pi}^\pi u^{2}(\theta,t) \, d\theta 
\end{gather}
$$
If this equation is true for any time $t$, then we must have that $u(\theta,t)= 0$

#### 2

##### a
Using our hint
$$
\begin{gather}
E(t) = \frac{1}{2}(u'^{2}+u^{2})\geq uu'
\end{gather}
$$
We know that $E'(t) = 2u'u'' +2uu'$. We'll continue, use the value of $u''$ and input it into this equation: 

$$
\begin{gather}
u'' = -b(t)u' -c(t)u 
\end{gather}
$$
We can now plug this into our derivative: 
$$
\begin{gather}
E'(t) = u'(-b(t)u'-c(t)u)+ uu' \\ \\ 
= -b(t)u'u' - c(t)u'u+uu' \\ \\
\leq \lvert b(t) \rvert u'^{2} + \lvert c(t) \rvert uu' + uu' 
\end{gather}
$$
Now, we consider when $b(t),c(t)=M$ or the max that they can be: 
$$
\begin{gather}
\leq M(u')^{2}+(1+M)uu' \\ \\
\leq M(u')^{2}+(1+M)E(t) \\ \\
= \gamma E(t) \hspace{.5cm} \gamma = 3M+1
\end{gather}
$$
Thus we've proven $E'(t)\leq\gamma E(t)$
##### b
We have that $E(t) \leq e^{ \gamma t }E(0)$ for $t \in [0,A]$. We'll first start by calculating $(e^{ -\gamma t }E(t))'$ 
$$
\begin{gather}
(e^{ -\gamma t }E(t))'= -\gamma te^{ -\gamma t }E(t) + e^{ -\gamma t }E'(t) \\ \\ 
= e^{ -\gamma t }(-\gamma tE(t)+E'(t))
\end{gather}
$$
we note that the quantity inside the parenthesis has to continuously decrease. This is because, we just proved that $E'(t)\leq\gamma E(t)$. Thus, as time $t$ continues $\gamma E(t)$, is always larger in magnitude than $E'(t)$ which makes $e^{ -\gamma t }(-\gamma tE(t)+E'(t))$ a negative number, or $(e^{ -\gamma t }E(t))' \leq 0$. 

##### c
We first have: 
$$
\begin{gather}
E(t) \leq e^{ \gamma t }E(0) = 0 
\end{gather}
$$
There are functions that exist such that $u(0)=u'(0)=0$ such as $x^{3}$, but there are no functions such that, derived from $E(t) = \frac{1}{2}(u'^{2}+u^{2})$ where $E(t) = 0$, $-u'^{2}=u^{2}$ unless $u(t) = 0$ for all $t \in[0,A]$. That is, $E(t)$ is a sum of squares. Thus $u(t) = 0$ $\forall t\in[0,A]$

##### d
We found earlier that 
$$
\begin{gather}
u''+b(t)u'+c(t)u = 0
\end{gather}
$$
we also know that: 
$$
\begin{gather}
v'' + b(t)v'+c(t)v = f(t) \\ \\ 
w'' + b(t)w'+c(t)w = f(t) \\ \\ 

f(t)-f(t) = 0
\end{gather}
$$
thus we can use this information to say the following: 
$$
\begin{gather}
u''+b(t)u'+c(t)u = v'' + b(t)v'+c(t)v - w'' - b(t)w'- c(t)w \\ \\ 
v'' + b(t)v'+c(t)v - w'' - b(t)w'- c(t)w = 0
\end{gather}
$$
thus, at $t=0$
$$
\begin{gather}
v'' = w''
\end{gather}
$$
which is also equivalent for $t\geq 0$. Thus we can rewrite the second to the last math line as follows: 
$$
\begin{gather}
b(t)v'+c(t)v - w'' - b(t)w'- c(t)w \\ \\ 
b(t)(v'-w')+c(t)(v-w) = 0
\end{gather}
$$

Since $b(t),c(t)$ are continuous, this equality is only true when $v=w$.
##### e

If in the equation $b(t),c(t),f(t)$ are periodic, we'll use the uniqueness assertion: if $\phi(t),\psi(t)$ are both solutions that satisfy equation 2 along with $\phi(0)=\psi(0)$, then $\phi(t) = \phi(t)$ as we've just showed in part d. Then we have 
$$
\begin{gather}
\phi''(t+P) + b(t+P)\phi'(t+P)+c(t+P)\phi(t+P) = f(t+P) \hspace{.5cm}t\geq 0
\end{gather}
$$
Thus, from earlier, ($b(t),c(t),f(t)$ are periodic):
$$
\begin{gather}
\phi''(x+P)+ b(t)\phi'(t+P)+c(t)\phi(t+P) = f(t) \hspace{.5cm} t\geq 0\\ \\ 
\end{gather}
$$
if $\psi(t) = \phi(t+P)$ then:
$$
\begin{gather}
\psi''(t) = b(t)\psi'(t)+c(t)\psi(t) = f(t)
\end{gather}
$$
Lastly, if $\phi(P) = \phi(0)$, then $\psi(0)=\phi(0)$. By our uniqueness assertion $\phi(t+P) = \psi(t)$ for all $t\geq 0$, thus $\phi$ is periodic. 


#### 3 

##### a
We have that $u_{t} = u_{x x}$, $u(-L,t) = u(L,t)=0$, $u(x,0)=f(x)$

We first start off with the derivative of $E(t)$
$$
\begin{gather}
E'(t) = \int _{-L}^L uu_{t} \, dx = \int _{-L}^L uu_{x x}\, dx  \\ \\ 
= uu_{x}|_{-L}^L - \int _{-L}^L u_{x}^{2}\, dx 
\end{gather}
$$
for similar reasons as part 2 1a, $u_{x}=0$ as the equation is periodic. Thus we have 
$$
\begin{gather}
E'(t) = = uu_{x}|_{-L}^L - \int _{-L}^L u_{x}^{2}\, dx \leq 0
\end{gather}
$$

##### b

We'll have $\phi$ be an additional solution with such boundary conditions: 
$$
\begin{gather}
\psi = u-\xi \\ \\
\psi(-L,t) = \psi(L,t) = 0
\end{gather}
$$
this situation is actually similar to 1b,
$$
\begin{gather}
\psi(L,t)-u(L,t) = \frac{1}{2}\int _{-L}^L u^{2}(x,t) \, dx = 0 
\end{gather}
$$
which is only true when 
$$
\begin{gather}
\xi(L,t) = u(L,t) \\ \\
\end{gather}
$$
which also applies to 
$$
\begin{gather}
\xi(-L,t) = u(-L,t)
\end{gather}
$$
thus $u$ must be unique under our conditions. 

##### c

When $u(x,t)$ is even, we have by convention $u(x,t) - u(-x,t)= 0$. From the previous part b we have that
$$
\begin{gather}
\psi(x,t) = u(x,t) - u(-x,t)
\end{gather}
$$
since a linear combination of the solution is also a solution, we have that: 
$$
\begin{gather}
\psi(x,t)_{t} = \psi_{x x} 
\end{gather}
$$
thus we have that: 
$$
\begin{gather}
\psi(x,0) = \xi(x)-\xi(-x) = 0
\end{gather}
$$
by uniqueness
$$
\begin{gather}
\psi(x,t) = \xi(x,t)-\xi(-x,t) = 0
\end{gather}
$$
Thus at any later time $t$ 
$$
\begin{gather}
u(x,t) = u(-x,t)
\end{gather}
$$


We are all done:)