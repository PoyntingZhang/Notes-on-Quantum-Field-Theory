## Positive frequency solution
$$
(i\gamma^\mu \partial_{\mu}-m)\psi=0
$$
Adopting the chiral representation of Clifford algebra:
$$
\begin{align}
&\gamma^\mu=\begin{pmatrix}0&\sigma^\mu\\ \bar{\sigma}^\mu&0\end{pmatrix} \\ \\
 
&\sigma=\begin{pmatrix}1&\vec{\sigma} \end{pmatrix}\\
\\
&\bar{\sigma}=\begin{pmatrix}1&-\vec{\sigma}\end{pmatrix}\\ \\
&i\gamma^\mu \partial_{\mu}-m=\begin{pmatrix}
-m&i\sigma^\mu \partial_{\mu}\\ i\bar{\sigma}^\mu \partial_{\mu}&-m
\end{pmatrix} \\ \\
&\begin{pmatrix}
-m&i\sigma^\mu \partial_{\mu}\\ i\bar{\sigma}^\mu \partial_{\mu}&-m
\end{pmatrix} \begin{pmatrix}u_{+}\\u_{-}\end{pmatrix}=\begin{pmatrix}0\\0\end{pmatrix}

\end{align}


$$



proposing a positive frequency solution:
$$
\begin{pmatrix}u_{+}\\u_{-}\end{pmatrix}=u(\vec{p})\exp(-ipx)
$$
back substitute into the Chirla form of the Dirac equation:
$$
\begin{pmatrix}-m& p \cdot\sigma\\p \cdot\bar{\sigma}&-m\end{pmatrix}\begin{pmatrix}u_{+}\\u_{-}\end{pmatrix}=\begin{pmatrix}0\\0\end{pmatrix}
$$
The solution is claimed to be:
$$
u(\vec{p})=\begin{pmatrix}\sqrt{ p \cdot \sigma }\xi\\\sqrt{ p \cdot \bar{\sigma} }\xi\end{pmatrix}
$$
The arbitrary vector $\xi$ gives a degree of freedom of two.
## Negative frequency solution
$$
\begin{pmatrix}v_{+}\\v_{-}\end{pmatrix}=v(\vec{p})\exp(ipx)
$$

$$
\begin{pmatrix}-m& -p\cdot\sigma\\-p \cdot\bar{\sigma}&-m\end{pmatrix}\begin{pmatrix}v_{+}\\v_{-}\end{pmatrix}=\begin{pmatrix}0\\0\end{pmatrix}
$$
the solution is claimed to be:

$$
v(\vec{p})=\begin{pmatrix}\sqrt{ p \cdot \sigma }\eta\\-\sqrt{ p \cdot \bar{\sigma} }\eta\end{pmatrix}
$$
Still notice that there are two independent degrees of freedom.
We have just analysed that the Dirac field has only four degrees of freedom hence any solution to the Dirac equation can be written as linear combinations of the two $u$ and two $v$ basis

identity:
$$
\begin{align}
\sqrt{ p \cdot \sigma }\cdot \sqrt{ p \cdot \bar{\sigma} }=m \\
\end{align}

$$



## Two dimensional spinor
The Dirac spinor is the 4-component spinor, while the two $\xi$ and the two $\eta$ 's are the two-component spinors, which corresponds to spin up and spin down.
helicity operator:
the rotation generator is $S^{ij}$:
$$
h=\frac{i}{2}\epsilon_{ijk}\hat{p^i}S^{ij}
$$
With such definition we can see that a spin up particle boosted along the z direction is with helicity:1/2(right handed), a spin down particle boosted along the z direction is with helicity -1/2(left handed).

$$
\begin{align}


u^s(\vec{p})=\begin{pmatrix}
\sqrt{ \sigma \cdot p }\xi^s\\\sqrt{ \bar{\sigma}\cdot p }\xi^s
\end{pmatrix} \\
 \\
v^s(\vec{p})=\begin{pmatrix}
\sqrt{ \sigma \cdot p }\eta^s\\-\sqrt{ \bar{\sigma}\cdot p }\eta^s
\end{pmatrix}
\end{align}

$$
some identieies:delta
Inner products:
$$
\begin{align} \\


u^{s\dagger}(\vec{p})\cdot u^r(\vec{p})=2p_{0} \delta^{rs} \\
\bar{u^{s}}(\vec{p})\cdot u^r(\vec{p})=2m \delta^{rs} \\
v^{s\dagger}(\vec{p})\cdot v^r(\vec{p})=2p_{0} \delta^{rs} \\
\bar{v^{s}}(\vec{p})\cdot v^r(\vec{p})=-2m \delta^{rs} \\
\bar{u^s}(\vec{p})\cdot v^r(\vec{p})=0 \\
u^{s\dagger}(\vec{p})\cdot v(-\vec{p})=0
\end{align}

