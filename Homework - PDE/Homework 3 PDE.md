#### 2.2.4

We first recognize that $u(x+h, t+k) + u(x-h,t-k) = u(x+k,t+h) +u(x-k,t-h)$ defines a parallelogram that looks like the following:

![[Pasted image 20240212003631.png|center|300]]

Where we'll define the following points:
- $J_{1} = (x+h, t+k),\hspace{.2cm} K_{1} = (x-h,t-k),\hspace{.2cm}J_{1} = (x+k,t+h)\hspace{.2cm} K_{2}=(x-k,t-h)$. 

We can use the  the derivation of the homogenous wave equation such that
$$
\begin{gather}
u(x,t) = F(x + ct) + G(x-ct) = \frac{1}{2}\left[ f(x-ct) +f(x+ct)+ \frac{1}{2c} \int _{x-ct} ^{x+ct} g(s) \, ds  \right]
\end{gather}
$$
Following from the previous math line, we know: 
$$
\begin{gather}
F(x,t) =\frac{1}{2}\left[ f(x-ct) - \int _{x+ct}^{x-ct} g(s)\, ds  \right] \\ \\ 
G(x,t) = \frac{1}{2} [f(x+ct)] - \int _{x-ct}^{x+ct} g(s) \, ds 
\end{gather}
$$
We reintroduce the change of variables of the form 
$$
\begin{gather}
\xi = x+ct  \hspace{.5cm} \eta = x-ct
\end{gather}
$$
We have that $x-ct =s, \hspace{.2cm} F(x-ct) = F(s), x+ct =s, G(x+ct) = G(s)$ where, since the $F(x,t), G(x,t)$  are constant along $\xi = x+ct  \hspace{.5cm} \eta = x-ct$, we have that $F(J_{1})=F(K_{1})$ and $G(J_{1}) =G(K_{2})$. For a full list of the relationships as well as a drawing: 
![[Pasted image 20240212010339.png|center|]]

$$
\begin{gather}
F(J_{1}) = F(K_{1}) \hspace{.5cm} F(J_{2}) = F(K_{2}) \\ \\ 
G(J_{1}) = G(K_{2}) \hspace{.5cm} G(K_{2}) = G(K_{1}) 
\end{gather}
$$
Now that we'll built the relationships, we'll apply them below to prove $u(x+h, t+k) + u(x-h,t-k) = u(x+k,t+h) +u(x-k,t-h)$: 

$$
\begin{gather}
u(J_{1}) + u(J_{2}) = [F(J_{1})+G(J_{1})]+ [F(J_{2})+ G(J_{2})] \\ \\ 

u(J_{1})+u(J_{2}) = [F(K_{1})+G(K_{2})] +[F{K_{2}}+G(K_{1})] \\ \\ 

\text{We move around terms:} \hspace{.2cm} \\ \\ 

u(J_{1}) + u(J_{2}) = [F(K_{1})+G(K_{1})] +[F(K_{2})+G(K_{2})] \\ \\ 
\end{gather}
$$
We notice that the right side of the last math line is $u(J_{1})+uJ_{2}=u(K_{1})+u(K_{2})$. Which proves
$$
\begin{gather}
u(x+h, t+k) + u(x-h,t-k) = u(x+k,t+h) +u(x-k,t-h)
\end{gather}
$$

#### 2.3.1

We'll return back to the basic ways to find max and mins from calculus. We first need to find the first derivative of $u$ equal to zero. That means we need $u_{t},u_{x} = 0$: 
$$
\begin{gather}
u_{t} = -2k \\ \\ 
u_{x} = -2x
\end{gather}
$$
Since $k>0$, $u_{t}$ is constant and thus has no max/min. 

![[Pasted image 20240212012604.png|center|300]]

Plugging into the equation $u(x,t) = 1-x^{2}-2kt$, when $x=0$ and $t=0$ $u$ is at a max, and when $x=1$ and $t=T$, $u$ is at a minimum. 

#### 2.3.2

We have from the maximum principle that "If $u(x,t)$ satisfies the diffusion equation in a rectangle (say, $0\leq x\leq l, 0\leq t\leq T$) in space-time, then the maximum value of $u(x,t)$ is assumed either initially $(t=0)$ or on the lateral sides $(x=0 \hspace{.2cm}\text{or} \hspace{.2cm} x=l$)"

![[Pasted image 20240212014046.png|center|300]]


##### a

 Assume that the maximum of $u$ occurs on the line $T$ on the purple tic mark . Then the value of $u$: $u(T)>u(T_{1})$ will continue to be the maximum. Otherwise, $u$ will have a maximum at $T_{1}>T$, suggesting $M(T)$ increases as a function of $T$ 

##### b

Similarly, assume that the minimum of $u$ occurs on the line $T$ on the purple tic mark. Then the value of $u$: $u(T)<u(T_{1})$ will continue to be the minimum. Otherwise, $u$ will have a minimum at $T_{1}>T$, suggesting $M(T)$ decreases as a function of $T$ 

