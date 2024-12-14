#### 10.3.2

We're told to verify the first six entries of the table on page 276 of Strauss. We have the equation

$$
\begin{gather}
Y_{l}^m (s) = P_{l}^m\dots
\end{gather}
$$
where, as per Strauss, we ignore the $\cos\theta e^{ i m\phi }$ term. Thus $Y$ reduces to the Eigenfunction of the associated Legendre equation which equals, 
$$
\begin{gather}
P_{l}^m(s)e^{ im\phi } = \frac{(-1)^m}{2^ll!}(1-s^{2})^{m/2} \frac{d^{l+m}}{ds^{l+m}}[(s^{2}-1)^l]
\end{gather}
$$
We begin with  $l,m=0$
$$
\begin{gather}
P_{0}^0(s)\underbrace{ e^{ i (0)\phi } }_{ 1 } = \frac{(-1)^0}{2^0 0!}(1-s^{2})^{0/2} \frac{d^{l+0}}{ds^{0}}[(s^{2}-1)^0] = \frac{1}{1}(1-s^{2})[(s^{2}-1)^0] = \boxed{1}
\end{gather}
$$
next $l=1,m=0$
$$
\begin{gather}
P_{1}^0(s) \underbrace{ e^{ i (0)\phi } }_{ 1 }= \frac{(-1)^0}{2^1 1!}(1-s^{2})^{0} \frac{d^{1}}{ds^{1}}[(s^{2}-1)^1] = \frac{1}{2}(1)(2s) = s = \cos\theta
\end{gather}
$$
next $l=1,m=\pm 1$
$$
\begin{gather}
P_{1}^{\pm1}(s)e^{ \pm i \phi } =\left[  \frac{(-1)^{\pm1}}{2}(1-s^{2})^{\pm1/2} \frac{d^{1\pm1}}{ds^{1\pm1}}[(s^{2}-1)^1]  \right]e^{  \pm i\phi }\\ \\ 
\begin{cases}
m=1 \hspace{.5cm}\left[  \left( -\frac{1}{2} \right)(1-s^{2})^{1/2}2 \right]e^{ i\phi } = -\sin(\theta)(\cos \phi+i\sin \phi) \sim \boxed{\sin(\theta)\cos \phi \hspace{.2cm}\text{and}\hspace{.2cm}\sin(\theta)\sin (\phi)} \\ \\

m=2 \hspace{.5cm}\left[  \left( -\frac{1}{2} \right) \sqrt{ \sin ^{2}(\theta) } \right]e^{ -i\phi } = \frac{\sin(\theta)}{2}(\cos(\phi)-i\sin (\phi)) = \boxed{\sin(\theta)\cos \phi \hspace{.2cm}\text{and}\hspace{.2cm}\sin(\theta)\sin (\phi)}
\end{cases}
\end{gather}
$$

