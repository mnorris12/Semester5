#### 10.17
The maximum amount of energy that can be stored in the Mylar filled capacitor corresponds to the dielectric strength $\frac{1.4\text{kilovoltz}}{(\text{meter})}$. Using unit conversions, that is, 
$$
\begin{gather}
E = \frac{1.4*10^4 V}{2.54*10^{-5}m} = 5.51*10^8 \frac{V}{m}
\end{gather}
$$
We know the capacitance is equal to $C = \kappa C_{0}$, where $C_{0} = \frac{\epsilon_{0}A}{s}$, where $A$ is the area of the capacitor and $s$ is the separation of the plates. The energy stored in the capacitor can be modeled by the equation $E = C \frac{\phi^{2}}{2} \frac{1}{V}$, where $\phi = E_{elec}*s$ and $V$ is the volume. Thus we can combine the equation such that
$$
\begin{gather}
E = \kappa \frac{\epsilon_{0}A}{s} \frac{(E_{elec} *s)^{2}}{2} * \frac{1}{V} = \frac{1}{2}(3.25)\left( 8.85*10^{-12} \frac{s^{2}C^{2}}{kgm^{3}} \right) \left( 5.51*10^{-8} \frac{V}{m} \right)^{2}  \\ \\ =
4.4*10^6 \frac{J}{m^{3}}
\end{gather}
$$
Using it's density $1400 \frac{kg}{m^{3}}$, we have
$$
\begin{gather}
\frac{4.4*10^6}{1400} \frac{J}{kg} = 3142 \frac{J}{kg}
\end{gather}
$$
To find how much the capacitor would lift of the ground, we use the fact that the electrodes and case account for 25 percent of the capacitor’s weight. Thus, Mylar accounts for $\frac{3}{4}$ the mass. We have $E = mgh$, 
$$
\begin{gather}
h = \frac{E}{mg}= \frac{3142}{\left( \frac{3}{4} \right)(9.81)} m = 427 m
\end{gather}
$$
#### 10.18

We're asked to find the capacitance of the second two capacitors. We begin with the first capacitor. Let's draw a picture, 

![[Pasted image 20240428191058.png]]

That is, we can model the second capacitor as a superposition of two different capacitors, one being a vacuum capacitor with separation $\frac{s}{2}$, and the other being a dieletric-filled capacitor with the same separation. Thus we have 
$$
\begin{gather}
C_{\text{vacuum}} = \frac{\epsilon_{0}A}{\left( \frac{s}{2} \right)} = 2C_{0}
\end{gather}
$$
where $C_{0}$ is the value of the capacitance of the first capacitor with separation $s$. With that said, the dielectric material will have capacitance
$$
\begin{gather}
C_{\text{dielectric}} = 2\kappa C_{0}
\end{gather}
$$
and since the capacitors are in series with each other, they add like resistances that we've seen in chapter three, 
$$
\begin{gather}
\frac{1}{2C_{0}}+\frac{1}{2\kappa C_{0}}  =\frac{2\kappa C_{0}}{\kappa+1} = C_{\text{tot}}
\end{gather}
$$
We now focus on the third capacitor and find its capacitance. Let's draw a picture, 

![[Pasted image 20240428191829.png|center]]

This is quite similar to the second capacitor except the area $A$ is divided in half an the capacitors are in parallel! Thus
$$
\begin{gather}
C_{\text{vacuum}} = \frac{\epsilon_{0}\left( \frac{A}{2} \right)}{s} \\ \\ 
C_{\text{dielectric}} = \frac{\kappa C_{0}}{2}  \\ \\ 
C_{\text{total}} = \frac{C_{0}(1+\kappa)}{2}
\end{gather}
$$
and we're all set!
#### 10.21

We are asked for the magnitude and direction of the dipole vector in three different scenarios. We begin with figure a, 

![[Physics E&M/E&M Figures/10.21 figure a.svg|center|250]]

The dipole moment vector becomes a discrete sum if there's a finite amount of charge. Thus we have
$$
\begin{gather}
\mathbf{p} =q\left( \frac{\sqrt{ 3 }d}{2} \right)+ q\left( \frac{\sqrt{ 3 }d}{2} \right) = 2q\left( \frac{\sqrt{ 3 }d}{2} \right) = q\sqrt{ 3 }d
\end{gather}
$$

where we've take the the top charge to be the origin since the configurations net charge is zero. It's direction points down

For figure b, we have

![[Physics E&M/E&M Figures/10.21 Figure b.svg|center|300]]

We we put the coordinate system in the middle of the square, then the positive charges magnitude together is equal and opposite the negative charges, thus the magnitude of the $\mathbf{p}=0$. If no magnitude then no direction. 

