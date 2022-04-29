# Definition of the Continuous Medium

## The Concept of Continuum

* Microscopic scale:
  * matter is made of atoms which may be grouped in molecules.
  * matter has gaps and spaces.
* Macroscopic scale:
  * atomic and molecular discontinuities are disregarded.
  * matter is assumed to be continuous.

## Continuous Medium or Continuum

* Matter is studied at a macroscopic scale: it <u>completely fills the space</u>, there exist no gaps or empty spaces.
* Assumption that the medium and is made of infinite particles (of infinitesimal size) whose properties are describable by <u>continuous functions</u> with continuous derivatives.

# Equations of Motion

## Material and Spatial points, Configuration

* A continuous medium is formed by an infinite number of particles which occupy different positions in space during their movement over time.
  * **==MATERIAL POINTS==**: particles
  * **==SPATIAL POINTS==**: fixed spots in space
* The **==CONFIGURATION==** $\Omega_t$ of a continuous medium at a given time ($t$) is the locus of the positions occupied by the material points of the continuous medium at the given time.

## Configurations of the Continuous Medium

> $\Omega_0$: non-deformed (or reference) configuration, at reference time $t_0$.
>
> $\Gamma_0$: non-deformed boundary.
>
> $X$: position vector of a particle at reference time.
>
> > $t_0=0$	$\rightarrow$ reference time

> $\Omega$ or $\Omega_t$: deformed (or present) configuration, at present time $t$.
>
> $\Gamma$ or $\Gamma_t$: deformed boundary.
>
> $x$: position vector of the same particle at present time.
>
> > $t\in[0,T]$	$\rightarrow$ current time

## Material and Spatial Coordinates

* the position vector of a given particle can be expressed in:

  * non-deformed or reference configuration

    $[\textbf{X}]=\begin{Bmatrix}X_1\\X_2\\X_3\end{Bmatrix}=\begin{Bmatrix}X\\Y\\Z\end{Bmatrix}\equiv$ material coordinates (capital letter)

  * deformed or present configuration

    $[\textbf{x}]=\begin{Bmatrix}x_1\\x_2\\x_3\end{Bmatrix}=\begin{Bmatrix}x\\y\\z\end{Bmatrix}\equiv$ spatial coordinates (small letter)

## Equations of Motion

* the motion of a given particle is described by the evolution of its spatial coordinates (or its position vector) over time.

  $\varphi(X,t)$ $\rightarrow$ $\begin{cases}\textbf{x}=\varphi(\text{particle label},t)=\textbf{x}(\text{particle label},t)\\x_i=\varphi_i(\text{particle label}, t)\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

  $\varphi(\text{particle label},t)$ is the motion that takes the body from a reference configuration to the current one.

* the **==Canonical Form==** of the Equation of Motion is obtained when the "particle label" is taken as its material coordinates

  particle label $\equiv\begin{Bmatrix}X_1&X_2&X_3\end{Bmatrix}^T\equiv\textbf{X}$	$\begin{cases}\textbf{x}=\varphi(\textbf{X},t)\stackrel{not.}{=}\textbf{x}(\textbf{X},t)\\x_i=\varphi(X_1,X_2,X_3,t)\space\space\space{i\in\{1,2,3\}}\end{cases}$

## Inverse Equation of Motion

* the inverse equations of motion give the material coordinates as a function of the spatial ones.

  $\varphi^{-1}(\textbf{x},t)$ $\rightarrow$ $\begin{cases}\textbf{X}=\varphi^{-1}(\textbf{x},t)\stackrel{not.}{=}\textbf{X}(\textbf{x},t)\\X_i=\varphi^{-1}_i(x_1,x_2,x_3,t)\space\space\space{i\in\{1,2,3\}}\end{cases}$

## Mathematical restrictions for $\varphi$ and $\varphi^{-1}$ defining a "physical" motion

* **Consistency condition**

  * $\varphi(\textbf{X},0)=\textbf{X}$, as $\textbf{X}$ is the position vector for $t=0$

* **Continuity condition**

  * $\varphi\in{C^1}$, $\varphi$ is continuous with continuous derivatives

* **Biunivocity condition**

  * $\varphi$ is biunivocal to guarantee that two particle do not occupy simultaneously the same spot in space and that particle does not occupy simultaneously more than one spot in space.

    ==Mathematically==: the "Jacobian" of the motion's equations should be different from zero:

    $J=\left|\dfrac{\part\varphi(\textbf{X},t)}{\part{\textbf{X}}}\right|=\text{det}\left[\dfrac{\part\varphi_i}{\part\textbf{X}_j}\right]\neq0$

* **==The "Jacobian" of the equations of motion should be "strictly positive"==**

  $J=\left|\dfrac{\part\varphi(\textbf{X},t)}{\part{\textbf{X}}}\right|=\text{det}\left[\dfrac{\part\varphi_i}{\part\textbf{X}_j}\right]>0$	$\Rightarrow$ density is always positive (to be proven)

### Example

the spatial description of the motion of a continuous medium is given by:

$\textbf{x}(\textbf{X},t)\equiv\begin{cases}x_1=X_1e^{2t}\\x_2=X_2e^{-2t}\\x_3=5X_1t+X_3e^{2t}\end{cases}\equiv\begin{cases}x=Xe^{2t}\\y=Ye^{-2t}\\z=5Xt+Ze^{2t}\end{cases}$

check the mathematical restrictions:

* **Consistency Condition** $\varphi(\textbf{X},0)=\textbf{X}$?

  $\textbf{x}(\textbf{X},t=0)=\begin{Bmatrix}x_1=X_1e^{2\cdot0}\\x_2=X_2e^{-2\cdot0}\\x_3=5X_1\cdot0+X_3e^{2\cdot0}\end{Bmatrix}=\begin{Bmatrix}X_1\\X_2\\X_3\end{Bmatrix}=\textbf{X}$	:heavy_check_mark:

* **Continuity Condition** $\varphi\in{C}^1$?					:heavy_check_mark:

* **Biunivocity Condition**?

  $J=\begin{vmatrix}\dfrac{x_i}{\part{X_j}}\end{vmatrix}=\begin{vmatrix}\dfrac{x_1}{\part{X_1}}&\dfrac{x_1}{\part{X_2}}&\dfrac{x_1}{\part{X_3}}\\\dfrac{x_2}{\part{X_1}}&\dfrac{x_2}{\part{X_2}}&\dfrac{x_2}{\part{X_3}}\\\dfrac{x_3}{\part{X_1}}&\dfrac{x_3}{\part{X_2}}&\dfrac{x_3}{\part{X_3}}\end{vmatrix}=\begin{vmatrix}e^{2t}&0&0\\0&e^{-2t}&0\\5t&0&e^{2t}\end{vmatrix}=e^{2t}\cdot{e^{-2t}}\cdot{e^{2t}}=e^{2t}\neq0$	$\forall{t}$	:heavy_check_mark:

* **Density positive**?		$J=\begin{vmatrix}\dfrac{\part\varphi(\textbf{X},t)}{\part{\textbf{X}}}\end{vmatrix}>0$		$J=e^{2t}>0$		:heavy_check_mark:

calculate the inverse equation of motion.

$x_1=X_1e^{2t}$  $\Rightarrow$  $X_1=\dfrac{x_1}{e^{2t}}=x_1e^{-2t}$

$x_2=X_2e^{-2t}$  $\Rightarrow$  $X_2=\dfrac{x_2}{e^{-2t}}=x_2e^{2t}$

$x_3=5X_1t+X_3e^{2t}$  $\Rightarrow$  $X_3=\dfrac{x_3-5X_1t}{e^{2t}}=(x_3-5(x_1e^{-2t})t)e^{-2t}=x_3e^{-2t}-5tx_1e^{-4t}$

$\Rightarrow$	$\textbf{X}\equiv\varphi^{-1}(\textbf{x},t)=\begin{cases}X_1=x_1e^{-2t}\\X_2=x_2e^{2t}\\X_3=x_3e^{-2t}-5tx_1e^{-4t}\end{cases}$

# Descriptions of Motion

* the mathematical description of the particle properties can be done in two ways:
  * material (Lagrangian) description
  * spatial (Eulerian) description

## Material or Lagrangian Description

* the physical properties are described in terms of the <u>**material coordinates**</u> and <u>**time**</u>.
* it focuses on what is occurring at a <u>**fixed material point**</u> (a particle, labeled by its material coordinates) as time progresses.
* normally used in <u>**solid mechanics**</u>.

## Spatial or Eulerian Description

* the physical properties are described in terms of the <u>**spatial coordinates**</u> and <u>**time**</u>.
* it focuses on what is occurring at a <u>**fixed point in space**</u> (a spatial point labeled by its spatial coordinates) as time progresses.
* normally used in <u>**fluid mechanics**</u>.

### Example

the equation of motion of a continuous medium is:

$\textbf{x}=\textbf{x}(\textbf{X},t)=\begin{cases}x=X-Yt\\y=Xt+Y\\z=-Xt+Z\end{cases}$

find the spatial description of the property whose material description is:

$\bar{\rho}(X,Y,Z,t)=\dfrac{X+Y+Z}{1+t^2}$

calculate the inverse equations:

$\begin{cases}x=X-Yt\space\space\Rightarrow\space\space X=x+Yt\\y=Xt+Y\space\space\Rightarrow\space\space X=\dfrac{y-Y}{t}\end{cases}\Rightarrow$  $x+Yt=\dfrac{y-Y}{t}$  $\Rightarrow$  $Yt^2+Y=y-xt$  $\Rightarrow$  $Y=\dfrac{y-xt}{1+t^2}$

$X=x+Yt=x+\left(\dfrac{y-xt}{1+t^2}\right)t=\dfrac{x+xt^2+yt-xt^2}{1+t}=\dfrac{x+yt}{1+t^2}$

$z=-Xt+Z$	$\Rightarrow$	$Z=z+Xt=z+\left(\dfrac{x+yt}{1+t^2}\right)t=\dfrac{z+zt^2+xt+yt^2}{1+t^2}$

$\Rightarrow$ $\textbf{X}=\varphi^{-1}(\textbf{x},t)=\begin{cases}X=\dfrac{x+yt}{1+t^2}\\Y=\dfrac{y-xt}{1+t^2}\\Z=\dfrac{z+zt^2+xt+yt^2}{1+t^2}\end{cases}$

$\bar{\rho}(X,Y,Z,t)=\dfrac{X+Y+Z}{1+t^2}=\dfrac{\left(\dfrac{x+yt}{1+t^2}\right)+\left(\dfrac{y-xt}{1+t^2}\right)+\left(\dfrac{z+zt^2+xt+yt^2}{1+t^2}\right)}{1+t^2}=\dfrac{x+y+yt+yt^2+z+zt^2}{(1+t^2)^2}\\=\rho(x,y,z,t)$

# Time Derivatives

## Material and Local Derivatives

* the time derivative of a given property can be defined based on the:
  * material description $\Gamma(\textbf{X},t)\rightarrow$**TOTAL** or **MATERIAL DERIVATIVE**
    * variation of the property w.r.t time following a specific particle in the continuous medium.
    * material derivative $\equiv\dfrac{\part\Gamma(\textbf{X},t)}{\part{t}}\rightarrow$$\begin{cases}\text{partial time derivative of the}\\\textbf{material description}\text{ of the property}\end{cases}$
  * spatial description $\gamma(\textbf{x},t)\rightarrow$**TOTAL** or **SPATIAL DERIVATIVE**
    * variation of the property w.r.t time in a fixed spot of space.
    * local derivative $\equiv\dfrac{\part\gamma(\textbf{x},t)}{\part{t}}\rightarrow$$\begin{cases}\text{partial time derivative of the}\\\textbf{spatial description}\text{ of the property}\end{cases}$

