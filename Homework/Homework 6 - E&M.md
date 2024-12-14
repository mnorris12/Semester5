#### 5.10

Let's draw a picture

![[Pasted image 20240229170703.png|center|300]]

We first find the electric field. The electric field should be: 
$$
\begin{gather}
E = \frac{V}{d} \\ \\
E = \frac{300}{\left( \frac{2}{100} \right)} = 1.5*10^4 
\end{gather}
$$
To find the number of electrons on the plate, we know that 
$$
\begin{gather}
VC=Q \hspace{.2cm} \text{where we have V} \hspace{.2cm}
\end{gather}
$$
So we must calculate $C$:
$$
\begin{gather}
C = \frac{A\epsilon_{0}}{l} = \frac{200cm}{\left( 2 \right)}\epsilon_{0} = 1m\epsilon_{0} \\ \\
\text{Thus} \hspace{.2cm} Q= (1m\epsilon_{0})(300) = (300\epsilon_{0}) = 2.6562*10^{-9}C \\ \\
\text{the charge of one electron is} \hspace{.2cm} 1.602*10^{-19} \\ \\
\frac{2.6562*10^{-9}}{1.602*10^{-19}} = 1.658*10^{10}
\text{electrons} \hspace{.2cm}\end{gather}
$$
Now let's think about motion!

When the frame of reference is moving eastward
- Q is invariant as usual
- The electric field should increase
$$
\begin{gather}
E'_{z} = \frac{E_{z}}{\sqrt{ 1- .6^2 }} = 18750
\end{gather}
$$
- Dimensions from $E\rightarrow E'$:
	- $20cm \rightarrow 20cm$
	- $10cm \rightarrow 10cm$
	- $2cm \rightarrow \frac{2cm}{\gamma} = \frac{16}{100}m$


When the frame of reference is moving westward: 
- Q is invariant as usual
- the electric field shouldn't change 
- Dimensions from $E \rightarrow E'$:
	- $20cm\rightarrow 20cm$
	- $10cm\rightarrow 10cm$
	- $2cm\rightarrow \frac{2}{\sqrt{ 1- .6^2 }} = 1.6$


#### 5.11

##### a

First we find the average separation between electrons. We know that the current is $\frac{5*10^{-8}C}{s}$. We now need to solve for $\beta$: 
$$
\begin{gather}
\beta = \sqrt{ 1-\frac{1}{\gamma^{2}} } = \sqrt{ 1-\frac{1}{(20)^{2}} } =  0.9987492178 \\ \\
\end{gather}
$$
We also know that $V_{0} = \beta c = 2.996*10^{8} \frac{m}{s}$. We can divide the value of the current by by the charge of an individual electron which will give us the number of electrons per second that passes through: 
$$
\begin{gather}
\frac{\left( 5*10^{-8} \frac{C}{s} \right)}{1.602*10^{-19}C} = 3.12500733\times10^{11} s^{-1}
\end{gather}
$$
Thus the average number of space between them should be this their initial speed $V_{0}$ divided by the previous mathline: 

$$
\begin{gather}
\frac{\left( 2.996*10^{8} \frac{m}{s} \right)}{3.12500733\times10^{11} s^{-1}} = 9.58797\times10^{-4} m
\end{gather}
$$
which is $\approx 1mm$

To find the electric field, we can use the fact that it's an electron beam, so it should be modeled as follows: 
$$
\begin{gather}
E= \frac{\lambda}{2\pi\epsilon_{0}r}
\end{gather}
$$
We first find the linear charge density
$$
\begin{gather}
\frac{\text{current}}{\text{speed of an electrons} \hspace{.2cm}} = \frac{ 5*10^{-8} \frac{C}{s} }{2.996*10^8 \frac{m}{s}} = 1.671*10^{-16} \frac{C}{m}
\end{gather}
$$
Thus the electric field should be:
$$
\begin{gather}
E = \frac{\left( 1.671*10^{-16} \frac{C}{m} \right)}{2\pi (8.854*10^{-12})1cm} = \boxed{3.00370352\times10^{-4} \frac{V}{m}}

\end{gather}
$$
##### b

