#### 8.10

Based on table 8.1 we have the following quantities, 
$$
\begin{gather}
Z = R + i\omega L+ \frac{1}{i\omega C} \\ \\ 
\frac{1}{Z_{tot}} = \frac{1}{R+i\omega L}+i\omega C
\end{gather}
$$
we can multiply the first term on the right side of the equation by its complex conjugate
$$
\begin{gather}
\frac{1}{Z_{tot}} = \frac{R-i\omega L}{(R+i\omega L)(R-i\omega L)} +i\omega C \\ \\ 
\frac{1}{Z_{tot}} = \frac{R-i\omega L}{R^{2}+\omega^{2}L^{2}}+i\omega C \\ \\ 
\frac{1}{Z_{tot}} = \underbrace{ \frac{R}{R^{2}+\omega^{2}L^{2}} }_{ \text{real part} } - \frac{i\omega L}{R^{2}+\omega^{2}L^{2}} + i\omega C \\ \\ 
\end{gather}
$$
If we let $\frac{1}{Z_{tot}} = 0$, and ignore the real part then we have
$$
\begin{gather}
0 = - \frac{i\omega L}{R^{2}+\omega^{2}L^{2}} + i\omega C \\ \\ 
0 = (i\omega)\frac{-L}{R^{2}+\omega^{2}L^{2}}+C \\ \\
0 = -\frac{L}{R^{2}+\omega^{2}L^{2}} + C \\ \\ 
C = \frac{L}{R^{2}+\omega^{2}L^{2}} \\ \\ 
\omega = \sqrt{ \frac{1}{C}-\frac{R^{2}}{L} }
\end{gather}
$$
Thus if this value is true for $\omega$, then we'll have that the impedance will be entirely real

#### 8.18

We have the following equations 
$$
\begin{gather}
\omega_{0} = \frac{1}{\sqrt{ LC }} \hspace{.5cm} \omega^{2}=\frac{1}{LC} - \frac{R^{2}}{4L^{2}}\hspace{.5cm}Q = \frac{\omega L}{R}
\end{gather}
$$
We can rewrite the middle equation such that 
$$
\begin{gather}
\omega^{2} = \omega_{0}^{2} -\frac{1}{4}\left( \frac{\omega^{2}}{Q^{2}} \right) \\ \\ 
\frac{\omega}{\omega_{0}} =  \left( 1 - \frac{\omega^{2}}{4\omega_{0}^{2}Q^{2}} \right)^{\frac{1}{2}} \\ \\ 
\end{gather}
$$
we use the binomial approximation, 
$$
\begin{gather}
\frac{\omega}{\omega_{0}} = 1-\frac{\omega^{2}}{8\omega_{0}^{2}Q^{2}}
\end{gather}
$$
to find the what percentage is the frequency $\omega$ is shifted from $\omega_{0}$, we use 
$$
\begin{gather}
\frac{\omega_{0}-\omega}{\omega_{0}} = 1-\frac{\omega}{\omega_{0}} 
\end{gather}
$$
so we can substitute in for the last term on the right, 
$$
\begin{gather}
\frac{\omega_{0}-\omega}{\omega_{0}} = 1- 1+\frac{\omega^{2}}{8\omega_{0}^{2}Q^{2}}= \frac{\omega^{2}}{8\omega_{0}^{2}Q^{2}} = \frac{1}{8Q^{2}} = \frac{1}{8(1000)^{2}} = 1.25*10^{-7}
\end{gather}
$$
To bring $Q$ from $\infty$ to 5, we have 
$$
\begin{gather}
\frac{1}{8(5)^{2}} = \frac{1}{8*25} = .005
\end{gather}
$$
We're all set!

#### 8.19 a

We have a fixed electromotive force $\mathcal{E} = 20V$. During a short period after the switch is closed, the current flowing the the resistor of the left circuit essentially negligible, so we worry only about the right part. Although the voltage eventually becomes negligible between the parallel current and inductor/resistors, it doesn't immediately. In such cases, we can treat $\omega$ as 
$$
\begin{gather}
\omega = \frac{1}{\sqrt{ LC }} \hspace{.5cm}\text{or} \hspace{.5cm} C = \frac{1}{\omega^{2}L}
\end{gather}
$$


