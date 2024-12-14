#### 2.36
##### Part 1

To understand if the center charge can escape the cube, we first need to the potential $\phi$ on the particle by all the other particles. We'll call our center particle WALL-E (like the movie). Let's draw a picture: 
![[Pasted image 20240207163131.png|center|500]]


Since potential energy is a scalar quantity and the path of WALL-E is restricted to the $x,y$ plane ($x_{1}$ for some $x$ on the line), we can make the potential energy function only of $x$. That is:
$$
\begin{gather}
\phi(x) = -\sum_{i=1}^8 k \frac{q_{i}}{r(x)}
\end{gather}
$$
where $0<x<\sqrt{ 2 }$. Let's begin our adventure with WALL-E at charge $q_{1}$. For symmetrical reasons, the potential due to charges $q_{3},q_{5},q_{7}$ are the same as $q_{1}$ (same distance from WALL-E as it approaches the midpoint of the designated edge)

![[Pasted image 20240207164537.png|center|500]]

Given our graph above: we have that $q_{2}$: 
$$
\begin{gather}
\phi_{q_{1},W} = \frac{kq_{1}}{\sqrt{ \left( 3 \right)+x^{2} }}
\end{gather}
$$
Thus the potential for $q_{1},q_{3},q_{5},q_{7}$ is:
$$
\begin{gather}
\phi_{q_{1},q_{3},q_{5},q_{7},W} = \frac{4kq_{1}}{\sqrt{3+x^{2} }}
\end{gather}
$$
##### Part 2
Now, with the same symmetry purposes, we'll calculate $\phi_{4}$ which will also give us $\phi_{8}$: 

![[Pasted image 20240207183930.png|center|500]]

Thus the potential for $q_{4}, q_{8}$ is:
$$
\begin{gather}
\phi_{q_{4},q_{8},W} = \frac{2kq_{1}}{\sqrt{ (\sqrt{ 2 }-x)^{2}+1 }}
\end{gather}
$$
##### Part 3
Lastly, with our nice symmetry argument $q_{2},q_{6}$:

![[Pasted image 20240207184442.png|center|500]]
 
$$
\begin{gather}
\phi_{q_{2},q_{6},W} = \frac{2kq_{1}}{\sqrt{ 1+\left( {\sqrt{ 2 }} +x \right)^{2} }}
\end{gather}
$$

##### Part 4
Thus the total potential is: 
$$
\begin{gather}
\phi(x) =  \frac{4kq_{1}}{\sqrt{ \left( 3 \right)+x^{2} }} + \frac{2kq_{1}}{\sqrt{ (\sqrt{ 2 }-x)^{2}+1 }} +\frac{2kq_{1}}{\sqrt{ 1+\left( {\sqrt{ 2 }} +x\right)^{2} }}
\end{gather}
$$
We'll graph this, but we'll leave out some constants.

$$
\begin{gather}
\phi(x) =  \frac{4}{\sqrt{ \left( 3 \right)+x^{2} }} + \frac{2}{\sqrt{ (\sqrt{ 2 }-x)^{2}+1 }} +\frac{2}{\sqrt{ 1+\left( {\sqrt{ 2 }} +x \right)^{2} }}
\end{gather}
$$
![[Pasted image 20240207191219.png|center]]

Since the electric field points below the purple function, the charge cannot escape 
#### 2.37

Since this is a decently simple problem, there won't be any figures/pictures included! We note that the electric field of a sphere that has a boundary uniform charge distribution which can be examined as if it were a point charge. Thus we have that: 
$$
\begin{gather}
E = \frac{kQ}{r^{2}}
\end{gather}
$$
where we've been told that $Q=1C$, and from NASA's fact sheet, we have that $r=6378\cdot 10^{3}m$. Then, the electric field is just: 
$$
\begin{gather}
E = \frac{k(1C)}{(6378\cdot 10^{3}m)^{2}}
\end{gather}
$$
The potential, in this case, is how strong a charge from $\infty$ would be pulled towards from the uniform shell. Thus our integral is 
$$
\begin{gather}
\phi = - \int _{\infty}^{6378\cdot 10^{3}} \frac{k}{r^{2}} \, dr = -\frac{k}{r}|_{\infty}^{6378\cdot 10^{3}} = -\frac{k}{6378\cdot 10^{3}}\left( \frac{C}{m} \right)
\end{gather}
$$

