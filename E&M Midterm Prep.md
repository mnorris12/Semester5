## Chapter 1
###### Equations 
- $F=\frac{1}{4\pi\epsilon_{0}}\sum_{j=1}^N \frac{ q_{0}qj\hat{r}_{0j}}{r^{2}_{0j}}$. 
- $\vec{F}=-\nabla \vec{U}$
- $\frac{F}{A} = \frac{1}{2}(E_{1}+E_{2})\sigma$ $\leftarrow$ Force per unit area on a layer of charge 
- $F=Eq$ which is the force of a charge due to the field 
- $E = \frac{1}{4\pi\epsilon_{0}}\sum_{j=1}^N \frac{q_{j}\hat{r}_{j}}{r^{2}_{j}}$
- The energy density of an electric field is $\boxed{\frac{\epsilon_{0} E^{2}}{2}}$ 
- $\boxed{\ddot{x}=-\omega^{2}x}$  simple harmonic motion - from the eight things to remember!
- if $\delta\ll 1$ then we can use the binomial approximation $(1-\delta)^n\approx 1-n\delta$.
- $\boxed{d(E)=\frac{kdq}{r^{2}}}$
- Flux through a surface $\boxed{\Phi=\int E\cdot da =\frac{q}{\epsilon_{0}}}$
- $\boxed{dq= (\text{length/surface area/volume})(\text{charge density type})}$ 
- $\boxed{E_{\text{plane}} = \frac{\sigma}{2\epsilon_{0}}}$
- For a sphere $\boxed{E(r) = \frac{V_{\text{encl}} \rho}{4\pi \epsilon_{0}r^{2}}}$
- **Just outside the surface of a sphere, which also corresponds for a slab** $\boxed{E=\frac{\sigma}{\epsilon_{0}}}$.
- $\boxed{AE = \frac{Q_{enc}}{\epsilon_{0}}}$
- **Moral for a slab: the electric field outside its boundaries is $\frac{\sigma}{\epsilon_{0}}$**
- $dW =\int _{a}^b -\frac{qdq}{4\pi\epsilon_{0}r^{2}}\, dr$ 
- $W = \int _{0}^Q \frac{qdq}{4\pi\epsilon_{0}}\left( \frac{1}{a}-\frac{1}{b} \right)\, dx$
- $U  = \frac{\epsilon_{0}}{2}\int E^{2} \, dv$
-  $U = \frac{1}{2}\sum_{j=1}^N \frac{1}{4\pi\epsilon_{0}} \frac{q_{j}q_{k}}{r_{jk}}$ where$k\neq j$
- Gauss's law: The flux of the electric field $E$ through any closed surface equals $\frac{1}{\epsilon_{0}}$ times the total charge enclosed by the surface thus 
$$
\begin{gather}
E_{\text{sphere} } =\frac{Q}{4\pi\epsilon_{0}r^{2}} \hspace{.5cm}E_{\text{line}} = \frac{\lambda}{2\pi\epsilon_{0}r} \hspace{.5cm}E_{\text{sheet}} = \frac{\sigma}{2\epsilon_{0}}
\end{gather}
$$
- ![[Screenshot 2024-03-21 at 9.18.43 AM.png]]
###### Moral and Definitions
- We actually though a lot about classical newtonian mechanics to solve some E&M Problems!
- When working with structures of charges, it's important to consider the symmetry of the shape and the superposition of the charges. 
- Equilibrium Configuration - no external forces, charges have settled still.
- To minimize/maximize potential energy we want $\frac{dU}{d\theta}=0$ when the second derivative is $\pm$.
- Two part questions usually involve making connections between the two. That is, the second part of the question could be a more applicative version of the second.
- Spherical shells can be treated as a point charge
- Moral for concentric shells: the charge outside of a sphere (uniform charge density too or just hallow sphere?) effectively contributes nothing to the electric field of the inner sphere
- Thus for two concentric shells, the electric field exists between the two. It can be calculated based on the work required to bring charges to the first then second sphere (second depends on the first)

## Chapter 2
###### Equations 

- $\phi=\frac{\text{Joules}}{\text{coul}}$
- $\phi = \sum_{\text{all sources}} \frac{q_{i}}{4\pi\epsilon_{0}r}$
- $\phi=-\int E\cdot ds$
- $\phi_{21} =- \int _{P_{1}}^{P_{2}}E \cdot ds$ $\leftarrow$ The electrostatic potential energy difference of a charge $q$ between points $P_{1}$ and $P_{2}$ 
- For potential energy of a uniform charged sphere  we have 
	- $\phi_{\text{out}}(r)=\frac{Q}{4\pi\epsilon_{0}r}$
	- $\phi_{\text{in}}(r)= \frac{kQ}{R}\left[ \frac{3}{2}-\frac{r^{2}}{2R^{2}} \right]$
-  $E = \frac{\lambda}{2\pi\epsilon_{0}r}$ $\leftarrow$ Electric Field of a line
- Electric Field due to a cylinder
	- $E_{\text{out}} =\frac{\rho a^{2}}{2\epsilon_{0}r} \hspace{.2cm}$
	- $E_{\text{in}}=\frac{\rho r}{2\epsilon_{0}}$