For Figure c, we have
![[Physics E&M/E&M Figures/10.21 Figure c.svg|center|300]]

we're we've made the origin of the coordinate systems superimposed on the upper left charge. We can split the $\mathbf{p}$ vector into $x,y$ components such that
$$
\begin{gather}
q_{x} = qd+ 2qd= 3qd \\ \\ 
q_{y} = -2qd+qd = -qd
\end{gather}
$$
Where for the $x$ component, the bottom left charge $-q$ has no magnitude, and for the $y$ component the upper right charge has no magnitude. Its total $x$ component is positive and total $y$ component is negative, so the vector points down diagonally towards the right. Thus the total magnitude of the $\mathbf{p}$ vector is
$$
\begin{gather}
\mathbf{p}_{\text{tot}} = \sqrt{ (3qd)^{2}+(-qd)^{2} } = \sqrt{ 10 }qd
\end{gather}
$$
we're all set. 
#### 10.28

We find the direction and the magnitude of the force vector for the central dipole in the presence of the two others as shown in the figure,

![[Physics E&M/E&M Figures/10.28 Figure.svg|center|300]]

The direction of the $\mathbf{F}$ vector on the central dipole is a combination of the two dipoles at the ends. Let's first start by finding the magnitude of the force vector due to the left dipole. When the tail of the electric field vector of the left dipole $E_{\text{left}}$ meets anywhere along the central dipole, it points only in the $y$ direction. Thus, 
$$
\begin{gather}
E_{y-left}= \frac{p}{4\pi\epsilon_{0}r^{3}}\sin(-90) = -\frac{p}{4\pi\epsilon_{0}b^{3}}

\end{gather}
$$
When the the electric field vector of the right dipole $E_{\text{right}}$ meets the parallel (on top of) of the central dipole, it points only in the $x$ direction. Thus we have
$$
\begin{gather}
E_{x-right}  = \frac{p}{2\pi\epsilon_{0}r^{3}}\cos(0)= \frac{p}{2\pi\epsilon_{0}b^{3}}
\end{gather}
$$
Where both of the electric field equations for the left and right dipole we're used from equation 10.18 in Purcell. We calculate the magnitude of the force vector $\mathbf{F}$ of the central dipole using electric field components we just found
$$
\begin{gather}
\mathbf{F} = \mathbf{p}\cdot \nabla \mathbf{E} \rightarrow\mathbf{p} \cdot\left( \frac{3p}{4\pi\epsilon_{0}b^{2}}, \frac{3p}{2\pi\epsilon_{0}b^{2}} \right) \\ \\ 
F_{x} = \frac{3p^{2}}{4\pi \epsilon_{0}b^{2}}\hspace{.5cm}F_{y} = \frac{3p^{2}}{2\pi\epsilon_{0}b^{2}}\\
\end{gather}
$$
We notice that that both the force components are positive, so it points in the upwards diagonally to the right.
#### 10.29

We have four different arrangements of two dipole moments of two neighboring polar molecules. We find the potential energy of arrangements. Let's first start with a picture, 
![[Physics E&M/E&M Figures/10.29 Figure.svg|center]]

Where the distance between each dipole is $d$. From equation 10.22 in Purcell we have that the total work done is, 
$$
\begin{gather}
pE(1-\cos(\theta))
\end{gather}
$$
Starting with case (a), if we bring the left dipole in from infinity, first allowing it to point to the left. then $\theta$ is zero and thus the total work done is zero from the equation above. In rotating it 90 degrees clockwise, this requires work which from the equation is just $W= \frac{p^{2}}{4\pi\epsilon_{0}d^{3}}$

For the second case (b) its the same situation, but instead we rotate the right dipole 90 degrees counterclockwise. So $W= \frac{-p^{2}}{4\pi\epsilon_{0}d^{3}}$ as the electric field points down. 

For the third case (c), if we bring the right dipole in from infinity, similar to how we treated (a), then $\theta$ is zero. Upon rotating the dipole to the right 90 degrees clockwise, we have
$$
\begin{gather}
\int _{90}^0 pE\sin\theta \, d\theta = pE\cos\theta|_{90}^0 =pE(0-1)=-pE
\end{gather}
$$
in this case, $E = \frac{2p}{4\pi\epsilon_{0}d^{3}}$, so we have $W = -\frac{2p^{2}}{4\pi\epsilon_{0}d^{3}}$. 

Lastly for the final case, its the same situation but in the integral goes from 90 to 180. Thus 
$$
\begin{gather}
\int _{90}^{180} pE\sin\theta \, d\theta = pE\cos\theta|_{90}^{180} =pE(0-(-1)) = pE
\end{gather}
$$
thus $W = \frac{2p^{2}}{4\pi\epsilon_{0}d^{3}}$. 

