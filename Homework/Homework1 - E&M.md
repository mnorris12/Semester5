#### 1(a). $iy + jx$
We have that $F(x,y) = y\hat{i} + x\hat{j}$. This will create a vector function whose magnitude depends on the values of $x,y$ values. We'll do a bit of math to condense $F(x,y)$: 
$$
\begin{gather}
F(x,y) = y\hat{i}+x\hat{j} = (1,0)y + (0,1)x = (y,0)+(x,0) = (y,x)
\end{gather}
$$
Here, $F(x,y)$ essentially flips the $x,y$ axis, with all the $x$ values being $y$ and vice versa. The magnitude for the vectors will increase away from the center, and can be determined by:
$$
\sqrt{(y)^{2}+(x)^{2}} \hspace{.5cm} \text{for any values of} \hspace{.1cm} x,y
$$
This gives us the following graph with no vector at the origin, (ignoring the "vector" parallel to the y axis ): 

![[Pasted image 20240125010533.png |center | 300 ]]

---

#### 1(b).  $\frac{(i+j)}{\sqrt{ 2 }}$

We have that $F = \frac{(i+j)}{\sqrt{ 2 }}$. This will create a vector function whose vector magnitudes/direction does not depend on $(x,y)$. We'll do a bit of math here before we draw the vector function 2-dimensionally:
$$
\begin{gather}
\frac{(1,0)+(0,1)}{\sqrt{ 2 }} = \left( \frac{1}{\sqrt{ 2 }}, 0 \right) + \left( \frac{1}{\sqrt{ 2 }}, 0 \right) = \left( \frac{1}{\sqrt{ 2 }}, \frac{1}{\sqrt{ 2 }}\right)\\ \\ 
\end{gather}
$$
Thus the "tail" of our vectors will be sketched out at increments of $\frac{1}{\sqrt{2}}$. Since we have that $F = (\frac{1}{\sqrt{ 2 }} , \frac{1}{\sqrt{ 2 }})$, all of our vectors will be at a constant length with magnitude:
$$
\begin{gather}
\sqrt{ \left( \frac{1}{\sqrt{ 2 }} \right)^{2} + \left( \frac{1}{\sqrt{ 2 }} \right)^{2}  } = \sqrt{ \frac{1}{4} } = \frac{1}{2}
\end{gather}
$$
Now we sketch (ignore the top comment on the image): 

![[Pasted image 20240127161825.png|center|300]]

---

#### 1(c). $ix - jy$

The process for this one is the same for the other ones, so we'll skip the explanation and do the math for $F(x,y)$:
$$
ix-jy = (1,0)x - (0,1)y = (x,0) + (0,-y) = (x,-y)
$$
The magnitude of the vectors are determined by:
$$
\sqrt{ x^{2} + (-y)^{2}}  =\sqrt{ x^{2} + y^{2} }
$$
So they'll get longer away from the origin, and there will be no vector components at the origin. It looks like the following:

 ![[Pasted image 20240128160828.png|center|300]]
---

#### 1(d). $iy$

Similarly to 1(c), we'll skip the explanation that we provided in parts a and b and do the math for $F(x,y)$:
$$
iy = (1,0)y = (y,0) 
$$
The magnitude of the vectors are determined by 
$$
\sqrt{ y^{2} }
$$
This means that all the vectors will have no x component. There will also not be a vector at the origin. The graph looks like the following: 
![[Pasted image 20240130020903.png|center|300]]


---
#### 2(a). $F = ix+yj+kz$

The trick to this question, is doing one integral for a singular square tells us the outcome of the others. Thus we'll start by dividing it into regions: 
![[Pasted image 20240128171451.png|center|300]]

Let's start by tackling the region 1. To do this, we'll create a parametrization $\sigma(x,y,z) = (0,y,z)$ and evaluate the integral: 
$$
\iint_{S} F\cdot \hat{n}\, dS = \int F(\sigma(x,y,z)) \cdot \left( \frac{ \partial \sigma }{ \partial y } \times \frac{ \partial \sigma }{ \partial z }  \right)\, dydz
$$
We note that $F(\sigma(x,y,z)) = (0,y,z)$ and $\left( \frac{ \partial \sigma }{ \partial y } \times \frac{ \partial \sigma }{ \partial z } \right) = (1,0,0)$. Thus the integral reduces to,
$$
\iint_{S} (0,y,z) \cdot(1,0,0) \, dydz  = \iint_{S} (0,0,0) \, dydz = 0 
$$
Thus the integral to the first region equals zero. With this in mind $F(\sigma(x,y,z)) \cdot \left( \frac{ \partial \sigma }{ \partial y } \times \frac{ \partial \sigma }{ \partial z }  \right)$ will equal 0 for the other two regions as, the partial cross product will have 0s where $F(\sigma(x,y,z))$ will have values. Thus the sum of all the regions is 0.

