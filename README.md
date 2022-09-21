![alt text](task1 "Task 1")
# 1. Obtain all positions:
Firstly introduce all variables and positions we know from the task already:
$\theta = \frac{OM}{R}$

$\omega_r = \frac{d\theta}{dt}$

Point $O_1$:
$O_1 = [0,0]$

Point $O_2$:
$O_2 = [2R, 0]$

### Point O
$x = r cos(\phi)$

$y = r sin(\phi)$

### Point A:
$x = r*cos(\phi) + R$

$y = r*sin(\phi)$

### Point M:
$ x = O_x + R + R*cos(\pi - \theta)$

$ y = O_y + R*sin(\theta)$, if $\sin(\theta)\leq 0$, then $-R sin(\theta) + O_y$

$OM = s_r(t) = 6\pi t^2$

$|v_r| = \frac{d s_r(t)}{dt} = 12 \pi t$

$v^n_r = \vec{\omega_r} \times \vec{R}$

$v_r = \frac{d s_r(t)}{dt} = \frac{|s_r|}{dt} \vec{\tau} +\frac{|v_r|^2}{R}\vec{n} = \vec{v}^\tau_r + \vec{v}^n_r$

# 2. Find absolute, transport and relative velocities and accelerations for M:
Condition for implementing the semicircle movement:

$$i = \begin{cases} 1, &sin(\theta) \geq 0\\  
-1, & sin(\theta) < 0 \end{cases}$$

Angular velocities based on the angles:

$$\omega_{\theta} =
\begin{pmatrix}  
0\\
0 \\
\theta' 
\end{pmatrix} = 
\begin{pmatrix}
0\\
0 \\
-\frac{3\pi t}{R}i 
\end{pmatrix}$$

$$\omega_{\phi} = 
\begin{pmatrix}  0\\ 0 \\ \phi' 
\end{pmatrix} = 
\begin{pmatrix}  0\\ 0 \\ \frac{\pi t^2}{2} 
\end{pmatrix}$$

Angular accelerations based for angles $\theta$ and $\phi$:

$$\epsilon_{\theta} =
\begin{pmatrix}  
0\\ 
0 \\
\omega_\theta' 
\end{pmatrix} 
= \begin{pmatrix}
0\\ 
0 \\
-\frac{3\pi}{R}i 
\end{pmatrix}$$

$$\epsilon_{\phi} = \begin{pmatrix} 
0\\
0 \\
\omega_\phi' 
\end{pmatrix} 
= \begin{pmatrix}  
0\\
0 \\
\pi t
\end{pmatrix}$$


$V^{tr}_M = V_O = \omega_\phi \times O_1O$, since the body D is moves translational.
$V^{rel}_M = \omega_\theta \times \rho_m$ where $\rho_m = \vec{NM}$

Relative acceleration:
$a^\tau_M = \epsilon_\phi \times \rho_M$\
$a^n_M = \omega_\phi \times (\omega_\phi \times \rho_M)$

Transport acceleration:
$a^{tr}_M = a_O + \epsilon_{tr} \times \rho_M = a^\tau_O + a^n_O $
$a^\tau_O = \epsilon_\phi \times O_1O$\
$a^n_O = \omega_\phi \times (\omega_phi \times O_1O$

# 3. Find t, when M reaches O point:
$OM = \frac{OM}{R} = 6\pi t^2 = 2\pi R * k$ , where $k \in N$

$t^2 = \frac{2 R*k}{6} = \frac{R*k}{3}$

$t = \sqrt{\frac{Rk}{3}}$
---
# 4. Draw plots or put on siulation for previous statement:
All previous statements are simulated in [geogebra](https://www.geogebra.org/m/vkfjvsvj).
