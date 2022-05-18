* Given a displacement field, the corresponding strain field is found:

  $\textbf{U}(\textbf{X},t)$	$\Rightarrow$	$E_{ij}=\dfrac{1}{2}\left({\dfrac{\part{U}_i}{\part{X}_j}+\dfrac{\part{U}_j}{\part{X}_i}+\dfrac{\part{U}_k}{\part{X}_i}\dfrac{\part{U}_k}{\part{X}_j}}\right)$	$\space\space\space\space{i,j\in\{1,2,3\}}$

  $\textbf{u}(\textbf{x},t)$	$\Rightarrow$	$\varepsilon_{ij}=\dfrac{1}{2}\left({\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}}\right)$	$\space\space\space\space{i,j\in\{1,2,3\}}$

* Is the inverse possible?

  $\boldsymbol{\varepsilon}(\textbf{x},t)$	$\Rightarrow$	$\textbf{u}(\textbf{x},t)$

# Compatibility Conditions

* Given an (arbitrary) symmetric second order tensor field, $\boldsymbol{\varepsilon}(\textbf{x},t)$, a displacement field, $\textbf{u}(\textbf{x},t)$, fulfilling $\nabla^s\textbf{u}(\textbf{x},t)=\boldsymbol{\varepsilon}(\textbf{x},t)$ cannot always be obtained:

  $\varepsilon_{ij}=\dfrac{1}{2}\left({\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}}\right)$	$\space\space\space\space{i,j\in\{1,2,3\}}$	$\begin{matrix}\text{6 PDEs}\\\text{3 unknowns}\end{matrix}$ $\Rightarrow$ $\begin{matrix}\text{OVERDETERMINED}\\\text{SYSTEM}\end{matrix}$

* For $\boldsymbol{\varepsilon}(\textbf{x},t)$ to match a symmetric strain tensor:

  * It must be integrable.

  * There must exist a displacement field from which it comes from.

    ​		   $\Downarrow$

  $\begin{matrix}\text{COMPATIBILITY CONDITIONS}\\\text{must be satisfied}\end{matrix}$

  > ==REMARK== Given $\textbf{u}(\textbf{x},t)$, there will always exist an associated strain tensor, $\boldsymbol{\varepsilon}(\textbf{x},t)$, obtainable through differentiation, which will automatically satisfy the compatibility conditions.

* The **compatibility conditions** are the conditions a symmetric 2^nd^ order tensor must satisfy in order to be a strain tensor and, thus, exist a displacement field which satisfies:

  $\varepsilon_{ij}=\dfrac{1}{2}\left({\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}}\right)$	$\space\space\space\space{i,j\in\{1,2,3\}}$

  * They guarantee the *continuity* of the continuous medium during the deformation process.

# Compatibility Equations of a Potential Field

* A vector field $\textbf{v}(\textbf{x},t)$ will be a **potential vector field** if there exists a scalar function $\phi(\textbf{x},t)$ (named potential function) such that:

  $\begin{cases}\textbf{v}(\textbf{x},t)=\nabla\phi(\textbf{x},t)\\\text{v}_{i}(\textbf{x},t)=\dfrac{\part{\phi(\textbf{x},t)}}{\part{x}_{i}}\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

  * Given a continuous scalar function $\phi(\textbf{x},t)$ there will always exist a potential vector field $\textbf{v}(\textbf{x},t)$.

  * Is the inverse true?

    $\textbf{v}(\textbf{x},t)$ $\Rightarrow$ $\exist\space{\phi(\textbf{x},t)}$ such that $\nabla\phi(\textbf{x},t)=\textbf{v}(\textbf{x},t)$ **?**

### Potential Field

* In component form,

  $\text{v}_i(\textbf{x},t)=\dfrac{\part{\phi(\textbf{x},t)}}{\part{x}_{i}}$ $\Rightarrow$ $\text{v}_i(\textbf{x},t)-\dfrac{\part{\phi(\textbf{x},t)}}{\part{x}_{i}}=0$	$i\in\{1,2,3\}$	$\underset{\Downarrow}{\begin{matrix}\text{3 eqns.}\\\text{1 unknown}\end{matrix}}$

  ​													$\begin{matrix}\text{OVERDETERMINED}\\\text{SYSTEM}\end{matrix}$

* Differentiating once these expressions with respect to $x_i$:

  $\dfrac{\part{\text{v}_i}}{\part{x}_j}=\dfrac{\part^2{\phi(\textbf{x},t)}}{\part{x}_i\part{x}_j}$	${i,j\in\{1,2,3\}}$	$\text{9 eqns.}$

### Compatibility Equations