#### 2.3.6

If $u$ and $v$ are two solutions then we have
$$
\begin{gather}
u_{t} = ku_{xx} \\ \\ 
v_{t} = ku_{xx}
\end{gather}
$$
Since $u\leq v$ for $0\leq t\leq\infty$: 
$$
\begin{gather}
v(x,0) - u(x,0) \geq 0 \\ \\ 
v(0,t) - u(0,t) \geq 0\\ \\ 
v(l,t) - u(l,t) \geq 0 \\ \\ 
\end{gather}
$$
We can subtract the two equations such that 

$$
\begin{gather}
v_{t} - u_{t} = (v-t)_{x} = kv_{xx} - ku_{x x} = k(v-u)_{x x}

\end{gather}
$$
If we replace $w$ with $v-u$;
$$
\begin{gather}
w_{t} = kw_{x x}
\end{gather}
$$
The minimal principle states that $w$ will have a minimum principle initially or somewhere along the boundary. The lowest $w$ is zero ($w\leq 0$), and $0\leq t\leq \infty$ and $0\leq x\leq l$. This proves the comparison principle: $v\geq u$ for  $0\leq t\leq \infty$ and $0\leq x\leq l$. 


#### 2.4.4

We begin with the initial formula: 
$$
\begin{gather}
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{-\infty}^{\infty} e^{ -(x-y)^{2}/4kt }\phi(y) \, dy \\ \\ 
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{ -(x-y)^{2}/4kt }\underbrace{ e^{ -y }  }_{ \text{from} \hspace{.2cm} \phi(x) = e^{ -x }}\, dy \\ \\ 

u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{ -(x-y)^{2}/4kt }e^{ -4kty/4kt } \, dy \\ \\ 

u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{ \frac{-(x-y)^{2}-4kty}{4kt} } \, dy \\ \\ 
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{ \frac{-(y-x)^{2}+4kty}{4kt} } \, dy \\ \\
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} \int_{0}^{\infty} e^{- \frac{(y-x+2kt)^{2}+4ktx -4k^{2}t^{2}}{4kt} } \, dy \\ \\ 
\end{gather}
$$
Since the function is in terms of $y$ we can begin taking out $e^{ \text{stuff} \hspace{.2cm}  }$that isn't: 
$$
\begin{gather}
u(x,t) = \frac{1}{\sqrt{ 4\pi kt }} e^{ 4ktx/4kt }e^{ 4k^{2}t^{2}/4kt }\int_{0}^{\infty} e^{-(y-x+2kt/\sqrt{ 4kt })^{2} } \, dy \\ \\ 
\frac{1}{\sqrt{ 4\pi kt }} e^{ -x+kt } \int _{0}^\infty e^{ -\left( \frac{(y_{0}x+skt)}{\sqrt{ 4kt }} \right)^{2} }\, dy \\ \\ 
\end{gather}
$$
We can rewrite this as 
$$
\begin{gather}
= \frac{1}{\sqrt{ \pi }}e^{ -x+kt }\int _{\frac{-x+2kt}{\sqrt{ 4kt }}}^\infty e^{ -p^{2} } \, dp 
\end{gather}
$$
We'll use the Gauss error function from page 51: 

$$
\begin{gather}
\text{erf(x)} \hspace{.2cm} = \frac{2}{\pi}\int _{0}^x e^{ -p^{2} } \, ds =  
\end{gather}
$$
The complementary error function is just the erf(x) evaluated at $1-$erf(x): 
$$
\begin{gather}
\text{erfc(x)} \hspace{.2cm} = \frac{2}{\sqrt{ \pi }} \int _{x}^\infty e^{ -p^{2} }\, dp 
\end{gather}
$$
So we have that:
$$
\begin{gather}
\int _{\frac{-x+2kt}{\sqrt{ 4kt }}}^\infty e^{ -p^{2} }\, dp = \frac{\sqrt{ \pi }}{2}\text{erfc} \left( \frac{-x+2kt}{\sqrt{ 4kt }} \right) 
\end{gather}
$$
Lastly
$$
\begin{gather}
u(x,t) = \frac{1}{2}e^{ (-x+krt) }\text{erfc}\left( \frac{-x+2kt}{\sqrt{ 4kt }} \right)
\end{gather}
$$
#### 2.4.11

##### a

The IVP for the diffusion equations:

$$
\begin{gather}
u_{t} = ku_{x x} \hspace{.5cm}u(x,0) = \phi(x)
\end{gather}
$$
The odd extension tells us that $\phi(-x) = -\phi(x)$ which we apply to our diffusion equation: 

