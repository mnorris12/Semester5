#### 1.35 
![[Pasted image 20240130203513.png|center|]]

We note the following given the question;
$$
\begin{gather}
F_{+on-} = (9\cdot 10^{-31})kg \left( -9.8 \frac{km}{s^{2}} \right) = -8.82\cdot 10^{-30} N = W \\ \\ 
\end{gather}
$$
Thus we we set the farthest right number equal to the force of the proton on the electron. We get 
$$
\begin{gather}
W = k \frac{-e^{2}}{r^{2}_{+on-}} \\ \\ 
\frac{w}{k} = -\frac{e^{2}}{r^{2}_{+on-}} \\ \\ 
r^{2}_{+on-} = \sqrt{ \left( \frac{e^{2}k}{W} \right) }


\end{gather}
$$
We plug in the values for $e,k,w$ to get a distance of 5 m 

#### 1.37
To help with the components of the charges, we flip the square 45 degrees right: 
![[Pasted image 20240130213828.png|center|300]]


Specifically, we're looking for 
$$
-F_{\uparrow} =F_{\downarrow}
$$
Where $F_{\uparrow}$ is the sum of the forces from charges $q_1, q_3,q_4$ on $q_2$ and and $F_{\downarrow}$ includes the force on $q_2$ by $Q_1$. Thus if we find $F_{\uparrow}$, we'll know $F_{\downarrow}$:
$$
\begin{gather}
F_{\uparrow} = \left[ F_{12} = k \frac{e^{2}\cos\theta \hat{j}}{l^{2}_{12}}+F_{32}= k \frac{e^{2}\hat{j}}{(\sqrt{ 2 }l_{32})^{2}}+ F_{42}  = k \frac{e^{2}\cos\theta\hat{j}}{l^{2}_{42}}\right] \\ \\ 
F_{\uparrow} = \frac{ke^{2}\hat{j}}{l^{2}}\left[ \cos\theta+\frac{1}{2}+\cos\theta \right] 
\end{gather}
$$
As we've said above, the square was tilted 45 degrees, so we'll replace $\theta$ with 45
$$
\begin{gather}
F_{\uparrow} = \frac{ke^{2}\hat{j}}{l^{2}}\left[ \cos(45)+\frac{1}{2}+\cos(45) \right] = \frac{ke^{2}}{l^{2}} \left[ \frac{2\sqrt{ 2 }+1}{2} \right]
\end{gather}
$$
Thus $F_{\downarrow}=$ $-\frac{ke^{2}}{l^{2}} \left[ \frac{2\sqrt{ 2 }+1}{2} \right]$, but we're looking for $Q$, thus we see that 
$$
\begin{gather}
 F= EQ= \frac{kq}{l^{2}}\left( q\left[ \frac{2\sqrt{ 2 }+1}{2} \right] \right) \\ \\ 
\text{Thus we know:} \hspace{.2cm} E =q\left[ \frac{2\sqrt{ 2 }+1}{2} \right]
\end{gather}
$$


#### 1.37b

We can find the potential energy by the $-W$: 
$$
\begin{gather}
-W = \frac{1}{4\pi\epsilon_{0}}\left( \frac{q^{2}}{l}+\frac{q^{2}}{\sqrt{ 2 }}+\frac{q^{2}}{l}-\frac{2Qq}{\sqrt{ 2 }l} \right) \\ \\ 
-W = \frac{1}{4\pi\epsilon_{0}}\left( \frac{\sqrt{ 2 }q^{2}}{\sqrt{ 2 }l} +\frac{q^{2}}{\sqrt{ 2 }l}+ \frac{\sqrt{ 2 }q^{2}}{\sqrt{ 2 }l}-\frac{2Qq}{\sqrt{ 2 }l}\right) \\ \\ 
-W = \frac{1}{4\pi\epsilon_{0}} \frac{\sqrt{ 2 }q^{2}+q^{2}+\sqrt{ 2 }q^{2}+2Qq}{\sqrt{ 2 }l} \\ \\
-W =\frac{ 2\sqrt{ 2 }q^{2}+q^{2}+2Qq}{\sqrt{ 2 }l}
\end{gather}
$$
We now plugin Q: 
$$
\begin{gather}
-W = \frac{2\sqrt{ 2 }q^{2}+q^{2}-2q^{2}\left[ \frac{2\sqrt{ 2 }+1}{2} \right]}{\sqrt{ 2 }l} \\ \\ 
\frac{2\sqrt{ 2 }q^{2}+q^{2}-q^{2}\left[{2\sqrt{ 2 }+1}\right]}{\sqrt{ 2 }l} \\ \\ 
\frac{0}{\sqrt{ 2 }l} = 0
\end{gather}
$$
Thus we've proved that the potential energy is 0

