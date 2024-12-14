#### 7.22

We know in general the flux through a solenoid (or more specifically through loop $C$), 
$$
\begin{gather}
\Phi= \pi r^{2}B \\ \\ 
\Phi = \pi r^{2} B_{0}(\sin(\omega t+\alpha))
\end{gather}
$$
Where $B_{0}$ is the amplitude, where $\omega$ is the angular frequency, and $\alpha$ is the position of the loop according to equation 7.20. Thus we have
$$
\begin{gather}
\mathcal{E} = -\frac{d\Phi}{dt} = -\pi r^{2}(B\omega )\cos(\omega t+\alpha)
\end{gather}
$$
The maximum magnitude of the oscillating electromotive force is when $\cos(\omega t+\alpha)=1$. Thus, similar to equation $7.22$, we have that,
$$
\begin{gather}
\mathcal{E}_{0} = B_{0}\pi r^{2}(\omega )
\end{gather}
$$
From page 359 we have that, 
$$
\begin{gather}
E = \frac{\mathcal{E}_{0}}{2\pi r} = \frac{B_{0}r}{2}(\omega) \\ \\
= (.0004T)\frac{.03m}{2} \frac{5\pi*10^6}{s} = 94 \frac{V}{m}
\end{gather}
$$

#### 7.26

We have the following picture

![[Pasted image 20240401202712.png|center]]

The magnetic field points out of the screen, thus using the right hand rule, the sea of charges in the metal bar experience a force that points down. We know this as the electromotive force. Similarly, there is also a force in the opposite direction of the velocity of the bar which we shall derive. We begin our analysis by finding the change in magnetic flux: 
$$
\begin{gather}
\frac{d\Phi(t)}{dt} = \frac{d}{dt}\int B \, da  = B(bv)
\end{gather}
$$
This gives us the value of the electromotive force $\varepsilon$. Further, we know from the section on Thevenin's theorem that
$$
\begin{gather}
-\frac{d\Phi(t)}{dt} = \mathcal{E} = IR \rightarrow \frac{\mathcal{E}}{R} = I
\end{gather}
$$
Thus we have 
$$
\begin{gather}
I(t) = \frac{B(bv)}{R}
\end{gather}
$$
We can use this current that we just found and plug it into the following equation that relates the current flowing through a wire with the force that acts upon it given by 6.14
$$
\begin{gather}
F =-IBb = -\left( \frac{B(bv)}{R} \right)Bb = -\frac{B^{2}b^{2}v}{R}
\end{gather}
$$
as it occurs in the opposite direction of the velocity. In general, we know that $F = ma = m\frac{dv}{dt}$, thus it we solve the differential equation using separation of variables,
$$
\begin{gather}
-\frac{B^{2}b^{2}v}{R}  = m \frac{dv}{dt} \\ \\ 
\frac{-B^{2}b^{2}v}{mR} = \frac{dv}{dt} \\ \\ 
-\frac{B^{2}b^{2}}{mR}\int  \, dt  = \int \frac{1}{v} \, dv \\ \\ 
-\frac{B^{2}b^{2}}{mR}t = \ln(v)  \\ \\ 
e^{ -\frac{B^{2}b^{2}}{mR}t }  = v
\end{gather}
$$
Thus, $v$ exponentially decays so it should never stop changing with respect to time, meaning that the rod, no matter how slow its velocity may be as time goes on, **continues to move**. 


#### 7.29

Let's first draw a picture!

![[Pasted image 20240331225836.png|center|400]]

We can find the electromotive force $\mathcal{E}$ as
$$
\begin{gather}
\mathcal{E}= wv(B_{1}-B_{2})
\end{gather}
$$
where we know the following quantities: 
$$
\begin{gather}
w = .08 m \\ \\ 
v = 5 \frac{m}{s} \\ \\ 
B_{1} = \frac{\mu_{0}I}{2\pi(.15)} \\ \ \
B_{2} = \frac{\mu_{0}I}{2\pi(.25)}
\end{gather}
$$
Thus we have the electromotive force. 