From the Oscilloscope, we can calculate the frequency. That is, it makes about four period over the time of 1$ms$. Thus we have the frequency equal to 
$$
\begin{gather}
\omega = 8\pi(10^3)s = 2.51*10^4 s
\end{gather}
$$
Thus we can calculate the capacitance
$$
\begin{gather}
C = \frac{1}{(2.5132*10^4 s)^{2}*.1H} = 1.58*10^{-7} F
\end{gather}
$$

#### 8.19 b

Adjacently, from page 392, we know the energy decreases by a factor of $\frac{1}{e}$ in time $t = \frac{1}{\alpha}$ where $\alpha = \frac{R}{2L}$. So we have 
$$
\begin{gather}
t = \frac{1}{\frac{R}{2L }} =\frac{2L}{R}
\end{gather}
$$
We've already determined that $(10^{-3})s$ has passed, so our time corresponds to **half** that value. We know the inductance is $.01H$. Thus we can calculate the resistance
$$
\begin{gather}
R = \frac{2L}{t} = \frac{2(.01h)}{.5*10^{-3}s} = 40\Omega
\end{gather}
$$
#### 8.19 c
Finally, we have to find the voltage flowing across the  oscilloscope. We notice that after 1 second of time, we essentially only care about the resistance due to the size of the initial resistor ($10^5$ohms), and the resistance in the inductor. That is because in a steady state for our RLC, there's no current flowing across the capacitor, and no voltage drop across the inductor. So we have
$$
\begin{gather}
V = 20\left( \frac{40}{10^5+40} \right) = .008V
\end{gather}
$$
#### 8.31 

The voltage across both of the parts of the circuits are equal. Thus our first plan of action is to find the complex currents for both parts of the circuit,
$$
\begin{gather}
I_{1} = \left( \frac{i\omega c}{R_{1}i\omega c+1} \right)V_{0} \hspace{.5cm}I_{2} = \left( \frac{1}{R_{2}+i\omega L} \right)
\end{gather}
$$
The voltage at each of the resistors is thus 
$$
\begin{gather}
V_{1} = V_{0}-I_{1}\left( \frac{1}{i\omega C} \right) \hspace{.5cm}V_{2} = V_{0}-I_{2}R_{2}
\end{gather}
$$
Thus the difference between the total voltage is just
$$
\begin{gather}
-I_{1}\left( \frac{1}{i\omega C} \right) + I_{2}R_{2} =  \left( \frac{i\omega c}{R_{1}i\omega c+1} \right)V_{0} \left( \frac{1}{i\omega C} \right)  + \left( \frac{1}{R_{2}+i\omega L} \right)V_{0}R_{2}  \\ \\ 
= -\frac{V_{0}R_{2}}{R_{2}+i\omega L} +\frac{V_{0}}{i\omega CR_{1}+1}
\end{gather}
$$
We notice that if we multiply the right fraction by $R_{2}$, given the condition that $R_{1},R_{2} = \frac{L}{C}$, the difference between the voltages are zero. Thus we've shown it's zero at any frequency.

#### 8.33

For the above circuit in figure 8.39, we solve for it's impedance
$$
\begin{gather}
Z = 1000 + \frac{1}{\frac{1}{4000}+i\omega \cdot 10^{-6}} = \frac{5000 +4i\omega}{1+4 \cdot 10^{-3}i\omega} \\ \\ 
= \frac{5000 +16\cdot 10^{-6}\omega^{2}-16i\omega}{1+16*10^{-6}\omega^{2}}
\end{gather}
$$
Thus we've arrived at the desired result for the first circuit. Now we prove the same thing for the second circuit
$$
\begin{gather}
\frac{1}{Z} = \frac{1}{5000} + \frac{1}{1250 + \frac{10^6}{.64i \omega}} = \frac{1}{5000} +\frac{.64*10^{-6}i\omega}{8 \cdot 10^{-4}i\omega+1}  \\ \\ 
= \frac{5000+4i\omega}{1_{4\cdot 10^{-3} i\omega}}
\end{gather}
$$
we notice that the final value for the second circuit is equivalent to one of the values we already found for the above circuit, so we've shown the desired result for the second circuit. As far as a general rule for the circuits, we can evaluate them based on $\omega=0,\infty$. That is, since the impedance is the same at any frequency, $\omega=0$, the resistance adds such that no current goes through the capacitors. 
$$
\begin{gather}
R_{1}+R_{2} = R_{3}
\end{gather}
$$
when $\omega=\infty$, the capacitor has no impedance, thus we have
$$
\begin{gather}
R_{1} = \frac{R_{3}R_{4}}{R_{3}+R_{4}}
\end{gather}
$$
We're all set!

