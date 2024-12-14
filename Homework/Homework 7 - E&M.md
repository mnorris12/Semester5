#### 6.29

We'll first draw a picture: 

![[Pasted image 20240305193545.png|center]]

We have that
$$
\begin{gather}
F = q(E +v\times B) \\ \\ 
F = \frac{dp}{dt} \\ \\ 
\frac{dp}{dt} = \frac{dv}{dt}(\gamma m) \\ \\ 
\end{gather}
$$
We're give that the electric field should equal $E = 0$. Thus we have:
$$
\begin{gather}
F = q(v\times B) = q(vB) \\ \\ 
\end{gather}
$$
Following, we have: 
$$
\begin{gather}
\frac{dv}{dt}(\gamma m) = q(vB) \\ \\ 
\frac{dv}{dt} = \frac{v^{2}}{R} \\ \\ 
\frac{\gamma mv^{2}}{R} = q(vB) \\ \\ 
\frac{mv^{2}}{qvB} = R \\ \\ 
\boxed{R = \frac{p}{qB}}
\end{gather}
$$
Now we focus on finding $\Delta\theta = \omega$:
$$
\begin{gather}
F = q(\vec{v}\times  \vec{B}) \\ \\ 
F = q \begin{pmatrix}
i&j&k \\
0&v_{y}&v_{z} \\
B_{x}&0&0
\end{pmatrix} \\ \\ 
F_{y} = q(v_{z}B_{x})\hat{j}\\ \\
F_{z} =-q (v_{y}B_{x})\hat{z} \\ \\ 
\end{gather}
$$
We can also write the force a different way, as to set that result and our previous y & z components results equal:
$$
\begin{gather}
F_{y} = \frac{dp_{y}}{dt} = \frac{d(\gamma mv_{y})}{dt} = \gamma m\dot{v_{y}} \\ \\ 
F_{z} = \gamma m  \dot{v_{z}} \\ \\ 
\end{gather}
$$
Thus 
$$
\begin{gather}
q(v_{z}B_{x}) = \gamma m\dot{v_{y}} \hspace{.5cm} \dot{v_{y}} = \frac{qv_{z}B_{x}}{\gamma m} \\ \\
-q (v_{y}B_{x})= \gamma m  \dot{v_{z}} \hspace{.5cm} \dot{v_{z}} = -\frac{qv_{y}B_{x}}{\gamma m}

\end{gather}
$$
ODE magic happens when we notice that the derivatives of $\dot{v_{y}},\dot{v_{z}}$
$$
\begin{gather}
\ddot{v_{y}} = \frac{q\dot{v_{z}}B_{x}}{\gamma m} \hspace{.5cm}\ddot{v_{z}} = \frac{q\dot{v_{y}}B_{x}}{\gamma m} 
\end{gather}
$$
Let's go with, $\ddot{v_{y}}$, (later it'll be clear that we could have gone with $\ddot{v_{z}}$ when finding $\Delta\theta = \omega$:

$$
\begin{gather}
\ddot{v_{y}} = -\left( \frac{qB_{x}}{\gamma m} \right)^{2}v_{y}
\end{gather}
$$
From the first ODE remark on the eight things to remember:
$$
\begin{gather}
-\omega^{2} = -\left( \frac{qB_{x}}{\gamma m} \right)^{2} \\ \\ 
\boxed{\omega = \frac{qB_{x}}{\gamma m}} \\ \\ 
\omega = \frac{2\pi}{T} \\ \\ 
\boxed{T = \frac{\gamma m\pi}{qB_{x}}}
\end{gather}
$$
We're all set!

#### 6.31

Let's draw a picture!

![[Pasted image 20240308164637.png|center|300]]

The key idea to solving this problem is making the connection between the current and magnetic field, and then understanding the direction of the magnetic field from the wires at each points. Let's do that! In general, we have: 
$$
\begin{gather}
B = \frac{\mu_{0}I}{2\pi r}
\end{gather}
$$
Which represents the magnitude of the magnetic field. Let's take a look at $P_{1}$

![[Pasted image 20240308165355.png|center|300]]

**Note, there should be a $2I$ in the upper left hand corner**. As mentioned in the picture, the magnetic field from the two wires that have current pointing out of the page equal 0! This means that for $P_{1}$ we only have to concerns ourselves with the wire coming with intensity pointing into the page ($2I$ wire):
$$
\begin{gather}
B_{P_{1}} = \frac{\mu_{0}I}{2\pi(\sqrt{ 2 }d)} = \boxed{\frac{\mu_{0}I\sqrt{ 2 }}{\pi d}}
\end{gather}
$$

