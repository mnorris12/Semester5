#### 9.14 Sphere with a hole

Let's start with a picture 

![[Physics E&M/E&M Figures/Drawing 2024-04-14 14.09.01.excalidraw.svg|center|400]]

Now let's write out the equations: 
$$
\begin{gather}
\int _{c} B \, ds  = \int \left( \mu_{0}\epsilon_{0}\frac{ \partial E }{ \partial t } +\mu_{0}J \right) \, da
\end{gather}
$$
We're going to show the two integrals are equivalent. We'll start with the integral on the left. Going back to chapter six, ampere's law tells us, 
$$
\begin{gather}
\int B \, ds = \mu_{0} \times (\text{current enclosed by path})
\end{gather}
$$
Since the line integral of $B$ over a closed path has the same value around every part of the whole, 
$$
\begin{gather}
\int B \, ds = \mu_{0}I
\end{gather}
$$
from equation 6.20. As for the right integral, from the picture, we immediately see that there's not current density on the shell of the sphere. Thus the integral reduces down to
$$
\begin{gather}
\int \left( \mu_{0}\epsilon_{0} \frac{ \partial E }{ \partial t }  \right)  \, da
\end{gather}
$$
Generally, we know the electric field at the surface of the sphere is $E = \frac{Q}{4\pi\epsilon_{0}R^{2}}$ where $R$ is the radius of the sphere. The change in $E$ with respect to time $\frac{dE}{dt}$ is equal to 
$$
\begin{gather}
\frac{dE}{dt}= \frac{dQ}{dt} \cdot \frac{1}{4\pi\epsilon_{0}R^{2}}
\end{gather}
$$
So we can plug that back into the integral noticing that $\frac{dQ}{dt} = I$
$$
\begin{gather}
\int \left( \mu_{0}I \frac{1}{4\pi R^{2}} \right) \, da \\ \\ 
\mu_{0}I \frac{1}{4\pi R^{2}} \int   \, da \\ \\
da = 4\pi R^{2} \rightarrow \mu_{0}I \frac{1}{4\pi R^{2}} \cdot 4\pi R^{2} = \mu_{0}I \\ \\

\end{gather}
$$
Thus both of the integrals equal $\mu_{0}I$ and our proof is complete. 

#### 8.15 Field inside a discharging capacitor

Let's draw a picture!

![[Physics E&M/E&M Figures/Drawing 2024-04-14 14.46.13.excalidraw.svg|center|400]]

We have the following equations used in the problems
$$
\begin{gather}
\int _{c} B \, ds  = \int \left( \mu_{0}\epsilon_{0}\frac{ \partial E }{ \partial t } +\mu_{0}J \right) \, da
\end{gather}
$$
We know, similarly to the last problem and from equation $6.21$, 
$$
\begin{gather}
\int _{C} B \, ds = \mu_{0}I = 2\pi rB
\end{gather}
$$
For the right side of the formula we have 
$$
\begin{gather}
\int \mu_{0}\epsilon_{0}\frac{ \partial E }{ \partial t }  \, da + \int \mu_{0} J\, da
\end{gather}
$$
The second integral equals zero as the conduction density inside the capacitor is zero. Thus for the first integral, we'll use some of the equation we've already derived for a capacitor in chapter 3
$$
\begin{gather}
\frac{dE}{dt}  = \frac{dV}{dt} \cdot \frac{1}{s} = \frac{I}{C} \cdot \frac{1}{s} = \frac{I}{Cs} \\ \\ 
C = \frac{\epsilon_{0}A}{s}  \\ \\ 
\frac{dE}{dt} = \frac{I}{\epsilon_{0}A}
\end{gather}
$$
Thus we can plug this back into our integral, 
$$
\begin{gather}
\int \mu_{0}\cancel{ \epsilon_{0} }\left( \frac{I}{\cancel{ \epsilon_{0} }A} \right) \, dA = \frac{\mu_{0} I}{A}\int  \, da \\ \\ 
\frac{\mu_{0}I}{\pi b^{2}}\cdot \pi r^{2} = \frac{\mu_{0}Ir^{2}}{b^{2}}
\end{gather}
$$
Now we can set this equal to the integral of the magnetic field over a curve 
$$
\begin{gather}
2\pi rB =  \frac{\mu_{0}Ir^{2}}{b^{2}} \\ \\ 
B = \frac{\mu_{0}Ir}{2\pi b^{2}}
\end{gather}
$$

