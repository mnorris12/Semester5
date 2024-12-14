#### Basic physics and math with astro applications 
$$
\begin{gather}
F = ma \\ \\ 
F_{\text{cent}} = \frac{m v^{2}}{r} \\ \\ 
F = \frac{GMm}{r^{2}}
\end{gather}
$$
The third equation is Newton’s universal law of gravitation. It represents the attractive force of two different bodies or masses separated by some distance $r$. The gravitational constant $G$ is $6.674*10^{-11} (\frac{m^{3}}{kg\cdot s})$

1. Combine the first and third to show that $g = 9.8 \hspace{.2cm} \frac{m}{s^{2}}$ on the Earth’s surface.

**Solution:** 
We set the equations equal and solve for $a$
$M = 5.9722\cdot10^{24} \hspace{.2cm}\text{kg}$ 
$G = 6.674*10^{-11} (\frac{m^{3}}{kg\cdot s^{2}})$
$r = 6371\cdot10^{3} \hspace{.2cm} m$

$$
\begin{gather}
F = ma \hspace{.5cm} F = \frac{GMm}{r^{2}} \\ \\
ma = \frac{GMm}{r^{2}} \\ \\
a = \frac{GM}{r^{2}} \\ \\ 
a = \frac{\left(6.674*10^{-11} (\frac{m^{3}}{kg\cdot s^{2}})\right)\left(5.9722\cdot10^{24} \hspace{.2cm} kg\right)}{\left(6371\cdot10^{3} \hspace{.2cm} m\right)^{2}} \\ \\ 
a = 9.8 \frac{m}{s^{2}}
\end{gather}
$$


2. Combine the second and third to show that $P^{2} =\frac{a^{3}}{M}$ for a circular orbit of a low-mass object (m) around a high mass object (M).
**Solution**:
$v = \frac{2\pi r}{P}$ which is the equation for tangential velocity where $P$ represents the period of the smaller object around the larger object. We use the second and third equation: 
$$
\begin{gather}
\frac{GMm}{r^{2}} = \frac{mv^{2}}{r} \\ \\ 
\frac{GM}{r^{2}} = \frac{v^{2}}{r} \\ \\ 
\frac{GM}{r^{2}}=\frac{4\pi^{2}r^{2}}{P^{2}r} \\ \\ 
GM =\frac{4\pi^{2}r^{3}}{P^{2}} \\ \\ 
P^{2}G = \frac{4\pi^{2}r^{3}}{M} \\ \\ 
P^{2} = \left( \frac{4\pi^{2}}{G} \right) r^{3}
\end{gather}
$$
and if we replace $r$ with $a$ representing the length of the semi-major axis in AU
$$
\begin{gather}
P^{2} = \left( \frac{4\pi^{2}}{G} \right) a^{3}
\end{gather}
$$


#### Q1. a

To find the distance a lightbulb would have to be so that it has the same brightness as Sirius, we’d need to use the equation to determine the flux given distance and luminosity of an object, $F = \frac{L}{4\pi d^{2}}$ We isolate $d$ or the distance from Sirius to earth,
$$
\begin{gather}
F_{s}   = 1.2*10^{-7}( W m^{-2} )\\ \\
F_{LB}= 1.2*10^{-7} (Wm^{-2}) = \frac{100W}{4\pi d ^{2}} \\ \\ 
d = \sqrt{ \frac{100W}{4\pi(1.2*10^{-7}Wm^{-2})} } = 8140(m) \hspace{.5cm} 8.140 (km)
\end{gather}
$$

#### Q1. b

The energy carried by a single photon of monochromatic light, $E=h\left( \frac{c}{\lambda} \right)$, is proportional to the wavelength of the light. Most lightbulbs emit a broad spectrum of light, but in the case of a light bulb that emits mostly in the infrared, it may be less efficient due to it’s nature to release it’s energy mostly in the form of heat. So if it’s visible light you’re looking for, the brightness would change by decreasing substantially. If you have an aperture for infrared, then I would think they would have similar amounts of brightness.


#### Q2. a

I like to think of the $m^{-2}$ in relation to concentric shells composed of the light of the star.  As the star emits light, the light spreads out and the energy per unit area of that shell decreases. Thus,  $m^{-2}$ comes from the area of the shell. The shell that touches the eye, telescope, or another apparatus determines the flux or apparent brightness. That’s how I think about it. 