- $E =\frac{kqR}{(x^{2}+r^{2})^{3/2}}$ $\leftarrow$ Electric field due to a ring with radius $r$ some distance away 
- $\phi_{r} =\frac{\sigma r}{\pi\epsilon_{0}}$ $\leftarrow$ Potential at a point on the rim of a disk
- Laplace's Equation $\nabla^{2}\phi=0$ where
	- $\nabla \phi = (\frac{ \partial  }{ \partial x },\frac{ \partial  }{ \partial y },\frac{ \partial  }{ \partial z })$
- $\nabla E = -\frac{\rho}{\epsilon_{0}}$
- $U = \frac{1}{2}\int \rho \phi \, dv = \frac{1}{2}\sum_{j=1}^N \frac{q_{j}kq_{k}}{r_{jk}} \hspace{.5cm} j\neq k$ $\leftarrow$ The energy required to assemble a group of charges from infinity is 
###### Morals and Definitions
- The gradient gives the direction in which $f$ has the largest rate of increase. 
- We define Electric Potential as the amount of work energy needed per unit of electric charge to move that charge from one position to another 
- Potential energy - total work required to assemble charge configuration
- You can take $-\nabla \phi = E$ to check that your answer for $\phi$ matches what you know about the electric field!
- Surface area of a cylinder $2\pi rl$
- Charge distributes itself so as to minimize the total potential energy 
- If $\vec{A}$ is any vector field with continuous derivatives, $\nabla \cdot(\nabla \times \vec{A}) = 0$ 

## Chapter 3
###### Equations

- $\nabla \vec{E}=\frac{-\rho}{\epsilon_{0}}$
- $\nabla^{2}\phi = -\frac{\rho}{\epsilon_{0}}$
- $Q = C\phi_{0}$
- $C_{\text{plate}} = \frac{\epsilon_{0}A}{s}$
- $U=\frac{1}{2}C\phi^{2} = \frac{\epsilon_{0}\mathbf{E}^{2}}{2}*vol$
- $\sigma = -\frac{Qh}{2\pi(r^{2}+h ^{2})^{3/2}}$ $\leftarrow$ surface charge density above a conducting plate with a charge on a particle
- $Q_{1} = C_{11}\phi_{1}+C_{12}\phi_{2}$
	- $Q_{2}=C_{21}\phi_{1}+C_{22}\phi_{2}$
- $F = \frac{Q^{2}}{2} \frac{d}{dx}\left( \frac{1}{C} \right)$ $\leftarrow$ force on capacitor sheet 
- $V =\frac{Q}{4\pi\epsilon_{0}}\left( \frac{1}{b}-\frac{1}{a} \right)$ $\leftarrow$ potential difference between two spherical shells
- $C=\frac{4\pi\epsilon_{0}ab}{a-b}$ $\leftarrow$ resulting capacitance of the two spherical shells
- $C_{\text{sphere}}=4\pi\epsilon_{0}r$
- $W = \frac{Q_{f}^{2}}{2C}$ $\leftarrow$ To charge the capacitor starting from the uncharged state to some final charge $Q_{f}$ requires the work.
- $\sigma=\epsilon_{0}E = \frac{\epsilon_{0} V}{s}$ $\leftarrow$ density of the surface charge on the inner surface of one capacitor plate

###### Moral & Definitions
- Image charges - find the information (electric field, charge distribution, force) above charges relative to a conduction plate. We ignore the conducting plate and place a charge or charge assemble of the opposite sign the same distance from the plate on it other side
- You can find capacitance by using flux to find the electric field, integrating over a path for potential, and then dividing $Q,q$ by that potential difference. 
- Capacitance tells us something about the shape and arrangements of the charge assemble
- If you are looking to justify you're reasoning, take a look at the page summary on pg. 156

## Chapter 4
###### Equations

- $\vec{J_{e}} = -eN_{e}\bar{\vec{u}}$ where $N_{e}$ is the number of electrons per unit volumn, $\bar{u}$ is the average velocity of all the electrons
- $I = JA$ 
- $\sigma = \epsilon_{0}E = \frac{\epsilon V}{S}$
- $div \vec{J}=-\frac{ \partial \rho }{ \partial t }$
- $V=IR$ $\leftarrow$ Ohm's law
- $P=I^{2}R$ $\leftarrow$ where power is the rate at which work is done. It's the power dissipated in an resistor
- $\vec{J}= \sigma \vec{E}$ where $\sigma$ is conductivity
- $R = \frac{\rho L}{A}$ where $\rho$ is the resistivity
- $\sigma \approx \frac{Ne^{2}\tau}{m}$ where $\tau$ is the mean time between collisions
- 

###### Moral & Definitions
- Input resistance: equivalent resistance between terminals $a$ and $b$
- $div \vec{J}= -\frac{ \partial \rho }{ \partial t }$ says if the charge in a region decreases (or increases), there must be current flowing out of (or into) that region
- Kirchhoff's rules - zero net current flow into any node, and zero net voltage drop around any loop
- Thévenin's Theorem states that any circuit is equivalent to a single voltage source $\epsilon_{eq}$ and a single resistor $R_{eq}$. 