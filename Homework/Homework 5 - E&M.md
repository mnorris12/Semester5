#### 4.19

We have from equation 4.6, we have that: 
$$
\begin{gather}
\mathbf{J}_{e} = -eN_{e} \bar{\mathbf{u}}
\end{gather}
$$
This will give us the electron density inside the electron synchrotron using the average velocity of all $10^{11}$ electrons. We know in general that the current $I =JA$. Thus we have
$$
\begin{gather}
I = (-eN_{e} \bar{\mathbf{u}})A = -\frac{4806}{\text{Vol}}A \left( \frac{C}{s} \right) = -\frac{4806}{L}\left( \frac{C}{s} \right) = -\frac{4806}{240} \left( \frac{C}{s} \right) = \\ \\ 
I = - .02 \frac{C}{s}
\end{gather}
$$
We actually note here that the current flow is opposite of the direction of the electron, so it should be: 
$$
\begin{gather}
I = .02 \left( \frac{C}{s} \right)
\end{gather}
$$
We're all set!

#### 4.26

Let's Draw ourselves a nice picture: 

![[Pasted image 20240224204039 1.png|center|500]]

I thought this problem, in its nature, was a lot similar to having two conducting slabs, as modeled in figure 3.14 and equation 3.12 in Purcell. The n-type semi-conductor and its negative junction slab provides a similar problem to a conductor slab and its surface charge (the same would be true for the p-type) That is, the above model is similar to: 

![[Pasted image 20240224204717.png|center|400]]

As a result, we can use equation 3.12:
$$
\begin{gather}
\sigma = \frac{\epsilon_{0}(V)}{s}
\end{gather}
$$
The important difference is that our slab is three dimensional, so we wouldn't want the surface charge which is what the above equation gives us. Instead, the charge density of the slab is 
$$
\begin{gather}
\sigma_{slab} = \frac{\epsilon_{0}(V)}{s^{2}} \\ \\ 
\end{gather}
$$
You can work out the units to find that $\sigma_{slab} = \frac{C}{m^{3}}$, which is the charge per volume we want! Okay, now time to plug in!

$$
\begin{gather}
\frac{(8.854*10^{-12})\left[ \frac{C^{2}}{Nm^{2}} \right](.3)\left[ \frac{Nm}{C} \right]}{(10^{-4})^{2}[m^{2}]} = 2.66 \cdot 10^{-4} \left[ \frac{C}{m^{3}} \right]
\end{gather}
$$
This value would be for the positive slab, and its negative counterpart will be for the negative slab. 

Now we consider drawing a graph that models the potential as a function of position. We can actually use Poisson's equation here: 
$$
\begin{gather}
\text{negative slab:} \hspace{.3cm}\frac{d^{2}\phi}{dx^{2}} = -\frac{(-\sigma)}{\epsilon_{0}} \hspace{.5cm}\leftarrow \text{concave up } \hspace{.2cm} \\ \\ 
\text{positive slab:} \hspace{.3cm}\frac{d^{2}\phi}{dx^{2}} = -\frac{(\sigma)}{\epsilon_{0}} \hspace{.5cm}\leftarrow \text{concave down} \hspace{.2cm}

\end{gather}
$$
Thus we have the following graph:

![[Pasted image 20240224212459.png|center|400]]


Lastly, for the electric field in the mid-plane, we can use the idea of flux: 
$$
\begin{gather}
\sigma = \frac{Q}{vol}  \hspace{.9cm} \phi=\oint E\cdot da \\ \\
EA = \frac{Q}{\epsilon_{0}} = \frac{\sigma \cdot vol}{\epsilon_{0}} \\ \\ 
E = \frac{\sigma vol}{A\epsilon_{0}} = \frac{\sigma d}{\epsilon_{0}}
\end{gather}
$$
where $d$ is the thickness of either of the slabs. This idea works because the electric field should be the same for either of the slabs, so it should be same for the mid-plane.

#### 4.29

We'll note that we can actually reduce the system of resistors: 
1. 
![[Pasted image 20240225022234.png|center|300]]
2. ![[Pasted image 20240225022358.png|center|300]]
3. ![[Pasted image 20240225022636.png|center|300]]
![[Pasted image 20240225022952.png|center|300]]