#### 2.42
##### (a)

We'll want to find the electric field inside the cylinder using flux from Gauss's law. We have that:
$$
\begin{gather}
\oint E\cdot \, da = 2\pi rlE = \frac{Q}{\epsilon_{0}} \\ \\ 
E(r) = \frac{Q(r)}{2\pi rl\epsilon_{0}}
\end{gather}
$$
We now find the the charge $Q(r)$ inside the sphere 
$$
\begin{gather}
Q = \rho \underbrace{ \pi r^{2} l }_{ \text{vol of cyl} \hspace{.2cm} }
\end{gather}
$$
Thus, we have that for the inside of the cylinder, the electric field using Gauss's Law is:
$$
\begin{gather}
\frac{\rho r^{2} \pi l}{2\pi rl\epsilon_{0}}= \frac{\rho r}{2\epsilon_{0}}
\end{gather}
$$
Which is consistent with Purcell. 
##### (b)
We've confirmed the field inside due to Gauss's law is $\frac{\rho r}{2\epsilon_{0}}$. We'll take this value of the field and integrate it to find the potential. Once we have that we'll use the known value for the electric field outside of the cylinder. Thus
$$
\begin{gather}
 \phi_{in} = -\int_{0}^{R_{1}} \frac{\rho r}{2\epsilon_{0}} \, dr = -\frac{\rho}{2\epsilon_{0}} \int _{0}^{R_{1}} r \, dr = - \frac{\rho R_{1}^{2}}{4\epsilon_{0}} \\ \\ 

\phi_{out} = -\int \frac{\rho a^{2}}{2\epsilon_{0}r} \, dr  = -\frac{\rho a^{2}}{2\epsilon_{0}} \int _{R_{1}}^{R_{2}} \frac{1}{r} \, dr = -\frac{\rho a^{2}}{2\epsilon_{0}}[\ln(R_{2})-\ln(R_{1})] \\ \\ 
\end{gather}
$$
Thus the function $\phi(r)$ is:

$$
\begin{gather} \phi
\begin{cases}
\frac{\rho R_{1}^{2}}{4\epsilon_{0}} \hspace{.5cm} 0 \rightarrow R_{1} \\
\phi_{in}+ \frac{\rho a^{2}}{2\epsilon_{0}}[\ln(R_{2})-\ln(R_{1})] \hspace{.5cm} R_{1}\rightarrow R_{2}
\end{cases}

\end{gather}
$$
#### 2.43

![[Pasted image 20240209001937.png|center|300]]

The electric field of a rod can be modeled by: 
$$
\begin{gather}
E = \frac{\lambda}{2\pi \epsilon_{0}r} 
\end{gather}
$$
Thus we'll integrate this: 
$$
\begin{gather}
k\lambda \int _{d}^{-d}  \frac{1}{(2d-z)}\, dx =  k\lambda \ln(2d-z)|_{d}^{-d}  = k\lambda \ln(3)\\ \\ 

\end{gather}
$$
For the second part of this question, we have that:

$$
\begin{gather}
\phi = k\Lambda \int _{-d}^d \frac{dz}{\sqrt{ z^{2} +x^{2}}} \, = k\lambda \ln\left[ \sqrt{ \left( \frac{z^{2}}{x^{2}}+1 \right) } + \frac{z}{x} \right] |_{-d} ^{d} \\ \\

