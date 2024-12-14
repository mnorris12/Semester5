Thu Aug 22

Learning Goals: 
- Establish an expression for centripetal acceleration
- Explain the Centrifuge


We know from basic kinematics that the change in velocity is the acceleration. More specifically, the change in magnitude or the numerical value of the velocity, the direction, or all represents acceleration. In uniform circular motion, the magnitude of the velocity is the same, but the direction is constantly changing. you experience this when you drive through curves. 

The figure below shows the instantaneous velocity $v_{1},v_{2}$ at two locations. The direction of the instantaneous velocity changes, and the direction of that change is always towards the center of the circle. It’s the same direction as our acceleration vector, and it (should) be 90 degrees from the velocity vector itself. Coming from some external force, we call the acceleration due to uniform circular motion the **centripetal acceleration**. Centripetal itself means “towards the center”.

![[Pasted image 20240822174830.png|center|300]]

As you can see in the top right corner of the picture, the change in the velocity, or $\Delta v$ points towards the center. We notice that since acceleration is constant, it can be calculated as such
$$
\begin{gather}
a_{c} = \frac{\Delta v}{\Delta t}
\end{gather}
$$
similar to $v = \frac{\Delta D}{\Delta t}$ for constant change in direction. $\Delta s$ represents the arc length as usual which is normally equal to the radian angle multiplied by the arc radius. 
$$
\begin{gather}
s = \theta \cdot r
\end{gather}
$$
Since $\theta$ is small, $\Delta s \approx\Delta r$
❔- Stax says “because Δ𝜃 is very small, the arc length Δ𝑠Δs is equal to the chord length Δ𝑟Δr for small time differences.” I’m not sure how this could be the case.

Now that we know the direction of the centripetal acceleration is towards the center, how do we calculate the magnitude? Well, in the figure above, the triangle made by $\Delta r,\Delta s$ is similar to the triangle made by the velocity vectors. They both have two equal sides, making them isosceles triangles. Using one of the properties of similar triangles, 
$$
\begin{gather}
\frac{\Delta v}{v} = \frac{\Delta s}{r}
\end{gather}
$$
Now, we know what $a_{c}$ is above so, 
$$
\begin{gather}
\Delta v = \frac{\Delta s\cdot v}{r} \\ \\ 
\frac{\Delta v}{\Delta t} = \frac{\Delta s \cdot v}{r\cdot\Delta t} \\ \ \
a_{c} = \frac{v}{r} \frac{\cdot\Delta s}{\Delta t}
\end{gather}
$$
Lastly, we know that since $\Delta s$ represents the change in distance that, 
$$
\begin{gather}
\frac{\Delta s}{\Delta t} =v \\ \\
a_{c} = \frac{v^{2}}{r}
\end{gather}
$$
This gives the acceleration of an object moving in a circle with speed $v$ and radius $r$. As you can infer, when the speed increases, the cent. acceleration exponentially increases. As the radius of the circle increases, the cent. acceleration decreases. This is why it’s quite dangerous to go around tight curves (small radius) at high speeds. 

We also find it useful to write $a_{c}$ in terms of the angular velocity. We know from kinematics that $v=r\omega$ for motion in a circle. Substituting that into the above equation, we have, 
$$
\begin{gather}
a_{c} = \frac{(r\omega)^{2}}{r} = r\omega^{2}
\end{gather}
$$
![[Pasted image 20240822182107.png|center|300]]

Above is an example of centripetal motion used in science. We have a **Centrifuge**. It turns out that Centripetal motion is great for separating substances of different densities once combined together. They are often scaled in terms of the centripetal acceleration they exhibit relative to the acceleration due to gravity ($g$). 
 