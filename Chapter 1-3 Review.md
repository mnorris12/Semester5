# Chapter 1 Where PDE's Come From
### 1.1 What is a Partial Differential Equation?
Defined as 
$$
\begin{gather}
F(x,y,u(x,y),U_{x}(x,y),u_{y}(x,y)) = F(x,y,u_{x},u_{y}) = 0
\end{gather}
$$
A linear Operator $\mathcal{L}$ is a linear transformation that can be applied to our solution. We have the following condition: 
$$
\begin{gather}
\mathcal{L}u = 0 
\end{gather}
$$
Then the equation is linear. 

Moral: A PDE has arbitrary functions in its solution. 
chain rule goes as follows: 
$$
\begin{gather}
\frac{ \partial  }{ \partial x } [f(g(x,t))] = f'(g(x,t)) \cdot \frac{ \partial g }{ \partial x } (x,t)
\end{gather}
$$
For the integrals of derivatives, we use Green's Theorem and the Divergence Theorem in A3
- Jacobians (change of variable in a double integral ) A.1
- Directional derivatives (A.1)

#### Conclusion
We introduce the concept of PDE, we discuss homogeneity, linearity of functions, a linear operator, and Strauss gives some helpful tips when we encounter situations that seem impossible with our calculus knowledge. 

#### 1.2 First-Order Linear Equations

We start by solving 
$$
\begin{gather}
au_{x}+bu_{y} = 0
\end{gather}
$$
We use the geometric method which utilizes the fact that the equation above is a directional derivative of u in the direction of the vector $V = (a,b)$ which must always be zero. $u(x,y)$ is constant on the characteristic lines $bx-ay$ and thus only depend on them. 
$$
\begin{gather}
u(x,y) = f(bx-ay)
\end{gather}
$$
Coordinate method - change of variables! 
$$
\begin{gather}
x'=ax+by \hspace{.5cm}y' = bx-ay
\end{gather}
$$
we involve the partial derivatives of u 
- We introduce the integration factor when we have the variable cofficient equation $$
\begin{gather}
u_{x}+yu_{y} = 0
\end{gather}
$$
General solution to the above equation is 
$$
\begin{gather}
u(x,y) = f(e^{ -x }y)
\end{gather}
$$
Moral:  Solutions of PDEs generally depend on arbitrary functions instead of constants. 

### 1.3 Flows, Vibrations, and Diffusions

Simple transport equation: 
$$
\begin{gather}
u_{t} +cu_{x} = 0
\end{gather}
$$
where $u_{t}$ is the rate of change of concentration which is proportional to the gradient $u_{x}$. 

Vibrating string: (we first derive the wave equation using tension)
we have that 
$$
\begin{gather}
u_{tt} = c^{2}u_{x x} \\ \\ 
c = \sqrt{ \frac{T}{\rho} }
\end{gather}
$$

Introduce the diffusion equation
$$
\begin{gather}
u_{t} = ku_{x x}
\end{gather}
$$
#### 1.4 Initial and Boundary Conditions

(D) u is specified (Dirichlet Conditions)
(N) the normal derivative $\frac{ \partial u }{ \partial n }$ is specified (Neumann Condition)
(R) $\frac{ \partial u  }{ \partial n }+au$ is specified ("Robin Condition")

#### 1.5 Well-Posed Problems

i - Existence: There exists at least one solution $u(x,t)$ satisfying all these conditions
ii - Uniqueness: There is at most one solution
iii - Stability: The unique solution $u(x,t)$ depends in a stable manner on the data of the problem. This means that if the data are changed a little, the coressponding solution changes only a little. 

This defines Well-Possedness

#### 1.6 Types of Second-Order Equations