$$
outer products:
$$
\begin{align}
\sum_{s=1}^2u^s(\vec{p})\bar{u^s}(\vec{p})=\not{p}+m \\
\sum_{s=1}^2v^s(\vec{p})\bar{v^s}(\vec{p})=\not{p}-m
\end{align}


$$
With all these algebric relations prepared we shall move on to quantise the Dirac field.
## Second quantisation of Dirac field
As usual since the theory is non-interacting, we quantise the field operator as superposition of plane wave solutions:
$$
\psi(x)=\sum_{s=1}^2\int \frac{d^3p}{(2\pi)^3} \frac{1}{\sqrt{2E_{\vec{p}}}}[b_{\vec{p}}^s u^s(\vec{p})e^{i\vec{p}\cdot \vec{x}}+c_{\vec{p}}^{s\dagger} v^s(\vec{p})e^{-i\vec{p}\cdot \vec{x}}]


$$
$$
\psi ^{\dagger}(x)=\sum_{s=1}^2\int \frac{d^3p}{(2\pi)^3} \frac{1}{\sqrt{2E_{\vec{p}}}}[b_{\vec{p}}^{s\dagger} u^{s\dagger}(\vec{p})e^{-i\vec{p}\cdot \vec{x}}+c_{\vec{p}}^{s} v^{s\dagger}(\vec{p})e^{i\vec{p}\cdot \vec{x}}]
$$
Applying a naive procedure of second quantisation, imposing the commutation relations:
$$
[\psi(\vec{x}),\psi ^{\dagger}(\vec{y})]=\delta(\vec{x}-\vec{y})\begin{pmatrix}
1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1
\end{pmatrix}
$$
It can be shown that it is equivalent to setting the relations:
$$
[b^s_{\vec{p}},b^{r\dagger}_{\vec{q}}]=(2\pi)^3\delta(\vec{p}-\vec{q})\delta^{rs}

$$
$$
[c^s_{\vec{p}},c^{r\dagger}_{\vec{q}}]=-(2\pi)^3\delta(\vec{p}-\vec{q})\delta^{rs}
$$
Notice that the negative sign here is odd. And if operator $c^s_{\vec{p}}$ represents an annihliation operator, then the state $\ket{\vec{p},s}$ would have a negative norm, which does not make sense! Thus the c operator without dagger must represents the creation operator.
Consider the Hamiltonian:
$$
\begin{align}
\mathcal{H}&=\pi \dot{\psi}-\mathcal{L} \\
&=-\bar{\psi}(i\gamma^i\partial_{i}-m)\psi \\
&=\bar{\psi}(-i\gamma^i\partial_{i}+m)\psi
\end{align}

$$
Consider the term:
$$
\begin{align}


(-i\gamma^i\partial_{i}+m)\psi&=(-i\gamma^i\partial_{i}+m)\sum_{s=1}^2\int \frac{d^3p}{(2\pi)^3} \frac{1}{\sqrt{2E_{\vec{p}}}}[b_{\vec{p}}^s u^s(\vec{p})e^{i\vec{p}\cdot \vec{x}}+c_{\vec{p}}^{s\dagger} v^s(\vec{p})e^{-i\vec{p}\cdot \vec{x}}] \\
&=\sum_{s=1}^2\int \frac{d^3p}{(2\pi)^3} \frac{1}{\sqrt{2E_{\vec{p}}}}[b_{\vec{p}}^s u^s(\vec{p})(-\gamma^ip_{i}+m)e^{i\vec{p}\cdot \vec{x}}+c_{\vec{p}}^{s\dagger} v^s(\vec{p})(\gamma^ip_{i}+m)e^{-i\vec{p}\cdot \vec{x}}]  \\
&=\sum_{s=1}^2\int \frac{d^3p}{(2\pi)^3} \frac{1}{\sqrt{2E_{\vec{p}}}}[b_{\vec{p}}^s u^s(\vec{p})(\gamma^0p_{0})e^{i\vec{p}\cdot \vec{x}}+c_{\vec{p}}^{s\dagger} v^s(\vec{p})(-\gamma^0p_{0})e^{-i\vec{p}\cdot \vec{x}}]  \\
&=\sum_{s}\gamma^0\int \frac{d^3p} {(2\pi)^3}\sqrt{ \frac{E_{\vec{p}}}{2} }[b_{\vec{p}}^s u^s(\vec{p})e^{i\vec{p}\cdot \vec{x}}-c_{\vec{p}}^{s\dagger}v^s(\vec{p})e^{-i\vec{p}\cdot \vec{x}}]

\end{align}
$$

We have used the fact that the $u,v$ functions as the plane wave solution to the Dirac equation:

$$\begin{align}
&\quad(\gamma^0p_{0}+\gamma^ip_{i}-m)u(\vec{p})=0 \\
&\to(-\gamma^ip_{i}+m)u(\vec{p})=\gamma^0p_{0}u(\vec{p}) \\
&\quad(-\gamma^0p_{0}-\gamma^ip_{i}-m)v(\vec{p})=0 \\
&\to(\gamma^ip_{i}+m)v(\vec{p})=-\gamma^0p_{0}v(\vec{p})
\end{align}

$$
$$
\begin{align}
\mathcal{H}=\bar{\psi}(-i\gamma^i\partial_{i}+m)\psi  \\
H=\sum_{s}\int d^3p(2\pi)^{-3}E_{\vec{p}}[b^{s\dagger}_{\vec{p}}b^s_{\vec{p}}-c_{\vec{p}}^sc^{s\dagger}_{\vec{p}}]
\end{align}
$$
Here is where the trouble comes in. 
As usual we can normalise the operators, swapping the c dagger and c. However this still leaves us with a minus sign. Now the Hamiltonian of the system is not bounded below!
## Anticommute relations
### Fermionic Quantisation
The spin-statistics theorem says that integer spin fields must be quantised as bosons, while half-integer spin fields must be quantised as fermions. Any attempt to do otherwise will lead to an inconsistency, such as the unbounded Hamiltonian.
commutation relations:
$$
[a^{\dagger}_{\vec{p}},a^{\dagger}_{\vec{q}}]=0
$$
leads to:
$$
a^{\dagger}_{\vec{p}}a^{\dagger}_{\vec{q} }\ket{vac}=a^{\dagger}_{\vec{q}}a^{\dagger}_{\vec{p}}\ket{vac}  
$$
that is :
$$
\ket{\vec{p},\vec{q}}=\ket{\vec{q},\vec{p}}
$$
Of course this holds for any bosons.
However for fermions:
$$
\ket{\vec{p},\vec{q}}=-\ket{\vec{q},\vec{p}}  
$$
This requires that:
$$
\{a^{s\dagger }_{\vec{p}},a^{r\dagger}_{\vec{q}}\}=0
$$
That is to say for fermions we requires anticommutators to describes the algebric structure of the operator space.
For Dirac field, the correct quantisation is:
$$
\{\psi_{\alpha}(\vec{x}),\psi ^{\dagger}_{\beta}(\vec{y})\}=\delta_{\alpha,\beta}\delta(\vec{x}-\vec{y})\\
\quad \text{other equals zero}
$$
This can be shown to be equivalent to the set of relations:
$$
\begin{align}
\{b^r_{\vec{p}},b^{s\dagger}_{\vec{q}}\}=(2\pi)^3\delta^{rs}\delta(\vec{p}-\vec{q})  \\
\{c^r_{\vec{p}},c^{s\dagger}_{\vec{q}}\}=(2\pi)^3\delta^{rs}\delta(\vec{p}-\vec{q}) \\

\end{align}


$$
And any other comutators equals zero.
The previous calculations holds, since we replaced all the commutators with anticommutatos. And we obtain the same expression for the Hamiltonian:
$$
\begin{align}
H&=\sum_{s}\int d^3p(2\pi)^{-3}E_{\vec{p}}[b^{s\dagger}_{\vec{p}}b^s_{\vec{p}}-c_{\vec{p}}^sc^{s\dagger}_{\vec{p}}] \\
&=\sum_{s}\int d^3p(2\pi)^{-3}E_{\vec{p}}[b^{s\dagger}_{\vec{p}}b^s_{\vec{p}}+c^{s\dagger}_{\vec{p}}c_{\vec{p}}^s-(2\pi)^3\delta(0)]
\end{align}

$$
## Ladder operators
Recall the Hamiltonian of the Harmonic oscillator:
$$
H=\hbar \omega \left( a^{\dagger}a+\frac{1}{2} \right)

$$
$$
[a,a^{\dagger}]=1
$$
$$

[H,a^{\dagger}]=\hbar \omega a^{\dagger} \quad [H,a]=-\hbar wa

$$
## Ladder operators for Dirac field:
$$
\begin{align}
[H,b_{\vec{p}}^r]=-E_{\vec{p}} b_{\vec{p}}^r\quad\quad[H,c_{\vec{p}}^r]=-E_{\vec{p}} c_{\vec{p}}^r\\ \\
[H,b_{\vec{p}}^{r \dagger}]=E_{\vec{p}}b_{\vec{p}}^{r \dagger}\quad\quad[H,c_{\vec{p}}^{r \dagger}]=E_{\vec{p}}c_{\vec{p}}^{r \dagger}
\end{align}

$$
That is to say we can again construct a tower of energy eigenstates by acting on the vacuum by the two sets of operators to create particles, and antiparticles, just as in the bosonic case.
