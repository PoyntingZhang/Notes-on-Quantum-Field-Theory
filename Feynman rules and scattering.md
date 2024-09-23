### Feynman rules for fermions:

* A factor $\frac{i(\not{p}+m)}{p^2-m^2+i\epsilon}$ for each internal fermion line
* A factor $\frac{i}{p^2-m^2+i\epsilon}$ for each internal boson line
* A factor $u^s(p)$ for an incoming fermion with moentum p and spin s
* A factor $\bar{v}^s(p)$ for an incoming antifermion with momentum p and spin s
* A factor $\bar{u}^s(p)$ for an outgoing fermion
* A factor $v^s(p)$ for an outgoing antifermion
* Trace over the matrix product arising from a fermion loop
* Add minus sign factors reflecting fermion statistics, the most common of which is a factor -1 for every fermion loop. For two indistinguishable final state, swapping the two would end up with a factor -1 as well.
* Each vertex contributes a factor of $-i\lambda$ where $\lambda$ is the coupling strength

### Revision on interaction picture 
Interaction picture:
$$
H=H_{0}+H'
$$
In Schrodinger picture:
$$
i \frac{d}{dt} \ket{\psi}=H\ket{\psi}

$$
operator $O$ stays as a constant
Since the state obeys a first order differential equation, we can find a unitary time evolution operator that satisfies:
$$
\ket{\psi(t)}=U(t,t')\ket{\psi(t')}

$$
$$
i \frac{d}{dt}U(t,t')=HU(t,t')
$$

In Heisenber picture:
$$
\frac{d}{dt}\ket{\psi}=0

$$
In order to hold the expectation invariant:
$$
\braket{ \psi(t) |O|\psi(t)  }=\braket{ \psi(0) |O(t)|\psi(0)  }  
$$
$$
O(t)=U^{\dagger}(t,0)OU(t,0)
$$
Interaction picture, this is something between the Schrodinger and Heisenber picture:
$$
\ket{\psi}_{I}=e^{iH_{0}t} \ket{\psi}_{S} \quad \ket{\psi}_{S}=e^{-iH_{0}t}\ket{\psi}_{I}  
$$
Substitute back into the Schrodinger equation:
$$
\begin{align}
i \frac{d}{dt}e^{-iH_{0}t}\ket{\psi}_{I}=(H_{0}+H')e^{-iH_{0}t}\ket{\psi}_{I} \\
e^{-iH_{0}t}\left( i \frac{d}{dt}\ket{\psi}_{I} \right)=H'e^{-iH_{0}t}\ket{\psi}_{I}  \quad\\ 
i \frac{d}{dt }\ket{\psi}_{I}=e^{iH_{0}t}H'e^{-iH_{0}t}\ket{\psi}_{I}\quad\quad   \\
\text{define:}\quad \quad H_{I}= e^{iH_{0}t}H'e^{-iH_{0}t}\quad\quad\quad\quad \\
\text{hence:}\quad\quad i \frac{d}{dt}\ket{\psi}_{I}=H_{I}\ket{\psi}_{I}\quad\quad\quad\quad  
\end{align}

$$
Hence the corresponding time evolution operator:
$$
i \frac{d}{dt} U(t,t')=H_{I}U(t,t')
$$
By Dyson formula:
$$
U(t,t')=\mathcal{T}\exp\left( -i \int_{t'}^t H_{I}(\tau)d\tau\right)
$$
### S matrix
We assume naively that the initial state and final state are eigenstates of the free theory with Hamiltonian $H_{0}$
$$
\mathcal{A}=\braket{ f |U_{I}(+\infty,-\infty)|i  }=\braket{ f|S|i  }  
$$
By definition of S matrix:
$$
S=U_{I}(+\infty,-\infty)=\mathcal{T}\exp\left( -i \int_{-\infty}^{+\infty}H_{I}(\tau)d\tau \right)
$$
In terms of the Hamiltonian density:
$$
S=\mathcal{T}\exp\left( -i \int d^4x\mathcal{H}_{I}(x) \right)
$$
With the definition of the S matrix, we get that to calculate the scattering amplitude due to an interaction, we need to follows the steps:
* Second quantise the interaction part of the Hamiltonian
* expand the S matrix, and sandwich the desired order of expansion between the initial state and final states of free theory.
* Notice the time ordering and moving the operators around to obtain a final result.
This is wehre the Feynman comes in, it is a general conclusion on this process with the aid of diagrams.