It looks like we've managed to reduce the circuit and find the equivalent resistance $R_{eq}$! To find the input resistance, we need to set the value of the equivalent resistance to $R_{0}$: 
$$
\begin{gather}
\frac{3R_{1}^{2}+2R_{1}R_{0}}{2R_{1}+R_{0}} = R_{0} \\ \\ 
3R_{1}^{2}+2R_{1}R_{0} = 2R_{0}R_{1} +R_{0}^{2} \\ \\ 
3R_{1}^{2} = R_{0}^{2} \\ \\ 
R_{1} = R_{0}\sqrt{ \frac{1}{3} }
\end{gather}
$$
Looks like we're all done!
#### 4.32

We have two graphite rods. We'll call the cylindrical one Craig and the other conical one Jimmy because why not. We have the following picture:

![[Pasted image 20240225001623.png|center|300]]

We have from equation 4.15, the resistance:
$$
\begin{gather}
R = \frac{L}{\sigma A}
\end{gather}
$$
We'll note that since Craig and Jimmy have the same length and are made of the same material, so the only change in Resistivity is given by a function of area, or more precisely, a function of radius. That is, the difference in their radius is the difference in the resistivity. Hopefully that's $\frac{a}{b}$.  

Thus we have that:
$$
\begin{gather}
R_{cyl} \sim R_{cone} \\ \\ 
\frac{L}{\sigma \pi( a)^{2}} = \frac{L}{\sigma \pi( b\eta)^{2}} \\ \\ 
\frac{1}{a^{2}} =\frac{1}{b^{2}\eta^{2}} \\ \\ 
a^{2} = b^{2} \eta^{2} \\ \\ 
\eta = \frac{a}{b}
\end{gather}
$$
thus the only change in the resistivity between Craig and Jimmy is $\eta=\frac{a}{b}$ or: 

$$
\begin{gather}
\frac{a}{b}R_{cyl} = R_{cone}
\end{gather}
$$

#### 4.36

Let's first draw a picture

![[Pasted image 20240225185755.png|center|500]]

That is we can model the infinite series like the first circuit which can effectively by modeled as the second picture. Thus we can solve for $R_{eq} = R$:
$$
\begin{gather}
R_{1} + \frac{R R_{2}}{R+R_{2}}= R \\ \\ 
R_{1}(R+R_{2}) +R R_{2} = R(R+R_{2}) \\ \\ 
-R^{2}+R_{1}R+R_{1}R_{2} = 0 \\ \\ 
\text{Binomial Approximation!} \hspace{.5cm} R = \frac{R_{1}+\sqrt{ R_{1} }\sqrt{ R_{1}+4R_{2} }}{2}
\end{gather}
$$
Where we've gone with positive binomial. We know prove the initial voltage decreases geometrically:

![[Pasted image 20240225190327.png|center|400]]

The current coming into an arbitrary box on the ladder is equal to the two current it splits into derived from our ordinary circuit rules. That is $I_{i} = I_{i1}+I_{i_{2}}$. Since each resistor between the nodes are the same, the split current that immediately travels down is $\frac{1}{a}$ (where $a$ is how much greater the initial current is than the split current) of the current coming into the box. Now let's focus further on that split current traveling down:

![[Pasted image 20240225190633.png|center|400]]

Then if $\frac{1}{a}I_{i} = I_{i_{1}}$ or $I_{i} = aI_{i_{1}}$, we can say that: 
$$
\begin{gather}
Ii = 2aI_{i_{1}}= 4aI_{i_{3}} = 8aI_{i_{5}} \dots
\end{gather}
$$
or simply that the current decreases geometrically. Since all the resistors between the nodes have the same value $R_{2}$ in the infinite ladder, then the voltage decrease should depend only on the current decrease. Thus the voltage decreases geometrically as well. 

#### 4.37

In question 4.36, we found our resistance to be: 
$$
\begin{gather}
R = \frac{R_{1}+\sqrt{ R_{1} }\sqrt{ R_{1}+4R_{2} }}{2}
\end{gather}
$$ 
under the conditions of this question $R_{1}= R_{2}$. Thus we'll use the above equation to solve for a new resistance $R_{new}$. For simplicity reasons, let's assume $R_{1}=R_{2}=1$:
$$
\begin{gather}
R_{new} = \frac{1+\sqrt{ 1 }\sqrt{ 1+4(1) }}{2} = \frac{1+\sqrt{ 5 }}{2}
\end{gather}
$$
Which is the golden ration. 
#### 4.39