For a comparison to the calculation of the electric field in figure of 7.16, we can rewrite what we have calculated above as
$$
\begin{gather}
\int _{C}B \, ds =\mu_{0}\epsilon_{0}\int \frac{ \partial E }{ \partial t }  \, da \rightarrow 2\pi rB=\mu_{0}\epsilon_{0}  \frac{d\Phi(E)}{dt}
\end{gather}
$$
which is connected to Faraday's laws of inductions which we used in figure 7.16
$$
\begin{gather}
\int _{C}E \, ds  = -\int \frac{ \partial B }{ \partial t }  \, da\rightarrow 2\pi rE = -\frac{d\Phi (B)}{dt}
\end{gather}
$$

The connection is grounded by the two Maxwell equations with curls. 

#### 9.26 An Electromagnetic Waves

###### a

We show an electromagnetic field in free space with the following equations satisfies Maxwells equations, 
$$
\begin{gather}
E_{x} = 0 \hspace{.5cm}E_{y} =E_{0}\sin(kx+\omega t) \hspace{.5cm}E_{z} = 0 \\ \\
B_{x} = 0 \hspace{.5cm}B_{y} = 0 \hspace{.5cm}B_{z} = -\left( \frac{E_{0}}{c} \right)\sin(kx+\omega t)
\end{gather}
$$
we list Maxwell's equations
$$
\begin{gather}
\nabla \times E = -\frac{1}{c} \frac{ \partial B }{ \partial t }  \\ \\ 
\nabla \times B = \mu_{0}\epsilon_{0}\frac{ \partial E }{ \partial t } + \mu_{0}J \\ \\ 
\nabla \cdot E = 0 \\ \\ 
\nabla \cdot B = 0
\end{gather}
$$
Immediately the last two equations are satisfied as their. To prove the first two components, we have, 

$$
\begin{gather}
\nabla \times E = \begin{pmatrix}
i&j&k \\
\partial_{x}&\partial_{y}& \partial_{z} \\
0 &E_{0}\sin(kx+\omega t)&0
\end{pmatrix} =E_{0}k\cos(kx+\omega t) \\ \\
-\frac{ \partial B }{ \partial t } =-\left( -\frac{E_{0}\omega}{c} \cos(kx+\omega t)\right) = \frac{E_{0}\omega}{c} \cos(kx+\omega t)
\end{gather}
$$

thus $\nabla \times E=-\frac{ \partial B }{ \partial t }$ when $k = \frac{\omega}{c}$. For the second equation we have 

$$
\begin{gather}
\nabla \times B = \begin{pmatrix}
i&j&k \\
\partial_{x} &\partial_{y}&\partial_{z} \\
0&0& -\left( \frac{E_{0}}{c} \right) \sin( kx+\omega t)
\end{pmatrix} = \frac{E_{0}}{c}k\cos(kx+\omega t) \\ \\ 
\frac{ \partial E }{ \partial t }  = E_{0}\omega \cos(kx+\omega t) \hspace{.5cm}\mu_{0}\epsilon_{0} = \frac{1}{c^{2}} \\ \\ 
\mu_{0}\epsilon_{0}\frac{ \partial E }{ \partial t }  = \frac{E_{0}\omega}{c^{2}} \cos(kx+\omega t) 
\end{gather}
$$
thus we have 
$$
\begin{gather}
 \frac{E_{0}k}{c} \cos(kx+\omega t) = \frac{E_{0}\omega}{c^{2}} \cos(kx+\omega t)  \\ \\ 
 E_{0}k \cos(kx+\omega t)  = \frac{E_{0}\omega}{c} \cos(kx+\omega t)
\end{gather}
$$
which, again, is true when $k = \frac{\omega}{c}$. 

###### b

The wavelength $\lambda$ is 
$$
\begin{gather}
\lambda = \frac{2\pi}{k} = \frac{2\pi c}{\omega} = \frac{2\pi\left( 3.0*10^8 \frac{m}{s} \right)}{10^{-10}s^{-1}} = 0.188 m \\ \\
\end{gather}
$$
The average energy density of a sinusoidal wave is 
$$
\begin{gather}
\frac{1}{2} \epsilon_{0} E_{0}^{2}= \frac{1}{2}\left( 8.854*10^{-12} \frac{C^{2}s^{2}}{kgm^{3}} \right)\left( 10^{3} \frac{V}{m} \right)^{2} = 4.427\times10^{-6} \frac{J}{m^{3}}
\end{gather}
$$
The power density is equal to the energy density multiplied by the speed.
$$
\begin{gather}
S = \frac{1}{2}\epsilon_{0}E_{0}^{2}c = 4.427\times10^{-6} \frac{J}{m^{3}} \cdot \left( 3.0*10^8 \frac{m}{s} \right) = 1328.1 \frac{J}{m^{2}s}
\end{gather}
$$
###### 9.28 Poynting vector and resistance heating