#### 8.37
 
In Figure 8.20, we have a capacitor, resistor, and Inductor in parallel. Equation 8.67 gives
$$
\begin{gather}
I(t) = \mathcal{E}_{0}\sqrt{ \left( \frac{1}{R} \right)^{2}+\left( \omega C-\frac{1}{\omega L} \right)^{2} }\cos(\omega t+\phi) \\ \\ 
\tan \phi = R\omega C-\frac{R}{\omega L}
\end{gather}
$$
We can now use this information to arrive at the following $\cos$ equation
$$
\begin{gather}
\cos \phi = \frac{\left( \frac{1}{R} \right)}{\sqrt{ \left( \frac{1}{R} \right)^{2} +\left( \omega C-\frac{1}{\omega L} \right)^{2} }}
\end{gather}
$$
The equation for the average power of a circuit is
$$
\begin{gather}
\bar{P} = \frac{1}{2} \mathcal{E}_{0} I_{0} \cos \phi = \frac{1}{2}\mathcal{E}_{0}(\mathcal{E}_{0})\sqrt{ \left( \frac{1}{R} \right)^{2}+\left( \omega C-\frac{1}{\omega L} \right)^{2} }\\ \\ 
\cdot \frac{1}{R}\sqrt{ \left( \frac{1}{R} \right)^{2}+\left( \omega C-\frac{1}{\omega L} \right)^{2} } = \frac{1}{2}\mathcal{E}_{0}^{2} \frac{1}{R}
\end{gather}
$$
which is the same for the power dissipated across a resistor. So we're all set!

#### 8.38 a

The impedance of the capacitor is $Z_{C} = -iR$. We add the capacitor impedances in parallel, so the total impedance
$$
\begin{gather}
Z_{tot} =  \frac{Z_{R}(Z_{R}+Z_{C})}{Z_{R}+(Z_{R}+Z_{C})} = \frac{Z_{R}^{2} +Z_{R}Z_{C}}{2Z_{R}+Z_{C}} = R \frac{1-i}{2-i}
\end{gather}
$$
#### 8.38 b

The complex current can be modeled as 
$$
\begin{gather}
\tilde{ I}_{tot} = \frac{\mathcal{E}_{0}}{Z} = \mathcal{E}_{0} \left(  R \frac{1-i}{2-i} \right)^{-1} = \frac{\mathcal{E}_{0}}{R} \frac{\sqrt{ 10 }}{2}e^{ i(\phi) } \\ \ \
I_{0} =\frac{\sqrt{ 10 }}{2} \frac{\mathcal{E}_{0}}{R} \hspace{.5cm} \phi=\tan^{-1}\left( \frac{1}{3} \right) = 18.435
\end{gather}
$$
#### 8.38 c

Similar to last equation, the average power dissipated over the circuit is 
$$
\begin{gather}
\bar{P} = \frac{1}{2}\mathcal{E}_{0}I_{0}\cos \phi
\end{gather}
$$
where, because $\tan \phi=\frac{1}{3}$, we have that $\cos \phi = \frac{3}{\sqrt{ 10 }}$. Thus we have, 
$$
\begin{gather}
\bar{P} = \frac{\sqrt{ 10 }}{4}\mathcal{E}_{0} \left( \frac{\mathcal{E}_{0}}{R} \right)\left( \frac{3}{\sqrt{ 10 }} \right) = \frac{3\mathcal{E}_{0}^{2}}{4R}
\end{gather}
$$