#### 1.38

![[Pasted image 20240203011544 1.png|center]]

We note that for the force on the center charge, in the event that it experiences a kick, the force on it will be $F_{qQ_{i}}=qE$. We'll also note that for simple harmonic motion, we have $\ddot{x} = -\omega^{2}x$. We start by expanding the Force $F_{qQ_{2}}=qE$, the force $Q_{2}$ on $q$: 
$$
\begin{gather}
F_{qQ_{2}} = \frac{kqQ_{2}}{(l+r)^{2}} = \frac{kqQ_{2}}{\left[ \frac{(l+r)^{2}}{l^{2}}l^{2} \right]} = \frac{kqQ_{2}}{\left( 1+\frac{r}{l} \right)^{2}l^{2}} \\ \\ 
\text{We now use the binomial approximation:} \\ \\ 
\frac{kqQ_{2}\left( 1-\frac{2r}{l} \right)}{l^{2}} = \frac{kqQ_{2}\left( 1-2 \frac{r}{l} \right)}{l^{2}}
\end{gather}
$$
We'll note that instead of doing the same work for $F_{qQ_{1}}$, it will instead be 
$$
\begin{gather}
F_{qQ_{1}} = \frac{kqQ_{2}\left( 1+2 \frac{r}{l} \right)}{l^{2}}
\end{gather}
$$
This proves that $q$ goes through simple harmonic motion as $r$ changes - the force of one of the two charges $Q_{1},Q_{2}$ will exceed the other and pull it in its own direction, causing oscillation.

We'll note that $F_{net}$ is the sum of the two above forces. Thus $F_{net}$ is
$$
\begin{gather}
\frac{kqQ}{l^{2}}\left[ \left( -1-\frac{2r}{l} \right)+\left( 1-\frac{2r}{l} \right) \right] = \frac{kqQ}{l^{2}}\left[ -\frac{4r}{l} \right] \\ \\ 

\text{This equals:} \hspace{.2cm} -\frac{4kqQ}{l^{3}}r
\end{gather}
$$
So we use the equation for the simple harmonic motion, which gives oscillation $\omega$: 
$$
\begin{gather}
2\sqrt{ \frac{kqQ}{l^{3}} }m
\end{gather}
$$

 
#### 1.39 
We have the following picture so that the reader will understand the used variables/directions:

![[Pasted image 20240203033456 1.png|center]]

By trigonometry we have that: 
$$
\begin{gather}
\cos\theta = \frac{y}{2x} \\ \\ 

\sin\theta = \frac{z}{2x} \\ \\ 
\end{gather}
$$
Now, we'll choose the potential energy method and consider the different kinds of forces there are. There should be 4 relationships for the x-path forces, and 1 term for each of the y and z-path forces. Thus the potential energy should thus be:

$$
\begin{gather}
U = \frac{4kqQ}{x} + k \frac{q^{2}}{z} + \frac{kQ^{2}}{y} \\ \\ 

\text{we put y,z in terms of x} \\ \\ 

z = 2x\cos\theta \\ \\ 

y = 2x\sin\theta \\ \\ 