* Considering the Schwartz Theorem,

  $\dfrac{\part{\text{v}_x}}{\part{x}}=\dfrac{\part^2{\phi}}{\part{x}^2}$	$\dfrac{\part{\text{v}_x}}{\part{y}}=\dfrac{\part^2{\phi}}{\part{x}\part{y}}$	$\dfrac{\part{\text{v}_x}}{\part{z}}=\dfrac{\part^2{\phi}}{\part{x}\part{z}}$

  $\dfrac{\part{\text{v}_y}}{\part{x}}=\dfrac{\part^2{\phi}}{\part{y}\part{x}}$	$\dfrac{\part{\text{v}_y}}{\part{y}}=\dfrac{\part^2{\phi}}{\part^2{y}}$	$\dfrac{\part{\text{v}_y}}{\part{z}}=\dfrac{\part^2{\phi}}{\part{y}\part{z}}$

  $\dfrac{\part{\text{v}_z}}{\part{x}}=\dfrac{\part^2{\phi}}{\part{z}\part{x}}$	$\dfrac{\part{\text{v}_z}}{\part{y}}=\dfrac{\part^2{\phi}}{\part{z}\part{y}}$	$\dfrac{\part{\text{v}_z}}{\part{z}}=\dfrac{\part^2{\phi}}{\part^2{z}}$

  * In this system of 9 equations, only 6 different 2^nd^ derivatives of the unknown $\phi(\textbf{x},t)$ appear:

    $\dfrac{\part^2{\phi}}{\part{x}^2}$, $\dfrac{\part^2{\phi}}{\part^2{y}}$, $\dfrac{\part^2{\phi}}{\part^2{z}}$, $\dfrac{\part^2{\phi}}{\part{x}\part{y}}$, $\dfrac{\part^2{\phi}}{\part{x}\part{y}}$ and $\dfrac{\part^2{\phi}}{\part{y}\part{z}}$

  * They can be eliminated and the following identities are obtained:

    $\dfrac{\part{\text{v}_x}}{\part{y}}=\dfrac{\part{\text{v}_y}}{\part{x}}$	$\dfrac{\part{\text{v}_x}}{\part{z}}=\dfrac{\part{\text{v}_z}}{\part{x}}$	$\dfrac{\part{\text{v}_y}}{\part{z}}=\dfrac{\part{\text{v}_z}}{\part{y}}$
  
* A scalar function $\phi(\textbf{x},t)$ which satisfies $\nabla\phi(\textbf{x},t)=\textbf{v}(\textbf{x},t)$ will exist if the vector field $\textbf{v}(\textbf{x},t)$ verifies:

  $\begin{rcases*}\dfrac{\part{\text{v}_y}}{\part{x}}-\dfrac{\part{\text{v}_x}}{\part{y}}=0\stackrel{def}{=}S_z\\\dfrac{\part{\text{v}_x}}{\part{z}}-\dfrac{\part{\text{v}_z}}{\part{x}}=0\stackrel{def}{=}S_y\\\dfrac{\part{\text{v}_z}}{\part{y}}-\dfrac{\part{\text{v}_y}}{\part{z}}=0=S_z\end{rcases*}$ where $\textbf{S}\equiv\begin{Bmatrix}S_x\\S_y\\S_z\end{Bmatrix}\equiv\begin{vmatrix}\hat{{\textbf{e}}}_1&\hat{{\textbf{e}}}_2&\hat{{\textbf{e}}}_3\\\dfrac{\part{}}{\part{x}}&\dfrac{\part{}}{\part{y}}&\dfrac{\part{}}{\part{z}}\\\text{v}_x&\text{v}_y&\text{v}_z\end{vmatrix}\equiv\nabla\cross\textbf{v}$

  ​							$\Downarrow$

  $\begin{matrix}\textbf{INTEGRABILITY}\\\textbf{(COMPATIBILITY)}\\\textbf{EQUATIONS}\\\text{of a potential}\\\text{vector field}\end{matrix}$ $\boxed{\begin{cases}\nabla\cross\textbf{v}=\textbf{0}\\\dfrac{\part{\text{v}_i}}{\part{x}_j}-\dfrac{\part{\text{v}_j}}{\part{x}_i}=0\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

  > ==REMARK== A functional relation can be established between these three equations.
  >
  > ​							$\nabla\cdot(\nabla\cross\textbf{v})=0$

#### Schwartz Theorem

* The **Schwartz Theorem** about **symmetry of second partial derivatives** guarantees that, given a continuous function $\Phi(x_1,x_2,\dots,x_n)$ with continuous derivatives, the following holds true:

  $\dfrac{\part^2{\Phi}}{\part{x}_i\part{x}_j}=\dfrac{\part^2{\Phi}}{\part{x}_j\part{x}_i}$	$\forall\space{i,j}$


# Compatibility Conditions for Infinitesimal Strain

* The infinitesimal strain field can be written as:

  $[\boldsymbol{\varepsilon}]=$$\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{xy}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{xz}&\varepsilon_{zy}&\varepsilon_{zz}\end{bmatrix}=$$\begin{bmatrix}\dfrac{\part{u_x}}{\part{x}}&\dfrac{1}{2}\left(\dfrac{\part{u_x}}{\part{y}}+\dfrac{\part{u_y}}{\part{x}}\right)&\dfrac{1}{2}\left(\dfrac{\part{u_x}}{\part{z}}+\dfrac{\part{u_z}}{\part{x}}\right)\\\cross&\dfrac{\part{u_y}}{\part{y}}&\dfrac{1}{2}\left(\dfrac{\part{u_y}}{\part{z}}+\dfrac{\part{u_z}}{\part{y}}\right)\\symmetrical&\cross&\dfrac{\part{u_z}}{\part{z}}\end{bmatrix}$

  ​							$\begin{matrix}\text{6 PDEs}\\\text{3 unknowns}\end{matrix}$

* The infinitesimal strain field can be written as:

  $\begin{cases}\varepsilon_{xx}-\dfrac{\part{u_x}}{\part{x}}=0\\\varepsilon_{yy}-\dfrac{\part{u_y}}{\part{y}}=0\\\varepsilon_{zz}-\dfrac{\part{u_z}}{\part{z}}=0\end{cases}$	$\begin{cases}\varepsilon_{xy}-\dfrac{1}{2}\left(\dfrac{\part{u_x}}{\part{y}}+\dfrac{\part{u_y}}{\part{x}}\right)=0\\\varepsilon_{xz}-\dfrac{1}{2}\left(\dfrac{\part{u_x}}{\part{z}}+\dfrac{\part{u_z}}{\part{x}}\right)=0\\\varepsilon_{yz}-\dfrac{1}{2}\left(\dfrac{\part{u_y}}{\part{z}}+\dfrac{\part{u_z}}{\part{y}}\right)=0\end{cases}$

  $\begin{matrix}\text{6 PDEs}\\\text{3 unknowns}\end{matrix}$	$\Rightarrow$	$\begin{matrix}\text{The system will have a solution only if certain}\\\textbf{compatibility conditions}\text{ are satisfied.}\end{matrix}$

## Compatibility Conditions

* The compatibility conditions for the infinitesimal strain field are obtained through **double differentiation** (single differentiation is not enough).

  $\left.\begin{matrix}\dfrac{\part^2\left(\varepsilon_{xx}-\dfrac{\part{u_x}}{\part{x}}\right)}{\part{x}^2,\part{y}^2,\part{z}^2,\part{xy},\part{xz},\part{yz}}=&\begin{matrix}\text{6}\\\text{equations}\end{matrix}\\\vdots&\vdots\\\vdots&\vdots\\\dfrac{\part^2\left(\varepsilon_{yz}-\dfrac{1}{2}\left(\dfrac{\part{u_y}}{\part{z}}+\dfrac{\part{u_z}}{\part{y}}\right)\right)}{\part{x}^2,\part{y}^2,\part{z}^2,\part{xy},\part{xz},\part{yz}}=&\begin{matrix}\text{6}\\\text{equations}\end{matrix}\end{matrix}\right\}$  $\Rightarrow$  $\begin{matrix}\text{6}\cross\text{6=36}\\\text{equations}\end{matrix}$