#### Q2. b

The flux of the sun on earth or $F_{\text{S on E}} = 1370(Wm^{-2})$.  If we want to calculate the luminosity of the sun, we can use flux equation and solve for luminosity
$$
\begin{gather}
F = \frac{L}{4\pi d^{2} } \\ \\ 
L = F(4\pi d^{2})
\end{gather}
$$
Thus, the sun’s luminosity, 
$$
\begin{gather}
L = (1370(Wm^-{2}))(4\pi(1.496*10^{11}m)^{2}) = 3.85*10^{26} W
\end{gather}
$$
Now that we have the sun’s luminosity, we need to convert 1.52 AU to meters,
$$
\begin{gather}
1.52(AU) \cdot \frac{1.496*10^{11}m}{1AU} = 2.27*10^{11}m
\end{gather}
$$
Now we can calculate the Flux of the sun on Mars, 
$$
\begin{gather}
F_{\text{s on m} } = \frac{3.85*10^{26}W}{4\pi(2.27*10^{11}m)^{2}} = 595 (Wm^{-2})
\end{gather}
$$
This is a little less than half the flux of the sun on earth. This makes sense because when we square their distances to the sun, the denominator for the flux on Mars is a little over double what is for Earth. 

#### Q2. C

We’ve already calculated the Luminosity of the sun which is about $3.85*10^{26}W$. If we wanted to find the surface flux of the sun, we’d use our flux equation as we’ve done previously noting that the sun’s radius is $6.69*10^8m$, 
$$
\begin{gather}
F_{\text{s on ss}} = \frac{3.85*10^{26}W}{4\pi(6.96*10^8m)^{2}} = 6.32*10^7Wm^{-2}
\end{gather}
$$
#### Q3. a

Stars that have more flux should have smaller magnitudes. This makes sense, because, without looking things up, the scale from 1-6 (or whatever number the finest telescope today can achieve), 1 represents the brightest. I would also expect that a redder star will be brighter in the $V$ filter, since the energy from the star is mostly converted into visibly light rather than something like heat. Also, and more definitively, since the 7800- 6220 angstroms range has more area under the $V$ filter curve (using figure 13.2) than $B$, it should have more transmittance (and thus brightness) in the $V$ filter. 

By definition of the magnitude scale, Vega, has a color index of $B-V=0$, which corresponds to a scale of redness (or blueness) of stars of the Blue-Visual color index. Because color indices depend on the stars surface temperature, a star who has $B-V>0$ will be a colder and thus redder star than one who has the same color index as Vega. Thus, star 2 is redder. 

#### Q3. b

To find the apparent magnitude of star 2, we can subtract the B-V color index of star 2 from star 1, 
$$
\begin{gather}
(B-V)_{1} -(B-V)_{2} = 0-1 = -1
\end{gather}
$$
Since $B_{S1} =B_{S2} = V_{S_{1}}$, we have, 
$$
\begin{gather}
10-10-10+V_{s_{2}} = -1 \\ \\ 
V_{s_{2}} = -1+10 = 9
\end{gather}
$$
Thus $V_{s_{2}}$ has apparent magnitude of 9. This makes sense as $(B-V)_{2}=10-9=1$. 

#### Q3. C

To find the distance of the binary system from a telescope, we first start by using the absolute magnitude of the main sequence star $M_{V}$,
$$
\begin{gather}
M_{v} = m_{v}-5\log\left( \frac{d}{10pc} \right) \\ \\ 
M_{v} - m_{v} = -5\log\left( \frac{d}{10pc} \right) \\ \\ 
\frac{m_{v}-M_{v}}{5} = \log\left( \frac{d}{10pc} \right) \\ \\ 
d = (10^{\frac{(m_{v}-M_{v})}{5}})\cdot 10pc
\end{gather}
$$
Given our answer in part b,  $m_{v}=9$. Since $M_{v}$ = 6.7, we have all the pieces we need. 
$$
\begin{gather}
d = 10^{2.3/5}*10pc = 29 pc
\end{gather}
$$
so the binary is 29$pc$ away. 

#### Q4