\lambda k\ln\left[ \frac{\sqrt{ \left( \frac{z^{2}}{x^{2}}+1 \right) } + \frac{z}{x}}{\sqrt{ \left( \frac{z^{2}}{x^{2}}+1 \right) } - \frac{d}{x}} \right]
\end{gather}
$$
In order to cancel out square roots, we multiply the top and the bottom of the stuff inside the $\ln$ by $\sqrt{ \left( \frac{z^{2}}{r^{2}}+1 \right) }+\frac{z}{x}$. Thus  the last math line becomes: 
$$
\begin{gather}
\ln\left( \left( \frac{2d^{2}}{x^{2}}-\frac{2d}{x}\sqrt{ \frac{d^{2}}{x^{2}}+1 }+1 \right)^{-1} \right) = \ln(3) \\ \\ 

\left( \left( \frac{2d^{2}}{x^{2}}-\frac{2d}{x}\sqrt{ \frac{d^{2}}{x^{2}}+1 }+1 \right)^{-1} \right) = 3 \\ \\

 \left( \frac{2d^{2}}{x^{2}}-\frac{2d}{x}\sqrt{ \frac{d^{2}}{x^{2}}+1 }+1 \right) = \frac{1}{3} \\ \\ 

-\frac{1}{3} = \frac{d^{2}}{x^{2}} - \frac{d}{x}\sqrt{ \frac{d^{2}}{x^{2}}+1 } \hspace{.5cm} \rightarrow a = \frac{d}{x} \\ \\ 

-\frac{1}{3} = a^{2}-a\sqrt{ a^{2}+1 } \\ \\ 

a^4 + \frac{2a^{2}}{3}+\frac{1}{9}= a^{2}(a^{2}+1) \\ \\ 

a^4 + \frac{2a^{2}}{3} +\frac{1}{9} = a^4 + a^{2} \\ \\ 

-\frac{a^{2}}{3} +\frac{1}{9} = 0 \\ \\ 

a^{2} = \frac{1}{3} \\ \\ 

a = \sqrt{ \frac{1}{3} } \\ \\ 

x = \frac{d}{\sqrt{ \frac{1}{3} }} \\ \\ 
x = d\sqrt{ \frac{9}{3} } = d\sqrt{ 3 }

\end{gather}
$$
thus, including the constants now, $x = k\lambda d\sqrt{ 3 }$ which is the same result as before. 

#### 2.44
![[Pasted image 20240210005835.png|center|300]]

The integral: 

$$
\begin{gather}
k\lambda \int _{d}^d \frac{1}{;\sqrt{ (z-d)^{2}+\left( \frac{3x}{2} \right)^2 }}\, dz = k\lambda\ln\left( \sqrt{ (z-d)^{2}+\left( \frac{3x}{2} \right)^{2} }-(z-d) \right) = k\Lambda\ln(3) \\ \\ 

\lambda k\left[ \left( \ln\left( \frac{3d}{2} \right)-\ln\left( \sqrt{ 4d^{2} +\frac{9d^{2}}{4} }-2d \right) \right) \right] = \lambda k\ln(3) \\ \\ 
\lambda k\left[ \ln\left( \frac{3d}{2} \right)-\ln\left( \frac{5d}{2}-2d \right) \right] \\ \\ 

\lambda k\left( \frac{\left( \frac{3d}{2} \right)}{\frac{d}{2}} \right) = \lambda k \ln(3)
\end{gather}
$$
For the second part of the question we have:

![[Pasted image 20240210011214.png|center|300]]

$$
\begin{gather}
\frac{\lambda}{4\pi\epsilon_{0}}\ln\left( \frac{\sqrt{ (z_{0}+d)^{2}+x_{0} }+z_{0}-d}{\sqrt{ (z_{0}+d)^{2}+x_{0}^{2} }+z_{0}+d} \right) \\ \\ 