* The compatibility conditions for the infinitesimal strain field are obtained through:

  $\begin{matrix}\text{18 equations for}\\\varepsilon_{xx},\varepsilon_{yy},\varepsilon_{zz}\end{matrix}$	$\begin{matrix}\dfrac{\part^2\varepsilon_{xx}}{\part{x^2}}=\dfrac{\part^3u_x}{\part{x^3}}&&\dfrac{\part^2\varepsilon_{yz}}{\part{x^2}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}\part{x}^2}+\dfrac{\part^3u_z}{\part{y}\part{x}^2}\right)\\\dfrac{\part^2\varepsilon_{xx}}{\part{y^2}}=\dfrac{\part^3u_x}{\part{x}\part{y}^2}&&\dfrac{\part^2\varepsilon_{yz}}{\part{y^2}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}\part{y}^2}+\dfrac{\part^3u_z}{\part{y}^3}\right)\\\dfrac{\part^2\varepsilon_{xx}}{\part{z^2}}=\dfrac{\part^3u_x}{\part{x}\part{z}^2}&\dots&\dfrac{\part^2\varepsilon_{yz}}{\part{z^2}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}^3}+\dfrac{\part^3u_z}{\part{y}\part{z}^2}\right)\\\dfrac{\part^2\varepsilon_{xx}}{\part{x}\part{y}}=\dfrac{\part^3u_x}{\part{x}^2\part{y}}&&\dfrac{\part^2\varepsilon_{yz}}{\part{x}\part{y}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}\part{x}\part{y}}+\dfrac{\part^3u_z}{\part{y}^2\part{x}}\right)\\\dfrac{\part^2\varepsilon_{xx}}{\part{x}\part{z}}=\dfrac{\part^3u_x}{\part{x}^2\part{z}}&&\dfrac{\part^2\varepsilon_{yz}}{\part{x}\part{z}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}^2\part{x}}+\dfrac{\part^3u_z}{\part{y}\part{x}\part{z}}\right)\\\dfrac{\part^2\varepsilon_{xx}}{\part{y}\part{z}}=\dfrac{\part^3u_x}{\part{x}\part{y}\part{z}}&&\dfrac{\part^2\varepsilon_{yz}}{\part{y}\part{z}}=\dfrac{1}{2}\left(\dfrac{\part^3u_y}{\part{z}^2\part{y}}+\dfrac{\part^3u_z}{\part{y}^2\part{z}}\right)\end{matrix}$	$\begin{matrix}\text{18 equations for}\\\varepsilon_{xy},\varepsilon_{xz},\varepsilon_{yz}\end{matrix}$

