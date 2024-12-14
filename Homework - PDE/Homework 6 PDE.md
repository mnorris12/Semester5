#### 4.3.6

###### a

We show that if 
$$
\begin{gather}
a_{0}=a_{1}=a
\end{gather}
$$
Then there are no negative eigenvalues if $a\geq 0$, there is one if $-\frac{2}{l}<a<0$, and two if $a<-\frac{2}{l}$. 

$a\geq 0$: 

Let's begin with the first case $a\geq 0$. This problem implies that there is the same amount of radiation at both ends of the rod which coincides with case one. Thus as stated just below equation 17 on page 97, there is **no** negative eigenvalues when $a>0$. Alternatively, the image of the graph $(\gamma,y)$ below shows the equation 16 on page 97, in which where the green and red function intersect, we have an eigenvalue. We have arbitrarily chose $l=3$. We notice that the green function never initially never intersects the red, and then flattens out to $\gamma=0$ still never intersecting: 

![[Pasted image 20240313233232.png|center|400]]

There are no positive intersections when $\gamma=x>0$, so no negative eigenvalues when $a>0$.
When $a=0$ then using our equation 16 as we did with the graph
$$
\begin{gather}
\tanh\gamma l = -\frac{0}{\gamma^{2}} \\ \\ 
\tanh\gamma l = 0 \\ \\ 
\gamma l = \tanh^{-1}(0) \\ \\ 
\gamma l = 0 \hspace{.5cm} \text{where} \hspace{.2cm}l \neq 0
\end{gather}
$$
Thus $\gamma=0$, but in the negative case we have $\lambda=-\gamma^{2}<0$ which is a contradiction, so there are no negative eigenvalues when $a=0$

$-\frac{2}{l}<a<0$:

![[Pasted image 20240313232936.png|center|400]]

We'll preform graphical analysis for this case. The red function corresponds to the static $\tanh\gamma l$, and the green function corresponds to $-\frac{(2a)\gamma}{\gamma^{2}+a^{2}}$. Here, we've chosen an arbitrary length $l=3$ again, and restricted $-\frac{2}{l}\leq a\leq 0$. Which is different than our case (but completely includes our case) we want to solve, marginally by the two endpoints. Note that the two functions become nearly the same as they approach 0 from the right, they however do not intersect towards limit. As visible, there is only one place for positive values of $\gamma$ where the two functions intercept. Thus on the interval $-\frac{2}{l}<a<0$, there is only one negative eigenvalue. 


$a<-\frac{2}{l }$

The same reasoning for the previous case applies for this case. Here you can see there are two intersections with corresponds to eigenvalues

![[Pasted image 20240313233113.png|center|400]]


###### b

We show that there is a zero eigenvalue if and only if $a=0,-\frac{2}{l}$

According to equation 15 on page 96, there is a zero eigenvalue if and only if 
$$
\begin{gather}
a_{0}+a_{l}= -a_{0}a_{l}l \\ \\ 
2a = -a^{2}l
\end{gather}
$$
which can only happen when *(1)* $a_{0},a_{l}<0$, or *(2)* $a_{0},a_{l}=0=a$. The former situation *(1)* becomes the case when $a_{0},a_{l}=-\frac{2}{l}<0$ which produces a zero eigenvalue. The ladder situation becomes the case when $a=0$ which also produced a zero eigenvalue. Thus we've shown that there i a zero eigenvalue if and only if $a=0, -\frac{2}{l}$


#### 5.1.4