\frac{\lambda}{4\pi\epsilon_{0}}\ln\left( \frac{\sqrt{ z_{0}^{2}-2z_{0}+d^{2}+x_{0}^{2} }+z_{0}-d}{\sqrt{ z_{0}^{2}+2z_{0} + d^{2} +x^{2} }+ z_{0} +d} \right)
\end{gather}
$$
We have that the equation for a ellipse
$$
\begin{gather}
\frac{x^{2}}{a^{2}-d^{2}}+\frac{z^{2}}{a^{2}} = 1 \\ \\ 
x^{2}+z^{2}-\frac{z^{2}d^{2}}{a^{2}} = a^{2}-d^{2} \\ \\ 

x^{2}+z^{2}-\frac{z^{2}d^{2}}{a^{2}} = a^{2}-d^{2} \\ \\ 
x^{2}+z^{2}+d^{2} = \frac{z^{2}d^{2}}{a^{2}} + a^{2} = \left( a\mp \frac{zd}{a} \right)^{2} \pm_{2}zd \\ \\ 
z^{2} + 2zd + d^{2} + x^{2} = \left( a \mp \frac{zd}{a} \right)^{2} \\ \\ 
\frac{\lambda}{4\pi\epsilon_{0}}\ln\left( \frac{\left( \sqrt{ a+\frac{zd}{a} } \right)^{2}+z_{0} -d}{\left( \sqrt{ a-\frac{zd}{a} } \right) +z_{0}+d}  \right) \\ \\ 

\frac{\lambda}{4\pi\epsilon_{0}}\ln\left( \frac{(a-d)(a+z)}{(a+d)(a+z)} \right)  = \frac{\lambda}{4\pi\epsilon_{0}}\ln \left( \frac{a+d}{a-d} \right)
\end{gather}
$$

#### 2.50


![[Pasted image 20240210012750.png|center|300]]

The potential energy is the sum of the both of the potential energies:

$$
\begin{gather}
U = \frac{\epsilon_{0}}{2} \int E^{2} \, dv +\frac{\epsilon_{0}}{2}\int E^{2} \, dv \\ \\ 

\end{gather}
$$
We'll get the potential energy for the sphere of charge $q$ and then we can replace the q with $Q-q$ for the second: 
$$
\begin{gather}
\frac{\epsilon_{0}}{2}\int\left(  \frac{kq}{r^{2}} \right)^{2} \, dv = \frac{\epsilon_{0}}{2} \int \frac{k^{2}q^{2}}{r^4}4\pi r^{2} \, dr  \\ \\ 

\frac{\epsilon_{0}}{2}k^{2}q^{2}4\pi \int_{R_{1}}^\infty \frac{1}{r^{2}} \, dr  = -\frac{\frac{\epsilon_{0}}{2}4\pi q^{2}k^{2}1}{r}|_{R_{1}}^\infty \\ \\ 

-\frac{4\pi q^{2}k^{2}\epsilon_{0}}{2}\left( \frac{1}{\infty}-\frac{1}{R_{1}} \right) = \frac{2\pi q^{2}k^{2}\epsilon_{0}}{R_{1}}
\end{gather}
$$
Thus the potential energy combined is: 

$$
\begin{gather}
U = \frac{2\pi q^{2}k^{2}\epsilon_{0}}{R_{1}} + \frac{2\pi (Q-q)^{2}k^{2}\epsilon_{0}}{R_{2}}
\end{gather}
$$
Upon minimizing with respect to $q$, we have that 

$$
\begin{gather}
q = \frac{R_{1}Q}{(R_{2}+R_{1})} \\ \\ 
Q-q = Q - \left[ \frac{R_{1}}{R_{2}+R_{1}} \right] = \frac{QR_{2}}{R_{2}+R_{1}}
\end{gather}
$$
The potential difference should be the individual difference in potentials of the spheres: 

$$
\begin{gather}
\frac{kq}{R_{1}} - \frac{k(Q-q)}{R_{2}} \\ \\ 

\frac{\frac{k(QR_{1})}{R_{2}+R_{1}}}{R_{1}} - \frac{\frac{kQR_{1}}{R_{2}+R_{1}}}{R_{2}} = \frac{kQ}{R_{2}+R_{1}}  -\frac{kQ}{R_{2}+R_{1}} = 0
\end{gather}
$$
We're all done!