* **All the third derivatives** of $u_x$, $u_y$ and $u_z$ appear in the equations:

  $\dfrac{\part^3u_x}{\part{x}^3,\part{x}^2{y},\part{x}^2{z},\part{y}^3,\part{y}^2{x},\part{y}^2{z},\part{z}^3,\part{z}^2{x},\part{z}^2{y},\part{x}{y}{z}}=$ $\text{10 derivatives}$

  $\dfrac{\part^3u_y}{\part{x}^3,\part{x}^2{y},\part{x}^2{z},\part{y}^3,\part{y}^2{x},\part{y}^2{z},\part{z}^3,\part{z}^2{x},\part{z}^2{y},\part{x}{y}{z}}=$ $\text{10 derivatives}$

  $\dfrac{\part^3u_z}{\part{x}^3,\part{x}^2{y},\part{x}^2{z},\part{y}^3,\part{y}^2{x},\part{y}^2{z},\part{z}^3,\part{z}^2{x},\part{z}^2{y},\part{x}{y}{z}}=$ $\text{10 derivatives}$

  which constitute 30 of the unknowns in the system of 36 equations:

  $f_n\left(\dfrac{\part{u_i}}{\part{x}_j\part{x}_k\part{x}_l},\dfrac{\part{\varepsilon_{ij}}}{\part{x}_k\part{x}_l}\right)=0$	$n\in\left\{1,2,\dots,36\right\}$

  ​	$^{\underbrace{\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space\space}_{\huge\text{30}}}$

* Eliminating the 30 unknowns, $\dfrac{\part{u_i}}{\part{x}_j\part{x}_k\part{x}_l}$, 6 equations (involving only strain derivatives) are obtained:

  $\boxed{\begin{cases}S_{xx}\stackrel{def}{=}\dfrac{\part^2\varepsilon_{yy}}{\part{z}^2}+\dfrac{\part^2\varepsilon_{zz}}{\part{y}^2}-2\dfrac{\part^2\varepsilon_{yz}}{\part{y}\part{z}}=0\\S_{yy}\stackrel{def}{=}\dfrac{\part^2\varepsilon_{zz}}{\part{x}^2}+\dfrac{\part^2\varepsilon_{xx}}{\part{z}^2}-2\dfrac{\part^2\varepsilon_{xz}}{\part{x}\part{z}}=0\\S_{zz}\stackrel{def}{=}\dfrac{\part^2\varepsilon_{xx}}{\part{y}^2}+\dfrac{\part^2\varepsilon_{yy}}{\part{x}^2}-2\dfrac{\part^2\varepsilon_{xy}}{\part{x}\part{y}}=0\\S_{xy}\stackrel{def}{=}-\dfrac{\part^2\varepsilon_{zz}}{\part{x}\part{y}}+\dfrac{\part}{\part{z}}\left(\dfrac{\part\varepsilon_{yz}}{\part{x}}+\dfrac{\part\varepsilon_{xz}}{\part{y}}-\dfrac{\part\varepsilon_{xy}}{\part{z}}\right)=0\\S_{xz}\stackrel{def}{=}-\dfrac{\part^2\varepsilon_{yy}}{\part{x}\part{z}}+\dfrac{\part}{\part{y}}\left(\dfrac{\part\varepsilon_{yz}}{\part{x}}-\dfrac{\part\varepsilon_{xz}}{\part{y}}+\dfrac{\part\varepsilon_{xy}}{\part{z}}\right)=0\\S_{yz}\stackrel{def}{=}-\dfrac{\part^2\varepsilon_{xx}}{\part{y}\part{z}}+\dfrac{\part}{\part{x}}\left(-\dfrac{\part\varepsilon_{yz}}{\part{x}}+\dfrac{\part\varepsilon_{xz}}{\part{y}}+\dfrac{\part\varepsilon_{xy}}{\part{z}}\right)=0\end{cases}}$  $\Rightarrow$  $\boxed{\mathbf{S}=\nabla\cross\left(\boldsymbol{\varepsilon}\cross\nabla\right)}$  $\begin{matrix}\textbf{COMPATIBILITY}\\\textbf{EQUATIONS}\\\text{for the infinitesimal}\\\text{strain tensor}\end{matrix}$

* The six equations are not functionally independent. They satisfy the equation,

  ​			$\nabla\cdot\mathbf{S}=\nabla\cdot\left(\nabla\cross\left(\boldsymbol{\varepsilon}\cross\nabla\right)\right)=\textbf{0}$

  * In indicial notation:

    $\begin{cases}\dfrac{\part{S_{xx}}}{\part{x}}+\dfrac{\part{S_{xy}}}{\part{y}}+\dfrac{\part{S_{xz}}}{\part{z}}=0\\\dfrac{\part{S_{xy}}}{\part{x}}+\dfrac{\part{S_{yy}}}{\part{y}}+\dfrac{\part{S_{yz}}}{\part{z}}=0\\\dfrac{\part{S_{xz}}}{\part{x}}+\dfrac{\part{S_{yz}}}{\part{y}}+\dfrac{\part{S_{zz}}}{\part{z}}=0\end{cases}$

* The compatibility equations can be expressed in terms of the permutation operator, $e_{ijk}$.

  $S_{ml}=e_{mjq}e_{lir}\varepsilon_{ij,qr}=0$	$m,l\in\{1,2,3\}$