The math seems sketchy, but we ignored the constants that Strauss told us to just before the table on 276. For instance, for $m=\pm 1$ we ignored the $i$ constant in our final boxed answers. We also ignored the negative on the $\sin$ for $m=1$ on the second stem and the $\frac{1}{2}$ for the second step, as well as the negative on the $i\sin(\phi)$ term. This will continue to happen throughout the rest of the terms in the table. We proceed with $l=2, m=0$
$$
\begin{gather}
P_{2}^0(s)e^{ i0\phi } = \frac{(-1)^0}{2^22!}(1-s^{2})^{0/2} \frac{d^{2}}{ds^{2}}[(s^{2}-1)^2] \\ \\ 
= \frac{1}{8}(12s^{2}-4) = \frac{3}{2}s^{2}-\frac{1}{2} \rightarrow \cancel{ \frac{1}{2} }(3s^{2}-1)\rightarrow 3\cos ^{2}\theta -1
\end{gather}
$$
Next we have $l=2,m=\pm 1$
$$
\begin{gather}
P_{2}^1(s)e^{ i\phi } = \frac{-1}{8}(1-s^{2})^{1/2}(24s)(\cos \phi+i\sin \phi) \\ \\ = \cancel{ -3 }s(1-s^{2})^{1/2} (\cos \phi+i\sin \phi) = \cos\theta \sin\theta((\cos \phi+\cancel{ i\sin \phi }))  \\ \\
=\cos\theta \sin\theta \cos \phi \\ \\ 
P_{2}^{-1} e^{ -i\phi }= \frac{1}{8}(1-s^{2})^{-1/2}(4s^{3}-4s)(\cos \phi+i\sin \phi) \\ \\  \rightarrow(1-s^{2})^{-1/2}(\cos^3\theta-\cos\theta)(\cos \phi+i\sin \phi)= \\ \\ \frac{1}{\sin\theta} \cos\theta(\cos ^{2}\theta-1)(\cos \phi+i\sin \phi) = \frac{1}{\sin\theta} \cos\theta \sin ^{2}\theta(\cos \phi+\cancel{ i\sin \phi })  \\ \\
=\cos\theta \sin\theta \cos \phi
\end{gather}
$$
For this last bit, we can just omit the $\frac{(-1)^m}{2^ll!}$ piece. We technically could have omitted it in for all the rest of the terms but it's too late now. We now have $l=2,m=\pm2$
$$
\begin{gather}
P_{2}^2e^{ 2i\phi } = (1-s^{2})*\cancel{ (24) }*(\cos 2\phi+i\sin 2\phi) = \sin ^{2}\theta(\cos 2\phi+2i\sin 2\phi) \\ \\ =\sin ^{2}\theta \cos 2\phi\cancel{ +\sin ^{2}\theta(2i\sin 2\phi) } \\ \\ 
P_{2}^{-2} e^{ -2i\phi } =\frac{1}{(1-s^{2})}(s^{4}-2 s^{2}+1 )(\cos 2\phi-i\sin 2\phi)  \\ \\ =\frac{1}{\sin ^{2}\theta}\sin^4\theta(\cos 2\phi-i\sin 2\phi) = \sin ^{2}\theta(\cos 2\phi-i\sin 2\phi) \\ \\ 
=\sin ^{2}\theta \cos(2\phi)
\end{gather}
$$
#### 10.3.10

A harmonic function satisfies the differential equation $\triangle v  = 0$ in the ball where $\lambda =0$. Because $\lambda$ is missing, our $R(r)$ equation in $v$ is of the Euler type with solution (with the aid of equation (25) on page 277), 
$$
\begin{gather}
R(r) = r^\alpha
\end{gather}
$$
where $\alpha^{2}-\alpha-\gamma=0$. For our $Y(\theta,\phi)$ component, we have the condition that $\gamma = l(l+1)$ for $Y_l^m(\theta,\phi)$. So thus we have $\alpha=-l-1$. Since we're interested in the harmonic solution outside of the ball, we reject the positive root $\alpha=l$. The solution to the laplacian is thus
$$
\begin{gather}
u= \sum_{l=0}^\infty \sum_{m=-l}^l A_{lm} r^{-l-1}P_{l}^m (\cos\theta)e^{ i m\phi }
\end{gather}
$$
We now seek to find the coefficient $A_{lm}$. We take the derivative and evaluate when $r=a$, or the boundary. Thus, our solution becomes, 
$$
\begin{gather}
\frac{ \partial u }{ \partial r } (a,\theta ,\phi) = \sum_{l=0}^\infty \sum_{m=-l}^lA_{lm}(-l-1)a^{-l-2}P_{l}^m(\cos\theta)e^{ im\phi } = -\cos\theta
\end{gather}
$$
Now, let's say that we have some set value of $m$. Then our solution becomes, 
$$
\begin{gather}
\frac{ \partial u }{ \partial r } (a,\theta,\phi)= \sum_{l=\lvert m \rvert}^\infty\underbrace{  A_{lm}(-l-1)a^{-l-2}P_{l}^me^{ i m\phi } }_{ \text{function of} \hspace{.2cm}\theta,\phi } =\underbrace{ -(P_{1}^0 (\cos\theta)) }_{ \theta }
\end{gather}
$$
we can rewrite the right side of the equation so that it equals, 
$$
\begin{gather}
-(P_{1}^0\cos(\theta)e^{ i(0)\phi }+0*P_{l}^m \cos(\theta)e^{ i m \phi })
\end{gather}
$$
Thus we know that for $m\neq 0,\mathbb{Z}$ along with $l \neq 1, \in\mathbb{N}$, that the solution $\frac{ \partial u }{ \partial r } (a,\theta,\phi)=0$. Thus we utilize the solution when $l=1,m=1$