Let's take a look at $P_{2}$

![[Pasted image 20240308170351.png|center|300]]

We see that the magnetic field contribution from the two non diagonal wires ($I$) combined, points in the antiparallel direction as the diagonal wire ($2I$). This means (since the change in current is exactly the change in the magnetic field in this case) the total field should be zero at $P_{2}$:
$$
\begin{gather}
\boxed{B_{P_{2}} = 0}
\end{gather}
$$

#### 6.37

This question is similar to a question we did long ago, so we can apply the same method! That is, there is a trick I applied that requires superposition. Here's a picture: 

![[Pasted image 20240308235502.png|center]]


As crafted in the picture, we can analogize a singular copper rod with 900 amps (with a off-center hole), as two copper rods, the outer with 1200 amps, inner with 300 amps, as a single rod unit with 900 amps. This gives: 
$$
\begin{gather}
B_{\text{2 rods}} = B_{\text{outer rod}} +B_{\text{inner rod}}
\end{gather}
$$
Because the magnetic field at $r=0$ or in the middle of the rod is 0, the magnetic field is just:
$$
\begin{gather}
B_{2 rods} = B_{\text{inner rod}} \\ \\ 
B_{\text{inner rod}} = \frac{2I}{rc} = \frac{2(300amps)}{(.002cm)\left( \frac{3.0*10^8m}{s} \right)} = \frac{\left(4\pi\cdot10^{-7}\right)\left(300\right)}{2\left(.002\right)\pi} = .003T \\ \ \
.003T \rightarrow 10^4(.003)G = \boxed{30G}
\end{gather}
$$

Since the direction of the current of the smaller rod is out of the page, then the direction of the magnetic field is counter clockwise!

#### 6.50

Let's start by drawing a picture:

![[Pasted image 20240309004239.png|center|300]]

We can actually approximate this by splitting the wire up into its components! If we look closely, it can be divided between two straight wires who have antiparallel currents, and a half circle:

![[Pasted image 20240309005339.png|center|300]]

The two antiparallel wires have a magnetic field pointing in the same direction. That is, using the right hand rule, their magnetic field point out of the screen even though their current components are antiparallel. Thus their components add. They each contribute half the magnetic field of a singular wire under our regular circumstances. The half ring contributes half the magnetic field provided in the expression of equation 6.54 which gives the magnetic field of a point at the center of a ring. Thus the electric field at point $P$ is: 
$$
\begin{gather}
B_{\text{net}}=B_{\text{half wires}} +B_{\text{half ring}}= \frac{\mu_{0}I}{2\pi r}+ \frac{\mu_{0} I}{4r} = \boxed{\frac{(\pi+2)\mu_{0}I}{4\pi r}}
\end{gather}
$$


#### 6.51

Let's draw a picture!

![[Pasted image 20240309013653.png|center|300]]

We'll notice that this question actually condenses to a similar example we solved in the book! More specifically, the example of a circular ring in chapter 6.5 gives us the proper details to solve this problem. The "equator" around the Earth's metallic core can be approximated as such circular ring. Thus we'll use the following equation for the magnetic field: 

$$
\begin{gather}
B_{z} = \frac{\mu_{0}Ib^{2}}{2(b^{2}+z^{2})^{3/2}} \\ \\ 
\text{solve for} \hspace{.2cm} I: \\ \\ 
I = \frac{B_{z}(2(b^{2}+z^{2})^{3/2})}{\mu_{0}Ib^{2}}
\end{gather}
$$
Now, in this case, $b$ represents the radius of the metallic core which is 3000 km or $3*10^6$m. $z$ is the distance from the center of the metallic core to the north pole which is $6*10^6$ m. We're given $B_{z} = .5G = 5*10^{-5}T$, and $\mu_{0}= 4\pi*10^-7 \frac{kgm}{C^{2}}$. Thus the intensity equals:
$$
\begin{gather}
I = \frac{\left(5\cdot10^{-5}\right)2\left(\left(3.0\cdot10^{6}\right)^{2}+\left(6\cdot10^{6}\right)^{2}\right)^{\frac{3}{2}}}{\left(4\pi\cdot10^{-7}\right)\cdot\left(3.0\cdot10^{6}\right)^{2}} = 2.67\times10^{9} amps
\end{gather}
$$
That pretty dang big. 


***Enjoy your spring break!***