* Or, alternatively:

  $\varepsilon_{ij,kl}+\varepsilon_{kl,ij}-\varepsilon_{ik,jl}-\varepsilon_{jl,ik}=0$	$i,j,k,l\in\{1,2,3\}$

  > ==NOTE== $\varepsilon_{ij,kl}=$$\dfrac{\part^2\varepsilon_{ij}}{\part{k}\part{l}}$	$i,j,k,l\in\{1,2,3\}$

  > ==REMARK== Any linear strain tensor (1^st^ order polynomial) with respect to the spatial variables will be compatible and, thus, integrable.

# Integration of the Infinitesimal Strain Tensor

## Preliminary Equations

* Rotation tensor $\boldsymbol{\Omega}(\textbf{x},t)$:

  $\begin{cases}\boldsymbol{\Omega}=\textit{skew}\left(\textbf{u}\otimes\nabla\right)=\dfrac{1}{2}\left(\textbf{u}\otimes\nabla-\nabla\otimes\textbf{u}\right)\\\Omega_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right)\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

* Rotation vector $\boldsymbol{\theta}(\textbf{x},t)$:

  $\boldsymbol{\theta}=\dfrac{1}{2}\nabla\cross\textbf{u}=$$\begin{bmatrix}\theta_1\\\theta_2\\\theta_3\end{bmatrix}=$$\begin{bmatrix}-\Omega_{23}\\-\Omega_{31}\\-\Omega_{12}\end{bmatrix}=$$\begin{bmatrix}-\Omega_{yz}\\-\Omega_{zx}\\-\Omega_{xy}\end{bmatrix}$	$\Rightarrow$	$\begin{bmatrix}\Omega(\theta)\end{bmatrix}=$$\begin{bmatrix}0&-\theta_3&\theta_2\\\theta_3&0&-\theta_1\\-\theta_2&\theta_1&0\end{bmatrix}$

* Differentiating $\boldsymbol{\Omega}(\textbf{x},t)$ with respect to $\mathcal{X}_k$:

  $\Omega_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right)$	$\Rightarrow$	$\dfrac{\part\Omega_{ij}}{\part{x}_k}=\dfrac{1}{2}\dfrac{\part}{\part{x}}\left[\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right]$

* Adding and subtracting the term $\dfrac{1}{2}\dfrac{\part^2u_k}{\part{x}_i\part{x}_j}$:

  $\begin{split}\dfrac{\part\Omega_{ij}}{\part{x}_k}&=\dfrac{1}{2}\dfrac{\part}{\part{x}_k}\left[\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right]+\dfrac{1}{2}\dfrac{\part^2u_k}{\part{x}_i\part{x}_j}-\dfrac{1}{2}\dfrac{\part^2u_k}{\part{x}_i\part{x}_j}=\\&=\dfrac{\part}{\part{x}_j}\underset{\Large{=\varepsilon_{ik}}}{\boxed{\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_k}+\dfrac{\part{u}_k}{\part{x}_i}\right)}}-\dfrac{\part}{\part{x}_i}\underset{\Large{=\varepsilon_{jk}}}{\boxed{\dfrac{1}{2}\left(\dfrac{\part{u}_j}{\part{x}_k}+\dfrac{\part{u}_k}{\part{x}_j}\right)}}=\dfrac{\part\varepsilon_{ik}}{\part{x}_j}-\dfrac{\part\varepsilon_{jk}}{\part{x}_i}\end{split}$

* Using the previous results, the derivative of $\boldsymbol{\theta}(\textbf{x},t)$ is obtained:

  $\nabla\theta_1\Rightarrow$$\begin{cases}\dfrac{\part\theta_1}{\part{x}}=-\dfrac{\part\Omega_{yz}}{\part{x}}=\dfrac{\part\varepsilon_{xz}}{\part{y}}-\dfrac{\part\varepsilon_{xy}}{\part{z}}\\\dfrac{\part\theta_1}{\part{y}}=-\dfrac{\part\Omega_{yz}}{\part{y}}=\dfrac{\part\varepsilon_{yz}}{\part{y}}-\dfrac{\part\varepsilon_{yy}}{\part{z}}\\\dfrac{\part\theta_1}{\part{z}}=-\dfrac{\part\Omega_{yz}}{\part{z}}=\dfrac{\part\varepsilon_{zz}}{\part{y}}-\dfrac{\part\varepsilon_{zy}}{\part{z}}\end{cases}$

  $\nabla\theta_2\Rightarrow$$\begin{cases}\dfrac{\part\theta_2}{\part{x}}=-\dfrac{\part\Omega_{zx}}{\part{x}}=\dfrac{\part\varepsilon_{xx}}{\part{z}}-\dfrac{\part\varepsilon_{xz}}{\part{x}}\\\dfrac{\part\theta_2}{\part{y}}=-\dfrac{\part\Omega_{zx}}{\part{y}}=\dfrac{\part\varepsilon_{xy}}{\part{z}}-\dfrac{\part\varepsilon_{yz}}{\part{x}}\\\dfrac{\part\theta_2}{\part{z}}=-\dfrac{\part\Omega_{zx}}{\part{z}}=\dfrac{\part\varepsilon_{xz}}{\part{z}}-\dfrac{\part\varepsilon_{zz}}{\part{y}}\end{cases}$

  $\nabla\theta_3\Rightarrow$$\begin{cases}\dfrac{\part\theta_3}{\part{x}}=-\dfrac{\part\Omega_{xy}}{\part{x}}=\dfrac{\part\varepsilon_{xy}}{\part{x}}-\dfrac{\part\varepsilon_{xx}}{\part{y}}\\\dfrac{\part\theta_3}{\part{y}}=-\dfrac{\part\Omega_{xy}}{\part{y}}=\dfrac{\part\varepsilon_{yy}}{\part{x}}-\dfrac{\part\varepsilon_{xy}}{\part{y}}\\\dfrac{\part\theta_3}{\part{z}}=-\dfrac{\part\Omega_{xy}}{\part{z}}=\dfrac{\part\varepsilon_{yz}}{\part{x}}-\dfrac{\part\varepsilon_{xz}}{\part{y}}\end{cases}$