$$
\begin{gather}
u_{t}(-x,t) = ku_{x x}(-x,t), \hspace{.5cm}u(-x,0) =\phi(-x)= -\phi(x)
\end{gather} 
$$
We now consider, from the hint, $u(-x,t)+u(x,t)$. The former satisfies the diffusion equation via odd extension and the latter is the general solution, thus a linear combination of the two functions should also be a solution which follows from the Linearity of $u$. Thus we have 
$$
\begin{gather}
(u(-x,t)+u(x,t))_{t} = k(u(-x,t)+u(x,t))_{x x}
\end{gather}
$$
We have: 
$$
\begin{gather}
u(x,0) = \phi(x) \hspace{.5cm} u(-x,0) = -\phi(x) \\ \\ 
-\phi(x) + \phi (x) = 0 \hspace{.5cm}-\phi(x) = \phi (x) \\ \\ 
\text{Thus} \hspace{.2cm} u(-x,0) = u(x,0)
\end{gather}
$$
A solution to a diffusion equation is automatically unique, thus 
$$
\begin{gather}
u(-x,t) = -u(x,t)
\end{gather}
$$
is our solution which shows that if $\phi(x)$ is an odd function, the solution $u(x,t)$ is also an odd function. 

##### b

We now show that the last statement is true for even functions. We have the following diffusion equation and initial conditions
$$
\begin{gather}
u_{t} = ku_{x x} \hspace{.5cm} u(x,0) = \phi(x)
\end{gather}
$$
An even function $\phi(x)$ implies that $\phi(-x) = \phi(x)$. This would imply for our solution
$$
\begin{gather}
u_{t}(-x,t) = ku_{x x}(-x,t). \hspace{.5cm} u(-x,0) = \phi(-x) =\phi(x)
\end{gather}
$$
Similar to are argument above, we have that the linear combinations of the even extension and our general solutions yield:
$$
\begin{gather}
(u(-x,t) - u(x,t))_{t} = k(u(-x,y)-u(x,t))_{x x} \\ \\ 
\end{gather}
$$
Again the solution of the diffusion equation that satisfies $u(-x,t)-u(x,t)=0$ is unique, which yields: 
$$
\begin{gather}
u(-x,t) = u(x,t)
\end{gather}
$$
so if $\phi(x)$ is an even function, then $u(x,t)$ is an even function. 

##### c

The wave equation needs two initial conditions: $\phi(x) = u(x,0)$ and $\psi( x) = u_{t}(x,0)$. We'll start off with odd functions similar to earlier. We'll prove that if our initial conditions are odd functions for the wave equation, then so is our solution: 

Proof:
Odd functions imply:
$$
\begin{gather}
\phi(-x) = -\phi(x) \\ \\ 
\psi(-x) = -\phi(x)
\end{gather}
$$
The IVP is $u(-x,t)$ such that: 
$$
\begin{gather}
u_{tt}(-x,t) = c^{2}u_{x x}(-x,t) \hspace{.5cm} \\ \\ 
u(-x,0)=\phi(-x) = -\phi(x) \\ \\ 
\hspace{.5cm}u_{t}(-x,0)=\psi(-x)=-\psi(x)
\end{gather}
$$

We'll use the same argument of the linear equations: 
$$
\begin{gather}
u(-x,0) +u(x,0) = -\phi(x) +\phi(x) = 0 \\ \\ 
u_{t}(-x,0) + u_{t}(x,0) = -\psi(x) + \psi(x) = 0 \\ \\
(u(-x,t)+u(x,t))_{tt} = c^{2}(u(-x,t)+u(x,t))_{x x} \\ \\ 
\text{which satisfies} \hspace{.2cm} u(-x,t)+u(x,t) = 0 
\end{gather}
$$
Since the solution to the wave equation with our initial condition is always unique, we have that
$$
\begin{gather}
u(-x,t) = -u(x,t)
\end{gather}
$$
which proves our earlier argument.

Now we'll prove the same argument for even functions. If $\phi,\psi$ is an even functions, we have that 
$$
\begin{gather}
\phi(-x) = \phi(x) \\ \\ 
\psi(-x) = \psi(x) \\ \\ 
\end{gather}
$$
We have that
$$
\begin{gather}
u(x,0) = \phi(x) \hspace{.2cm} u_{t}(x,0) = \psi(x) \\ \\ 
u(-x,0) = \phi(-x) = \phi(x) \hspace{.2cm}u_{t}(-x,0) = \psi(-x) = \psi(x) \\ \\ 
\end{gather}
$$
bringing back our linear combination argument: 
$$
\begin{gather}
\phi(x) -\phi(x) = u(-x,0) -u(x,0) = 0 \\ \\
u_{t}(-x,0) - u_{t}(x,0) = \psi(x) -\psi(x) = 0 \\ \\ 
\end{gather}
$$
Finally we have
$$
\begin{gather}
u(-x,t) = u(x,t)
\end{gather}
$$
So since $\phi(x),\psi(x)$ are even functions, then $u(x,t)$ is even as well. 