#### 2.56
![[Pasted image 20240210020657.png|center|300]]

We build up the sphere from 0 to $a$ where the amount of work to add a new spherical shell is 
$$
\begin{gather}
dw =dq\phi_{\text{shell} \hspace{.2cm}} 
\end{gather}
$$
where $\phi_{\text{shell} \hspace{.2cm}}$ has been provided from equation 2.30. To find the total work, we'll integrate the last math line: 

$$
\begin{gather}
W = \frac{\sigma}{\pi\epsilon_{0}}\int _{0}^a \sigma^2\pi^{r} \, dx \hspace{.5cm} \sigma=. \frac{Q}{\pi r^{2}} \\ \\ 

\frac{\sigma}{\pi\epsilon_{0}}\int _{0}^a \sigma^2\pi r^{2} \, dx = \frac{\sigma^{2}2\pi}{\pi\epsilon_{0}} \frac{r^{3}}{3}|_{0}^a \\ \\ 

\frac{\sigma^{2}2\pi}{\pi\epsilon_{0}}  \frac{a^{3}}{3} \\ \\ 

\frac{2\sigma^{2}a^{3}}{3\epsilon_{0}} = \frac{2\left( \frac{Q^{2}}{\pi^{2}a^4} \right)a^{3}}{3\epsilon_{0}} = \frac{2Q^{2}}{3\pi^{2}a\epsilon_{0}}
\end{gather}
$$
We've arrived at the same answer as Purcell. Let's compare this to building up a hollow spherical sphere with uniform charge. These hollow spheres can be though of as point charges. Let's calculate U
$$
\begin{gather}
U = \frac{\epsilon_{0}}{2} \int _{a}^\infty \left( \frac{kQ}{r^{2}} \right)^{2} 4\pi r^{2} \, dr = \frac{k^{2}Q^{2}\epsilon_{0}4\pi}{2}\int _{a}^\infty \frac{1}{r^{2}} \, dr \\ \\ 

\frac{k^{2}Q^{2}\epsilon_{0}4\pi}{2}\left( -\left[ 0-\frac{1}{a} \right] \right) \\ \\ 

\frac{4\pi\epsilon_{0}k^{2}Q^{2}}{2a} = \frac{\frac{4\pi\epsilon_{0}}{(4\pi\epsilon_{0})^{2}}Q^{2}}{2a} = \frac{\frac{Q^{2}}{4\pi\epsilon_{0}}}{2a} = \frac{Q^{2}}{8\pi\epsilon_{0}a}
\end{gather}
$$
Upon comparing, the energy stored in the electric field of a charge disk is 1/$\begin{gather}\frac{12\epsilon_{0}a}{3\pi}\end{gather}$ the energy required to build up a sphere with hallow shells of uniform density


#### 2.74

##### a

We have the following picture:

![[Pasted image 20240209214103.png|center|300]]

We're also told that for $z>0\hspace{.5cm} \phi=\phi_{0}e^{ -kz }\cos(kx)$. Laplacian's equation exclaims that $\nabla^{2}\phi = 0$. Thus we'll use the equation for $\phi$ and take the gradient twice
$$
\begin{gather}
\nabla: \hspace{.5cm} \left( \frac{ \partial  }{ \partial x }  ,\frac{ \partial  }{ \partial y } ,\frac{ \partial  }{ \partial z } \right)(\phi_{0}e^{-kx)}\cos(kx)) \\ \\  \\ 

= -\phi_{0}e^{ -kz }\sin(kx) - \phi_{0}ke^{ -kz }\cos(kx) \\ \\ \\ 

\nabla^{2}: \left( \frac{ \partial^{2} }{ \partial x^{2} } ,\frac{ \partial^{2} }{ \partial y^{2} },\frac{ \partial  }{ \partial z^{2} }  \right) \\ \\ \\ 

-\phi_{0}e^{ -kz }\cos(kx)+\phi_{0}k^{2}e^{ -kz }\cos(kx) = 0
\end{gather}
$$
Thus we've proven that Laplacian's equation applies.

