## Hamiltonian
$$
H=\frac{1}{2m}[\vec{p}-q\vec{A}]^{2} 
$$
This is the Hamiltonian of the electron with charge q constrained in a 2D plane.
## Kinetic momentum
define:
$$
\vec{\pi}=\vec{p}-q\vec{A}
$$
We find the commutation relations of the two components of $\vec{\pi}$
$$
\begin{align}
\left[\pi_{x},\pi_{y}\right]&=\left[p_{x}-qA_{x},p_{y}-qA_{y}\right] \\
&=\left[p_{x},-qA_{y}\right]+\left[-qA_{x},p_{y}\right] \\
&=i\hbar q(\partial _{x}A_{y}-\partial_{y}A_{x}) \\
&=i\hbar qB
\end{align}

$$
## Constructing the ladder operator
$$
a=\frac{1}{\sqrt{ 2q\hbar B }}(\pi_{x}+i\pi_{y})\quad a^{\dagger}=\frac{1}{\sqrt{ 2q\hbar B }}(\pi_{x}-i\pi_{y})
$$
find the commutator:
$$
\begin{align}
\left[a,a^{\dagger}\right]&=\frac{1}{2q\hbar B}\left[\pi_{x}+i\pi_{y},\pi_{x}-i\pi_{y}\right] \\
&=\frac{1}{2q\hbar B}\left[\pi_{x},-i\pi_{y}\right]+\left[i\pi_{y},\pi_{x}\right] \\
&=\frac{1}{2q\hbar B}(q\hbar B+q\hbar B) \\
&=1
\end{align}

$$
## Represent the Hamiltonian with ladder operator $a$

consider the product of the ladder operators:
$$
\begin{align}
a^{\dagger}a&=\frac{1}{2q\hbar B}(\pi_{x}+i\pi_{y})(\pi_{x}-i\pi_{y}) \\
&=\frac{1}{2q\hbar B}(\pi_{x}^{2}+\pi_{y}^{2}+i\left[\pi_{y},\pi_{x}\right]) \\
&=\frac{1}{2q\hbar B}(\vec{\pi}^{2}+i(-iq\hbar B)) \\
&=\frac{1}{2q\hbar B}(\vec{\pi}^{2})+\frac{1}{2} \\

\end{align}

$$
Hence after some manipulation:
$$
\begin{align}
H&=\frac{1}{2m}\vec{\pi}^{2} \\
&=\frac{1}{2m}2q\hbar B\left( a^{\dagger}a-\frac{1}{2} \right) \\
&=\hbar \omega_{c}\left( a^{\dagger}a-\frac{1}{2} \right)
\end{align}
$$
where we define the cyclotron frequency of the electron to be
$$
\omega_{c}=\frac{qB}{m}
$$
Now by representing the Hamiltonian interms of the ladder operators we conclude that:the lowest energy level of the electron in a 2D confinement is $-\frac{1}{2}\hbar \omega_{c}$
of course for electron the value of $q$ is negative which is $-e$ and the lowest energy level is positive.
and the ground state should be eliminated by the ladder operator $a$

Since we have not chosen a gauge, we have no explicit form of the vector potential $\vec{A}$ , actually to find the explicit wave function of the lowest energy state we shall impose an explicit form of the vector potential.
## Circular gauge

Choosing the curcular guage:
$$
\vec{A}=\left(-\frac{1}{2}By, \frac{1}{2}Bx ,0\right)

$$
The picture is vivid to explain the name of the gauge. If we plot the vector potential on a 2D plane, it looks circular! 
### The ladder operator 
Now we write the ladder operator explicitly:
$$
\begin{align}
a&=\frac{1}{\sqrt{ 2q\hbar B }}(\pi_{x}+i\pi_{y}) \\
&=\frac{1}{\sqrt{ 2q\hbar B }}(p_{x}+ip_{y}-q(A_{x}+iA_{y})) \\
&=\frac{1}{\sqrt{ 2q\hbar B }}\left( -i\hbar(\partial_{x}+i\partial_{y})-q\left( -\frac{1}{2}By+\frac{1}{2}iBx \right) \right) \\
&=\frac{1}{\sqrt{ 2q\hbar B }}\left( -2i\hbar \partial_{\bar{z}} -\frac{iBq}{2}(x+iy) \right) \\
&=\frac{1}{\sqrt{ 2q\hbar B }}\left( -2i\hbar \partial_{\bar{z}} -\frac{iBq}{2}z  \\
\right) \\
&=\frac{1}{\sqrt{ 2q\hbar B }}(-2i\hbar)\left( \partial_{\bar{z}}+\frac{Bq}{4\hbar}z \right)
\end{align}

$$
Now we state the form of the null space of the operator a
$$
\psi (z)=f(z)\exp\left( -\frac{Bq}{4\hbar}|z|^{2} \right)
$$
where the function $f(z)$ is analytic.

That is to say the ground state of the Landau levels possesses a large number of degeneracy, since we only require that the function $f(z)$ to be analytic!
## Another set of operators

Now we propose another set of operaors:
$$
\tilde{\pi}=\vec{p}+q\vec{A}
$$
indefining such operator we find out the commutators between $\tilde{\pi}$ and $\pi$ depends on the choice of gauge.
In the choice of a circular gauge, the commutators vanishes, i.e.
$$
\left[\pi,\tilde{\pi}\right]=0
$$
the commutation relations of $\tilde{\pi}$ is as follows:
$$
\left[\tilde{\pi}_{x},\tilde{\pi}_{y}\right]=-iq\hbar B
$$
## Another set of ladders

Define:
$$
b=\frac{1}{\sqrt{ 2q\hbar B }}(\tilde{\pi}_{x}-i\tilde{\pi}_{y})\quad b^{\dagger}=\frac{1}{\sqrt{ 2 q\hbar B}}(\tilde{\pi}_{x}+i\tilde{\pi}_{y})
$$
With such definition, we find the commutator
$$
\left[b,b^{\dagger}\right]=1
$$
The calculation is just as before.

Hence with such definition we know that there exists the ground state of the Landau levels would also be in the null space of the operator $b$

by definition:
$$
\begin{align} 
b&\propto (p_{x}-ip_{y}+q(A_{x}-iA_{y})) \\
&\propto -i\hbar(\partial_{x}-i\partial_{y})+q\left( -\frac{1}{2}B \right)(y+ix) \\
&\propto -2i\hbar \partial_{z}-\frac{iqB}{2}(x-iy) \\
&\propto \partial_{z}+\frac{qB}{4\hbar}\bar{z}

\end{align} 

$$
Hence the null space of it has the form of 
$$
\exp\left( -\frac{qB}{4\hbar} |z|^{2} \right)
$$
Hence:
$$
\ket{0,0}= \exp\left( -\frac{qB}{4\hbar} |z|^{2} \right)
$$
consider the $b^{\dagger}$ operator:
$$
b^{\dagger}\propto \partial_{\bar{z}}-\frac{qB}{4\hbar}z
$$
act this operator on the ground state, we obtain:
$$
\ket{0,m}\propto\left( \frac{z}{l_{B}} \right)^{m}\exp\left( -\frac{l_{B}}{4}|z|^{2} \right) 
$$
Now we see the ground state of the Landau levels have the explicit form as above.