We'll first start off by providing a picture! Luckily for us, figure 4.21 in Purcell works to describe our situation: 

![[Pasted image 20240225161221.png|center|300]]

Alright, let's talk Power: 
$$
\begin{gather}
P = I^{2}R = IV
\end{gather}
$$
We gather from figure 4.21 that $I = \frac{\mathcal{E}}{(R+R_{i})}$ and $V = \mathcal{E} - IR_{i}$. Thus we have that:
$$
\begin{gather}
P = \frac{\mathcal{E}}{R+R_{i}} (\mathcal{E} - IR_{i}) \\ \\ 
P = \frac{\mathcal{E}^{2}}{R+R_{i}} - \frac{\mathcal{E}IR_{i}}{R_{i}+R} = \frac{\mathcal{E}^{2}}{R+R_{i} } - \frac{\mathcal{E}^{2}R_{i}}{(R_{i}+R)^{2}} \\ \\ 
\text{used WolframAlpha to reduce} \hspace{.2cm} \\ \\ 

P = \frac{\mathcal{E}^{2}R}{(R_{i}+R)^{2}}
\end{gather}
$$
Now we'll want to find the derivative of $P$ with respect to $R$  and set that equal to 0. This should give us $R$  associated with the maximum or minimum value of the power. As you could imagine, the derivative immediately looks cumbersome, so again we use WolframAlpha:
$$
\begin{gather}
\frac{dP}{dR}  = \frac{\mathcal{E}^{2}(R-Ri)}{(R+R_{i})} = 0 \\ \\ 
\mathcal{E}^{2}(R-Ri) = 0 \\ \\
R-R_{i} = 0 \\ \\ 
R =R_{i}
\end{gather}
$$
Thus the value of $R$ at a maximum or minimum is $R_{i}$. We just need to find if this is a max or min. We'll consider the situation when $R\leq R_{i}$ and $R\geq R_{i}$:
$$
\begin{gather}
R\leq R_{i}:\hspace{.5cm} \frac{dP}{dR} = - \frac{\mathcal{E}^{2}(-\text{value})}{(+\text{value})} \rightarrow\text{+value} \hspace{.2cm}
\end{gather}
$$
Since the derivative is positive, then the power is increasing until $R=R_{i}$
$$
\begin{gather}
R\geq R_{i}: \hspace{.5cm}\frac{dP}{dR} = -\frac{\mathcal{E}^{2}(+\text{value})}{(+\text{value})} \rightarrow -\text{value} 
\end{gather}
$$
thus, after $R=R_{i}$ the derivative is negative, so the power is decreasing. 

We conclude that this suggests the behavior of a maximum when $R = R_{i}$!
#### 4.40 

We'll first start by drawing a picture:

![[Pasted image 20240225143944.png|center|300]]

We want to show that we can obtain values for the current specifically $I_{1}, I_{2}$ using ordinary circuit formulas, and that those values should be equal to the process that requires the conditions that $I_{1}+I_{2} =I_{0}$ and the minimum power dissipation. 

We'll start with the ordinary circuit formulas: 
$$
\begin{gather}
V_{1} = I_{1}R_{1} \\ \\ 
V_{2}= I_{2}R_{2} \\ \\ 
\text{since the resistors are in parallel} \hspace{.5cm} V_{1}=V_{2} \hspace{.5cm} \text{thus} \hspace{.2cm} \\ \\ 

I_{1}R_{1} = I_{2}R_{2} \\ \\ 
I_{1} = \frac{I_{2}R_{2}}{R_{1}}  \hspace{.5cm}\underbrace{ I_{2} = I_{0}-I_{1}  }_{ \text{ordinary Kirchhoff rules} \hspace{.2cm} } \\ \\ 
I_{1} =\frac{ R_{2}I_{0} - R_{2}I_{1}}{R_{1}} \\ \\ 
I_{1}R_{1} = R_{2}I_{0} - R_{2}I_{1} \\ \\ 
I_{1}(R_{1}+R_{2}) = R_{2}I_{0} \\ \\ 
I_{1} = \frac{R_{2}I_{0}}{(R_{1}+R_{2})}
\end{gather}
$$
We'll show we can get the same thing by minimizing the power:

