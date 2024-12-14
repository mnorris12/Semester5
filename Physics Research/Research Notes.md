##### Strelka Computer Cluster Examination

Questions:
- What is a computer cluster?
	- In short, a computer cluster is a network of computers that work together to accomplish a single. There are different types of computer clusters, but all balance the workload or tasks provided, and are optimal for high speed task perfomance. They're typically used in data management, scientific research, financial modeling, etc
- "The cluster consists of 18 nodes, each with two CPUs with an additional head node to handle user logins and job scheduling."
	- What is a node, what is a CPU, what is a head node?
		- A node is a computer.  A CPU or Central Processing Unit is like the brain of a computer/mode. It preformes many tasks like arithmetic calculations, stores and executes instructions, logic operations, datamovement, etc. Modern CPU are composed of multiple cores which in themselves execute multiple instructions independently. The speed and efficiency of a CPU is messured in gigahertz, and the number of instructions it can handle per clock cycle is measured in IPS. 
	- 12 mid-memory nodes (384GB - 512GB RAM)
	- 3 high-memory nodes (768GB RAM)
	- 1 high-CPU node (72 cores)
	- 2 GPU nodes, each with 4x NVIDIA 2080 Ti GPUs
	- Over 700TB storage
	- High speed Infiniband networking
- What does all the stuff above mean and refer to?
	- I think with the information provided above, you can decipher what each of those things mean. They are just in reference to the capabilities and pre  fomance of the node/computer. 
- I would suggest doing a look around in Slurm. It's where all the "jobs" are submitted
	- There's also a Slurm's command page that might be interesting


#### Fri June 21

$$
\begin{gather}
\ln(a)
\end{gather}
$$

#### PTA Vanderbilt

Gravitational Wave Theory: 
1. Einstein Field Equations
$$
\begin{gather}
G_{\mu r} = \frac{8\pi G}{c^4} \cdot \underbrace{ T_{\mu r} }_{ \text{stress energy tensor} }
\end{gather}
$$
all the information encoded in general relativity are from the Einstein eq $G_{\mu r}$. 

A lot of GR is making terms disapear by going to a different coordinate system




##### Tue July 9
Vocabulary: 
- SAM (Semi-Analytic Models)
- Holodeck - nanograv astroWG
- magnetic flux freezing
- dispersion sweep
- Subpulse Drifting
- Pulse Nulling

Timing Response due to GWs

1. $g_{\mu \nu}$ $\rightarrow$ $ds^{2} = g_{\mu \nu}dx^\mu dx^\nu$

Introduction to Statistical inference: 
##### Thu July 11

$$
\begin{gather}
TOA = t_{0}+NP- \frac{1}{c}\hat{n} \cdot \vec{D}+ R_{gw}(t)
\end{gather}
$$