## Convective Derivative

* remember: $\textbf{x}=\textbf{x}(\textbf{X},\text{t})$, therefore, $\gamma(\textbf{x},\text{t})=\gamma(\textbf{x}(\textbf{X},\text{t}),\text{t})=\Gamma(\textbf{x},\text{t})$

* the material derivative can be computed in terms of spatial descriptions:

  material derivative $\rightarrow$ $\stackrel{not.}{=}\dfrac{d}{dt}\gamma(\textbf{x},t)\stackrel{not.}{=}\dfrac{D}{Dt}\gamma(\textbf{x},t)=\dfrac{\part\Gamma(\textbf{X},t)}{\part{t}}=$

  $=\dfrac{d}{dt}\gamma(\textbf{x}(\textbf{X},t),t)=\dfrac{\part\gamma(\textbf{x},t)}{\part{t}}+\underbrace{\dfrac{\part\gamma}{\part{x_i}}}_{[\nabla\gamma]_i}\cdot\underbrace{\dfrac{\part{x_i}}{\part{t}}}_{\left[\dfrac{\part{\textbf{x}}}{\part{t}}\right]_i}=\dfrac{\part\gamma(\textbf{x},t)}{\part{t}}+\underbrace{\underbrace{\dfrac{\part\gamma}{\part\textbf{x}}}_{\nabla\gamma(\textbf{x},t)}\cdot\underbrace{\dfrac{\part\textbf{x}}{\part{t}}}_{\textbf{v}(\textbf{x},t)}}_{\textbf{v}(\textbf{x},t)\cdot\nabla\gamma(\textbf{x},t)}=$

* generalizing for any property:

  $\underbrace{\dfrac{d\varkappa(\textbf{x},t)}{dt}}_{\text{material derivative}}=\underbrace{\dfrac{\part\varkappa(\textbf{x},t)}{\part{t}}}_{\text{local derivative}}+\underbrace{\textbf{v}(\textbf{x},t)\cdot\nabla\varkappa(\textbf{x},t)}_{\text{convective rate of change (convective derivative)}}$

  > ==REMARK== the spatial Nabla operator is defined as: $\nabla=\dfrac{\part}{\part{x}_i}\hat{\textbf{e}}_i$

### Example

given the following equation of motion:

$\textbf{x}(\textbf{X},t)=\begin{cases}x=X+Yt+Zt\\y=Y+2Zt\\z=Z+3Xt\end{cases}$

and the spatial description of a property $\rho(\textbf{x},t)=3x+2y+3t$

calculate its material derivative.

* **Option #1: Computing the material derivative from material descriptions**

  ​	obtain $\rho$ as a function of $\textbf{X}$ by replacing the Eqns. of motion into $\rho(\textbf{x},\text{t})$:

  ​	$\rho(\textbf{x},t)=\rho(\textbf{x}(\textbf{X},t),t)=\bar\rho(\textbf{X},t)=3(X+Yt+Zt)+2(Y+2Zt)+3t\\=3X+3Yt+2Y+7Zt+3t$

  ​	calculate its material derivative as the partial derivative of the material description:

  ​	$\dfrac{d\rho(\textbf{x},t)}{dt}\Bigr|_{\textbf{x}=\textbf{x}(\textbf{X},t)}=\dfrac{\part\bar\rho(\textbf{X},t)}{\part{t}}=\dfrac{\part}{\part{t}}(3X+3Yt+2Y+7Zt+3t)=3Y+7Z+3$

  ​	$\dfrac{d\rho(\textbf{x},t)}{dt}\Bigr|_{\textbf{x}=\textbf{x}(\textbf{X},t)}=\dfrac{\part\bar\rho(\textbf{X},t)}{\part{t}}=3+3Y+7Z$

* **Option #2: Computing the material derivative from spatial descriptions**

  ​	$\dfrac{d\rho(\textbf{x},t)}{dt}=\dfrac{\part\rho(\textbf{x},t)}{\part{t}}+\textbf{v}(\textbf{x},t)\cdot\nabla\rho(\textbf{x},t)$

  ​	applying this on $\rho(\textbf{x},t)$:

​		$\begin{cases} \dfrac{\part\rho(\textbf{x},t)}{\part{t}}=\dfrac{\part}{\part{t}}(3x+2y+3t)=3\\ \textbf{v}(\textbf{x},t)\Bigr|_{\textbf{x}=\textbf{x}(\textbf{X},t)}=\dfrac{\part\textbf{x}}{\part{t}}=\begin{bmatrix}\dfrac{\part}{\part{t}}(X+Yt+Zt)\\\dfrac{\part}{\part{t}}(Y+2Zt)\\\dfrac{\part}{\part{t}}(Z+3Xt)\end{bmatrix}=\begin{bmatrix}Y+Z\\2Z\\3X\end{bmatrix}\\ \nabla\rho(\textbf{x},t)=\begin{bmatrix}\dfrac{\part\rho(\textbf{x},t)}{\part{x}}\\\dfrac{\part\rho(\textbf{x},t)}{\part{y}}\\\dfrac{\part\rho(\textbf{x},t)}{\part{z}}\end{bmatrix}=\begin{bmatrix}\dfrac{\part}{\part{x}}(3x+2y+3t)\\\dfrac{\part}{\part{y}}(3x+2y+3t)\\\dfrac{\part}{\part{z}}(3x+2y+3t)\end{bmatrix}=\begin{bmatrix}3\\2\\0\end{bmatrix} \end{cases}$