We want to use the Cosine Fourier Series on $(-\pi,\pi)$  such that $\phi(x)= \lvert \sin x \rvert$. Thus,
$$
\begin{gather}
\lvert \sin x \rvert = A_{0}+\sum_{n=1}^\infty A_{n}\cos\left(nx \right) \\ \\ 
l = \pi \\ \\ 
\text{w.t.s} \hspace{.5cm} \sum_{n=1}^\infty \frac{1}{4n^{2}-1} \hspace{.5cm}\sum_{n=1}^\infty \frac{(-1)^n}{4n^{2}-1}
\end{gather}
$$
For the above equation of $\phi(x)$, we actually don't need $A_{0}$ to find the sums in question (it ends up canceling to 0 in the next integral anyway). We actually only need $A_{n}$, so let's determine that by mulitplying $\phi(x)*\cos(mx)$. Although it may seem arbitrary, it leads us to some useful identities that Strauss has identified. We'll then integrate that product on both sides
$$
\begin{gather}
\int _{-\pi}^{\pi} \lvert \sin x \rvert(\cos(mx)) \, dx = \sum_{n=1}^\infty An\int \cos(nx)(\cos (mx)) \, dx 
\end{gather}
$$
The right hand integral $=0$ when $m\neq n$ (pg. 106) and $l=\pi$ when $m=n$ (107). The $m\neq n$ is obviously not fruitful, so we'll keep the case $m=n$ case.  
$$
\begin{gather}
\int _{-\pi}^{\pi} \lvert \sin x \rvert\cos nx \, dx = A_{n}\pi
\end{gather}
$$
Notice that the $m$ has changed to $n$ (again, they are equal). Also notice that the sum vanishes, because we only want one value of $n$ ($n=m$). We used Wolframe Alpha for the left hand integral, which gives us 
$$
\begin{gather}
\int _{-\pi}^{\pi} \lvert \sin x \rvert\cos nx \, dx  = -\frac{2(\cos(n\pi)+1)}{\pi(n^{2}-1)} = A_{n}
\end{gather}
$$
Now we can plug this back into the equation for $\phi(x)=\lvert \sin x \rvert$,
$$
\begin{gather}
\lvert \sin x \rvert = A_{0} +\sum_{n=1}^\infty -\frac{2(\cos(n\pi)+1)}{\pi(n^{2}-1)}(\cos nx)
\end{gather}
$$
Again, we'll drop the $A_{0}$, because we only want the sums. Now let's do some rearranging!
$$
\begin{gather}
\sum_{n=1}^\infty -\frac{2}{\pi} \frac{\cos(n\pi)+1}{(n^{2}-1)}\cos(nx)= -\frac{2}{\pi}\sum_{n=1}^\infty \frac{\cos(n\pi)+1}{(n^{2}-1)}\cos(nx) = -\frac{2}{\pi}\sum_{n=1}^\infty( \frac{(-1)^n+1) }{(n^{2}-1)}\cos(nx)
\end{gather}
$$
For the inside of the last sum , we'll notice that if $n$ is odd, the entire sum is 0. So we'll want the case when $n$ is even. We can thus say $n=2N$ as the produce of an even number with a even,odd number is always even. Thus
$$
\begin{gather}
-\frac{2}{\pi}\sum_{n=1}^\infty \frac{2}{((2N)^{2}-1)}\cos(nx) = -\frac{4}{\pi}\sum_{n=1}^\infty \frac{1}{(4(N)^{2}-1)}\cos(nx) = \lvert \sin x \rvert
\end{gather}
$$
To complete the question, we can choose arbitrary values of $x$ on the interval $(-\pi,\pi)$, 
$$
\begin{gather}
x = 0: \hspace{.5cm}0 = -\frac{4}{\pi}\sum_{n=1}^\infty \frac{1}{4(N)^{2}-1} \\ \\ 
x = \frac{\pi}{2}: \hspace{.5cm} 1= -\frac{4}{\pi}\sum_{n=1}^\infty \frac{(-1)^n}{4(N)^{2}-1}
\end{gather}
$$
We have the sums we desire, so we're all done!

#### 5.14