---
#### 2(b). $F = (ix+jy)(ln(x^2+y^2))$

We first realize that for the top and bottom of the cylinder
$$
\int \mathbf{F} \cdot \, d\mathbf{a}  = 0
$$
![[Pasted image 20240128203013.png|center|300]]
as due to their orientation, it's the same integral but different signs. Thus we only focus on the cylindrical part. we note:
$$
\begin{gather}
F =(ix+jy)(\ln(x^{2}+y^{2}) ) \\ \\ 
\text{In cylindrical Coordinates:} \hspace{.5cm}R\hat{r} =ix+jy \hspace{.2cm}\text{and} \hspace{.2cm} x^{2}+y^{2} = R^{2}(\cos ^{2}(\theta)+\sin ^{2}\theta)=R^{2}
\end{gather}
$$
Thus the inside of our integral should look like: 
$$
\begin{gather}
\int _{surface} \mathbf{F} \cdot  \, d\mathbf{A} = \int _{\sigma} \mathbf{F} \, dA\hat{r} \\ \\ 
\int R\ln(R^{2}) \hat{r}\hat{r}\, dA = R\ln R^{2}\int  \, dA = R\ln(R^{2})\pi R^{2}h
\end{gather}
$$
Thus the final answer for this integral is $dA = R\ln(R^{2})\pi R^{2}h$ 

---
#### 2(c). $F = (ix+jy+kz)e^{-(x^2 + y^2 + z^2)}$
![[Pasted image 20240128210813.png|center|300]]

Similar to the previous example, we can cleverly parametrize the information in parenthesis (values in cartesian coordinates) with spherical coordinates: 
$$
\begin{gather}
F = (ix+jy+kz)e^{x^{2}+y^{2}+z^{2}} \\ \\ 
\text{the parametrization for a sphere is:} \hspace{.5cm} \sigma(\rho,\theta,\phi)=(r\cos\theta \sin \phi, r\sin \phi r\sin\theta, r\cos \phi) \\ \\ 
\end{gather}
$$
We note the following conversions from cartesian to spherical 
$$
\begin{gather}
x^{2}+y^{2}+z^{2} =R^{2} \hspace{.5cm} \hspace{.5cm} \text{eq. of the circle}\\ \\ 
(ix+jy+kz) = R\hat{r} \\ \\ 
F(x,y,z) = R\hat{r}e^{-(R^{2})} \\ \\


\end{gather}
$$
Thus we build the integral: 
$$
\begin{gather}
\int _{surface} \mathbf{F} \cdot  \, d\mathbf{A} = \int _{\sigma} \mathbf{F} \, dA\hat{r} \\ \\ 
\int _{surface} Re^{-(R^{2})} \hat{r}\, d\mathbf{A} = \int _{\sigma} Re^{-(R^{2})} \hat{r} \hat{r}\, \, dA = Re^{-(R^{2})}(2\pi r^{2})
\end{gather}
$$
Thus the answer is $Re^{-(R^{2})}(2\pi r^{2})$. 

---
#### 2(d). $F = (iE(x))$

We have $F=iE(x)$ where $E(x)$ is an arbitrary scalar function of $x$. Immediately, we know this means that the vectors on the left, right, top, and bottom sides are on/parallel to the surface. Thus the surface integrals over them are 0.
![[Pasted image 20240128221745.png|center|300]]

We thus concentrate only on the front and back. We create a parametrization for the front and back:
$$
\begin{gather}
\sigma(x,y,z) = (x,E(x),z) \\ \\ 
( \frac{ \partial \sigma }{ \partial y } \times \frac{ \partial \sigma }{ \partial z } ) = E(x)_{y}\hat{i}
\end{gather}
$$
Note: The back face of the cube has vectors pointing in, but our convention is outside normal, thus its value will be the negative of the front face. We build the integral: 
$$
\begin{gather}
\int _{0}^b E(x)_{y}\hat{i} \hat{i}\, dydz = \int _{0}^b E(x)\, \underbrace{ dydz }_{ b^{2} } = b^{2}[E(b)-E(0)]
\end{gather}
$$
Thus our final answer is $b^{2} [E(b)-E(0)]$