​		$\dfrac{d\rho(\textbf{x},t)}{dt}=\dfrac{d\rho(\textbf{x}(\textbf{X},t),t)}{dt}=3+\underbrace{\underbrace{\begin{bmatrix}Y+Z&2Z&3X\end{bmatrix}}_{[\textbf{v}]^T}\underbrace{\begin{bmatrix}3\\2\\0\end{bmatrix}}_{[\nabla\rho]}}_{\textbf{v}\cdot(\nabla\rho)}=3+3Y+3Z+4Z$

​		$\dfrac{d\rho(\textbf{x},t)}{dt}\Bigr|_{\textbf{x}=\textbf{x}(\textbf{X},t)}=3+3y+7Z$

# Velocity and Acceleration

## Velocity

* **<u>Time derivative</u>** of the equation of motion.

  * material description of the velocity:

    time derivative of the equations of motion

    > ==REMARK== remember the equations of motion are of the form:
    >
    > $\textbf{x}=\varphi(\textbf{X},t)\stackrel{not.}{=}\textbf{x}(\textbf{X},t)$

    $\begin{cases}\textbf{V}(\textbf{X},t)=\dfrac{\part\textbf{x}(\textbf{X},t)}{\part{t}}\\V_i(\textbf{X},t)=\dfrac{\part{x_i}(\textbf{X},t)}{\part{t}}\space\space\space{i\in\{1,2,3\}}\end{cases}$

  * spatial description of the velocity:

    velocity is expressed in terms of $\textbf{x}$ using the inverse equation of motion:

    $\textbf{V}(\textbf{X}(\textbf{x},t),t)$  $\Rightarrow$  $\textbf{v}(\textbf{x},t)$

## Acceleration

* **<u>Material time derivative</u>** of the velocity field.

  * material description of acceleration:

    derivative of the material description of velocity:

    $\begin{cases}\textbf{A}(\textbf{X},t)=\dfrac{\part\textbf{V}(\textbf{X},t)}{\part{t}}\\A_i(\textbf{X},t)=\dfrac{\part{V_i}(\textbf{X},t)}{\part{t}}\space\space\space{i\in\{1,2,3\}}\end{cases}$

  * spatial description of acceleration:

    $\textbf{A}(\textbf{X},t)$ is expressed in terms of $\textbf{x}$ using the inverse equations of motion:

    $\textbf{A}(\textbf{X}(\textbf{x},t),t)$  $\Rightarrow$  $\textbf{a}(\textbf{x},t)$

    or $\textbf{a}(\textbf{x},t)$ is obtained directly through the material derivative of $\textbf{v}(\textbf{x},t)$:

    $\begin{cases}\textbf{a}(\textbf{x},t)=\dfrac{d\textbf{v}(\textbf{x},t)}{dt}=\dfrac{\part\textbf{v}(\textbf{x},t)}{\part{t}}+\textbf{v}(\textbf{x},t)\cdot\nabla\textbf{v}(\textbf{x},t)\\a_i(\textbf{x},t)=\dfrac{d\text{v}_i(\textbf{x},t)}{dt}=\dfrac{\part\text{v}_i(\textbf{x},t)}{\part{t}}+\text{v}_k(\textbf{x},t)\cdot\frac{\part\text{v}_i}{\part{x_k}}\textbf{v}(\textbf{x},t)\space\space\space{i\in\{1,2,3\}}\end{cases}$

### Example

consider a solid that rotates at a constant angular velocity $\omega$ and has the following equation of motion:

$\textbf{x}(\underbrace{R,\phi}_{\text{label of particle}},t)\rightarrow\begin{cases}x=R\space{\text{sin}(\omega{t}+\phi)}\\y=R\space{\text{cos}(\omega{t}+\phi)}\end{cases}$

$\rightarrow$ (non-canonical equations of motion)

Find the velocity and acceleration of the movement described in both, material and spatial forms.

> Using the expressions
>
> $\begin{cases}\text{sin}(a\pm{b})=\text{sin}a\cdot\text{cos}b\pm\text{cos}a\cdot\text{sin}b\\\text{cos}(a\pm{b})=\text{cos}a\cdot\text{cos}b\mp\text{sin}a\cdot\text{sin}b\end{cases}$

**The equation of motion can be rewritten as**:

$\begin{cases}x=R\space\text{sin}(\omega{t}+\phi)=R\space\text{sin}(\omega{t})\cdot\text{cos}\phi+R\space\text{cos}(\omega{t})\cdot\text{sin}\phi\\y=R\space\text{cos}(\omega{t}+\phi)=R\space\text{cos}(\omega{t})\cdot\text{cos}\phi-R\space\text{sin}(\omega{t})\cdot\text{sin}\phi\end{cases}$

For $\text{t}=0$, the equation of motion becomes: $\begin{cases}X=R\space\text{sin}\phi\\Y=R\space\text{cos}\phi\end{cases}$

Therefore, the equation of motion in terms of the material coordinates is:

$\begin{cases}x=R\space\text{sin}(\omega{t}+\phi)=\overbrace{\boxed{R}\space\text{sin}(\omega{t})\cdot\boxed{\text{cos}\phi}}^{Y\sin(\omega{t})}+\overbrace{\boxed{R}\space\text{cos}(\omega{t})\cdot\boxed{\text{sin}\phi}}^{X\cos(\omega{t})}=X\cos(\omega{t})+Y\sin(\omega{t})\\y=R\space\text{cos}(\omega{t}+\phi)=\underbrace{\boxed{R}\space\text{cos}(\omega{t})\cdot\boxed{\text{cos}\phi}}_{Y\cos(\omega{t})}-\underbrace{\boxed{R}\space\text{sin}(\omega{t})\cdot\boxed{\text{sin}\phi}}_{X\sin(\omega{t})}=-X\sin(\omega{t})+Y\cos(\omega{t})\end{cases}$