Fun with unit conversions! 1 $nm$ is equal to $10^{-7}m$ so 656 $nm$ is $6.56*10^{-7}$ $m$. We can now calculate the energy of a single photon in this monochromatic light, 
$$
\begin{gather}
E = \frac{(6.626*10^{-34} J\cancel{ s })\left( 3.0*10^8 \frac{\cancel{ m }}{\cancel{ s }} \right)}{(6.56*10^-7\cancel{ m })} = 2.83*10^{-19} J
\end{gather}
$$
Using the the conversion factor from $J$ to $eV$ on page 111, 
$$
\begin{gather}
2.83*10^{-19}J \cdot \frac{1 eV}{(1.602*10^{-19}J)} = 1.79 eV
\end{gather}
$$
#### Q5

If the photon that should excite our bound electron has a wavelength of 656 $nm$, and we want the electron, upon absorbing the photon, to excite from one level to another, it would have to be in level $n=3$, in the Paschen series. This is because the difference $\Delta E$ between $n=1$ and $n=2$ is $(13.61-3.40)eV = 10.21eV$ which is greater than the energy our photon can provide, so after absorbing our photon in $n=1$, it will still be in $n=1$. It is also why the photon can’t excite an electron in the ground state. If the bound electron starts in $n=2$, then after absorbing $1.79$ $eV$ from the photon, it would have energy $E=-1.89 eV$, which isn’t quite enough energy required for $n=3$. If it starts in $n=3$, the energy threshold needed is only $.67eV$ to achieve $n=4$ or higher, thus our bound electron would need to be in $n=3$ if it wanted to move from one level to another.  


#### Q6. a

If your dog has temperature 310 $K$ and is roughly $.3$ $m^{2}$, we know immediately that she emits mostly in the infrared. This makes sense because electromagnetic energy emission of her body are usually, just like humans, seen with infrared detectors rather than the naked eye. 

#### Q6. b
To find how many Joules she emits per day, we’ll use the Stefan-Boltzmann law,
$$
\begin{gather}
F = \sigma T^4 \\ \\ 
F = \left( 5.67*10^{-8} \frac{W}{m^{2}K^4} \right)(310K)^4 = 524W
\end{gather}
$$
This makes sense, because like a light bulb, humans emit about 100W. Since Watts is equal to $\frac{J}{s}$, we just have to multiply our answer by a seconds to day conversion factor, 
$$
\begin{gather}
 524W \cdot\frac{(86400s)}{1 \hspace{.2cm}\text{day}} = 4.52*10^7\frac{J}{\text{day}}
\end{gather}
$$
Every day, your dog radiates about $4.52*10^7 \frac{J}{day}$. 

#### Q7

From the open stax, the average velocity of gas with many nitrogen molecules can be calculated by
$$
\begin{gather}
\bar{v} = \sqrt{ \frac{8}{\pi}\cdot \frac{kT}{m} } \\ \\
\bar{v} = \sqrt{ \frac{8}{\pi} \cdot \frac{(1.38*10^{-23}m^{2}kgs^{-2}K^{-1})(300K)}{4.65\cdot10^{-26}kg} } \\ \\ 
\bar{v} = \sqrt{ 227000 \frac{m^{2}}{s^{2}}} = 476 \frac{m}{s}
\end{gather}
$$
So the nitrogen in the air travels about 476 $\frac{m}{s}$.

#### Q8. a 

Fun with unit conversions! I have some handy unit conversions from my physics 6 text book, so I’ll just convert and jug, 
$$
\begin{gather}
1 Pa = 1(N m^{-2}) = 1\left( kg\cdot \frac{m}{s} \right)m^{-2} = 1 \left( \frac{kg}{s^{2}m} \right) 
\end{gather}
$$
The farthest right almost looks like Joules, but not quite. We know, 
$$
\begin{gather}
J  = \frac{kgm^{2}}{s^{2}}
\end{gather}
$$
if we then multiply joules that by $m^{-3}$, 
$$
\begin{gather}
\frac{kgm^{2}}{s^{2}} \cdot m^{-3} = \frac{kg}{s^{2}m}
\end{gather}
$$
which is back to where we were. Thus pressure can be expressed as $Jm^{-3}$ or as energy per volume (energy density).

#### Q8. b