$$
\begin{gather}
\frac{ \partial u }{ \partial r } (a,\theta,\phi) = A_{1,0}(-2)a^{-3} \cos\theta = -\cos\theta \\ \\ 
A_{1,0} = \frac{a^{3}}{2}
\end{gather}
$$
Thus our final solution for $u$ is, 
$$
\begin{gather}
u = \frac{a^{3}}{2}*\left( \frac{1}{r^{2}} \right)\cos\theta = \frac{a}{2r^{2}}\cos\theta
\end{gather}
$$


#### 10.5.5

We have that if $u$ satisfies Bessel's equation, we show that $v = z^\alpha u(\lambda z^\beta)$ satisfies, 
$$
\begin{gather}
v'' + \frac{1-2\alpha}{z}v'+\left[ (\lambda\beta z^{\beta-1})^{2}-\frac{s^{2}\beta^{2}-\alpha^{2}}{z^{2}} \right]v = 0
\end{gather}
$$
Let's assume that $u$ satisfies Bessel's differential equation, or equation (1) in chapter 10.5. We first start off by finding the first and second derivatives of $v$. Then we'll expand some of the terms into the differential equation above.  Finally, we can plug them back into this equation, 
$$
\begin{gather}
v = z^\alpha u(\lambda z^\beta) \\ \\ 
v' = \alpha z^{\alpha-1}u(\lambda z^\beta) +z^\alpha (\beta\lambda z^{\beta-1})u'(\lambda z^\beta) \\ \\ 
v''= \cancel{ \alpha^{2}z^{\alpha-2}u(\lambda z^\beta) }+\beta^{2}\lambda^{2} z^{\alpha+2\beta-2}u''(\lambda z^\beta)+\beta^{2}\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta) \\ \\ 
\cancel{ +2\alpha\beta\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta)-\beta\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta) - \alpha z^{\alpha-2}u(\lambda z^\beta) }
\end{gather}
$$
Now that we have the derivatives, let's take the the second term in the differential equation $v'$ and it's attached coefficient
$$
\begin{gather}
\frac{1-2\alpha}{z}v' =\frac{1-2\alpha}{z} (\alpha z^{\alpha-1}u(\lambda z^\beta) +z^\alpha (\beta\lambda z^{\beta-1})u'(\lambda z^\beta))
 \\ \\ =  \cancel{ -2\alpha\beta\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta)+\beta\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta) }-2\alpha^{2}z^{\alpha-2}u(\lambda z^\beta)+\cancel{ \alpha z^{\alpha-2}u(\lambda z^\beta)  }
\end{gather}
$$

Immediately, we notice that in the first two terms of our differential equation many terms cancel. Our differential equation is thus
$$
\begin{gather}
\beta^{2}\lambda^{2} z^{\alpha+2\beta-2}u''(\lambda z^\beta)+\beta^{2}\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta)-\alpha^{2}z^{\alpha-2}u(\lambda z^\beta)+\left[ (\lambda\beta z^{\beta-1})^{2}-\frac{s^{2}\beta^{2}-\alpha^{2}}{z^{2}} \right]v
\end{gather}
$$