The inverse equation of motion is easily obtained

$\begin{matrix}x=X\cos(\omega{t})+Y\sin(\omega{t})\Rightarrow X=\dfrac{x-Y\sin(\omega{t})}{\cos(\omega{t})}\space\space\space\space\space\space\\y=-X\sin(\omega{t})+Y\cos(\omega{t})\Rightarrow X=\dfrac{-y+Y\cos(\omega{t})}{\sin(\omega{t})}\end{matrix}\Rightarrow\begin{equation*}\begin{CD}\dfrac{x-Y\sin(\omega{t})}{\cos(\omega{t})}=\dfrac{-y+Y\cos(\omega{t})}{\sin(\omega{t})}\\@VVV\end{CD}\end{equation*}$

​									$x\sin(\omega{t})-Y\sin^2(\omega{t})=-y\cos(\omega{t})+Y\cos^2(\omega{t})$

​									$x\sin(\omega{t})+y\cos(\omega{t})=Y\underbrace{\left(\sin^2(\omega{t})+\cos^2(\omega{t})\right)}_{=1}$

$X=\dfrac{x-\left(x\sin(\omega{t})+y\cos(\omega{t})\right)\sin(\omega{t})}{\cos(\omega{t})}=\dfrac{x}{\cos(\omega{t})}-\dfrac{x\sin^2(\omega{t})}{\cos(\omega{t})}-\dfrac{y\cos(\omega{t})\sin(\omega{t})}{\cos(\omega{t})}=$

$=x\underbrace{\dfrac{1-\sin^2(\omega{t})}{\cos(\omega{t})}}_{=\cos(\omega{t})}-y\sin(\omega{t})$

So, the equation of motion and its inverse in terms of the material coordinates are:

$\boxed{\textbf{x}(\textbf{X},t)\rightarrow\begin{cases}x=X\cos(\omega{t})+Y\sin(\omega{t})\\y=-X\sin(\omega{t})+Y\cos(\omega{t})\end{cases}}$		$\rightarrow$ canonical equations of motion

$\boxed{\textbf{X}(\textbf{x},t)\rightarrow\begin{cases}X=x\cos(\omega{t})-y\sin(\omega{t})\\Y=x\sin(\omega{t})+y\cos(\omega{t})\end{cases}}$		  $\rightarrow$ inverse equations of motion

**Velocity in material description** is obtained from $\textbf{V}(\textbf{X},t)=\dfrac{\part\textbf{x}(\textbf{X},t)}{\part{t}}$

$\textbf{V}(\textbf{X},t)=\dfrac{\part\textbf{x}(\textbf{X},t)}{\part{t}}=\begin{cases}\dfrac{\part{x}}{\part{t}}=\dfrac{\part}{\part{t}}\left(X\cos(\omega{t})+Y\sin(\omega{t})\right)\\\dfrac{\part{x}}{\part{t}}=\dfrac{\part}{\part{t}}\left(-X\sin(\omega{t})+Y\cos(\omega{t})\right)\end{cases}$

$\textbf{V}(\textbf{X},t)=\begin{Bmatrix}V_x\\V_y\end{Bmatrix}=\begin{Bmatrix}-X\omega\sin(\omega{t})+Y\omega\cos(\omega{t})\\-X\omega\cos(\omega{t})-Y\omega\sin(\omega{t})\end{Bmatrix}$

**Velocity in spatial description** is obtained introducing $\textbf{X}(\textbf{x},t)$ into $\textbf{V}(\textbf{X},t)$:

$\begin{cases}x=X\cos(\omega{t})+Y\sin(\omega{t})\\y=-X\sin(\omega{t})+Y\cos(\omega{t})\end{cases}\rightarrow$ $\textbf{v}(\textbf{x},t)=\textbf{V}(\textbf{X}(\textbf{x},t),t)=\begin{Bmatrix}\text{V}_x\\\text{V}_y\end{Bmatrix}=\begin{matrix}\overbrace{\left[-X\sin(\omega{t})+Y\cos(\omega{t})\right]}^{y}\omega\\\underbrace{\left[-X\cos(\omega{t})-Y\sin(\omega{t})\right]}_{-x}\omega\end{matrix}=\begin{Bmatrix}\omega{y}\\-\omega{x}\end{Bmatrix}$

$\boxed{\textbf{v}(\textbf{x},t)=\begin{Bmatrix}\text{V}_x\\\text{V}_y\end{Bmatrix}=\begin{Bmatrix}\omega{y}\\-\omega{x}\end{Bmatrix}}$

**Acceleration in material description** is obtained applying: $\textbf{A}(\textbf{X},t)=\dfrac{\part\textbf{V}(\textbf{X},t)}{\part{t}}$

$\textbf{A}(\textbf{V},t)=\dfrac{\part\textbf{V}(\textbf{X},t)}{\part{t}}=\begin{cases}\dfrac{\part{V}_x}{\part{t}}=-X\omega^2\cos(\omega{t})-Y\omega^2\sin(\omega{t})\\\dfrac{\part{V}_y}{\part{t}}=X\omega^2\sin(\omega{t})-Y\omega^2\cos(\omega{t})\end{cases}$

$\textbf{A}(\textbf{V},t)=\begin{Bmatrix}A_x\\A_y\end{Bmatrix}=-\omega^2\begin{Bmatrix}X\cos(\omega{t})+Y\sin(\omega{t})\\-X\sin(\omega{t})+Y\cos(\omega{t})\end{Bmatrix}$