We want the Fourier Coefficient of $\phi(x)=\lvert \sin x \rvert$ on the interval $(-\pi,\pi)$ that vanishes. We know from page 114 that, 
$$
\begin{gather}
odd\cdot even=odd \\ \\ 
\end{gather}
$$
Additionally, we know from equation 5 on page 115 that 
$$
\begin{gather}
\int _{\pi}^\pi odd\, dx =0
\end{gather}
$$
We know that $\lvert \sin(x) \rvert$ is an even function as $\lvert \sin(-x) \rvert=\lvert -\sin (-x) \rvert=\lvert \sin(x) \rvert$, and that $\sin(x)$ is an odd function. Therefore, we want an integral that contains the product of both 
$$
\begin{gather}
\lvert \sin(x) \rvert \cdot \sin(x)
\end{gather}
$$
The corresponding coefficient is thus, 
$$
\begin{gather}
l=\pi\hspace{.5cm}B_{n} = \frac{1}{l}\int _{\pi}^\pi \lvert \sin(x) \rvert\sin nx \, dx 
\end{gather}
$$
on the full Fourier Series for $n\in\mathbb{Z}$. 

#### 5.3.9

We have that
$$
\begin{gather}
X(b) = \alpha X(a)+\beta X'(a)\hspace{.5cm}X'(b)= \gamma X(a) + \delta X'(a) \\ \\ 
\end{gather}
$$
We want to show that these boundary conditions are symmetric given $\alpha\delta-\beta\gamma = 1$. We define symmetry of boundary conditions to be 
$$
\begin{gather}
f'(x)g(x)-f(x)g'(x)|_{x=a}^{x=b}
\end{gather}
$$
where we'll additionally have that
$$
\begin{gather}
f'(x) = X_{1}'(x) \hspace{.5cm}g(x) = X_{2}(x) \\ \\ 
f(x) = X_{1}(x) \hspace{.5cm}g'(x) = X_{2}'(x)
\end{gather}
$$
Now we can start the problem! We can use the information in the last math line to state the following information,
$$
\begin{gather}
X_{1}(b)X_{2}(b)- X_{1}(b)X_{2}'(b) - X_{1}'(a) X_{2}(a)+X_{1}(a)X_{2}'(a)
\end{gather}
$$
We can expand this to the following,
$$
\begin{gather}
(\gamma X_{1}(a)+\delta X_{1}(a))(\alpha X_{2}(a)+\beta X_{2}'(a))-(\alpha X_{1}(a)+\beta X_{1}'(a))(\gamma X_{2}(a)+\delta X_{2}'(a)) \\ \\
-X_{1}'(a) X_{2}(a)+X_{1}(a)X_{2}'(a)
\end{gather}
$$
This can be expanded to the following, 
$$
\begin{gather}
\cancel{ \gamma\alpha X_{1}(a)X_{2}(a) }+\gamma\beta X_{1}(a)X_{2}'(a)+\delta\alpha X_{1}'(a)X_{2}(a)+\cancel{ \delta\beta X_{1}'(a)X_{2}'(a)+ } -\cancel{  \alpha\gamma X_{1}(a)X_{2}(a) } \\ \\ -\alpha\beta X_{1}(a)X_{2}'(a)C-\beta\gamma X_{1}'(a)X_{2}(a)-\cancel{ \beta\delta X_{1}'(a)X_{2}'(a) } - X_{1}'(a) X_{2}(a)+X_{1}(a)X_{2}'(a) \\ \\ =
X_{1}(a)X_{2}'(a)(\gamma\beta-\alpha\beta) +X_{1}'(a)X_{2}(a)[\delta\alpha-\beta\gamma] - X_{1}'(a) X_{2}(a)+X_{1}(a)X_{2}'(a) \\ \\ 
=X_{1}(a)X_{2}'(a)[-1] +X_{1}'(a)X_{2}(a)[1] - X_{1}'(a) X_{2}(a)+X_{1}(a)X_{2}'(a) =0\\ \\
\text{where we've used} \hspace{.2cm} \alpha\delta-\beta\gamma = 1 \hspace{.5cm}-\alpha\delta+\beta\gamma = -1
\end{gather}
$$
Thus, we're all done!

#### 5.4.15
We have the following conditions
$$
\begin{gather}
\phi(x)\equiv 1 \hspace{.5cm} 0<x<\pi \hspace{.5cm}\sum_{n=0}^\infty B_{n}\cos\left[ \left( n+\frac{1}{2} \right)x \right]
\end{gather}
$$
The expansion would be 
$$
\begin{gather}
1=  B_{1}\cos\left[ \left( 1+\frac{1}{2} \right)x \right] +B_{2}\cos\left[ \left( 2+\frac{1}{2} \right)x \right] + B_{3}\cos\left[ \left( 3+\frac{1}{2} \right)x \right]\dots
\end{gather}
$$
###### a

We first calculate the coefficient $B_{n}$. We have from equation 4 on pg. 125: 
$$
\begin{gather}
B_{n}  = \frac{f,X_{n}}{(X_{n},X_{n})} = \frac{1,\cos\left[ \left( n+\frac{1}{2} \right)x \right] }{\left( \cos\left[ \left( n+\frac{1}{2} \right)x \right],\cos\left[ \left( n+\frac{1}{2} \right)x \right] \right)} = \\ \\ 
\frac{\int_{0}^\pi \cos\left[ \left( n+\frac{1}{2} \right)x \right]  \, dx}{\int _{0}^\pi \cos ^{2}\left[ \left( n+\frac{1}{2} \right)x \right] \, dx } = \frac{2(4n+2)\cos(\pi n)}{(2n+1)(2\pi n-\sin(2\pi n)+\pi)} = \frac{4\cos(\pi n)}{(2\pi n+\pi)}
\end{gather}
$$
###### b

We can now expand the interval for $x$ such that $-2\pi<x<2\pi$. This values of $x$ that correspond with $\phi(x)=1$ are the interval of $-\pi,0$ such that $x \in(-\pi,0)$. That is 
$$
\begin{gather}
\sum_{n=0}^\infty \frac{4(-1)^n}{2\pi n+\pi}\cos\left( \left( n+\frac{1}{2} \right)x \right) = 1
\end{gather}
$$
this was tested by choosing several intervals in $-2\pi<x<2\pi$ and then determining which gave 1 rather than 0 or -1

###### c
We have that Persevals inequality on page 133 asserts that
$$
\begin{gather}
\int _{0}^\pi \lvert 1 \rvert^{2} \, dx = \sum_{n=0}^\infty \left\lvert  \frac{4(-1)^n}{(2n+1)\pi}  \right\rvert^{2}\int _{0}^\pi \left\lvert  \cos\left( n+\frac{1}{2} \right)x  \right\rvert^{2}\, dx = \\ \\ 
\frac{8}{\pi^{2}} \sum_{n=0}^\infty \frac{1}{(2n+1)^{2}}\int _{0}^\pi \cos[(2n+1)x]+1 \, dx  \\ \\ 
= \frac{8}{\pi}\sum_{n=0}^\infty \frac{1}{(2n+1)^{2}}
\end{gather}
$$
the last term equals $\pi$ using example for from the same page. So we have
$$
\begin{gather}
\frac{\pi^{2}}{8}= \frac{1}{3^{2}}+\frac{1}{5^{2}}+\frac{1}{7^{2}}\dots
\end{gather}
$$
### Part 2

#### 1

##### a

Let's define a function $h$: $[0,5]$ where $h(x)=f(x)$. We know that $h(x)$ is a continuous periodic function on  closed interval, and as a result, it is uniformly continuous on $[0,5]$. Now let $M_{0}>0$. Then there exists $m>0$ such that 
$$
\begin{gather}
\lvert h(u)-h(v) \rvert<M_{0} \hspace{.5cm} \forall u,v \in [0,2],\lvert u-v \rvert<m
\end{gather}
$$
If we have $x,y \in\mathbb{R}$ such that $\lvert x-y \rvert<m$, then there exists $u,v \in[0,2]$ such that $\lvert u-v \rvert<m$ and $x-u,y-v\in\mathbb{Z}$. So if we have that $f(x)=h(u)$ and $f(y)=h(v)$ then we have
$$
\begin{gather}
\lvert (f(x)-f(y)) \rvert \rightarrow \lvert C_{n}(f) \rvert < M_{0}
\end{gather}
$$