We determined in part a that $1 Pa = 1\left( \frac{kg}{s^{2}m} \right)$. The units of momentum are $\frac{kg\cdot m}{s}$. Momentum per unit area per time is thus, 
$$
\begin{gather}
\underbrace{ \frac{kg\cdot m}{s} }_{ \text{momentum} } \cdot \underbrace{ \frac{1}{sm^{2}} }_{ \text{per unit area per time} } =  1\left( \frac{kg}{s^{2}m} \right)
\end{gather}
$$
which is equal to a pascal. Therefore, pressure can be thought of as momentum flux. 

#### Q9. a

The formula for the gravitational potential energy, 
$$
\begin{gather}
U = \frac{GMm}{R} = \frac{(6.67*10^{-11}(N\cdot \frac{m^{2}}{kg^{2}}) )\cdot\left(1kg\right)\left(5.97\cdot10^{24}kg\right)}{\left(6.37\cdot10^{6}m\right)} = 6.25*10^7Nm = 6.25*10^7 J
\end{gather}
$$

for anywhere else on earth, $6.37*10^6m<R<0m$. This implies that as you go closer to the Earth’s center, your gravitational potential energy increases. 

#### Q9. b

I enjoy this question because the derivation process is seen in various places. I’ll elaborate before getting into my answer. It made me think of the energy stored in an electric field, or, 
$$
\begin{gather}
U = \frac{\epsilon_{0}}{2} \int E^{2}\cdot \, dvol
\end{gather}
$$
which is one reason why it makes sense to me that there’s gravitational potential energy stored in mass. Just making some connections to somewhat unrelated things. 

Anyhow, we return to our gravitational potential energy equation, 
$$
\begin{gather}
U = -\frac{GMm}{R} 
\end{gather}
$$
If we want the gravitational potential energy of a sphere with a uniform mass distribution, we can essentially add up the gravitational potential energy for all the concentric shells with radius $0<r<R$. We think about the change in $U,m$, and then the larger mass $M$ becomes the total mass in some radius $0<r<R$. It looks like,
$$
\begin{gather}
du  = -\frac{GM_{r}dm}{r} =- \frac{GM_{r}}{r} (\rho \cdot 4\pi r^{2}dr)
\end{gather}
$$
 $\rho$ is the mass per volume of a solid sphere with some $r$, so it can be defined as $\rho =\frac{M_{r}}{\frac{4}{3}\pi r^{3}}=\frac{3M_{r}}{4\pi r^{3}}$. Thus, $M_{r}= \frac{4\pi r^{3}\rho}{3}$. Really, $\rho$ doesn’t have to be defined by $M_{r}$. As long as the mass and radius are proportional, it’s all good . I just did that for simplicity. Anyway, we can simplify, 
 $$
\begin{gather}
du  = -GM_{r}(\rho \cdot 4 \pi r dr) = -G \frac{4\pi r^{3}\rho}{3}\cdot(\rho \cdot4\pi r dr) = -\frac{G(16\pi^{2}r^4\rho^{2})}{3}
\end{gather}
$$
Now we integrate from o to $R$ and clean up, 
$$
\begin{gather}
\int  \, du = U =- \frac{16G\rho^{2}\pi^{2}}{3}\int_{0}^r r^4  \, dr  =- \frac{16G\rho^{2}\pi^{2}}{3} \frac{R^5}{5} = -\frac{16G\rho^{2}\pi^{2}R^5}{15}
\end{gather}
$$
This is what I got. Now, checking the solution, they replaced $\rho$ for $\frac{M}{\left( \frac{4}{3}\pi R^{3} \right)}$ or $\frac{3M}{4\pi R^{3}}$. So if I plug that into what I got, 
$$
\begin{gather}
-\frac{16G\left( \frac{3M}{4\pi R^{3}} \right)^{2}\pi^{2}R^5}{15} = -\frac{16G\left( \frac{9M^{2}}{16\pi^{2}R^6} \right)\pi^{2}R^5}{15} = \\ \\ 
-\frac{9M^{2}G}{15R} = -\frac{3M^{2}G}{5R} = -\frac{3}{5} \frac{GM^{2}}{R}
\end{gather}
$$
So it seems like I landed at the same result, albeit with a less aesthetic presentation. 