Let's draw a picture!

![[Physics E&M/E&M Figures/Drawing 2024-04-14 19.05.44.excalidraw.svg|center]]

We have that the magnetic field is equal to 
$$
\begin{gather}
B = \mu_{0}I / 2\pi r
\end{gather}
$$
We have that the Poynting vector is equal to 
$$
\begin{gather}
S = E \times \frac{B}{\mu_{0}}
\end{gather}
$$
From the right hand rule, if $E$ points parallel to the length of the wire, and $B$ points tangentially along the wire, then $S$ points inside the wire which makes sense. We have that the total energy flowing through the wire with respect to $t$, 
$$
\begin{gather}
P = S(2\pi Rl) = \frac{1}{\cancel{ \mu_{0} }}E \frac{\cancel{ \mu_{0} }I}{\cancel{ 2\pi R }}\cdot \cancel{ 2\pi R }l = \underbrace{ El }_{ V }I = VI
\end{gather}
$$

#### 9.32 A Lorentz invariant

We want to show that the value 
$$
\begin{gather}
E^{2}-c^{2}B^{2}
\end{gather}
$$
is invariant. Let's write down some helpful equations, 
$$
\begin{gather}
E = E_{\parallel} +E_{\perp} \hspace{.5cm} B =B_{\parallel}+B_{\perp} \\ \\ 
E_{\parallel}' =E_{\parallel}\hspace{.5cm}E_{\perp}' = \gamma(E_{\perp}+v\times B_{\perp}) \\ \\ 
B_{\parallel}' = B_{\parallel} \hspace{.5cm}B_{\perp}' = \gamma\left( B_{\perp}-\left( \frac{v}{c^{2}} \right)\times E_{\perp} \right)
\end{gather}
$$
We now start to calculate the parallel and perpendicular components of the $E^{2}-c^{2}B^{2}$, 
$$
\begin{gather}
E^{2'} -c^{2}B^{2'}  = 

(E_{\parallel}'+E_{\perp}')-c^{2}(B_{\parallel}'+B_{\perp}') \\ \\ 
(E_{\parallel}'^{2}-c^{2}B_{\parallel}'^{2} ) + (E_{\perp}'^{2}-c^{2}B_{\perp}'^{2})
\end{gather}
$$
since the parallel components are the same in all frames, the parallel components of $E,B$ satisfy the equation. Now we work out the perpendicular components. 
$$
\begin{gather}
E_{\perp}'^{2} =  \gamma^{2}(E_{\perp}+v\times B_{\perp}) (E_{\perp}+v\times B_{\perp})  = \gamma^{2}(E_{\perp}^{2}+\cancel{ 2E_{\perp}(v B_{\perp}) }+(v\times B_{\perp})^{2}) \\ \\

B_{\perp}'^{2} = \gamma^{2}\left( B_{\perp}-\left( \frac{v}{c^{2}} \right)\times E_{\perp} \right)\left( B_{\perp}-\left( \frac{v}{c^{2}} \right)\times E_{\perp} \right) = \\ \\  \gamma^{2}\left( B_{\perp}^{2}- \cancel{ 2B_{\perp}\left( \frac{v}{c^{2}} \right) E_{\perp }^{2}  }\\ \\ 
+\frac{v^{2}E_{\perp}^{2}}{c^{4}}\right  ) \\ \\ 
E_{\perp}'^{2}-c^{2}B_{\perp}'^{2} = \gamma^{2}E_{\perp}^{2}+\gamma^{2}v^{2}B_{\perp}^{2}+\gamma^{2} c^{2}B_{\perp}^{2}- \frac{\gamma^{2}v^{2}E_{\perp}^{2}}{c^2} \\ \\
E_{\perp}^{2}\gamma^{2} (1-\frac{v^{2}}{c^{2}}) - c^{2}B_{\perp}^{2}\gamma^{2}(1-\frac{v^{2}}{c^{2}}) = E_{\perp}^{2}-c^{2}B_{\perp}^{2}
\end{gather}
$$
Thus we've shown that they are invariant quantities. 