,The next term we'll write out is, 
$$
\begin{gather}
\left[ (\lambda\beta z^{\beta-1})^{2}-\frac{s^{2}\beta^{2}-\alpha^{2}}{z^{2}} \right] * z^\alpha u(\lambda z^\beta)  \\ \\
=-\beta^{2}s^{2}z^{\alpha-2}u(\lambda z^\beta)+\alpha^{2}z^{\alpha-2}u(\lambda z^\beta) +\beta^{2}\lambda^{2}z^{\alpha+2\beta-2}u(\lambda z^\beta)
\end{gather}
$$
Now out original differential equation reduces to
$$
\begin{gather}
\beta^{2}\lambda^{2} z^{\alpha+2\beta-2}u''(\lambda z^\beta)+\beta^{2}\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta)\cancel{ -\alpha^{2}z^{\alpha-2}u(\lambda z^\beta)  }\\ \\ -\beta^{2}s^{2}z^{\alpha-2}u(\lambda z^\beta)+\cancel{ \alpha^{2}z^{\alpha-2}u(\lambda z^\beta) } +\beta^{2}\lambda^{2}z^{\alpha+2\beta-2}u(\lambda z^\beta) = \\ \\ 

\beta^{2}\lambda^{2} z^{\alpha+2\beta-2}u''(\lambda z^\beta)+\beta^{2}\lambda z^{\alpha+\beta-2}u'(\lambda z^\beta)-\beta^{2}s^{2}z^{\alpha-2}u(\lambda z^\beta)+\beta^{2}\lambda^{2}z^{\alpha+2\beta-2}u(\lambda z^\beta)
\end{gather}
$$
Now, we'll divide the very last line by the coefficient on the $u''$ term, 
$$
\begin{gather}
u''(\lambda z^\beta)+\frac{1}{\lambda z^\beta}u'(\lambda z^\beta)+\left( 1-\frac{s^{2}}{\lambda^{2}z^{2\beta}} \right)u
\end{gather}
$$
Assume for a moment that $\lambda z^\beta=d$, then our equation becomes 
$$
\begin{gather}
u''(d)+\frac{1}{d}u'(d)+\left( 1-\frac{s^{2}}{d^{2}} \right)u
\end{gather}
$$
which satisfies our original Bessel's differential equation and equals zero! Thus we've shown when $v = z^\alpha u(\lambda z^\beta)$, then
$$
\begin{gather}
v'' + \frac{1-2\alpha}{z}v'+\left[ (\lambda\beta z^{\beta-1})^{2}-\frac{s^{2}\beta^{2}-\alpha^{2}}{z^{2}} \right]v = u''(d)+\frac{1}{d}u'(d)+\left( 1-\frac{s^{2}}{d^{2}} \right)u =0
\end{gather}
$$
Our proof is complete!

#### 10.6.4

We show that the following is true,
$$
\begin{gather}
\int _{-1}^1 x^{2}P_{l}(x) \, dx =0
\end{gather}
$$
In general, we know the integral will always be zero when, 
$$
\begin{gather}
\int _{-1}^1 x^{n-1}P_{l}(x) \, dx \hspace{.5cm}l\geq n
\end{gather}
$$
This is because the the value of $P_{l}(x)$ will always have a degree higher than our $x$ term. As a result, the integral from $-1\leq x\leq 0$ and $0\leq x\leq-1$ will always be equal. Thus their subtraction will always be zero. Let's take a few test terms of the first integral to check, 
$$
\begin{gather}
\int _{-1}^1 x^{2}P_{2}(x) \, dx = \frac{1}{2}\left( \frac{3x^5}{5}-\frac{x^{3}}{3} \right)|_{-1}^{1} = .27 \\ \\ 
\int _{-1}^1 x^{2}P_{3}(x) \, dx = \frac{1}{2}\left( \frac{5x^6}{6}-\frac{3x^4}{4} \right) =0\\ \\
\int _{-1}^1 x^{2}P_{4}(x) \, dx =\frac{1}{8}(5x^7-6x^5+x^{3})=0
\end{gather}
$$
As visible by the integrals, when the coefficient of $x$ is $\geq 3$, the integral equals zero. 

#### 10.6.5

We find the values of $a_{l}$ given that from the values $(-1,0)$, $f(x)=0$ and $(0,1)$, $f(x) = x$ where we have, 
$$
\begin{gather}
f(x) = \sum_{l=0}^\infty a_{l}P_{l}(x)
\end{gather}
$$
we now take the case when $(-1,0)$, 
$$
\begin{gather}
f(x) = \sum_{l=0}^\infty a_{l}P_{l}(x) = 0*P_{l}(x) \\ \\ 
a_{l} = 0
\end{gather}
$$