(**OPTION #1**): **Acceleration in spatial description** is obtained by replacing the inverse equation of motion into $\textbf{A}(\textbf{X},t)$:

$\textbf{a}(\textbf{x},t)=\textbf{A}(\textbf{X}(\textbf{x},t),t)=\\=-\omega^2\begin{Bmatrix}(x\cos(\omega{t})-y\sin(\omega{t}))\cos(\omega{t})+(x\sin(\omega{t})+y\cos(\omega{t}))\sin(\omega{t})\\-(x\cos(\omega{t})-y\sin(\omega{t}))\sin(\omega{t})+(x\sin(\omega{t})+y\cos(\omega{t}))\cos(\omega{t})\end{Bmatrix}$

$\textbf{a}(\textbf{x},t)=-\omega^2\begin{Bmatrix}x\underbrace{(\cos^2(\omega{t})+\sin^2(\omega{t}))}_{=1}+y\underbrace{(-\sin(\omega{t})\cos(\omega{t})+\cos(\omega{t})\sin(\omega{t}))}_{=0}\\x\underbrace{(-\cos(\omega{t})\sin(\omega{t})+\sin(\omega{t})\cos(\omega{t}))}_{=0}+y(x\sin(\omega{t})+y\underbrace{(\sin^2(\omega{t})+\cos^2(\omega{t}))}_{=1}\end{Bmatrix}$

$\boxed{\textbf{a}(\textbf{x},t)=\begin{Bmatrix}\text{a}_x\\\text{a}_y\end{Bmatrix}=\begin{Bmatrix}-\omega^2{x}\\-\omega^2{y}\end{Bmatrix}}$

(**OPTION #2**): **Acceleration in spatial description** is obtained by directly calculating the material derivative of the velocity in spatial description:

$\textbf{a}(\textbf{x},t)=\dfrac{d\textbf{v}(\textbf{x},t)}{dt}=\dfrac{\part\textbf{v}(\textbf{x},t)}{\part{t}}+\textbf{v}(\textbf{x},t)\cdot\nabla\textbf{v}(\textbf{x},t)$

$\textbf{a}(\textbf{x},t)=\dfrac{\part}{\part{t}}\begin{Bmatrix}\omega{y}\\-\omega{x}\end{Bmatrix}+\begin{bmatrix}\omega{y}&-\omega{x}\end{bmatrix}\begin{bmatrix}\dfrac{\part}{\part{x}}\\\dfrac{\part}{\part{y}}\end{bmatrix}\begin{bmatrix}\omega{y}&-\omega{x}\end{bmatrix}=$

​	$=\begin{Bmatrix}0\\0\end{Bmatrix}+\begin{bmatrix}\omega{y}&-\omega{x}\end{bmatrix}\begin{bmatrix}\dfrac{\part}{\part{x}}(\omega{y})&\dfrac{\part}{\part{x}}(\omega{x})\\\dfrac{\part}{\part{y}}(\omega{y})&\dfrac{\part}{\part{y}}(\omega{x})\end{bmatrix}=\begin{bmatrix}\omega{y}&-\omega{x}\end{bmatrix}\begin{bmatrix}0&-\omega\\\omega&0\end{bmatrix}=\begin{Bmatrix}-\omega^2x\\-\omega^2y\end{Bmatrix}$

$\boxed{\textbf{a}(\textbf{x},t)=\begin{Bmatrix}-\omega^2{x}\\-\omega^2{y}\end{Bmatrix}}$

# Stationarity and Uniformity

## Stationary properties

* A property is **stationary** when its <u>spatial description</u> is not dependent on time.

  $\varkappa(\textbf{x},t)=\varkappa(\textbf{x})$

  > ==REMARK== in certain fields, the term **steady-state** is more commonly used.

  * the local derivative of a stationary property is zero.

    $\varkappa(\textbf{x},t)=\varkappa(\textbf{x})$	$\iff$	$\dfrac{\part\varkappa(\textbf{x},t)}{\part{t}}=0$

  * the time-independence in the spatial description (stationary) does not imply time-independence in the material description:

    $\varkappa(\textbf{x},t)=\varkappa(\textbf{x})$	$\xcancel{\iff}$	$\bar\varkappa(\textbf{X},t)=\bar\varkappa(\textbf{X})$

    > ==REMARK== this is easily understood if we consider, for example a stationary velocity:
    >
    > $\textbf{v}(\textbf{x},t)=\textbf{v}(\textbf{x})=\textbf{v}(\textbf{x}(\textbf{X},t))=\textbf{V}(\textbf{X},t)$

## Uniform properties

* A property is **uniform** when its <u>spatial description</u> is not dependent on the spatial coordinates.

  $\varkappa(\textbf{x},t)=\varkappa(t)$

  * if its spatial description does not depend on the coordinates (uniform character of the property), neither does its material one.

    $\varkappa(\textbf{x},t)=\varkappa(t)$	$\iff$	$\bar\varkappa(\textbf{X},t)=\bar\varkappa(t)$

# Trajectory (path-line)

## Trajectory or pathline

* A **trajectory** or **pathline** is the locus of the <u>positions occupied by a given particle</u> in space throughout time.

  > ==REMARK== a trajectory can also be defined as the path that a particle follows through space as a function of time

## Equation of the trajectories

* The equation of a given particle's trajectory is obtained <u>particularizing the equation of motion</u> for that particle, which is identified by its material coordinates $\textbf{X}^\ast$.

  $\begin{cases}\textbf{x}(t)=\mathbf{\varphi}(\textbf{X},t)\Bigr|_{\textbf{X}=\textbf{X}^\ast}=\mathbf\phi(T)\\x_i(t)=\varphi_i(\textbf{X},t)\Bigr|_{\textbf{X}=\textbf{X}^\ast}=\phi_i(T)\space\space{i\in\{1,2,3\}}\end{cases}$

* Also, from the velocity field in spatial description, $\textbf{v}(\textbf{x},t)$:

  * a family of curves is obtained from:

    $\dfrac{d\textbf{x}(t)}{dt}=\textbf{v}(\textbf{x}(t),t)$	$\Rightarrow$	$\textbf{x}=\phi(C_1,C_2,C_3,t)$		$[1]$

  * particularizing for a given particle by imposing the consistency condition in the reference configuration:

    $\textbf{x}(t)\Bigr|_{t=0}=\textbf{X}$	$\Rightarrow$	$\textbf{X}=\phi(C_1,C_2,C_3,0)$	$\Rightarrow$	$C_i=\varkappa_i(\textbf{X})$		$[2]$

  * Replace $[2]$ in $[1]$, the equation of the trajectories in canonical form

    $\textbf{x}=\phi(C_1(\textbf{X}),C_2(\textbf{X}),C_3(\textbf{X}),t)=\varphi(\textbf{X},t)$

### Example

Consider the following velocity field:

$\textbf{v}(\textbf{x},t)=\begin{Bmatrix}\omega{y}\\-\omega{x}\end{Bmatrix}$

Obtain the equation of the trajectories.

We integrate the velocity field:

$\dfrac{d\textbf{x}(t)}{dt}=\textbf{v}(\textbf{x},t)$	$\Rightarrow$	$\begin{cases}\dfrac{dx(t)}{dt}=\text{v}(\textbf{x}_x,t)=\omega{y}\\\dfrac{dy(t)}{dt}=\text{v}(\textbf{x}_y,t)=-\omega{x}\end{cases}$

This is a crossed-variable system of differential equations. We derive the 2^nd^ eq. and replace it in the 1^st^ one,

$\dfrac{d^2y(t)}{dt^2}=-\omega\dfrac{dx(t)}{dt}=-\omega^2y$	$\Rightarrow$	$y^{\prime\prime}+\omega^2y=0$

The characteristic equation: $r^2+\omega^2=0$

Has the characteristic solutions: $r_j=\pm{i}\omega$  $j\in\{1,2\}$

And the solution of the problem is:

$y(t)=Real\space{Part}\left\{Z_1e^{iwt}+Z_2e^{iwt}\right\}=C_1\cos(\omega{t})+C_2\sin(\omega{t})$

And, using $\dfrac{dy}{dt}=-\omega{x}$, we obtain

​						$x=-\dfrac{1}{\omega}\dfrac{dy}{dt}=-\dfrac{1}{\omega}(-C_1\sin(\omega{t})+C_2\cos(\omega{t}))$

So, the general solution is:

​						$\begin{cases}x(C_1,C_2,t)=C_1\sin(\omega{t})-C_2\cos(\omega{t})\\y(C_1,C_2,t)=C_1\cos(\omega{t})+C_2\sin(\omega{t})\end{cases}$

The canonical form is obtained from the initial conditions:

$\textbf{x}(C_1,C_2,t)=\textbf{X}$	$\Rightarrow$	$\begin{cases}X=x(C_1,C_2,0)=C_1\overbrace{\sin(\omega\cdot0)}^{=0}-C_2\overbrace{\cos(\omega\cdot0)}^{=1}=C_2\\Y=\space{y}(C_1,C_2,0)=C_1\underbrace{\cos(\omega\cdot0)}_{=1}+C_2\underbrace{\sin(\omega\cdot0)}_{=0}=C_1\end{cases}$

This result in:

$\boxed{\textbf{x}(\textbf{X},t)\rightarrow\begin{cases}x=Y\sin(\omega{t})-X\cos(\omega{t})\\y=Y\cos(\omega{t})+X\sin(\omega{t})\end{cases}}$  

## Streamline

* The **streamlines** are a family of curves which for every instant in time, are the <u>velocity field envelopes</u>

  > ==REMARK== Two streams lines can never cut each other, is it true?

  * Streamlines are defined for any given time instant and change with the velocity field.

    > ==REMARK== The **envelopes** of vector field are the curves whose tangent vector at each point coincides (in direction and sense but not necessarily in magnitude) with the corresponding vector of the vector field.

### Equation of the Streamlines

* The equation of the streamlines is of the type:

  $\dfrac{dx}{\text{v}_x}=\dfrac{dy}{\text{y}_y}=\dfrac{dz}{\text{v}_z}=d\lambda(=ds)$	$\Rightarrow$	$\dfrac{d\textbf{x}}{d\lambda}=\textbf{v}$

* Also, from the velocity field in spatial description, $\textbf{v}(\textbf{x},\text{t}^\ast)$ at a given time instant $\text{t}^\ast$:

  * a family of curves is obtained from:

    $\dfrac{d\textbf{x}(\lambda)}{d\lambda}=\textbf{v}(\textbf{x}(\lambda),t^\ast)$	$\Rightarrow$	$\textbf{x}=\phi(C^\prime_1,C^\prime_2,C^\prime_3,t^\ast)$

  * where each group $(C^\prime_1,C^\prime_2,C^\prime_3)$ identifies a streamline $\textbf{x}(\lambda)$ whose points are obtained assigning values to the parameter $\lambda$.

  * for each time instant $\text{t}^\ast$ a new family of curves is obtained.

## Trajectories and Streamlines

* For a <u>stationary</u> velocity field, the <u>trajectories and the streamlines coincide</u> - PROOF:

  1. If $\textbf{v}(\textbf{x},t)=\textbf{v}(\textbf{x})$:

     * Eq. trajectories:

       $\dfrac{d\textbf{x}(t)}{dt}=\textbf{v}(\textbf{x}(t),t)$  $\Rightarrow$ $\textbf{x}=\phi(C_1,C_2,C_3,t)$

     * Eq. streamlines:

       $\dfrac{d\textbf{x}(\lambda)}{d\lambda}=\textbf{v}(\textbf{x}(\lambda),\cancel{t^\ast})$  $\Rightarrow$ $\textbf{x}=\phi(C^\prime_1,C^\prime_2,C^\prime_3,\cancel{t^\ast})$

       The differential equations only differ in the denomination of the integration parameter ($\text{t}$ or $\lambda$), so the solution to both systems MUST be the same.

### Example

Consider the following velocity field:

$\text{v}_i=\dfrac{x_i}{1+t}$	$i\in\{1,2,3\}$

Obtain the equation of the trajectories and the streamlines associated to this vector field.

Do they coincide? Why?

**Eq. trajectories:**	$\dfrac{d\textbf{x}(t)}{dt}=\textbf{v}(\textbf{x}(t),t)$

introducing the velocity field and rearranging:

$\dfrac{dx_i}{dt}=\dfrac{x_i}{1+t}$	$\Rightarrow$	$\dfrac{dx_i}{x_i}=\dfrac{dt}{1+t}$

integrating both sides of the expression:

$\displaystyle\int\dfrac{1}{x_i}dx_i=\displaystyle\int\dfrac{1}{1+t}dt$	$\Rightarrow$	$\ln{x_i}=\ln(1+t)+\ln{C_i}=\ln{C_i}(1+t)$

The solution:	$\boxed{x_i=C_i(1+t)}$

**Eq. streamlines:**	$\dfrac{d\textbf{x}(\lambda)}{d\lambda}=\textbf{v}(\textbf{x}(\lambda),t^\ast)$

introducing the velocity field and rearranging:

$\dfrac{dx_i}{d\lambda}=\dfrac{x_i}{1+t}$	$\Rightarrow$	$\dfrac{dx_i}{x_i}=\dfrac{d\lambda}{1+t}$

integrating both sides of the expression:

$\displaystyle\int\dfrac{1}{x_i}dx_i=\displaystyle\int\dfrac{1}{1+t}d\lambda$	$\Rightarrow$	$\ln{x_i}=\dfrac{\lambda}{1+t}+K_i$	$\Rightarrow$  $x_i=\displaystyle {e^{\left(\cfrac{\lambda}{1+t}+K_i\right)}}=\underset{=C_1}{\boxed{e^{K_i}}}e^{\left(\cfrac{\lambda}{1+t}\right)}$

The solution:	$\boxed{x_i=C_1e^{\left(\cfrac{\lambda}{1+t}\right)}}$

## Streamtube

* A **streamtube** is a surface composed of streamlines which pass through the points of a closed contour fixed in space.
  * In stationary cases, the tube will remain fixed in space throughout time. In non-stationary cases, it will vary (although the closed contour line is fixed).

# Control and Material Surfaces

## Control Surface

* A **control surface** is a fixed surface in space which does not vary in time.

  ​			$\sum:=\left\{\textbf{x}|f(\text{x},\text{y},\text{z})=0\right\}$

  * Mass (particles) can flow across a control surface.

## Material Surface

* A **material surface** is a mobile surface in the space constituted always by the same particles.

  * In the **reference configuration**, the surface $\sum_0$ will be defined in terms of the material coordinates:

    ​		$\sum_0:=\left\{\textbf{X}|f(\text{X},\text{Y},\text{Z})=0\right\}$

    * The set of particles (material points) belonging the surface are the same at all times

  * In **spatial description** $F(X,Y,Z)=F(X(\textbf{x},t),Y(\textbf{x},t),Z(\textbf{x},t))=f(\textbf{x},t)=f(x,y,z,t)$

    ​		$\sum_t:=\left\{\textbf{x}|f(x,y,z,t)=0\right\}$

    * The set of spatial points belonging to the surface depends on time
    * The material surface **moves in space**

* <u>Necessary and sufficient condition</u> for a mobile surface in space, implicitly defined by the function $f(x,y,z,t)$, to be a material surface is that the **material derivative** of the function **is zero**:

  * *Necessary*: if it is a material surface, its material description does not depend on time:

    ​	$f(\textbf{x},t)\rightarrow{f(\textbf{x}(\textbf{X},t),t)}=F(\textbf{X},\xcancel{t})$	$\Rightarrow$	$0=\dfrac{d}{dt}f(\textbf{x},t)=\dfrac{\part{F}(\textbf{X})}{\part{t}}=0$

  * *Sufficient*: if the material derivative of $\text{f}(\textbf{x},\text{t})$ is null:

    ​	$f(\textbf{x},t)\rightarrow{f(\textbf{x}(\textbf{X},t),t)}=F(\textbf{X},\xcancel{t})$	$\Rightarrow$	$0=\dfrac{d}{dt}f(\textbf{x},t)=\dfrac{\part{F}(\textbf{X})}{\part{t}}\Rightarrow$ $F(\textbf{X},t)\equiv{F(\textbf{X})}$

    The surface $\sum_t:=\left\{\textbf{x}|f(\textbf{x},t)=0\right\}=\left\{\textbf{X}|F(\textbf{X})=0\right\}$

    contains always the same set of the particles (it is a material surface)

## Control Volume

* A **control volume** is a group of fixed points in space situated in the interior of a closed control surface, which does not vary in time.

  ​		$V:=\left\{\textbf{x}|f(\textbf{x})\le0\right\}$

  > ==REMARK== The function $\text{f}(\textbf{x})$ is defined so that $\text{f}(\textbf{x})<0$ corresponds to the points inside $V$.

  * Particles can enter and exit a control volume.

## Material Volume

* A **material volume** is a (mobile) volume enclosed inside a material boundary or surface.

  * In the **reference configuration**, the volume $V_0$ will be defined in terms of the material coordinates:

    $V_0:=\left\{\textbf{X}|f(\textbf{X})\le0\right\}$

    * The particles $\textbf{X}$ in the volume are the same at all times.

  * In **spatial description**, the volume $\text{V}_\text{t}$ will depend on time.

    $V_t:=\left\{\textbf{x}|f(\textbf{x},t)\le0\right\}$

    * The set of spatial points belonging to the volume depends on time
    * The material volume **moves in space along time**