* Considering the displacement gradient tensor $\textbf{J}(\textbf{x},t)$,

  $\begin{cases}\textbf{J}=\dfrac{\part\textbf{u}(\textbf{x},t)}{\part\textbf{x}}=\boldsymbol{\varepsilon}+\boldsymbol\Omega\\J_{ij}=\dfrac{du_i}{dx_{j}}=\underset{\huge=\varepsilon_{ij}}{\boxed{\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}\right)}}+\underset{\huge=\Omega_{ij}}{\boxed{\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right)}}=\varepsilon_{ij}+\Omega_{ij}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

* Introducing the definition of $\boldsymbol{\theta}(\textbf{x},t)$, the components of $\textbf{J}(\textbf{x},t)$ are rewritten:

  $\begin{bmatrix}\theta_1\\\theta_2\\\theta_3\end{bmatrix}=$$\begin{bmatrix}-\Omega_{23}\\-\Omega_{31}\\-\Omega_{12}\end{bmatrix}=$$\begin{bmatrix}-\Omega_{yz}\\-\Omega_{zx}\\-\Omega_{xy}\end{bmatrix}$
  
  |        | $j=1$                                                      | $j=2$                                                      | $j=3$                                                      |
  | ------ | ---------------------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
  | $i=1:$ | $\dfrac{\part{u_x}}{\part{x}}=$$\varepsilon_{xx}$          | $\dfrac{\part{u_x}}{\part{y}}=$$\varepsilon_{xy}-\theta_3$ | $\dfrac{\part{u_x}}{\part{z}}=$$\varepsilon_{xz}+\theta_2$ |
  | $i=2:$ | $\dfrac{\part{u_y}}{\part{x}}=$$\varepsilon_{xy}+\theta_3$ | $\dfrac{\part{u_y}}{\part{y}}=$$\varepsilon_{yy}$          | $\dfrac{\part{u_y}}{\part{z}}=$$\varepsilon_{yz}-\theta_1$ |
  | $i=3:$ | $\dfrac{\part{u_z}}{\part{x}}=$$\varepsilon_{xz}-\theta_2$ | $\dfrac{\part{u_z}}{\part{y}}=$$\varepsilon_{yz}+\theta_1$ | $\dfrac{\part{u_z}}{\part{z}}=$$\varepsilon_{zz}$          |
  
* The integration of the strain field $\boldsymbol{\varepsilon}(\textbf{x},t)$ is performed in two steps:

  1. Integration of derivative of $\boldsymbol{\theta}(\textbf{x},t)$ using the 1^st^ order PDE system derived for $\nabla\theta_1$, $\nabla\theta_2$ and $\nabla\theta_3$. The solution will be of the type:

     $\boxed{\theta_i=\tilde\theta_i(x,y,z,t)+c_i(t)\space\space\space\space{i\in\{1,2,3\}}}$

     The integration constants $c_i(t)$ can be obtained knowing the value of the rotation vector in some points of the medium (boundary conditions).

  2. Known $\boldsymbol{\varepsilon}(\textbf{x},t)$ and $\boldsymbol{\theta}(\textbf{x},t)$, $\textbf{u}$ is integrated using the 1^st^ order PDE system derived for $\textbf{u}\otimes\nabla$. The solution will be:

     $\boxed{u_i=\tilde{u}_i(x,y,z,t)+c^\prime_i(t)\space\space\space\space{i\in\{1,2,3\}}}$

     The integration constants $c^\prime_i(t)$ can be obtained knowing the value of the displacements in some point of space (boundary conditions)

  > ==REMARK== If the compatibility equations are satisfied, these equations will be integrable.

* The integration constants that appear imply that an integrable strain tensor $\boldsymbol{\varepsilon}(\textbf{x},t)$ will determine the movement in any instant of time except for a rotation $\textbf{c}(t)\stackrel{not.}{=}\hat{\boldsymbol{\uptheta}}(t)$ and a translation $\textbf{c}^\prime(t)\stackrel{not.}{=}\hat{\textbf{u}}(t)$:

  $\boldsymbol{\varepsilon}(\textbf{x},t)$	$\Rightarrow$	$\begin{cases}\boldsymbol{\uptheta}(\textbf{x},t)=\tilde{\boldsymbol{\uptheta}}(\textbf{x},t)+\hat{\boldsymbol{\uptheta}}(\textbf{x},t)\\\textbf{u}(\textbf{x},t)=\tilde{\textbf{u}}(\textbf{x},t)+\hat{\textbf{u}}(\textbf{x},t)\end{cases}$

