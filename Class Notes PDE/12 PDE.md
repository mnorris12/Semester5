#### Strauss's Explanation of Completeness

Considers Fourier series as a special case (a fews special cases) of Strum-Liouville eigenvalue problems

For instance we have the following ODE: 
$$
\begin{gather}
X'' = \lambda X \\ \\ 
\text{homogeneous boundary conditions:} \hspace{.2cm} AX'(a)+BX(a) = 0 \\ \\ 
 CX'(a)+DX(a) = 0
\end{gather}
$$
where $A,B,C,D$ as pairs are not both $0$

Example: Let's use Dirichlet boundary conditions: 
$$
\begin{gather}
[a,b] = [0,\pi] \\ \\ 
\text{Dirichlet Boundary Condition:} 
\end{gather}
$$
You can verify that $\Lambda$ is not positive and under these B conditions its negative. The general solution to $X(x) = c\cos(\omega x)+d\sin(\omega x)$ where $c=0,d\neq 0$, when $x=0$. When $x=\pi$ we have that $d\neq 0$ and $\sin\omega \pi=0$. Thus $\omega\in\mathbb{Z}$. 

**Fact:** 
1. There is a countable number of eigenvalues $\lambda_{1}\dots\lambda n$
	1. $\lvert \lambda_{i} \rvert\rightarrow\infty$
2. For eigenvalue $\lambda_{i}$
	1. $\exists a$ eigenfunction $X(x)$ unique up to a non zero scalar
	2. Suppose: boundary condition is symmetric then we have: 
$$
\begin{gather}
X_{1},X_{2} \hspace{.5cm} \text{then} \hspace{.5cm} X_{1}'X_{2}-X_{1}X_{2}' =0 \\ \\ 
\lambda_{1}\dots\lambda_{n} \in\mathbb{R} \hspace{.5cm} \text{if symmetric}
\end{gather}
$$
3.  we have that 
$$
\begin{gather}
\int _{a}^b X_{\lambda_{i}} \cdot \langle X_{\lambda_{i}} \rangle = 0 \hspace{.2cm}\text{if} \hspace{.2cm} \lambda_{i} \neq\lambda_{j}
\end{gather}
$$
	1. This is actually related to problem 3 on the problem set 
4. {$X_{\lambda_{i}}$} is complete!
	1. Def: A family of orthogonal functions $(\phi_{i})$ on $[a,b]$ is complete if 
	2. $$
\begin{gather}
g \in L_{2}(a,b) | (g|\phi_{i}) = 0 \hspace{.5cm} \forall i \\ \\
(g|\phi_{i}) = \int _{a}^b g(x) \Phi_{i}(x)  \, dx \\ \\ 
\text{Example} \\ \\ 
[0,1] \hspace{.5cm} (e^{ 2\pi \sqrt{ -1 }nx }) \hspace{.2cm} \text{ is complete} \hspace{.2cm} n\in \mathbb{Z} \hspace{.2cm} if \hspace{.2cm}g\in L_{2} (0,1) \\ \\ 
\text{and} \hspace{.2cm} c_{n}(g)= \int _{0}^1 (e^{ 2\pi \sqrt{ -1 }nx }) g(x)  \, dx  = 0  \hspace{.5cm}\forall_{n}\in Z \hspace{.5cm} then \hspace{.2cm} g=0

\end{gather}
$$
		for every $f\in L_{2}(a,b)$. Now $\lim_{ N \to \infty }\| f-\sum_{o\leq i\leq N} \frac{f|\phi}{(\phi_{i}|\phi_{i})}\phi_{i}\mid|_{L_{2}} = 0$  where $\sum_{o\leq i\leq N} \frac{f|\phi}{(\phi_{i}|\phi_{i})}\phi_{i}$ is the projection of $f$ to $\sum_{0\leq i\leq N}\mathbb{C}\phi_{i}$ 