$$
\begin{gather}
\mathcal{E} = (.08m)\left( \frac{5m}{s} \right)\left( \frac{\mu_{0}(100A)}{2\pi(.1m)} \right) = 5.3*10^{-5} V
\end{gather}
$$
Thus if we have the following relationship,
$$
\begin{gather}
\mathcal{E} = RI \\ \\ 
\text{where}\hspace{.5cm}\frac{\mathcal{E}}{R}\approx 0 
\end{gather}
$$
we want a large resistance $R$ such that the current is approximately zero, thus we can choose the resistance to be $1\hspace{.2cm}ohm$ or greater. 

#### 7.30

![[Pasted image 20240402005333.png|center|300]]


Since the loop moves through a changing magnetic field, there's a force applied to the loop. The work necessary to keep the velocity constant is just the opposite magnitude of that force.  We can find the force due to the magnetic field with the same equation we use for 7.26, and then take the opposite of that, 
$$
\begin{gather}
Fv = I(B_{1}-B_{2})wv \\ \\
F =I(B_{1}-B_{2})w  \\ \\ 
(B_{1}-B_{2}) = \frac{IR}{wv} \\ \\
F = I^{2}R
\end{gather}
$$
This is the amount work required to move the loop over some time $dt$. As for the amount of energy dissipated over the same interval of time, we recognize that a reference to the power dissipated over the resistor during such a time can be used  
$$
\begin{gather}
P=I^{2}R
\end{gather}
$$



#### 7.44

We're given on page 368, the energy density in a magnetic field as 
$$
\begin{gather}
B_{U} = \frac{1}{2\mu_{0}}B^{2}
\end{gather}
$$
Given that $B = 3*10^{-10}T$, we have the energy density 
$$
\begin{gather}
B_{U} = \frac{1}{2(1.257*10^{-10}) \frac{Tm}{A}} (3*10^{-10}T)^{2} = 3.58*10^{-14} \frac{J}{m^{3}}
\end{gather}
$$
The total volume of a disk is $\pi r^{2}w$ where $w$ is the width. Thus we multiply this volume by the energy in the magnetic field of the galaxy
$$
\begin{gather}
 3.58*10^{-14} \frac{J}{m^{3}} \left( \pi\left( \frac{1}{2}*10^{21} m\right)^2 *10^{19}m\right) = 2.81*10^{47}J
\end{gather}
$$
Using the fact that all the stars in the galaxy radiate about $\frac{10^{37}J}{s}$ we can divide this quantity by what we have for the energy in the magnetic field. 
$$
\begin{gather}
\frac{2.81*10^{47}J}{10^{37} \frac{J}{s}} = 2.81*10^{10}s \approx 888y
\end{gather}
$$
That's not very long when we think about the age of the universe and the age of the bodies of such stars involved!

#### 7.45

From the previous question, we have that
$$
\begin{gather}
B_{U} = \frac{1}{2\mu_{0}}B^{2} \\ \ \
B_{U} = \frac{\left(10^{10}\right)^{2}}{2\left(1.257\cdot10^{-6}\right)} =3.98*10^{25} \frac{J}{m^{3}}\\ \\ 
\end{gather}
$$
we'll notice that $J = \frac{kgm^{2}}{s^{2}}$ thus the units of our energy density $B_{U}$ is $\frac{kg}{ms^{2}}$. In order to get the proper units, we need to divide by the speed of light squared according to $E=mc^{2}$. Thus 
$$
\begin{gather}
3.98*10^{25} \frac{J}{m^{3}} \left( 3.0*10^8 \frac{m}{s} \right)^{-2} = 4.4*10^{8} \frac{kg}{m^{3}}
\end{gather}
$$

#### 7.46
Let's grab the original picture

![[Screenshot 2024-04-02 at 2.46.55 AM.png|center|300]]

we want to find $\tau = \mu_{0}a\sigma$ given the following information, 
$$
\begin{gather}
U = \frac{B^{2}}{2\mu_{0}}(vol) \\ \\ 
R\approx \frac{\pi}{a\sigma} \\ \\
B = \frac{\mu_{0}I^{2}}{a}
\end{gather}
$$
Thus we can plug that information into $\tau=\frac{U}{I^{2}R}$ 
$$
\begin{gather}
\tau = \frac{\left( \frac{B^{2}}{2\mu_{0}} (\pi a^{3})\right)}{I^{2}\left( \frac{\pi}{a\sigma} \right)} =
 \frac{\left( \frac{\left( \frac{\mu_{0}I}{a} \right)^{2}}{2\mu_{0}} (\pi a^{3})\right)}{I^{2}\left( \frac{\pi}{a\sigma} \right)} \\ \\ 
 =\frac{\mu_{0}\pi I^2a}{2I^{2}\left( \frac{\pi}{a\sigma} \right)} = \frac{\mu_{0}a^{2}\sigma}{2}\approx \mu_{0}a^{2}\sigma