\text{Thus, U equals:} \\ \\ 
U = k \left[ \frac{4qQ}{x}+\frac{q^{2}}{2x\sin\theta}+\frac{kQ^{2}}{2x\cos\theta} \right]
\end{gather}
$$
As suggested by the problem, we need to minimize $U$, thus we need to take its derivative with respect to $\theta$ at 0:

$$
\begin{gather}
\frac{dU}{d\theta} = k \left[ \frac{q^{2}}{2x}\left( \frac{d}{d\theta} \frac{1}{\sin\theta} \right)+\frac{Q^{2}}{2x}\left( \frac{d}{d\theta} \frac{1}{\cos\theta} \right) \right] = 0 \\ \\ 
\text{We divide by k and move second term:} \\ \\ 

\frac{q^{2}}{2x}\left( \frac{\cos\theta}{\sin ^{2}\theta} \right) = \frac{Q^{2}}{2x}\left( \frac{\sin\theta}{\cos ^{2}\theta} \right) \\ \\ 

q^{2} \frac{\cos ^{3}\theta}{\sin ^{3}\theta} = Q^{2} \\ \\ 
\text{thus we have:}
\tan ^{3}\theta = \frac{q^{2}}{Q^{2}}
\end{gather}
$$
Lastly, we'll have to prove that this is a minimum rather than maximum. This means the second derivative $\frac{d^{2}U}{d\theta^{2}}$ should be $>0$ from $0\leq\theta\leq 90$. 

$$
\begin{gather}
\frac{d^{2}U}{d\theta^{2}} = \frac{k}{2x}\left( \frac{Q^{2}}{\cos\theta} +\frac{q^{2}}{\sin\theta}\right)
\end{gather}
$$
which from the above intervals, the second derivative is always positive. 

#### 1.48
We take a look at the following picture to help understand what's happening:

![[Pasted image 20240203125110 1.png|center|300]]

We'll first start by finding $E(r)$ which is some function of the electric field dependent on $r$
$$
\begin{gather}
E(r) = \frac{kdq}{r^{2}} \\ \\ 
\text{where dq} = \lambda Ad\theta \hspace{.5cm}r^{2} = \sqrt{ z^{2}+R^{2} } \\ \\ 

\text{Thus} \hspace{.2cm}E(r) = \frac{k\lambda AD\theta}{\sqrt{ z^{2}+R^{2} }^{2}} = \frac{k\lambda Ad\theta}{z^{2}+R^{2}} \\ \\ 
\end{gather}
$$
For a linear charge density, we need to further account for the z direction $\cos\psi$
![[Pasted image 20240203125705 1.png|center|300]]

Thus we have that 
$$
\begin{gather}
E(r) = \frac{k\lambda Ad\theta}{z^{2}+R^{2}} \left( \frac{z}{\sqrt{ z^{2}+R^{2} }} \right) = \frac{kAz\lambda d\theta}{(z^{2}+R^{2})^{3/2}}
\end{gather}
$$
We now integrate:

$$
\begin{gather}
\frac{kAz\lambda}{(z^{2}+R^{2})^{3/2}} \int d\theta =\frac{Az\lambda}{2\epsilon_{0}(z^{2}+R^{2})^{3/2}} = E
\end{gather}
$$
The max value of the electric field is the derivative of $E = \frac{dE}{dz} = 0$. To avoid the complication of unnecessary constants, we'll only consider the following equation $F(z)$
$$
\begin{gather}
F(z) = \frac{z}{(z^{2}+R^{2})^{3/2}}\\ \\ 

F'(z) = \frac{(z^{2}+R^{2})-3z^{2}}{(z^{2}+R^{2})^{5/2}} = 0 \\ \\ 

-2z^{2} = -R^{2}\\ \\
2z^{2}=R^{2} \\ \\ 
z= \sqrt{ \frac{R^{2}}{2} }
\end{gather}
$$
Thus the electric field is at a maximum when $z= \sqrt{ \frac{R^{2}}{2} }$.
#### 1.56(a)

![[Pasted image 20240201195818.png|center]]