---
#### 3(a). $F=ix+jy+kz$

We verify that $$
\begin{gather}
\iint_{s} \mathbf{F}\cdot \hat{n} \, d\mathbf{S} = \iiint_{v} \nabla \cdot F dV \hspace{.5cm}\text{give that } F= ix+ jy +kz
\end{gather}$$
Each of the parametrizations for the faces that have a 0 for either $x,y,z$ =0 for the reasons stated in the previous example. That leaves the top, front, and right face. Let's start with the top, the other two sides should be the same process thus the same answer.
$$
\begin{gather}
F_{top} = (x,y,b) \\ \\ 
\int _{top} b \, \underbrace{ dxdy  }_{ b^{2} } = b^{3} \hspace{.5cm}\text{Thus the volume is} \hspace{.1cm}b^{3}
\end{gather}
$$
Or, using the divergence theorem:
$$
\begin{gather}
\iiint_{v}\left( \frac{ \partial  }{ \partial x }, \frac{ \partial  }{ \partial y }, \frac{ \partial  }{ \partial z }   \right)(x,y,z)\ dV= \iiint_{V} (1+1+1) \ dV = 3\iiint_{V}dV = 3b^{3}
\end{gather}
$$
---
#### 3(b). $\mathbf{F} = \hat{e}_{r}\mathbf{r}+\hat{e}_{z}\mathbf{z}$ 

Let's first start by condensing $\mathbf{F}$:
$$
F = \hat{e}_{r}r + \hat{e}_{z}z = F = \hat{i}x + \hat{j}y +\hat{k}z
$$
We immediately see that, similarly to the last couple problems, the inner side faces and the bottom quarter circle integral is $0$. To reiterate, the vectors flowing through these regions, flow parallel to the surface itself, thus the integral is 0. This is not the case for the top quarter circle and quarter cylinder. We solve first for the top circle:
$$
\begin{gather}
 F = \hat{i}x + \hat{j}y +\hat{k}h \hspace{.5cm} \\ \\ 
\int F \, dA  = \int (\hat{i}x + \hat{j}y +\hat{k}h) \underbrace{ \hat{k}\, dA  }_{ d\vec{A} } \\ \\
\int h\hat{k}\hat{k} \, dA = h\int dA \, dx = \frac{h(\pi R^{2})}{4}
\end{gather}
$$
Now for the quarter cylinder. We note that the vectors pointing from the surface have an $x,y$ component in cartesian component, but have just $r$ component radially. Consequently: 
$$
\begin{gather}
\int R \hat{e}_{r}+\hat{e}_{z}z\, dA  = \int R \hat{e}_{r}+\hat{e}_{z}z\, \, dA(\hat{e}_{r})
\end{gather}
$$
Thus we have: 
$$
\begin{gather}
\int R\hat{e}_{r} (\hat{e}_{r})+\hat{e}_{z}(\hat{e}_{r})\, dA = \int R \, dA  = R\int  \, dA = R 2\pi rh
\end{gather}
$$
When we add the results for the top quarter circle and quarter cylinder we have 
$$
\frac{h(\pi R^{2})}{4} + \frac{R (2\pi Rh)}{4} = \frac{3\pi R^{2}h}{4}
$$

Divergence Theorem: 
$$
\begin{gather}
\int \nabla \cdot F \, dV = \int (1+1+1) \, dV = 3\int  \, dV = \frac{3(\pi R^{2}h)}{4}   
\end{gather}
$$
It checks out!

---

#### 3(c). $F = \hat{e}_r r^2$
$$
\begin{gather}
F = \hat{e}_{r}r^{2} \hspace{.5cm}r = ix+jy+kz \hspace{.5cm}\text{ F is a function of r} \\ \\ 
\int R^{2}\hat{e}_{r} \, dA = \int R^{2}\hat{e}_{r}\hat{e}_{r} \, dA  \\ \\ 
R^{2}\int  \, dA = R^{2} (4\pi R^{2}) = R^4(4\pi)
\end{gather}
$$
![[Pasted image 20240130003402.png|center|300]]

where the vector coming from the small area $d\mathbf{A} =dA  \hat(e)_{r}$

We do the same for the divergence. 
$$
\begin{gather}
\int \nabla \cdot F \, dV = \int (4x+4y+4z) \, dV = \iiint 4(r)r^{2}\sin\theta \, d\theta d\phi dr  \\ \\ 
4\pi{4}\int_{0}^R r^{3} \, dr = \frac{16R^4\pi}{4}
\end{gather}
$$
Checks out!
