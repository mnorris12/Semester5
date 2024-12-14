#### 1.1.9 
Show that the functions $c_{1}+c_{2}\sin ^{2}(x)+c_{3}\cos ^{2}(x)$ form a vector space. Find a basis of it. What is it's dimension?

Solution: 

To show that the functions form a vector space, they have to follow certain axioms: vector addition and scalar multiplication: 
$$
\begin{gather}
\text{Vector addition:} \hspace{.5cm} (c_{1}+c_{2}\sin ^{2}x+c_{3}\cos ^{2}x)+ (c_{4}+c_{5}\sin ^{2}x+c_{6}\cos ^{2}x) = \\
c_{1+4}+ (c_{2+5})\sin ^{2}x + c_{3+6}\cos ^{2}x
\end{gather}
$$
Functions of the same form as the original was returned, so this condition was met. Now scalar multiplication: 
$$
\begin{gather}
\text{Scalar multiplication:} \hspace{.5cm} \begin{pmatrix}
c_{4}  \\
c_{5} \\
c_{6} \\
\end{pmatrix}
(c_{1}+c_{2}\sin ^{2}x+c_{3}\cos ^{2}x) = \\
c_{1\cdot_{4}}+c_{2\cdot_{5}}\sin ^{2}x+ c_{3\cdot_{6}}\cos ^{2}x
\end{gather}
$$
Which is of the same form as the original, thus the conditions have been met to be a vector space. 

- We now find a basis for the function. we'll use the following trigonometric properties: 
$$
\sin ^{2}x = \frac{1-\cos(2x)}{2} \hspace{.5cm} \text{and} \hspace{.5cm}\cos ^{2}x = \frac{1+\cos(2x)}{2}
$$
Thus we can rewrite our original function as: 
$$
\begin{gather}
c_{1} + c_{2}\frac{(1-\cos(2x))}{2} +c_{3} \frac{1+\cos(2x)}{2} \\ \\ 
c_{1} + \frac{1}{2}[c_{2}-c_{2}(\cos (2x))+c_{3}(c_{3}\cos(2x))] \\ \\ 
c_{1}+ \frac{1}{2}(c_{2}+c_{3})[(\cos(2x))(-c_{2}+c_{3})] \\ \\ 
c_{1}+c_{\frac{2+3}{2}}c_{-2+3} \cos(2x)
\end{gather}
$$
thus we end up with the matrix: 
$$
\begin{gather}
\begin{pmatrix}
c_{2} \\
c_{\frac{2+3}{2}}\cdot c_{-2+3} \\ 
\end{pmatrix} (1,\cos(2x)) \hspace{.5cm} \text{dim=2}
\end{gather}
$$
--- 
#### 1.2.2

We have that $3u_{y}+u_{xy}= 0$. We've been given a hint that we can substitute $v=u_{y}$:

$$
\begin{gather}
3v +v_{x} = 0
\end{gather}
$$
We notice carefully that this is the ODE (first order linear) form $\frac{dy}{dx}+p(x)y = g(x)$ where $g(x)= 0$. Furthermore: 
$$
\begin{gather}
\frac{dy}{dx} \rightarrow v_{x} \\ \\ 

p(x) \rightarrow 3 \\ \\ 

y \rightarrow v \\ \\
\end{gather}
$$
with this in mind, the next step of solving this equation is to identify a function $\mu(x)$ such that: 
$$
\begin{gather}
\mu(x) = e^{\int p(x) \, dx } \hspace{.2cm}\rightarrow e^{\int 3 \, dx } =e^{3x} \\ \\ 
\end{gather}
$$
thus we'll multiply $\mu(x)$ to all the terms in our PDE: 

$$
\begin{gather}
3e^{3x}v +e^{3x}v_{x} = (e^{3x}v)' = 0 \hspace{.5cm} \text{we integrate w/r/t/x} \\ \\ 
\int (e^{3x}v)' \, = \int 0 \, \\ \\ 

e^{3x}v = f(y) \\ \\ 

v = f(y)e^{-3x} \\ \\ 

u_{y}(x,y) = f(y)e^{-3x} \hspace{.5cm} \text{we integrate w/r/t/y next} \\ \\

\int u_{y}(x,y) = \int f(y)e^{-3x} \, \\ \\ 

u(x,y) = F(y)e^{-3x} + g(x)
\end{gather}
$$

We're all set!

#### 1.2.9

We have the equation $u_{x}+u_{y}=1$. We'll use the method of characteristics here and try to utilize solving an ODE from this PDE. Let's label some functions
$$
\begin{gather}
y(\zeta,0) = \zeta, \hspace{.5cm} \frac{dy}{dx} = 1 
\end{gather}
$$
Thus if $u_{x}+u_{y}=1$ then so must $\frac{ \partial u }{ \partial x }$. We'll integrate that to get our equation.
$$
\begin{gather}
du = dx \\ \\ 

\int  \, du = \int  \, dx \\ \\ 

u = x + f(\zeta) \\ \\ 

y  = x+\zeta \\ \\ 

\zeta = y - x \\ 
\end{gather}
$$
Thus we have
$$
\begin{gather}
u(x,y) = x + f(y-x)
\end{gather}
$$