* A displacement field can be constructed from this uniform rotation and translation:

  $\textbf{u}^\ast(\textbf{x},t)=\hat{\boldsymbol{\Omega}}(\hat{\theta}(t))\cdot\textbf{x}+\hat{\textbf{u}}(t)$

  ​		$\Rightarrow$	$\begin{cases}\textbf{u}^\ast\otimes\nabla=\hat{\Omega}\\\nabla^s(\textbf{u}^\ast)=\dfrac{1}{2}\left(\textbf{u}^\ast\otimes\nabla+(\textbf{u}^\ast\otimes\nabla)^T\right)=\dfrac{1}{2}\left(\hat{\Omega}+\hat{\Omega}^T\right)=\textbf{0}\end{cases}$

* This corresponds to a **rigid solid movement**.

# Compatibility Equations in a Deformation Rate Field

* There is a correspondence between

  $\boxed{\begin{matrix}\textbf{u}\\\boldsymbol{\varepsilon}(\textbf{u})\\\varepsilon_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}\right)\\\Omega_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}\right)\\\boldsymbol{\uptheta}=\dfrac{1}{2}\nabla\cross\textbf{u}\end{matrix}}$	$\iff$	$\boxed{\begin{matrix}\textbf{v}\\\textbf{d}(\textbf{v})\\d_{ij}=\dfrac{1}{2}\left(\dfrac{\part{\text{v}}_i}{\part{x}_j}+\dfrac{\part{\text{v}}_j}{\part{x}_i}\right)\\\text{w}_{ij}=\dfrac{1}{2}\left(\dfrac{\part{\text{v}}_i}{\part{x}_j}-\dfrac{\part{\text{v}}_j}{\part{x}_i}\right)\\\boldsymbol{\upomega}=\dfrac{1}{2}\nabla\cross\textbf{v}\end{matrix}}$

* The concept of compatibility conditions can be extended to deformation rate tensor $\textbf{d(v)}$.

### Example

Obtain the velocity field corresponding to the deformation rate tensor:

​			$\left[\textbf{d}(\textbf{x},t)\right]=$$\begin{bmatrix}0&te^{ty}&0\\te^{ty}&0&0\\0&0&te^{tz}\end{bmatrix}$

such that in point $(1,1,1)$ the following conditions is fulfilled:

$\left.\textbf{v}(\textbf{x},t)\right|_{x=(1,1,1)}=$$\begin{Bmatrix}2e^t\\e^t\\e^t\end{Bmatrix}$	$\left.\boldsymbol{\upomega}(\textbf{x},t)\right|_{x=(1,1,1)}=$$\dfrac{1}{2}\nabla\cross\textbf{v}=$$\begin{Bmatrix}0\\0\\-te^t\end{Bmatrix}$

Consider the correspondence: $\boxed{\begin{matrix}\textbf{u}\\\boldsymbol{\varepsilon}(\textbf{u})\\\boldsymbol{\uptheta}=\dfrac{1}{2}\nabla\cross\textbf{u}\end{matrix}}$	$\iff$	$\boxed{\begin{matrix}\textbf{v}\\\textbf{d}(\textbf{v})\\\boldsymbol{\upomega}=\dfrac{1}{2}\nabla\cross\textbf{v}\end{matrix}}$

Take the expressions derived for $\nabla\theta_1$, $\nabla\theta_2$ and $\nabla\theta_3$ substitute $\boldsymbol{\uptheta}(\textbf{x},t)$ with $\boldsymbol{\upomega}(\textbf{x},t)$ and $\boldsymbol{\upvarepsilon}(\textbf{x},t)$ with $\textbf{d}(\textbf{x},t)$:

$\nabla\upomega_1\Rightarrow$$\begin{cases}\dfrac{\part{\upomega_1}}{\part{x}}=\dfrac{\part{d_{xz}}}{\part{y}}-\dfrac{\part{d_{xy}}}{\part{z}}=0-0\\\dfrac{\part{\upomega_1}}{\part{y}}=\dfrac{\part{d_{yz}}}{\part{y}}-\dfrac{\part{d_{yy}}}{\part{z}}=0-0\\\dfrac{\part{\upomega_1}}{\part{z}}=\dfrac{\part{d_{zz}}}{\part{y}}-\dfrac{\part{d_{zy}}}{\part{z}}=0-0\end{cases}$		$\Rightarrow$	$\upomega_1(t)=C_1(t)$

$\nabla\upomega_2\Rightarrow$$\begin{cases}\dfrac{\part{\upomega_2}}{\part{x}}=\dfrac{\part{d_{zz}}}{\part{z}}-\dfrac{\part{d_{xz}}}{\part{x}}=0-0\\\dfrac{\part{\upomega_2}}{\part{y}}=\dfrac{\part{d_{zy}}}{\part{z}}-\dfrac{\part{d_{yz}}}{\part{x}}=0-0\\\dfrac{\part{\upomega_2}}{\part{z}}=\dfrac{\part{d_{xz}}}{\part{z}}-\dfrac{\part{d_{zz}}}{\part{x}}=0-0\end{cases}$		$\Rightarrow$	$\upomega_2(t)=C_2(t)$

