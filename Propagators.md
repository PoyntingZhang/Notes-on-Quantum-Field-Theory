$$
\overbrace{\psi(x)\bar{\psi}(y)}=T(\psi(x)\bar{\psi}(y))-:\psi(x)\bar{\psi}(y):=S_{F}(x-y)
$$
$$
S_{F}(x-y)=i \int \frac{d^4p}{(2\pi)^4}e^{-ip\cdot(x-y)}\frac{\gamma \cdot p+m}{p^2-m^2+i\epsilon}
$$
Now we may check that it is indeed the propagator of the Dirace fermion field.
By definition of propagaror:
$$
\begin{align}
S_{F}(x-y)&:=\braket{ 0 |T(\psi(x))\bar{\psi} (y)|0 }  \\
 
\end{align}

$$
if $x^0>y^0$:
$$
S_{F}(x-y)=\braket{ 0 |\psi(x)\bar{\psi})(y|0  } 
$$
if $x^0<y^0$:
$$
S_{F}(x-y)=\braket{ 0 |-\bar{\psi}(y)\psi(x) |0 } 
$$
Notice that different from the Bosons, the time ordering operator take up a minus sign as swapping the operator once.
we are going to find the vaues of $S_{F}(x^0>y^0)$and$S_{F}(x^0<y^0)$respectively:
$$
\psi(x)=\sum_{s}\int \frac{d^3p}{(2\pi)^3}[b_{\vec{p}}^su^s(\vec{p})e^{-ip\cdot x}+c^{s\dagger}_{\vec{p}}v^s(\vec{p})e^{ip\cdot x}]
$$
$$
\bar{\psi}(y)=\sum_{r}\int \frac{d^3q}{(2\pi)^3}[b^{r\dagger}_{\vec{q}}\bar{u}^r(\vec{q})e^{iq\cdot y}+c_{\vec{q}}^r\bar{v}^r(\vec{q})e^{-iq\cdot y}]
$$
$$
\begin{align} \\
S_{F}(x^0>y^0)&=\braket{0|\psi(x)\bar{\psi}(y)|0} \\
&=\braket{0|\sum_{s}\int \frac{d^3p}{(2\pi)^3}[b_{\vec{p}}^su^s(\vec{p})e^{-ip\cdot x}+c^{s\dagger}_{\vec{p}}v^s(\vec{p})e^{ip\cdot x}]\sum_{r}\int \frac{d^3q}{(2\pi)^3}[b^{r\dagger}_{\vec{q}}\bar{u}^r(\vec{q})e^{iq\cdot y}+c_{\vec{q}}^r\bar{v}^r(\vec{q})e^{-iq\cdot y}]|0} \\
&=\braket{0|\sum_{s}\int \frac{d^3p}{(2\pi)^3}u^s(\vec{p})\bar{u}^s(\vec{p})e^{-ip\cdot(x-y)}|0} \\
&=\int \frac{d^3p}{(2\pi)^3}\sum_{s}u^s(\vec{p})\bar{u}^s(\vec{p})e^{-ip\cdot(x-y)} \\
&=\int \frac{d^3p}{(2\pi)^3} \frac{1}{2E_{\vec{p}}}  (\not{p}+m)e^{-ip\cdot(x-y)} 

\end{align} 

$$
$$
\begin{align}
S_{F}(x^0<y^0)&=\braket{0|-\bar{\psi}(y)\psi(x)|0} \\
&=-\braket{0|\sum_{r}\int \frac{d^3q}{(2\pi)^3}[b^{r\dagger}_{\vec{q}}\bar{u}^r(\vec{q})e^{iq\cdot y}+c_{\vec{q}}^r\bar{v}^r(\vec{q})e^{-iq\cdot y}]\sum_{s}\int \frac{d^3p}{(2\pi)^3}[b_{\vec{p}}^su^s(\vec{p})e^{-ip\cdot x}+c^{s\dagger}_{\vec{p}}v^s(\vec{p})e^{ip\cdot x}]|0} \\
&=-\braket{0|\sum_{r}\sum_{s}\int \int \frac{d^3qd^3p}{(2\pi)^{3}}c_{\vec{q}}^rc^{s\dagger}_{\vec{p}}\bar{v}^r(\vec{q})v^s(\vec{p})e^{-iq\cdot y}e^{ip\cdot x}|0} \\
&=-\sum_{s}\int \frac{d^3p}{(2\pi)^3} \frac{1}{2E_{\vec{p}}}  (\not{p}-m)e^{ip\cdot(x-y)}
\end{align}

$$
Where we have utilised the relation that:
$$
\braket{0|b_{\vec{p}}^sb^{r\dagger}_{\vec{q}}|0}=\{b_{\vec{p}}^s,b^{r\dagger}_{\vec{q}}\}=(2\pi)^3\delta(\vec{p}-\vec{q})\delta^{rs}
$$
Then we can show that indeed the Greens function of the Dirac equation is the Propagator of the field by integrating over  $p_{0}$ and choose the integration contour properly
### Wick's theorem:
$$
\begin{align}  
T(\phi_{1}\phi_{2}\phi_{3}\dots)=:\phi_{1}\phi_{2}\phi_{3}\dots:+:\text{all the other contractions}:


\end{align} 

$$
This is the same for the fermionic operators:
$$
T(\psi_{1}\psi_{2}\psi_{2}\dots)=:\psi_{1}\psi_{2}\psi_{2}\dots:+:\text{all the other contractions:}
$$
Notice that the difference between the two is:
$$
T(\phi_{1}\phi_{2})=T(\phi_{2}\phi_{1})\quad T(\psi_{1}\psi_{2})=-T(\psi_{2}\psi_{1})
$$
$$
:\phi_{1}\phi_{2}:=:\phi_{2}\phi_{1}:\quad :\psi_{1}\psi_{2}:=-:\psi_{2}\psi_{1}:
$$
$$
\overbrace{\phi_{1}\phi_{2}}=\overbrace{\phi_{2}\phi_{1}}\quad\overbrace{\psi_{1}\psi_{2}}=-\overbrace{\psi_{2}\psi_{1}}
$$
