---
dg-publish: false
---


### 12/28/2023

# Chapter 1: Basic Equations 
Let's add this in here to see if it will register it

## Section 1.1: Definitions 
- A **differential equation** is any equation that contains a derivative, whether ordinary or partial. 
	- Ex: 
	- $$F = ma$$
	- Or, it's another differential form:
	- $$m\left(\frac{d^{2}u}{d^{2}t}\right) = F \left( t, u, \frac{du}{dt} \right)$$
	- Here's more differential equation examples: $$ay'' + by' + cy = g(t)$$ 
	- $$\sin(y)\left( \frac{d^{2}y}{dx^{2}} \right) = (1-y)\left( \frac{dy}{dx}+y^{2}e^-5y \right)$$
	- $$y^4 + 10y''' - 4y' + 2y = \cos (t)$$
	- $$\frac{\partial^{3} u}{\partial x^{2} \partial t} = 1 + \frac{\partial u}{\partial y}$$


- The **Order** of differential equations is the largest derivative present in the differential equation. First order would be velocity, second would be acceleration, third would be jerk, etc
	- definition is independent of equation being partial or ordinary

- A differential equation is called an **ordinary differential equation**, if it has ordinary derivatives in it. Likewise, a differential equation is called a **partial differential equation** if it has partial derivatives in it. 

 **Linear differential equation** is any differential equation that can be written in the following form: 
- $$a_{n}(t)y^n(t)+a_{n-1}(t)y^{(n-1)} (t) + \dots + a_{1}(t)y'(t) + a_{0} (t)y(t) = g(t)$$
	- Its derivatives and neither the function or its derivatives occur to any power other than the first power. Also note that neither the function or its derivatives are "inside" another function like $\sqrt{ y' }$
	- If a differential equation can't be written in the above form then it's a **non-linear differential equation 

 A **solution** to a differential equation on a interval  $\alpha < t < \beta$ is any function that exists on that interval $

- Example Problem: 
	![[Pasted image 20231228210326.png]] Solution: 
	- *We first find the first and second derivatives*: $$\begin{cases} y = x^\left( -\frac{3}{2} \right) \\ y' = -\frac{3}{2}x^\left( -\frac{5}{2} \right) \\ y'' = \frac{15}{4} x^\left( -\frac{7}{2} \right) \\  \end{cases}$$
	- *Then we plug those values into the original equation:*
	 $$4x^2 \frac{15}{4} x^\left( -\frac{7}{2} \right) + 12x -\frac{3}{2} x^\left( -\frac{5}{2} \right) + 3x^\left( -\frac{3}{2} \right) = 0$$
	 - *Continue simplifying:*
	 $$15x^(-3/2) - \frac{36}{2} x^\left( -\frac{3}{2} \right) + 3x^\left( -\frac{3}{2} \right) = 0  $$
	 - *Lastly, we find that:*
	 $$15x^\left( -\frac{3}{2} \right) - 18x^\left( -\frac{3}{2} \right) + 3x^\left( -\frac{3}{2} \right) = 0$$
	 $$ 0=0$$
	 - *Thus we've proved that  $y(x) = x^\left( -\frac{3}{2} \right)$ is a solution to $4x^2 y''  + 12xy' + 3y$

- **Initial Condition(s)** are a condition, or set of conditions that determine what solution we are after. They are of the form $y(t_0) = y_0$  and/or $y^(k) (t_0) = y_k$ 
	- $$y(4) = 4^\left( \frac{3}{2} \right) = \frac{1}{(\sqrt{ 4 })^3} = \frac{1}{8}$$
	- $$y'(4) = -\frac{3}{2}4^\left( \frac{-5}{2} \right) = -\frac{3}{2} \frac{1}{(\sqrt{ 4 })^5} = -\frac{3}{64}$$
	- Thus $y(x) = x^\left( \frac{-3}{2} \right)$ is the only solution to this differential equation that satisfies these two initial conditions.


- An **initial value problem (IVP)** is a differential equation along with an appropriate number of initial conditions. For example: 
	![[Pasted image 20231228222602.png]]
	or 
	![[Pasted image 20231228222646.png]]

- The **general solution** to a differential equation is the most general form that the solution can take and doesn't take any initial conditions into account
	 ![[Pasted image 20231228223026.png]]
	Proof: 

### 01/07/2024

- (Conn.) The **general solution** to a differential equation is the most general form that the solution can take and doesn't take any initial conditions into account
	 ![[Pasted image 20231228223026.png]]
	Proof: 
		- We take note of our derivatives
			- $$\begin{cases} y(t) = \frac{3}{4} + \frac{c}{t^2} \\ y'(t) = -2 \frac{c}{t^-3} \\ \end{cases}$$
		- Then we plug in the derivatives to the second equation
			-  $$ 2t(-2 \frac{c}{t^3}) + 4(\frac{3}{4} + \frac{c}{t^2}) = 3$$ 
		- We simplify
			- $$ \frac{-4c}{t^2} + 3 + \frac{4c}{t^2} = 3$$ $$3=3$$

##### Actual Solution

- The **Actual Solution** to a differential equation is the specific solution that not only satisfies the differential equation, but also satisfies the given initial initial condition(s). 
	- ![[Pasted image 20240107190330.png]]
	  - Solution:
		  - We find $y(1)$
			  $$ y(1) = \frac{3}{4} + c$$
			  $$-4 = \frac{3}{4} + c$$
			  $$\frac{-19}{4} = c$$
		- Thus with c, we can rewrite $y(t)$
			$$y(t) = \frac{3}{4} + \frac{-19}{4t^2}$$
		- So $y'(t)$ is,
			$$y'(t) = \frac{38}{4t^3}$$
		- we now plug our new original and differentiated equation into the IVP and simplify,
			$$2t(\frac{38}{4t^3})+4(\frac{3}{4} + \frac{c}{t^2}) = 3$$
			$$\frac{38}{2t^3} + 3 + \frac{4c}{t^2} = 3$$
			$$\frac{19}{t^2} + 3 + \frac{-19}{t^2} = 3$$$$3=3$$

- From the last example we can see that once we have the general solution to a differential equation finding the actual solution is nothing more than applying the initial conditions(s) and solving for the constant(s) that are in the general solution. 

##### Implicit/Explicit Solution
- An **Explicit Solution**  is any solution that is given in the form $y = y(t)$. In other words, the only place that $y$ actually shows up is once on the left side and only raised to the first power. 
- An **Implicit Solution** is any solution that isn't in explicit form. Note that it is possible to have either general implicit/explicit solutions and actual implicit/explicit solutions. 
	- ![[Pasted image 20240107192824.png]]
	- ![[Pasted image 20240107192847.png]]
	- Solution
		We are aware that the implicit solution to Example 8 is $y^2 = t^2 - 3$  and thus to find the explicit solution where we get, specifically, $y =$,  we take the square root on both sides. This leads to a slight problem as we end up with two solutions $$ y = \pm\sqrt{t^2 - 3} $$
		We then need to use the initial condition $y(2) = -1$ and we find that the actual explicit solution is $$y = -\sqrt{ t^2 - 3 }$$
		It will not be always be possible to find an explicit solution, and we we wont always be given an initial condition to help determine which of the two functions would be the explicit solution. 


### Section 1.2: Direction Fields 

To  begin the discussion of **Direction Fields**, we first think about a simple case of a falling object. We'll say for instance that that object has two forces acting on it $F_G = mg$ and $F_A = -\gamma(v)$  where we denote the positive direction to be in the direction of $F_G$. We then can create a differential equation by coming the forces: $$m\frac{dv}{dt} = mg - \gamma v$$
We give values to $g, m, \gamma,$ $$\frac{dv}{dt} = 9.8 -0.196v$$
We thin begin to think about what exactly this tells us. Since it's a derivative, any value of $v\le 50$, the derivative is positive, the original function is increasing. At $v=50$ we have that the derivative, which tells us the slope of the tangent line at a particular point on the original, is zero, thus the tangent line is horizontal:
	![[Pasted image 20240107200053.png|300]]
If we expanded this graph using many velocities $v<50$ we'd get a slope field correspondingly, 
	![[Pasted image 20240107200420.png|300]]
	- We note that anything above 50 would imply the object could defy gravity and start going upwards, which would seem as strange as it sounds
		- Note, that you should NEVER assume that the derivative will change signs where the derivative is zero. It is easy enough to check so you should always do so. And although it sounds strange for $v>50$ we shall continue talking about this assumption
We could continue to plug in values of $v>50$. Let's add some arrows and more graphs, 
	![[Pasted image 20240107201143.png|300]] 
This graph above is called the **directional field** for the differential equation.

So why do we care? There are two nice pieces of information that can be readily found from the direction field for a differential equation. 
1. **Sketch of Solution**. Since the arrows in the direction fields are in fact tangents to the actual solutions to the differential equations we can use these as guides to sketch the graphs of solutions to the differential equations 
2. **Long Term Behavior**. In many cases we are less interested in the actual solutions to the differential equations as we are in how the solutions behave as $t$ increases. Direction fields, if we can get our hands on them, can be used to find information about this long term behavior of the solution.
For instance, suppose we wanted to know the solution that has value $v(0) = 30$ looks like. We would start at $v(t) = 30$ when $t=0$ and we know the curve should flatten out at $v=50$. This gives us the figure below, 
	![[Pasted image 20240107202011.png|300]]
Let's get a better idea how the solutions are behaving for this differential equation with a graph. 
	![[Pasted image 20240107202137.png|300]] 
	We would call this set of solutions we've graphed a **family of solutions curves** or the set of **integral curves**. 
	For our falling object, it looks like all of the solutions will approach $v=50$ as $t$ increases. 


Ex: say for instance we have a differential equation $y' = y - x$, for this kind of differential equation, we can set the derivative equal to some constant $c$ which will give us a family of equations called **isoclines** that we can plot and on each of these curves the derivative will be a constant value of $c$.
	![[Pasted image 20240107203900.png|300]] 
	From here, we want to add different tangents for each of the isoclines, 
	![[Pasted image 20240107204058.png|300]] 
	If we image the isoclines no longer as integer number, or thinking about the tangents between each isocline, we would have, 
	![[Pasted image 20240107204223.png|300]]
	We now begin putting integral curves from the previous examples 
	![[Pasted image 20240107204259.png|300]]

### Section 1.3: Final Thoughts

For a few final thoughts before we moving on to the techniques to solving the differential equations, any equation will be concerned with answering one or more of the following questions: 
1. **Given a differential equation will a solution exist?**
	- Not all differential equations will have solutions and its nice to know that ahead of time. If there isn't a solution why waste our time trying to find something that doesn't exist? This questions is usually called the **existence questions** in a differential equations course. 
2. **If a differential equation does have a solution how many are there?**
	- We want to know how many solutions there are for a differential equation
		- what are the initial conditions required to produce a single unique solution to the differential equation?
		- Only one of our solutions will be accurate, but we will have no way of knowing which one is the correct solution for that particular circumstance.  
3. **If a differential equation does have a solution can we find it?**
	- The answer is not always yes. Just because we know a solution to a differential equation exists, doesn't mean we'll find it. 