We note by Gauss's Law that $\Phi_{\text{whole cube}} = \oint E \cdot da = \frac{q}{\epsilon_{0}}$ for the entire cube. We also note that for each side of the cube, the vectors point outward direction, thus the flux through each surface should be the same:
![[Pasted image 20240201200147.png|center|300]]

Thus the flux of through once surface should be $\frac{q}{6\epsilon_{0}}$.

#### 1.56b

We consider if the point charge was at one of the edges of the sphere. To better see this, we can flip the sphere until it reaches a diamond shape like so: ![[Pasted image 20240201201931.png|center|400]]
We observe that for the three sides connecting the small spherical charge, they have vectors pointing along the sides themselves, thus the flux through them are zero. We deal with the top three which all have same flux and distance from the charge itself. So the total flux through this case for each side is $\frac{1}{3}$ of the total flux of the cube. 

#### 1.61

![[Pasted image 20240202231157 1.png|center]]

We think about adding up the potential energy of the sphere, by adding up the change in work required to configure more charge on the sphere:
$$
\begin{gather}
-dw = E(r)dq
\end{gather}
$$
Where we note that $E(r) = \frac{kq(r)}{r}$. Thus we must find $q(r)$:

$$
\begin{gather}
q(r) = \rho V = \frac{\rho(4\pi r^{3})}{3}
\end{gather}
$$
Thus we find $E(r)$:
$$
\begin{gather}
\frac{k \frac{4}{3}\pi r^{3}\rho}{r} = \frac{4}{3}\pi kr^{2}\rho
\end{gather}
$$
We know that $dq =4\pi r^{2}dr$. Thus we have $-dw$ and we integrate: 

$$
\begin{gather}
-dw = \left( \frac{4}{3} \pi r^{2} \rho \right)(4\pi r^{2}dr\rho) = \frac{16\pi^{2}\rho^{2}kr^4}{3} \\ \\ 
\text{we integrate:} \hspace{.2cm} \int _{0}^R \frac{16\pi^{2}\rho^{2}kr^4}{3}\, dr \\ \\ 
\frac{16\pi^{2}\rho^{2}k}{3} \int r^4 \, dr  = \frac{16\pi^{2}\rho^{2}k}{15}R^5
\end{gather}
$$
#### 1.69

First, we notice that we can interpret a sphere being cut out of the larger sphere, as the sphere of radius A being added to a sphere of negative uniform density charge of radius $\frac{a}{2}$:

![[Pasted image 20240202165030 1.png]]

We start with location A (we decide that $\downarrow$= $+\hat{z}$):

$$
\begin{gather}
E_{+A} = 0 \hspace{.5cm} \text{all the charges cancel out so no electric field} \\ \\ 

E_{-A} = \frac{kQ_{in}}{r^{2}} (-\hat{z}) \hspace{.5cm} \text{where we have to find Q and} \hspace{.2cm} r = \frac{a}{2} \\ \\ 

\end{gather}
$$
Thus we find $Q_{{in}}$ for $E_{-A}$
$$
\begin{gather}
Q_{-A} = -\rho V = -\frac{\rho 4\pi \left( \frac{a}{2} \right)^{3}}{3} = -\frac{\rho a^{3}\pi}{6}
\end{gather}
$$
Now we're able to calculate $E_{-A}$:
$$
\begin{gather}
E_{-A} = \frac{k\left( \frac{-\rho a^{3}\pi}{6} \right)}{\left( \frac{a}{2} \right)^{2}}(-\hat{z}) = \frac{2k\rho\pi a}{3}
\end{gather}
$$

We now move to location B. We'll start first with the larger circle of radius a:

$$
\begin{gather}
E_{+B} = \frac{kQ_{in}}{r^{2}} (-\hat{z}) \hspace{.5cm}\text{where we find what}\hspace{.2cm}Q_{in} \text{is} \\ \\ 
 \\ \\ 

Q_{in} = \rho V = \frac{-4\rho_{4}\pi a^{3}}{3} \\ \\ 

