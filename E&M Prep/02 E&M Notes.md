## #1 01122024

# Chapter 1 Electrostatics: Charges and Fields 

Which equals (1.9)$$ = \int_{r=\infty}^{r_{12}} \left( -\frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{2}}{r^2}\right)dr = \frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{2}}{r_{12}}$$
	- With $q_1, q_{2}$ in coulombs, and $r_{12}$ in meters, Eq. (1.9) gives the work in *Joules*.

Thank to the additivity of electrical interactions, which we have already emphasized (1.11), $$\begin{gather} -\int F_{3} \cdot ds \, = - \int (F_{31}+F_{32})\cdot ds \,  \\ = -\int F_{31} \cdot ds \, - \int F_{32}\cdot ds \,   \end{gather}$$
That is, the work required to bring $q_3$ to $P_3$ is the sum of the work needed when $q_1$ is present alone and that needed when $q_2$ is present alone (1.12), $$W_{3} = \frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{3}}{r_{31}} + \frac{1}{4\pi\epsilon_{0}} \frac{q_{2}q_{3}}{r_{32}}  $$
We call $U$ the **electrical potential energy** of this particular system, $$U = \frac{1}{4\pi \epsilon_{0}} (\frac{q_{1}q_{2}}{r_{12}} + \frac{q_{1}q_{3}}{r_{13}} + \frac{q_{2}q_{3}}{r_{23}})$$
- The potential energy belongs to the configuration as a whole meaning there is no meaningful way of assigning a certain fraction of it to one of the charges.
- In this case we have chose the zero of potential energy to correspond to the situation with the three charges already in existence but infinitely far apart from one another. 

- Exercise

	- ![[Screenshot 2024-01-13 at 12.42.17 PM 1.png]]![[Screenshot 2024-01-13 at 12.42.30 PM 1.png]]- Solution: The above figure shows that there are four different types of pairs which is represented by the yellow picture below 
	![[Screenshot 2024-01-13 at 2.04.50 PM 1.png|300]]
	1D -  there'll be 12 different pairs, that is,  for the 12 different edges not double counting
	2D - there'll be 12 different pairs, that is, 2 diagonals for each of the 6 faces not double counting 
	3D - There'll be two types of 3D pairs to focus on, the 4 diagonals, and the 8 half diagonals emanating from the center
	Thus the potential energy is $$U = \frac{1}{4\pi\epsilon_{0}}\left( 8 \cdot \frac{(-2e^2)}{\frac{\sqrt{ 3 }b}{2}} + 12 \cdot \frac{e^2}{b} + 12 \frac{e^2}{\sqrt{ 2 }b} +4\cdot \frac{e^2}{\sqrt{ 3 }b} \right)$$
	The energy is positive which indicates that work had to be done on the system to assemble it. If the electrons were to fly apart from this configuration, the total system would have would have Kenetic energy $U$ no matter the fashion on their disassembly.
	One way of writing the instruction for the sum over pairs is this, $$U = \frac{1}{2} \sum^N_{j=1} \sum_{k\neq j} \frac{1}{4\pi\epsilon_{0}} \frac{q_{j}q_{k}}{r_{jk}}$$
	The double-sum notation, $\sum^N_{j=1}\sum_{k\neq j}$ says: take $j=1$ and sum over $k=2,3,4,.., N$; then take $j=2$ and sum over $k=1,3,4,..,N$; and so on through $j=N$. Clearly this includes every pair twice, and to correct for that we put in front the factor $1/2$ 
	