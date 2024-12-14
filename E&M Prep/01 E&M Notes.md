
##  #1 01072024

# Chapter 1 Electrostatics: Charges and Fields 

##### 1.1 Electric Charge

In this chapter we shall study the physics of stationary electric charges - **electrostatics.** 

The electron's charge is negative; its antiparticle, called the **positron**, has a positive charge, but its mass is precisely the same as that of the electron. 

The proton's antiparticle is called simply an **antiproton**; its electric charge is negative. 

Two other properties of electric charge are essential in the electrical structure of matter: charge is **conserved**, and charge is **quantized**. 

##### 1.2 Conservation of Charge

The total charge in an isolated system never changes. By **isolated** I mean that no matter is allowed to cross the boundary of the system.

The "particles" of light called **photons**, carry no charge at all. 
- Within the system charged particles of light called photons carry no charge at all 
	- For instance, a thin-walled box in a vacuum exposed to gamma rays might become the scene of a "pair-creation" event in which a high-energy photon ends its existence with the creation of an electron and a position.
		- ![[Screenshot 2024-01-07 at 3.51.13 PM 1.png|300|150 ]]
		- An event that **would** violate the law we have just stated would be the creation of a positively charged particle **without** the simultaneous creation of a negatively charged particle. 

Theorem 1.11
- The total electric charge in an isolated system, that is, the algebraic sum of the positive and negative charge present at any time, never changes. 
The total electric charge of an isolated system is a relativistically invariant number 

##### 1.3 Quantization of Charge

We denote the magnitude of the charge of an electron $e$. (When we pay attention to sign, we write -$e$ for the charge on the electron itself.) 
**Ion** - a molecule with an electron missing or an extra electron attached. 

We now know that the internal structure of all the strongly interacting particles called **hadrons** - a class that includes the proton and neutron - involves basic units called **quarks** whose electrical charges come in multiples of $e/3$.
- The proton, for example, is made with three quarks, two with charge $2e/3$ and one with charge $-e/3$. The neutron contains one quark with charge $2e/3$ and two quarks with charge $-e/3$. 

##### 1.4 Coulomb's Law

The interactions between electric charges at rest is described by Coulomb's law: two stationary electric charges repel or attract one another with a force proportional to the product of the magnitude of the charges and inversely proportional to the square of the distance between them. This can be stated in vector form: 
- 1.1 $$F_{2} =k \frac{q_{1}q_{2}\hat{r}_{21}}{r^2_{21}} $$
- Here $q_1$ and $q_2$ are numbers (scalars) giving the magnitude and sign of the respect charges, $\hat{r}_{21}$ is the unit vector in the direction from charge 1 to charge 2, and $F_2$ is the force acting on charge 2. 
- Expresses that like charges repel and unlike charges attract. 
- Also, the forces obeys Newton's third law; that is, $F_2 = -F_1$. 
- We can define the coulomb as two like charges, each of 1 coulomb, repel one another with a force of $8.988(10^9)$ Newtons when they are 1 meter apart. 
- We define $k$ (where C is the SI unit of charge **coulomb**),
	- (1.2) $$k = 8.988* {10^9} \frac{Nm^2}{C^2}$$ 
The magnitude of $e$, the fundamental quantum of electric charge, happens to be about $1.602(10^{-19}) C$ 
- so if you wish, you may think of a coulomb as defined to be the magnitude of the charge contained in $6.242(10^{18})$ electrons. 
- Instead of $k$, it is customary (for historical reasons) to introduce a constant $\epsilon_0$ which is defined by 
- (1.3)$$k \equiv \frac{1}{4\pi\epsilon_{0}} \to \epsilon_{0} \equiv= \frac{1}{4\pi k} = 8.854(10^{12}) \frac{C^2}{Nm^2} \space \left( or \frac{C^2}{kgm^2} \right). $$
- In terms of $\epsilon_0$, Coulomb's Law in Eq. (1.1)  takes the form 
- (1.4)$$ F = \frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{2}\hat{r}_{21}}{r^2_{21}}$$![[Screenshot 2024-01-07 at 5.10.21 PM 1.png|300|150]]


## 01/08/2024

##### 1.4 Coulombs Law

The only way we have of detecting and measuring electric charges is by observing the interaction of charged bodies. 

As it stands, the significant physical content is the statement of inverse-square dependence and the implication that electric charge is additive in its effect. 

The force with which two charges interact is not changed by the presence of a third charge, no matter how many charges we have in our system. 
- Coulomb's law can be used to calculate the interaction of every pair. This is the basis for superposition. **Superposition** means combining two sets of sources into one system by adding the second system "on top of" the first without altering the configuration of either one. 
- Our principle ensures that the force on a charge placed at any point in the combined system will be the vector sum of the forces that each set of sources, acting alone, causes to act on a charge at that point. 
- Thus the physics of electrical interactions comes into full view only when we have more than two charges. 
	- Thus we can assert that, with thee charges $q_1, q_2, q_3$ occupying any positions whatsoever, the force on any one of them, such as $q_3$, is correctly given by the following equation: (1.8) $$F = \frac{1}{4\pi\epsilon_{0}}\frac{q_{3}q_{1}\hat{r}_{31}}{r^2_{31}} + \frac{1}{4\pi\epsilon_{0}}\frac{q_{3}q_{2}\hat{r}_{32}}{r^2_{32}}$$
Two hundred years after Cavendish's two shell experiment inspired by Benjamin Franklin, the question of distance and wether its effect would break Coulomb's law became of interest. Is there a range where it breaks down completely?
- The first is the domain of very small distances less than $10^{-16}m$ where the electromagnetic theory as we know it may not work at all. 
- By the method Cavendish, the opposite scenario of astronomically large distances isn't feasible.
	- We do, however, observe certain large-scale electromagnetic phenomena that prove the laws of classical electromagnetism work over very large distances, like planetary magnetic fields. 

##### 1.5 Energy of a system of charges

In principle, Coulomb's law is all there is to electrostatics. Given the charges and their location, we can find all the electrical forces. 

Energy is a useful concept here because electrical forces are **conservative**. 

How much work does it take to bring two particles at great distance apart, only $r_{12}$ distance apart? It actually makes no difference if we bring $q_1$ to $q_2$ or vice versa. In either case, the work done is the integral of the product: force times displacement, where these are signed quantities. Therefore $$W = \int (applied force) \cdot (dispalcement)$$
Which equals (1.9)$$ = \int_{r=\infty}^{r_{12}} \left( -\frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{2}}{r^2}\right)dr = \frac{1}{4\pi\epsilon_{0}} \frac{q_{1}q_{2}}{r_{12}}$$
	- With $q_1, q_{2}$ in coulombs, and $r_{12}$ in meters, Eq. (1.9) gives the work in *Joules*.