We're all set
#### 10.32
Let's first start of with a picture!

![[Physics E&M/E&M Figures/10.32 Figure.svg|center]]

We estimate the amount of energy required to separate an ion with charge $e$ from a water molecule. 

Since the oxygen molecule is negatively charged, and the hydrogen molecules are positively charged, the negatively charged ion will be closer to the hydrogen. We model the water molecule as a dipole. The electric field of the dipole water molecule is $E = \frac{2p}{4\pi\epsilon_{0}r^{3}}$. Furthermore, we know that the the resulting force on the ion is $F =qE = \frac{2pe}{4\pi\epsilon_{0}r^{3}}$. Thus, we find the amount of work required to bring the ion from some initial distance to infinity
$$
\begin{gather}
\int _{1.5Ang}^\infty \frac{2pe}{4\pi\epsilon_{0}r^{3}}  \, dx =\frac{pe}{4\pi\epsilon_{0}(1.5Ang)^{2}} \\ \\  = \frac{(6.13*10^{-30}Cm)\left(1.602*10^{-19}c \right)}{4\pi\left( 8.85*10^{-12} \frac{s^{2}C^{2}}{kgm^{3}} \right) (1.5*10^{-10})^{2}} = 3.9*10^{-19}J\\ \\ 

\end{gather}
$$

we're all done!
#### 11.12

###### a

We find the the magnitude of the dipole moment of the earth. We know from equation 11.15 in Purcell, 

$$
\begin{gather}
B_{r}= \frac{\mu_{0}m}{2\pi r^{3}}\cos\theta
\end{gather}
$$
where $\theta=0$, thus we have
$$
\begin{gather}
m = \frac{B_{r}2\pi r^{3}}{\mu_{0}} = (6.2*10^{-5}T) \frac{2\pi(6.378*10^4km)^{3}}{4\pi*10^{-7} \left( \frac{kgm}{C^{2}} \right)} = 8.04\times10^{22} \frac{J}{T}
\end{gather}
$$
###### b

We imagine the source of the field is a current ring with on the circumference of the earth's matellic core with radius 3000. We remember for chapter six the that magnetic field of a ring is given by
$$
\begin{gather}
B_{z} = \frac{\mu_{0}Ib^{2}}{2(b^{2}+z^{2})^{3/2}} \hspace{.5cm}\text{field on axis}
\end{gather}
$$
Here $b=3000$ and $z$ is the radius of the earth. Thus we have
$$
\begin{gather}
I = \frac{2B(b^{2}+z^{2})^{3/2}}{\mu b^{2}} = \frac{2(6.2*10^{-5}T)(3000km^{2}+(6.378*10^4km)^{2})^{3/2}}{4\pi*10^{-7}\left( \frac{kgm}{C^{2}} \right)(3000)^{2}} =2.85\times10^{9} A
\end{gather}
$$

#### 11.25

We calculate the energy required to rotate the magnetite in the bacterium 90 degrees in the Earth's field. 

We first begin by calculating the dipole moment of one of the crystals. We see from equations 11.75 and 11.76 that $m$ has units of $\frac{\text{joules}}{tesla}$ and $M$ has units of $\frac{\text{joules}}{\text{tesla}*\text{m}^{3}}$. So to find $m$, we just need to multiply $M$ by the volume of the magnetite which is $(5*10^{-8}m)^{3}$. Thus we have, 
$$
\begin{gather}
m = 4.8*10^5 *(5*10^{-8}m)^{3}= 6\times10^{-17} \frac{J}{T}
\end{gather}
$$
The work required is the integral
$$
\begin{gather}
W = \int _{0}^{90}N \, d\theta = \int _{0}^{90}mB\sin\theta \, dx =mB(1-\cos\theta)|_{0}^{90} = mb
\end{gather}
$$
If we have 10 to 20 crystals then $W = (10-20)mB$ where $10-20$ is range instead of a value. Thus we have
$$
\begin{gather}
W = (10-20)*\left( 6*10^{-17} \frac{J}{T} \right)(5.5*10^{-5}T) = (3.3\times10^{-20}-6.6\times10^{-20})J
\end{gather}
$$
where the answer is a range instead of subtraction. At the end of section 11.6, Purcell tells us that $kT$ at room temperature is roughly $4*10^{-21}J$. As a ratio to the work we just calculated, we have
$$
\begin{gather}
\frac{W}{kT} = \frac{(3.3\times10^{-20}-6.6\times10^{-20})J}{4*10^{-21}J} = 8.25-16.5
\end{gather}
$$
We're all done! Have a great summer break Professor Brown! It's been a joy to be your student!

![[d0bc3a613366a00e76c022659c3b1ccb.png|center|300]]