Thus in the case when $(0,1)$ we have
$$
\begin{gather}
f(x) = \sum_{l=0}^\infty a_{l}P_{l}(x) = x \\ \\ 
f(x) = \sum_{l=0}^\infty a_{l}P_{l}(x) = P_{1}(x)  \\ \\ 
f(x) = \sum_{l=0}^\infty a_{l}P_{l}(x) = P_{1}(x) +\underbrace{ 0*P_{l}(x) }_{ l \neq 1,\in \mathbb{N} }
\end{gather}
$$
Thus we see that $f(x)$ is zero unless $l=1$ in such case we have, 
$$
\begin{gather}
f(x) = a_{1}P_{1}(x) =P_{1}(x) \\ \\
a_{1}=1
\end{gather}
$$
Now we recover our coefficient at the origin or when $x=0$, 
$$
\begin{gather}
f(0)=\sum_{l=0}^\infty a_{l}P_{l}(0) = 0
\end{gather}
$$
Looking closely, we notice that for values of $P_{l}(0)$, when $l$ is odd, all the terms have an $x$ in them, and if $x=0$, then $P_{l}(0)=0$. If we have $l$ as even, $P_{l}(0)\neq 0$, as there is always a constant term at the end. Since $P_{l}(0)$ can be both zero and non-zero, to make the $f(0)=0$, then $a_{l}=0$ must be true. Thus we conclude. 
$$
\begin{gather}
\begin{cases}
a_{l} =0 \hspace{.5cm}(-1,0) \\
a_{l} =0 \hspace{.5cm}(0) \\
a_{1} = 1 \hspace{.5cm}(0,1) \\
 a_{l \neq 1, \in \mathbb{N}} =0 \hspace{.5cm}(0,1)
\end{cases}
\end{gather}
$$
#### 10.6.6

We find $u$ in the ball where $r<a^{3}$ when $u(a,\theta,\phi) = \cos ^{2}\theta$. Similar to our work in 10.3.10 we know the general solution is
$$
\begin{gather}
u= \sum_{l=0}^\infty \sum_{m=-l}^l A_{lm} r^{l}P_{l}^m (\cos\theta)e^{ i m\phi }
\end{gather}
$$
where we reject the negative root $\alpha=-l-1$ which would lead to a singularity at the origin. Now we find the coefficient $A_{lm}$ using the boundary conditions, 
$$
\begin{gather}
u(a,\theta,\phi) = \sum_{l=0}^\infty \sum_{m=-l}^l A_{lm} a^{l}P_{l}^m (\cos\theta)e^{ i m\phi }=\cos ^{2}\theta
\end{gather}
$$
Let's say we know the specific value of $m$, then $u$ becomes, 
$$
\begin{gather}
u(a,\theta,\phi) = \sum_{l=\lvert m \rvert}^\infty A_{lm}a^l P_{l}^m(\cos\theta)e^{ i m\phi } = \cos ^{2}\theta \\ \\ 
\end{gather}
$$
we notice that the middle equation is in terms of $\theta,\phi$ and the right hand side is only in terms of $\theta$. Thus we can rewrite solution as , 
$$
\begin{gather}
 \sum_{l=\lvert m \rvert}^\infty A_{lm}a^l P_{l}^m(\cos\theta)e^{ i m\phi } = (P_{1}(\cos\theta))^{2}e^{ i(0)\phi }+0*e^{ i m\phi }
\end{gather}
$$
Thus we have that $l=1,m=0$. Thus we have, 
$$
\begin{gather}
u(a,\theta,\phi) = A_{l,0}a\cos\theta=\cos ^{2}\theta \\ \\ 
A_{l,0} = \frac{\cos\theta}{a}
\end{gather}
$$
thus our final solution is,
 $$
\begin{gather}
u(r,\theta,\phi) = \frac{r}{a}\cos ^{2}\theta
\end{gather}
$$