\end{gather}
$$
We now plug in $a =3000km$ and the conductivity $\sigma = 10^{16}(ohm-m)^{-1}$
$$
\begin{gather}
\tau = \left( 4\pi*10^{-7} \frac{kgm}{C^{2}} \right)(10^{16}(ohm-m)^{-1})(3000km)^{2} \approx 1*10^{13}s
\end{gather}
$$
#### 7.47

![[Screenshot 2024-04-02 at 3.01.59 AM.png|center|200]]

The picture is above! Since the disk and rod are both metals, they can be considered sea of charges. In either direction the current flows across the disk, the magnetic field will point parallel to the rod. Now looking at the direction of each dynamo, we can see the direction of the velocity, and we already know the direction of the magnetic field  The trick here is to consider handedness such that, if we know the direction of velocity and magnetic field, we know the direction of the force. Using the right hand rule, if the velocity travels counterclockwise looking from the top, the force points inwards, which is what we don't want as it would eventually decrease the current flow. Thus we would consider the bottom figure to be the potential dynamo!

#### 6.41

Using equation 6.24 (as we've developed in chapter two), we'll use Stokes Theorem such that 
$$
\begin{gather}
\int _{C}F \, ds = \int _{S}\nabla \times F \, da  
\end{gather}
$$
Where $F$ is some vector, $C$ is some boundary (curve), $S$ is some domain (surface). Thus applying this to the vector potential $A$, 
$$
\begin{gather}
\int _{C}A \, ds  = \int _{S} \nabla \times A \, da = \int _{S}B \, da = \Phi 
\end{gather}
$$

#### 6.49 
We'll first start of by drawing a picture!

![[Pasted image 20240401004423.png|center|300]]

We know generally for the uniform surface charge of a disk
$$
\begin{gather}
\lambda = \frac{dq}{2\pi dr} \\ \\ 
dq = \lambda 2\pi dr
\end{gather}
$$
we know that the current as a function of time is 
$$
\begin{gather}
I = \frac{dq}{dt} = \frac{2\pi\lambda  dr}{dt}
\end{gather}
$$
we'll notice that $\frac{dr}{dt}$ is velocity equal to $r\omega$ thus 
$$
\begin{gather}
I = 2\pi\lambda r\omega
\end{gather}
$$
We can connect this to the Biot Savart Law which is 
$$
\begin{gather}
dB = \frac{\mu_{0}I}{4\pi} \frac{dl\times r}{r^{3}}
\end{gather}
$$
The reason why we can use the Biot Savart law here, is because it follows for finding the magnetic field of the small length $dl$ on the rim of the disk. We can integrate this from $0$ to $R$ once we've plugged in and simplified for $dB$ such that
$$
\begin{gather}
dB = \frac{\mu_{0}}{4\pi}(2\pi\lambda r\omega) \frac{dl\times r}{r^{3}} \\ \\ 
dB = \frac{\mu_{0}}{2}\lambda r\omega \left( \frac{dlr}{r^{3}} \right) = \frac{\mu_{0}}{2}\lambda\omega\left( \frac{dl}{r} \right)
\end{gather}
$$
We notice that we can divide the linear charge density $\frac{\lambda}{r}$ to get $\sigma$. Thus, 
$$
\begin{gather}
\frac{\mu_{0}}{2}\sigma \omega dl
\end{gather}
$$

Now we integrate: 
$$
\begin{gather}
\int dB  = \int _{0}^R \frac{\mu_{0}}{2}\sigma \omega dl = \frac{\mu_{0}\sigma\omega R}{2} = B
\end{gather}
$$
Thus inside the disk, the magnetic field is uniform, and so it equals the $B$ we just found.