We'll have to recalculate the average distance, this time in the frame of the electrons. The change in the separation can be accounted for by multiplying its value in the lab frame by a factor of $\gamma$:
$$
\begin{gather}
d' = d\gamma = 20(1mm) = 20mm = .02 m
\end{gather}
$$
The linear charge density changes by a factor of $\frac{1}{\gamma}$ so, so should the electric field: 
$$
\begin{gather}
\boxed{E' = \frac{\lambda}{2\pi\epsilon_{0}r} \frac{1}{\gamma} = 1.44 \cdot10^{-5} \frac{V}{m}}
\end{gather}
$$

#### 5.15

All we have to do show equation (5.15) holds for Gauss's law, is integrate the primed electric field. What's a little more subtle is that we have to know the change in area in the integral, or that $dA - r'^{2}\sin\theta d\theta d\phi$

$$
\begin{gather}
E' = \frac{Qk}{\gamma r'^{2}} \int \frac{1}{(1-\beta^{2}\sin^2\theta')^{3/2}} \, dA  \\ \\ 
dA = r'^{2} \sin\theta d\theta d\phi \\ \\ 
E' = \frac{Qk}{\gamma}\iint_{0}^\pi \frac{\sin\theta'}{(1-\beta^{2}\sin^2\theta')^{3/2}}\, d\theta d\phi \\ \\ 
E' = Qk \int_{0}^{2\pi} 2\pi \, d\phi  = \frac{Q 4\pi}{4\pi\epsilon_{0}} = \boxed{\frac{Q}{\epsilon_{0}}}
\end{gather}
$$
We're all set 

#### 5.16

We know the perpendicular component of the electric field: 
$$
\begin{gather}
E' = \frac{Q}{4\pi\epsilon_{0}r'^{2}} \leftarrow \hspace{.2cm} \text{where} \hspace{.2cm} r' = r \hspace{.5cm}\text{no length contraction} \hspace{.2cm} \\ \\ 
1 \frac{V}{m} = 10^{10} \frac{Q}{4\pi\epsilon_{0}r^{2}} \\ \\ 
\frac{4\pi\epsilon_{0}r^{2}}{10^{10}} = Q = 1.602*10^{-19} \\ \\ 
r = \sqrt{ \frac{Q10^{10}}{4\pi\epsilon_{0}} } \\ \\ 
\boxed{r= 3.795}
\end{gather}
$$
The thickness of the pancake corresponds with the $r'$:
$$
\begin{gather}
r' = \frac{r}{\gamma} \\ \\ 
r' = \frac{3.795}{10^{10}} = \boxed{3.79451754\times10^{-10}}
\end{gather}
$$
#### 5.18

Usually we see the following diagram after some time $t=0$

![[Pasted image 20240229194402.png|center|300]]
##### a

The diagram itself suggests that an electron that was previously stationary, then accelerated with some velocity causing the electric field lines to appear as it does at time $t=0$. The radius of the pancake is $15$cm. We also can calculate how long it took the information (field lines) to reach $.015$m: 
$$
\begin{gather}
\frac{.015}{(3.0*10^8)} = 5*10^{-10}s
\end{gather}
$$
![[Pasted image 20240229201138.png|center|300]]

All the outer field lines point directly to time $t=12$, we can also look at the only perpendicular outer field line to tell at what time the electron stopped on the axis. Thus we can find the speed of the electron: 
$$
\begin{gather}
\frac{\left( \frac{12}{100} \right)}{5*10^{-10}} = \boxed{2.4*10^{8} \frac{m}{s}}
\end{gather}
$$

##### b

To find the electron at $t= -7.5*10^{-10}s$, this should correspond to the position of the electron before $0$cm, thus we'll add the time it took to get to time $t=0$ and the time we want in question for our answer: 
$$
\begin{gather}
\left(2.4\cdot10^{8}\cdot\left(-2.5\cdot10^{-10}\right)\right)s =\boxed{ - .06 m }
\end{gather}
$$
##### c
We have to use the following equation: 
$$
\begin{gather}
E' = \frac{Q}{4\pi\epsilon_{0}r'^{2}} \frac{1-\beta^{2}}{(1-\beta^{2}\sin ^{2}(\theta))^{3/2}} = \frac{\left(1.602\cdot10^{-19}\right)}{4\pi\cdot\left(8.854\cdot10^{-12}\right)\left(.06\right)^{2}}\left(1-\left(.8\right)^{2}\right) \\ \\ 
= \boxed{1.43983634\times10^{-7} \frac{V}{m}}
\end{gather}
$$
#### 5.19

We'll draw a picture and explain how it works!

![[Pasted image 20240304230157.png|center|300]]

The picture above describes the collision of the two particles. Since the kenetic energy has dissipated and no charge remains after the collision, we expect at some time $t$ that there is no charge enclosed by the radius $ct$ that joins the positive and negative charges. The field lines in blue and red represent the how they would be had the two charged not interacted after some time $t$.

According to appendix H, which provides the radiation by an accelerated charge (in this case two), the electric field would be determined by the following equation:
$$
\begin{gather}
\boxed{E_{\theta} = \frac{qa\sin\theta}{4\pi\epsilon_{0}c^{2}R}}
\end{gather}
$$
This would imply that as time continues, and thus the radius $ct$ continues (the sphere grows), the electric field lines fall of at a rate proportional to $\frac{1}{R}$.  
#### 5.20

We set the following equations equal to each other: 
$$
\begin{gather}
\Phi_{EA} = \Phi_{FD} \\ \\ 
 \frac{\frac{Q2\pi}{4\pi\epsilon_{0}}}{\frac{Q2\pi}{4\pi\epsilon_{0}}}\int_{0}^{\theta_{0}}\sin\theta \, d\theta  = \frac{1}{\gamma^{2}}\int_{0}^{\phi_{0}} \frac{\sin\theta}{(1-\beta^{2}\sin ^{2}\phi)^{3/2}}  \, d\phi \\ \\ 
  \int_{0}^{\theta_{0}}\sin\theta \, d\theta = \frac{1}{\gamma^{2}}\int_{0}^{\phi_{0}} \frac{\sin\phi}{(1-\beta^{2}\sin ^{2}\phi)^{3/2}}  \, d\phi \\ \\ 
  -\cos(\theta) + 1 = \frac{1}{\gamma^{2}}\left( -\frac{\cos \phi}{(1-\beta^{2})\sqrt{ 1-\beta^{2}\sin\theta }} \right)|_{0}^{\phi_{0}} \\ \\ 
  \cos\theta = \frac{\cos \phi}{\sqrt{1-\beta^{2}\sin ^{2}\phi }} \\ \\ 

  
\end{gather}
$$
we'll focus specifically on the right side of the equation: 
$$
\begin{gather}
\frac{\cos \phi}{\sqrt{1-\beta^{2}\sin ^{2}\phi }} = \frac{1}{\sqrt{\sec ^{2}\phi-\beta^{2}\tan ^{2}\phi }}
\\ \\ 
= \frac{1}{\sqrt{ 1+\tan ^{2}\phi-\beta^{2}\tan ^{2}\phi }} = \frac{1}{\sqrt{ 1+\tan ^{2}\phi(1-\beta^{2}) }}
\end{gather}
$$
now we bring them back together
$$
\begin{gather}
\cos\theta = \frac{1}{\sqrt{ 1+\tan ^{2}\phi(1-\beta^{2}) }} \\ \\ 
\cos(\theta) \sqrt{ 1+\tan ^{2}\phi(1-\beta^{2}) } = 1 \\ \\ 
\cos ^{2}\theta(1+\tan ^{2}\phi(1-\beta^{2})) = 1 \\ \\ 
1-\cos ^{2}\theta = \frac{\cos ^{2}\theta \tan ^{2}\phi}{\gamma^{2}} \\ \\ 
\gamma^{2}\sin ^{2}\theta = \cos ^{2}\theta \tan ^{2}\phi \\ \\
\boxed{\gamma \tan\theta=\tan \phi}
\end{gather}
$$
We're all set!

#### 1.

The following is a spacetime diagram of the event!

![[Screenshot 2024-03-04 at 11.59.43 PM.png|center|300]]

The axis lines from $t',x'$ have been determined by: 
$$
\begin{gather}
t' = \frac{1}{\beta} \hspace{.5cm} x' = \beta \\ \\ 
t' = 2 \hspace{.5cm} x'=\frac{1}{2}
\end{gather}
$$

We know from appendix G2 that: 
$$

\begin{gather}
x' = \gamma x-\frac{\gamma\beta t}{c} \hspace{.5cm}t'= \gamma t-\frac{\gamma\beta x}{c} \\ \ \

\boxed{x' \approx 4.62 \hspace{.5cm}t'\approx 6.92}
\end{gather}
$$
#### 2.

Let's draw a picture!

![[Screenshot 2024-03-05 at 1.42.35 PM.png|center|300]]

We'll first determine the axis lines from $t',x'$ have been determined by: 
$$
\begin{gather}
t' = \frac{1}{\beta} \hspace{.5cm} x' = \beta \\ \\ 
t' =\frac{5}{3} \hspace{.5cm} x' = \frac{3}{5}
\end{gather}
$$
We know from appendix G2: 
$$
\begin{gather}
x' = \gamma x - \frac{\gamma\beta t}{c} \hspace{.5cm} t' = \gamma t - \frac{\gamma\beta x}{c} \\ \\ 
\boxed{x' = 6.25 \hspace{.5cm} t' = 1.87}
\end{gather}
$$
We're all set!