E_{+B} = \frac{k\left( \frac{-4\rho_{4}\pi a^{3}}{3} \right)}{a^{2}} = \frac{-4\pi k\rho_{4} a}{3}
\end{gather}
$$
And then lastly we find what $E_{-B}$ is: 

$$
\begin{gather}
E_{-B} = \frac{kQ_{in}}{r^{2}} \hspace{.5cm} \text{where we find}\hspace{.2cm} Q_{in}  \\ \\ 

Q_{in} = \rho V = \frac{-\rho 4\pi}{3}(a^{3}) = \frac{-\pi\rho a^{3}}{6} 
\end{gather}
$$
We notice that the $Q_{in}$ for $E_{-B}$ is the same as charge as it was for $E_{-A}$. The difference in the electric field from $E_{-A}$ to $E_{-B}$ is the change in $a$ or the radius: 

$$
\begin{gather}
E_{-B} = \frac{k\left( \frac{-\pi\rho a^{3}}{6} \right)}{\left( \frac{3}{2} a \right)^{2}}(-\hat{z}) = \frac{k\pi\rho a^{3}}{\frac{9}{4}a^{2}}\left( \frac{1}{6} \right)= \frac{2\pi\rho k a}{27}
\end{gather}
$$
Now we add the two charges for the position B to obtain both the magnitude and the direction:

$$
\begin{gather}
E_{+B}+ E_{-B} = \frac{-4\pi k\rho_{4} a}{3} +\frac{2\pi\rho k a}{27} = -\frac{34\pi k\rho a}{27}
\end{gather}
$$

#### 1.72
Let's draw a diagram of the slab and the plane:

![[Pasted image 20240202225125 1.png|center|300]]

We make a couple of notes: 
- no matter the distance from the plane, the electric field is constant
- For the cylinder, only the faces matter as the electric field vectors point parallel to the "side"

With that information we can talk about the charge E outside of the system, or $E_{out}$
$$
\begin{gather}
E_{out} = \underbrace{ \frac{\sigma}{2\epsilon_{0}} }_{ \text{plane} }+ \underbrace{ \frac{\rho d}{2\epsilon_{0}} }_{ slab }
\end{gather}
$$
Now that we've found the charge outside of the system, we find the charge inside the system $E_{in}$, in which it's total with $E_{out}$ will be the vector field everywhere: 

$$
\begin{gather}
AE_{in} = \frac{Q_{in}}{\epsilon_{0}} \hspace{.5cm} \text{where we have to find} \hspace{.2cm}Q_{in} \\ \\ 
Q_{in} = \sigma A +\rho rA \hspace{.2cm}\text{thus we have:} \\ \\ 
E_{in} = \frac{\sigma +\rho r}{\epsilon_{0}}
\end{gather}
$$
Thus the sum of $E_{out}$ and $E_{out}$ equal: 
$$
\begin{gather}
\frac{2\sigma+\rho d+2\sigma r}{2\epsilon_{0}}
\end{gather}
$$

#### 1.77

We imagine for a moment the simple case of the charges two stationary protons feel on each other. We have that $F_{12}= -F_{21}$, where force one proton feels is the same magnitude but opposite the direction of the other.

![[Pasted image 20240203132043 1.png|center]]
We want that same property once we imbed them in the electron jelly. To clarify, we'll think of the electron jelly as a point charge with magnitude $-2e$. If we want the forces the protons experience because of the negative point charges to be equal, then they have to be equidistance from the center where the center is the negative point charge itself  

![[Pasted image 20240203132419 1.png|center]]

Now we think of the sphere itself:

We first start of by finding $q(a)$ which is the total charge that each proton will experience in the jelly (where R would be the total radius of the sphere): 
$$
\begin{gather}
q(r) = -\frac{2e(V_{\text{sphere(a)}})}{V_{\text{total}}}\\ \\ 

q(r) = -2e\left( \frac{a^{3}}{R^{3}} \right)
\end{gather}
$$
We next use this charge function to find the amount of electric field the protons will feel at some distance a away from the center:

$$
\begin{gather}
E(a) = \frac{kqv}{a^{2}} = -\frac{2ek}{a^{2}}\left( \frac{a^{3}}{R^{3}} \right) = -\frac{2eka}{R^{3}}
\end{gather}
$$
We use this electric field function to find the force each proton will field by the electron jelly. The sum of that force, and the repulsive force they experience due to the other, will equal zero. We can use this knowledge to find $a$ 

$$
\begin{gather}
F = e(E(a)) +e \frac{ke}{(2a)^{2}} = -\frac{2e^{2}ka}{R ^{3}} +\frac{e^{2}k}{4a^{2}} = 0\\ \\ 

\frac{e^{2}k}{4a^{2}} = \frac{2e^{2}ka}{R^{3}} \\ \\ 

\frac{1}{4a^{2}}= \frac{2a}{R^{3}} \\ \\ 

R^{3} = 8a^{3} \\ \\ 

a = \frac{R}{2}
\end{gather}
$$

#### 1.82(a)

![[Pasted image 20240203143207 1.png|center]]

The energy of the system is the potential energy

$$
\begin{gather}
U = \frac{\epsilon_{0}}{2} \int _{\text{entire field}} E^{2} \, dv 
\end{gather}
$$
Where, due to symmetry reasons, we only care about the $\hat{r}$ direction. Thus we start by finding $E$ using the flux equation: 

$$
\begin{gather}
\oint E \cdot dA = \frac{Q_{in}}{\epsilon_{0}} \\ \\ 
\end{gather}
$$
Where when $r<a$ and $r>b$, the electric field is 0 as Q is zero. Thus we have from the flux: 
$$
\begin{gather}
EA = \frac{Q}{\epsilon_{0}} \\ \\ 

E 4\pi r^{2} = \frac{Q}{\epsilon_{0}} \\ \\ 

E = \frac{Q}{4\pi r^{2}\epsilon_{0}}
\end{gather}
$$
Thus we take the integral from $a<r<b$ to get the potential energy:

$$
\begin{gather}
U = \frac{\epsilon_{0}}{2} \int _{a}^b E^{2}\, dv \\ \\ 

U = \frac{\epsilon_{0}}{2}\int _{a}^b \frac{Q^{2}}{16\pi^{2}r^{4}\epsilon_{0}} r^{2}\sin\theta\, dr d\theta d\phi \\ \\ 
\frac{Q^{2}}{8\pi\epsilon_{0}} \int _{a}^b \frac{1}{r^{2}}\, dr = \frac{q^{2}}{8\pi\epsilon_{0}}\left( -\frac{1}{r}|_{a}^b \right) = \frac{Q^{2}}{8\pi\epsilon_{0}}\left( \frac{1}{a} - \frac{1}{b} \right)
\end{gather}
$$

#### 1.82(a)
Wasn't exactly sure how to approach this one, so for time purposes here's where I got to:

![[Pasted image 20240203153157 1.png|center]]

we recognize that $-dw = E(r)dq$. Thus we need to find $E(r)$ and then integrate over $dq$
$$
\begin{gather}
E(r) = -\frac{kq}{r^{2}} \\ \\ 
-\int_{0}^W  \, dw  = \int _{0}^q \, -\frac{kq}{r^{2}}dq  =-\frac{kq^{2}}{r^{2}} \\ \\ 
-\frac{q^{2}}{4p\pi\epsilon_{0}} \\ \\ \hspace{.5cm} \text{Now we integrate from a to b} \\ \\ 
-\frac{q^{2}}{4\pi\epsilon_{0}} \int _{s}^b \frac{1}{r^{2}}\, dr \\ \\ 
=\frac{q^{2}}{4\pi\epsilon_{0}}(-2r^-1)|_{a}^b = -\frac{2q^{2}}{4\pi\epsilon_{0}}\left( \frac{1}{a}-\frac{1}{b} \right)
\end{gather}
$$