We use the first requirement that $I_{1}+I_{2} = I_{0}$ or $I_{2} = I_{0}-I_{1}$. The requirement of the minimum power dissipation is that the total power dissipation $P_{tot} = P_{1}+P_{2}$ is a minimum because of the staple way current would distribute itself. In other words, the derivative of total power set equal zero will give you the current associated with the minimum value of the power. So we have: 
$$
\begin{gather}
P_{tot} = I_{1}^{2}R_{1}+(I_{0}-I_{1})^{2}R_{2} = (I_{1})^{2}R_{1}+R_{2}I_{0}^{2}-2R_{2}I_{0}I_{1}+R_{2}I_{1}^{2} \\ \\ 
\text{we now minimize!} \hspace{.2cm} \\ \\
\frac{dP_{tot}}{dI_{1}} = 2I_{1}R_{1} + 0 -2R_{2}I_{0} +2R_{2}I_{1} = 0 \\ \\ 
2I_{1}R_{1} + 2R_{2}I_{1} = 2R_{2}I_{0} \\ \\ 
I_{1}(2R_{1}+2R_{2}) = 2R_{2}I_{0} \\ \\
I_{1} = \frac{2R_{2}I_{0}}{2R_{1}+2R_{2}} = \frac{R_{2}I_{0}}{R_{1}+R_{2}}
\end{gather}
$$

Which is the same result as before! Pretty sweet. 


#### 4.46

We'll first start off by considering the open circuit voltage. To do that, we'll reduce the circuit given in figure 4.58 to the following:

![[Pasted image 20240225201651.png|center|300]]

That is, when the circuit is open, we can disregards the bottom loop as current doesn't flow through it. Thus we can find the current: 
$$
\begin{gather}
I = \frac{V}{R} \\ \\ 
I = \frac{120V}{20\Omega} = 6A
\end{gather}
$$
Next, $\mathcal{E}_{eq} = \frac{120V}{2}$ where the denominator comes from the quantity of the resistors in the circuit. The resistance $R_{eq}$ can be found when $\mathcal{E} = 0$ or the following diagram 

![[Pasted image 20240225203336.png|center|300]]

where the two 10 ohms circuits are in parallel, and then following circuit would be in series with the 15 ohms. Thus $R_{eq} = 15+5 = 20\Omega$ 

Using the suggested hint from exercise 4.39, the maximum power dissipated is when $R=R_{eq} = 20$. We also have that $I = \frac{\mathcal{E}}{(R_{eq}+R)} = 1.5 A$. We have that 
$$
\begin{gather}
P = I^{2}R= (1.5)^{2}(20) = 45 \frac{J}{s}
\end{gather}
$$
We're all done!

#### 4.48

The battery transfers a charge $Q_{f}$ (final charge) through a constant potential difference of $\mathcal{E}$. This tells us about the work that the battery must do: 
$$
\begin{gather}
W_{b} = Q_{f}\mathcal{E} \hspace{.5cm} Q_{f} \rightarrow \text{final charge on capacitor} \hspace{.2cm}
\end{gather}
$$
We'll show this again by finding the work due to the following: 
$$
\begin{gather}
W = E_{\text{capacitor}} +E_{\text{resistor}}
\end{gather}
$$
 The final energy of the capacitor equals half the work required to bring charge $Q_{f}$ through our potential difference: 
$$
\begin{gather}
E_{\text{capacitor}} = \frac{Q_{f}\mathcal{E}}{2}
\end{gather}
$$
and the energy dissipated from the resistor requires an integral of the power: 
$$
\begin{gather}
\int _{0}^\infty I^{2}R\, dx = \frac{\mathcal{E}^{2}}{R} \int _{0}^\infty e^{ \frac{-2t}{RC} }\, dt \\ \\ 

= -\frac{\mathcal{E}Q_{f}}{2} e^{ \frac{-2t}{RC} }|_{0}^\infty = \frac{\mathcal{E}Q_{f}}{2} = E_{\text{resistor}}
\end{gather}
$$
Thus we have: 
$$
\begin{gather}
W = E_{\text{capacitor}} +E_{\text{resistor}} \\ \\ 
W = \frac{Q_{f}\mathcal{E}}{2} + \frac{Q_{f}\mathcal{E}}{2} = Q_{f}\mathcal{E}
\end{gather}
$$