Remark: 
$$
\begin{gather}
\lvert \lvert f \rvert \rvert_{L^{2}}^{2} =\lvert \lvert  \sum_{o\leq i\leq N} \frac{f|\phi}{(\phi_{i}|\phi_{i})}\phi_{i} \rvert \rvert_{L^{2}}^{2} +\lvert \lvert f- \sum_{o\leq i\leq N} \frac{f|\phi}{(\phi_{i}|\phi_{i})}\phi_{i} \rvert \rvert_{L^{2}}^{2}
\end{gather}
$$
and $\forall \psi\in\sum_{i}^{N} \mathbb{C}\phi_{i}$ $\rightarrow$ $\lvert \lvert f-\phi \rvert \rvert_{L^{2}}^{2} \geq\lvert \lvert f- \sum_{o\leq i\leq N} \frac{f|\phi}{(\phi_{i}|\phi_{i})}\phi_{i} \rvert \rvert_{L^{2}}^{2}$

Now let's assume that $\lvert \lvert \phi_{i} \rvert \rvert_{L^{2}} = 1$ then we have that 
$$
\begin{gather}
f \rightarrow(\underbrace{ (f|\phi_{i}) }_{ c_{i} })_{i} \\ \\
\lvert \lvert f \rvert \rvert^{2} \geq \sum_{i=0} ^N \lvert c_{i} \rvert^{2} \rightarrow\sum_{i=0}^\infty \lvert c_{i} \rvert^{2} \leq \lvert f \rvert
\end{gather}
$$
Thus we have that $\sum_{i}c_{i}\phi_{i}$ converges in $L_{2}(a,b)$. This means that 
$$
\begin{gather}
\forall\epsilon>0 \hspace{.5cm} \exists N_{n} \hspace{.2cm} s.t \\ \\ 
\left\lvert  \left\lvert  \sum_{N_{1}\leq i\leq N_{2}} c_{i}\phi_{i} \right\rvert  \right\rvert_{L^{2}(a,b)} <\epsilon \hspace{.5cm} \forall N_{2}\geq N_{1}\geq N_{0} \\ \\ 
\sum_{i} d_{i} \hspace{.2cm} \text{converges} \\ \\ 
\forall\epsilon \hspace{.2cm} \exists N_{0}=N_{0}(\epsilon) \\ \\
\text{s.t} \hspace{.2cm} \left\lvert  \sum_{N_{1}} ^{N_{2}} d_{i}  \right\rvert <\epsilon \hspace{.5cm} \forall N_{2}\geq N_{1}\geq N_{0} 
\end{gather}
$$

Let's look at some examples of Eigenvalue problems!

 homogeneous Dirichlet boundary condition:  $$
\begin{gather}
\sin(\pi nx)_{n\geq 1} \\ \\
\text{you get a complete family of functions}
\end{gather}
$$
Homogeneous Neumann boundary condition: 
$$
\begin{gather}
\cos(\pi nx) \hspace{.5cm} n\geq 0
\end{gather}
$$
where 
$$
\begin{gather}
\begin{pmatrix}
\sin 2\pi nx \\
\cos 2 nx
\end{pmatrix} \text{is complete in} \hspace{.2cm}L_{2}(0,1)
\end{gather}
$$
with the previous boundaries for $n$. 

Let's do a proof!
$$
\begin{gather}
(e^{ 2\pi \sqrt{ -1 }nx }) \hspace{.2cm} n\in \mathbb{Z} \hspace{.2cm} on \hspace{.2cm} [0,1] \\ \\ 
\text{suppose} \hspace{.2cm} (f|e^{ 2\pi \sqrt{ -1 }nx } ) = 0 \\ \\
\text{want} \hspace{.2cm} f=0
\end{gather}
$$
Let's assume that $f$ is continuous. To prove this, we want to prove $T_{n} = \frac{\cos ^{2}(2\pi nx)}{\int_{0}^1 \cos ^{2}(2\pi nx) \, dx}$. This suffices to show that $f(0)= 0$. We say that $\int _{0}^1 T_{n}(x) \, dx =1$, $T_{n}(x)\geq 0 \hspace{.2cm} \forall x$, $\forall\delta>0 \hspace{.5cm}0\leq\delta \leq \frac{1}{4}$, $\lim_{ \lvert x \rvert \to \delta } T_{n}(x)= 0$ 