##### b

We'll notice that we've already found the $E$, the electric field as, $E=-\nabla \phi$. Thus the electric field should be: 
$$
\begin{gather}
E = -\nabla \phi = -[-\phi_{0}e^{ -kz }\sin(kx),0,-\phi_{0}ke^{ -kz }\cos(kx)]
\end{gather}
$$
This looks like: 

![[Pasted image 20240209222126.png|600]]
3-dimensionally, it's this sheet, but constant in the y-direction
##### c

Since the sheet has charge only on the $xy-$plane, we shouldn't see any charge distributed above the surface of the sheet. That is the charge is only distributed in the $xy-$plane. This turns our Electric field into
$$
\begin{gather}
E  = [\sin(kz),0,\cos(kx)] \\ \\
\end{gather}
$$
We note for a sheet charge that 
$$
\begin{gather}
Q = E_{8}\pi^{2}x^{2}\epsilon_{0}\\ \\ 

Q = x^{2}(\sin x+\cos x)
\end{gather}
$$
Where we've annoyed unnecessary constants for an easier graphing process. This produces the following charge distribution along the $xy-$plane:
![[Pasted image 20240209224204.png|center|400]]
#### 2.78

##### a

We want to show that $div(\nabla \times A) = 0$. We'll say that $\vec{A} = (A_{1},A_{2},A_{3})$. We'll first start of by finding $\nabla \times A$:

$$
\begin{gather}
\nabla \times A = \begin{pmatrix}
\hat{i} & \hat{j} & \hat{k} &  \\
\frac{ \partial  }{ \partial x } &\frac{ \partial  }{ \partial y }  &\frac{ \partial  }{ \partial z }  \\
A_{1} & A_{2} & A_{3} \end{pmatrix} = \\ \\ 
\left[ \frac{ \partial A_{3} }{ \partial y } - \frac{ \partial A_{2} }{ \partial z }  \right] \hat{i}-\left[ \frac{ \partial A_{3} }{ \partial x } - \frac{ \partial A_{1} }{ \partial z } \right]\hat{j} + \left[ \frac{ \partial A_{2} }{ \partial x } -\frac{ \partial A_{1} }{ \partial y }  \right]\hat{k} \\ \\ 
\end{gather}
$$
Now, we take the $div$ of that answer
$$
\begin{gather}
\underbrace{ \left( \frac{ \partial A_{3} }{ \partial x\partial y } -\frac{ \partial A_{3} }{ \partial y\partial x }   \right) }_{ 0 }-\underbrace{ \left( \frac{ \partial A_{2} }{ \partial x\partial z } -\frac{ \partial A_{2} }{ \partial x \partial y }  \right) }_{ 0 }+ \underbrace{ \left( {\frac{ \partial A_{1} }{ \partial y \partial z} } - \frac{ \partial A_{1} }{ \partial y \partial z }  \right) }_{ 0 } \\ \\ 
=0
\end{gather}
$$
##### b

Let's first assume that 
$$
\begin{gather}
\vec{F} = \nabla  \times A \\ \\
\end{gather}
$$
if we take the integrals $\iint (F) \cdot \, \vec{d}s$ over a closed surface we can implement Gauss's Law: 
$$
\begin{gather}
\iint F \, \vec{d}S = \iiint \nabla \cdot F dW
\end{gather}
$$
Where the triple integral is a volume. Next we have that: 

$$
\begin{gather}
\iiint\nabla \cdot\vec{F} dW = \iint_{S_{1}} F\cdot \, ds + \iint_{S2} F\cdot \, ds 
\end{gather}
$$
Now we'll notice using Stokes, that the very last integral is just the negative of the first. As a result:

$$
\begin{gather}
\iiint\nabla \cdot\vec{F} dW = \iint_{S_{1}} F\cdot \, ds - \iint_{S_{1}} F\cdot \, ds = 0

\end{gather}
$$