$\nabla\upomega_2\Rightarrow$$\begin{cases}\dfrac{\part{\upomega_3}}{\part{x}}=\dfrac{\part{d_{xy}}}{\part{x}}-\dfrac{\part{d_{xx}}}{\part{y}}=0-0\\\dfrac{\part{\upomega_3}}{\part{x}}=\dfrac{\part{d_{yy}}}{\part{x}}-\dfrac{\part{d_{xy}}}{\part{y}}=0-t^2e^{ty}\\\dfrac{\part{\upomega_3}}{\part{z}}=\dfrac{\part{d_{yz}}}{\part{x}}-\dfrac{\part{d_{xz}}}{\part{y}}=0-0\end{cases}$	 $\Rightarrow$	$\upomega_3(y,t)=\displaystyle\int_{}^{}{-t^2e^{ty}dy}=-te^{ty}+C_3(t)$

For point $(1,1,1)$:

​	$\left\{\boldsymbol{\upomega}(\textbf{x},t)\right\}=$$\dfrac{1}{2}\nabla\cross\textbf{v}=$$\begin{Bmatrix}0\\0\\-te^t\end{Bmatrix}$

So,

$\begin{rcases*}\upomega_1=0=C_1(t)\\\upomega_2=0=C_2(t)\\\upomega_3=-te^t=\left[-te^t+C_3(t)\right]_{\textbf{x}=(1,1,1)}\end{rcases*}$	$\Rightarrow$	$\begin{matrix}C_1(t)=0\\C_2(t)=0\\C_3(t)=0\end{matrix}$

Therefore, for any point,

​					$\boxed{\left\{\boldsymbol{\upomega}(\textbf{x},t)\right\}=\begin{Bmatrix}0\\0\\-te^t\end{Bmatrix}}$

Taking the expressions

|        | $j=1$                                                   | $j=2$                                                   | $j=3$                                                   |
| ------ | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| $i=1:$ | $\dfrac{\part\text{v}_x}{\part{x}}=$$d_{xx}$            | $\dfrac{\part\text{v}_x}{\part{y}}=$$d_{xy}-\upomega_3$ | $\dfrac{\part\text{v}_x}{\part{z}}=$$d_{xz}+\upomega_2$ |
| $i=2:$ | $\dfrac{\part\text{v}_y}{\part{x}}=$$d_{xy}+\upomega_3$ | $\dfrac{\part\text{v}_y}{\part{y}}=$$d_{yy}$            | $\dfrac{\part\text{v}_y}{\part{z}}=$$d_{yz}-\upomega_1$ |
| $i=3:$ | $\dfrac{\part\text{v}_z}{\part{x}}=$$d_{xz}-\upomega_2$ | $\dfrac{\part\text{v}_z}{\part{y}}=$$d_{yz}+\upomega_1$ | $\dfrac{\part\text{v}_z}{\part{z}}=$$d_{zz}$            |

The components of the velocities can be obtained:

$\begin{rcases*}\dfrac{\part\text{v}_x}{\part{x}}=d_{xx}=0\\\dfrac{\part\text{v}_x}{\part{y}}=d_{xy}-\upomega_3=te^{ty}-(-te^{ty})=2te^{ty}\\\dfrac{\part\text{v}_x}{\part{z}}=d_{xz}+\upomega_2=0+0\end{rcases*}$	$\Rightarrow$	$\text{v}_x(y,t)=$$\displaystyle\int_{}^{}{2te^{ty}}dy=$$2e^{ty}+C^\prime_1(t)$

   $\begin{rcases*}\dfrac{\part\text{v}_y}{\part{x}}=d_{xy}+\upomega_3=te^{ty}+(-te^{ty})=0\\\dfrac{\part\text{v}_y}{\part{y}}=d_{yy}=0\\\dfrac{\part\text{v}_y}{\part{z}}=d_{yz}-\upomega_1=0-0\end{rcases*}$	$\Rightarrow$	$\text{v}_y(t)=$$C^\prime_2(t)$

​			  $\begin{rcases*}\dfrac{\part\text{v}_z}{\part{x}}=d_{xz}-\upomega_2=0-0\\\dfrac{\part\text{v}_z}{\part{y}}=d_{yz}+\upomega_1=0+0\\\dfrac{\part\text{v}_z}{\part{z}}=d_{zz}=te^{tz}\end{rcases*}$	$\Rightarrow$	$\text{v}_z(z,t)=$$\displaystyle\int_{}^{}{te^{tz}}dz=$$e^{tz}+C^\prime_3(t)$

For point $(1,1,1)$:

$\left\{\textbf{v}(\textbf{x},t)\right\}=$$\begin{Bmatrix}2e^t\\e^t\\e^t\end{Bmatrix}$

So,

$\begin{rcases*}\text{v}_x=2e^t=\left[2e^{ty}+C^\prime_1(t)\right]_{\textbf{x}=(1,1,1)}\\\text{v}_y=e^t=C^\prime_2(t)\\\text{v}_z=e^t=\left[e^{tz}+C^\prime_3(t)\right]_{\textbf{x}=(1,1,1)}\end{rcases*}$	$\Rightarrow$	$\begin{matrix}C^\prime_1(t)=0\\C^\prime_2(t)=e^t\\C^\prime_3(t)=0\end{matrix}$

Therefore, for any point,

​					$\boxed{\left\{\textbf{v}(\textbf{x},t)\right\}=\begin{Bmatrix}2e^{ty}\\e^t\\e^{tz}\end{Bmatrix}}$


