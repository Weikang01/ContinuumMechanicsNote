* **Deformation**: transformation of a body from a reference configuration to a current configuration.
  * Focus on the **relative movement** of a given particle w.r.t the particles in its neighborhood (at differential level).
  * It includes **changes of size and shape.**

# Deformation Gradient Tensor

## Continuous Medium in Movement

* 
  * $\Omega_0$: non-deformed (or reference) configuration, at reference time $t_0$.
  * $X$: Position vector of a particle at reference time.
* 
  * $\Omega$ or $\Omega_t$: deformed (or present) configuration, at present time $t$.
  * $x$: Position vector of a particle at present time.

## Fundamental Equation of Deformation

* The Equations of Motion:

  $\begin{cases}x_i=\varphi_i(X_1,X_2,X_3,t)\stackrel{not.}{=}x_i(X_1,X_2,X_3,t)\space\space\space\space{i\in\{1,2,3\}}\\\textbf{x}=\mathbf{\varphi}(\textbf{X},t)\stackrel{not.}{=}\textbf{x}(\textbf{X},t)\end{cases}$

* Differentiating w.r.t $\textbf{X}$:

  $\boxed{\begin{cases}dx_i=\dfrac{\part{x_i(\textbf{X},t)}}{\part{X_j}}dX_j\stackrel{not.}{=}F_{ij}(\textbf{X},t)dX_j\space\space\space\space{i\in\{1,2,3\}}\\d\textbf{x}=\dfrac{\part{\textbf{x}(\textbf{X},t)}}{\part{\textbf{X}}}dX_j\stackrel{not.}{=}\textbf{F}(\textbf{X},t)\cdot{d\textbf{X}}\end{cases}}$ Fundamental equation of deformation

  where $\textbf{F}(\textbf{X},t)$ is the (material) deformation gradient tensor

## Material Deformation Gradient Tensor

* The (material) deformation gradient tensor:

  $\begin{cases}\textbf{F}(\textbf{X},t)\stackrel{not.}{=}\textbf{x}(\textbf{X},t)\otimes\overline{\nabla}\\F_{ij}=\dfrac{\part{x_i}}{\part{X_j}}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

  > ==REMARK== The material Nabla operator is defined as: $\overline{\nabla}=\dfrac{\part{}}{\part{X_i}}\hat{{\textbf{e}}}_i$
  >
  > $[\overline{\nabla}]=\begin{bmatrix}\dfrac{\partial}{X_1}\\\dfrac{\partial}{X_2}\\\dfrac{\partial}{X_3}\end{bmatrix}$

  $[\textbf{F}]=[\textbf{x}\otimes\overline{\nabla}]=\overbrace{\begin{bmatrix}\text{x}_1\\\text{x}_2\\\text{x}_3\end{bmatrix}}^{=[\textbf{x}]}\overbrace{\begin{bmatrix}\dfrac{\partial}{\partial{X_1}}&\dfrac{\partial}{\partial{X_2}}&\dfrac{\partial}{\partial{X_3}}\end{bmatrix}}^{=[\overline{\nabla}]^T}=\begin{bmatrix}\dfrac{\part{x_1}}{\part{X_1}}&\dfrac{\part{x_1}}{\part{X_2}}&\dfrac{\part{x_1}}{\part{X_3}}\\\dfrac{\part{x_2}}{\part{X_1}}&\dfrac{\part{x_2}}{\part{X_2}}&\dfrac{\part{x_2}}{\part{X_3}}\\\dfrac{\part{x_3}}{\part{X_1}}&\dfrac{\part{x_3}}{\part{X_2}}&\dfrac{\part{x_3}}{\part{X_3}}\end{bmatrix}$

* $\textbf{F}(\textbf{X},t)$:

  * is a primary measure of deformation

  * characterizes the variation of relative placements in the neighborhood of a **material** point (particle).

    $\boxed{d\textbf{x}=\textbf{F}(\textbf{X},t)\cdot{d\textbf{X}}}$

## Inverse (spatial) Deformation Gradient Tensor

* The inverse Equations of Motion:

  $\begin{cases}X_i=\varphi^{-1}_i(x_1,x_2,x_3,t)\stackrel{not.}{=}X_i(x_1,x_2,x_3,t)\space\space\space\space{i\in\{1,2,3\}}\\\textbf{X}=\mathbf{\varphi^{-1}}(\textbf{x},t)\stackrel{not.}{=}\textbf{X}(\textbf{x},t)\end{cases}$

* Differentiating w.r.t $\textbf{x}$:

  $\boxed{\begin{cases}dX_i=\dfrac{\part{X_i(\textbf{X},t)}}{\part{x_j}}dx_j\stackrel{not.}{=}F^{-1}_{ij}(\textbf{x},t)dx_j\space\space\space\space{i\in\{1,2,3\}}\\d\textbf{X}=\dfrac{\part{\textbf{X}(\textbf{x},t)}}{\part{\textbf{x}}}dx_j\stackrel{not.}{=}\textbf{F}^{-1}(\textbf{x},t)\cdot{d\textbf{x}}\end{cases}}$

  where $\textbf{F}^{-1}(\textbf{x},t)$ is the inverse (spatial) deformation gradient tensor

## Inverse (spatial) Deformation Gradient Tensor

* The spatial (or inverse) deformation gradient tensor: $\boxed{d\textbf{X}=\textbf{F}^{-1}(\textbf{x},t)\cdot{d\textbf{x}}}$

  $\begin{cases}\textbf{F}^{-1}(\textbf{x},t)\equiv\textbf{X}(\textbf{x},t)\otimes\nabla\\F^{-1}_{ij}=\dfrac{\part{X_i}}{\part{x_j}}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

  > ==REMARK== The spatial Nabla operator is defined as: $\nabla=\dfrac{\part{}}{\part{x_i}}\hat{{\textbf{e}}}_i$
  >
  > $[\nabla]=\begin{bmatrix}\dfrac{\partial}{x_1}\\\dfrac{\partial}{x_2}\\\dfrac{\partial}{x_3}\end{bmatrix}$

  $[\textbf{F}^{-1}]=[\textbf{X}\otimes\nabla]=\overbrace{\begin{bmatrix}\text{X}_1\\\text{X}_2\\\text{X}_3\end{bmatrix}}^{=[\textbf{X}]}\overbrace{\begin{bmatrix}\dfrac{\partial}{\partial{x_1}}&\dfrac{\partial}{\partial{x_2}}&\dfrac{\partial}{\partial{x_3}}\end{bmatrix}}^{=[\nabla]^T}=\begin{bmatrix}\dfrac{\part{X_1}}{\part{x_1}}&\dfrac{\part{X_1}}{\part{x_2}}&\dfrac{\part{X_1}}{\part{x_3}}\\\dfrac{\part{X_2}}{\part{x_1}}&\dfrac{\part{X_2}}{\part{x_2}}&\dfrac{\part{X_2}}{\part{x_3}}\\\dfrac{\part{X_3}}{\part{x_1}}&\dfrac{\part{X_3}}{\part{x_2}}&\dfrac{\part{X_3}}{\part{x_3}}\end{bmatrix}$

* $\textbf{F}^{-1}(\textbf{x},t)$:

  * is a primary measure of deformation
  * characterizes the variation of relative placements in the neighborhood of a **spatial** point.
  * It is **not** the spatial description of the material deformation gradient tensor.

## Properties of the Deformation Gradients

* the *spatial* deformation gradient tensor is the inverse of the *material* deformation gradient tensor:

  $\dfrac{\part{x_i}}{\part{X_k}}\dfrac{\part{X_k}}{\part{x_j}}=\dfrac{\part{x_i}}{\part{x_j}}=\delta_{ij}$	$\Rightarrow$	$\textbf{F}\cdot\textbf{F}^{-1}=\textbf{F}^{-1}\cdot\textbf{F}=\textbf{1}$

* if $\textbf{F}$ is not dependent on the space coordinates, $\textbf{F}(\textbf{X},t)\equiv\textbf{F}(\textbf{X})$ the deformation is said to be ==homogeneous==.

  * every part of the solid body deforms as the whole does.
  * the associated motion is called **affine**.

* if there is **no motion**, $\textbf{x}=\textbf{X}$ and $\textbf{F}=\dfrac{\part{\textbf{x}}}{\part{\textbf{X}}}=\textbf{F}^{-1}=\textbf{1}$.

### Example

compute the deformation gradient and inverse deformation gradient tensors for a motion equation with Cartesian components given by,

$[\textbf{x}]=\begin{bmatrix}X+Y^2t\\Y(1+t)\\Ze^t\end{bmatrix}$

using the results obtained, check that $\textbf{F}\cdot\textbf{F}^{-1}=\textbf{1}$.

### Solution

The Cartesian components of the deformation gradient tensor are,

$[\textbf{F}(\textbf{X},t)]=\textbf{x}\otimes\overline{\nabla}^T=\begin{bmatrix}X+Y^2t\\Y(1+t)\\Ze^t\end{bmatrix}\cdot\begin{bmatrix}\dfrac{\partial}{\partial{X}}&\dfrac{\partial}{\partial{Y}}&\dfrac{\partial}{\partial{Z}}\end{bmatrix}=\begin{bmatrix}1&2Yt&0\\0&1+t&0\\0&0&e^t\end{bmatrix}$

The Cartesian components of the inverse motion equation will be given by,

$[\textbf{X}]=[\varphi^{-1}(\textbf{x},t)]=\begin{bmatrix}X=x-\dfrac{y^2t}{(1+t)^2}\\Y=\dfrac{y}{1+t}\\Z=ze^{-t}\end{bmatrix}$	$\left[\underbrace{\textbf{F}(\textbf{X}(\textbf{x},t),t)}_{\textbf{f}(\textbf{x},t)}\right]=\left[\textbf{f}(\textbf{x},t)\right]=\begin{bmatrix}1&\dfrac{2yt}{(1+t)}&0\\0&1+t&0\\0&0&e^t\end{bmatrix}$

The Cartesian components of the inverse deformation gradient tensor are,

$[\textbf{F}^{-1}(\textbf{x},t)]=\begin{bmatrix}1&-\dfrac{2yt}{(1+t)^2}&0\\0&\dfrac{1}{1+t}&0\\0&0&e^{-t}\end{bmatrix}$

And it is verified that $\textbf{F}\cdot\textbf{F}^{-1}=\textbf{1}$:

$\textbf{F}\cdot\textbf{F}^{-1}=\begin{bmatrix}1&\dfrac{2yt}{(1+t)}&0\\0&1+t&0\\0&0&e^t\end{bmatrix}\cdot\begin{bmatrix}1&-\dfrac{2yt}{(1+t)^2}&0\\0&\dfrac{1}{1+t}&0\\0&0&e^{-t}\end{bmatrix}=\begin{bmatrix}1&-\dfrac{2yt}{(1+t)^2}+-\dfrac{2yt}{(1+t)^2}&0\\0&\dfrac{1+t}{1+t}&0\\0&0&e^te^{-t}\end{bmatrix}=\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}=[\textbf{1}]$

# Displacements

* **Displacement**: relative position of a particle, in its current (deformed) configuration at time t, with respect to its position in the initial (undeformed) configuration.

* **Displacement field**: displacement of all the particles in the continuous medium.

  * Material description (Lagrangian form):

    $\begin{cases}\textbf{U}(\textbf{X},t)=\textbf{x}(\textbf{X},t)-\textbf{X}\\U_i(\textbf{X},t)=x_i(\textbf{X},t)-X_i\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

  * Spatial description (Eulerian form):

    $\begin{cases}\textbf{u}(\textbf{x},t)=\textbf{x}-\textbf{X}(\textbf{x},t)\\u_i(\textbf{x},t)=x_i-X_i(\textbf{x},t)\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

## Displacement Gradient Tensor

$\begin{cases}\textbf{U}(\textbf{X},t)=\textbf{x}(\textbf{X},t)-\textbf{X}\\U_i(\textbf{X},t)=x_i(\textbf{X},t)-X_i\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

* Differentiating $\textbf{U}$ w.r.t. $\textbf{X}$:

  $\dfrac{\part{U_i}(\textbf{X},t)}{\part{X_j}}=\underbrace{\dfrac{\part{x_i}(\textbf{X},t)}{\part{X_j}}}_{F_{ij}}-\underbrace{\dfrac{\part{X_i}}{\part{X_j}}}_{\delta_{ij}}=F_{ij}-\delta_{ij}\stackrel{def}{=}J_{ij}$

$\boxed{\begin{cases}J_{ij}=\dfrac{\part{U_i}}{\part{X_j}}=F_{ij}-\delta_{ij}\space\space\space\space{i,j\in\{1,2,3\}}\\\textbf{J}\stackrel{def}{=}\textbf{U}(\textbf{X},t)\otimes\overline\nabla=\textbf{F}-\textbf{1}\end{cases}}$	$\Rightarrow$	Material Displacement Gradient Tensor

$\begin{cases}\textbf{u}(\textbf{x},t)=\textbf{x}-\textbf{X}(\textbf{x},t)\\u_i(\textbf{x},t)=x_i-X_i(\textbf{x},t)\space\space\space\space{i\in\{1,2,3\}}\end{cases}$

* Differentiating $\textbf{u}$ w.r.t $\textbf{x}$:

  $\dfrac{\part{u_i}(\textbf{x},t)}{\part{x_j}}=\underbrace{\dfrac{\part{x_i}}{\part{x_j}}}_{\delta_{ij}}-\underbrace{\dfrac{\part{X_i}(\textbf{x},t)}{\part{x_j}}}_{F^{-1}_{ij}}=\delta_{ij}-F^{-1}_{ij}\stackrel{def}{=}j_{ij}$

$\boxed{\begin{cases}j_{ij}=\dfrac{\part{u_i}}{\part{x_j}}=\delta_{ij}-F^{-1}_{ij}\space\space\space\space{i,j\in\{1,2,3\}}\\\textbf{j}\stackrel{def}{=}\textbf{u}(\textbf{x},t)\otimes\nabla=\textbf{1}-\textbf{F}^{-1}\end{cases}}$	$\Rightarrow$	Spatial Displacement Gradient Tensor

> ==REMARK== If motion is a **pure shifting**:
>
> $\textbf{x}(\textbf{X},t)=\textbf{X}+\textbf{U}(t)$ $\Rightarrow$ $\textbf{F}=\dfrac{\part{\textbf{x}}}{\part{X}}=\textbf{1}=\textbf{F}^{-1}$ and $\textbf{j}=\textbf{J}=\textbf{0}$

# Strain Tensors

* $\textbf{F}$ characterizes changes of relative placements during motion **but is not a suitable measure of deformation for engineering purposes**:

  * It is not null when no changes of distances and angles take place, e.g., in rigid-body motions.

* **Strain** is a normalized measure of deformation which **characterizes the changes of distances and angles between particles**.

  * It reduces to zero when there is no change of distances and angles between particles.

* Consider $\mathbf{P}$ is a particle in the material configuration, and $\mathbf{Q}$, another particle which has the distance $dS$ from $\mathbf{P}$.

  $\begin{cases}d\textbf{x}=\textbf{F}\cdot{d\textbf{X}}\\dx_i=F_{ij}dX_j\end{cases}$

  $\begin{cases}d\textbf{X}=\textbf{F}^{-1}\cdot{d\textbf{x}}\\dX_i=F^{-1}_{ij}dx_j\end{cases}$

  * where $dS$ is the length of segment $d\textbf{X}$ : $dS=\sqrt{d\textbf{X}\cdot{d\textbf{X}}}$
  * and $ds$ is the length of segment $d\textbf{x}$ : $ds=\sqrt{d\textbf{x}\cdot{d\textbf{x}}}$

## Strain Tensors

Since

​	$\begin{cases}d\textbf{X}=\textbf{F}^{-1}\cdot{d\textbf{x}}\\dX_i=F^{-1}_{ij}dx_j\end{cases}$	$\begin{cases}d\textbf{x}=\textbf{F}\cdot{d\textbf{X}}\\dx_i=F_{ij}dX_j\end{cases}$

​	$dS=\sqrt{d\textbf{X}\cdot{d\textbf{X}}}$	$ds=\sqrt{d\textbf{x}\cdot{d\textbf{x}}}$

* One can write:

$\begin{cases}(ds)^2=d\textbf{x}\cdot{d\textbf{x}}=[d\textbf{x}]^T\cdot{[d\textbf{x}]}=[\textbf{F}\cdot{d\textbf{X}}]^T\cdot{[\textbf{F}\cdot{d\textbf{X}}]}=d\textbf{X}\cdot\textbf{F}^{-1}\cdot\textbf{F}\cdot{d\textbf{X}}\\(ds)^2=dx_k\cdot{dx_k}=F_{ki}dX_iF_{kj}dX_j=dX_iF_{ki}F_{kj}dX_j=dX_iF^T_{ik}F_{kj}dX_j\end{cases}$

$\begin{cases}(dS)^2=d\textbf{X}\cdot{d\textbf{X}}=[d\textbf{X}]^T\cdot{[d\textbf{X}]}=[\textbf{F}^{-1}\cdot{d\textbf{x}}]^T\cdot{[\textbf{F}^{-1}\cdot{d\textbf{x}}]}\stackrel{not.}{=}d\textbf{x}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot{d\textbf{x}}\\(dS)^2=dX_k\cdot{dX_k}=F^{-1}_{ki}dx_iF^{-1}_{kj}dx_j=dx_iF^{-1}_{ki}F^{-1}_{kj}dx_j=dx_iF^{-T}_{ik}F^{-1}_{kj}dx_j\end{cases}$

> ==REMARK== The convention $\left[(\bullet)^{-1}\right]^T\stackrel{not.}{=}(\bullet)^T$ is used.

## Green-Lagrange Strain Tensor

$(ds)^2=d\textbf{X}\cdot\textbf{F}^T\cdot\textbf{F}\cdot{d\textbf{X}}$	$(dS)^2=d\textbf{X}\cdot{d\textbf{X}}$

* subtracting:

$(ds)^2-(dS)^2=d\textbf{X}\cdot\textbf{F}^T\cdot\textbf{F}\cdot{d\textbf{X}}-d\textbf{X}\cdot{d\textbf{X}}=d\textbf{X}\cdot\textbf{F}^T\cdot\textbf{F}\cdot{d\textbf{X}}-d\textbf{X}\cdot{\textbf{1}}\cdot{d\textbf{X}}\\=d\textbf{X}\cdot\underbrace{(\textbf{F}^T\cdot\textbf{F}-\textbf{1})}_{\stackrel{def}{=}2\textbf{E}}\cdot{d\textbf{X}}=2d\textbf{X}\cdot\textbf{E}\cdot{d\textbf{X}}$

* The **Green-Lagrange** or **Material Strain Tensor** is defined:

  $\begin{cases}\textbf{E}(\textbf{X},t)=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})\\E_{ij}(\textbf{X},t)=\dfrac{1}{2}(F_{ki}\cdot{F_{kj}}-\delta_{ij})\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

* $\textbf{E}$ is symmetrical:

  $\begin{cases}\textbf{E}^T=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})^T=\dfrac{1}{2}(\textbf{F}^T\cdot(\textbf{F}^T)^T-\textbf{1}^T)=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})=\textbf{E}\\E_{ij}=E_{ji}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

## Euler-Almansi Strain Tensor

$(ds)^2=d\textbf{x}\cdot{d\textbf{x}}$	$(dS)^2=d\textbf{x}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot{d\textbf{x}}$

* Subtracting:

$(ds)^2-(dS)^2=d\textbf{x}\cdot{d\textbf{x}}-d\textbf{x}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot{d\textbf{x}}=d\textbf{x}\cdot\textbf{1}\cdot{d\textbf{x}}-d\textbf{x}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot{d\textbf{x}}\\=d\textbf{x}\cdot\underbrace{(\textbf{1}-\textbf{F}^T\cdot\textbf{F})}_{\stackrel{def}{=}2\textbf{e}}\cdot{d\textbf{x}}=2d\textbf{x}\cdot\textbf{e}\cdot{d\textbf{x}}$

* The **Euler-Almansi** or **Spatial Strain Tensor** is defined:

  $\begin{cases}\textbf{e}(\textbf{x},t)=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})\\e_{ij}(\textbf{x},t)=\dfrac{1}{2}(\delta_{ij}-F^{-1}_{ki}\cdot{F^{-1}_{kj}})\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

* $\textbf{e}$ is symmetrical:

  $\begin{cases}\textbf{e}^T=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})^T=\dfrac{1}{2}(\textbf{1}^T-(\textbf{F}^{-1})^T\cdot(\textbf{F}^{-T})^T)=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-T})=\textbf{e}\\e_{ij}=e_{ji}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

## Particularities of the Strain Tensors

* The **Green-Lagrange** and the **Euler-Almansi Strain Tensors** are **<u>different tensors</u>**.

  * They are <u>not</u> the material and spatial descriptions of a same strain tensor.

  * They are affected by different vectors ($d\textbf{X}$ and $d\textbf{x}$) when measuring distances:

    $\boxed{(ds)^2-(dS)^2=2d\textbf{X}\cdot\textbf{E}\cdot{d\textbf{X}}=2d\textbf{x}\cdot\textbf{e}\cdot{d\textbf{x}}}$

* The **Green-Lagrange Strain Tensor** is inherently obtained in material description, $\textbf{E}=\textbf{E}(\textbf{X},t)$.

  * By substitution of the inverse Equations of Motion, $\textbf{E}=\textbf{E}(\textbf{X}(\textbf{x},t),t)=\textbf{E}(\textbf{x},t)$

* The **Euler-Almansi Strain Tensor** is inherently obtained in spatial description, $\textbf{e}=\textbf{e}(\textbf{X},t)$.

  * By substitution of the Equation of Motion, $\textbf{e}=\textbf{e}(\textbf{x}(\textbf{X},t),t)=\textbf{e}(\textbf{X},t)$.

## Strain Tensors in terms of Displacements

* Substituting $\textbf{F}^{-1}=\textbf{1}-\textbf{j}$ and $\textbf{F}=\textbf{J}+\textbf{1}$ into

  $\textbf{E}=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})$ and $\textbf{e}(\textbf{x},t)=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})$:

  $\boxed{\begin{cases}\textbf{E}=\dfrac{1}{2}\left[(\textbf{1}+\textbf{J}^T)\cdot(\textbf{1}+\textbf{J})-\textbf{1}\right]=\dfrac{1}{2}\left[\textbf{J}+\textbf{J}^T+\textbf{J}^T\cdot\textbf{J}\right]\\E_{ij}=\dfrac{1}{2}\left[\dfrac{\part{U}_i}{\part{X}_j}+\dfrac{\part{U}_j}{\part{X}_i}+\dfrac{\part{U}_k}{\part{X}_i}\dfrac{\part{U}_k}{\part{X}_j}\right]\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

  $\boxed{\begin{cases}\textbf{e}=\dfrac{1}{2}\left[\textbf{1}-(\textbf{1}-\textbf{j}^T)\cdot(\textbf{1}-\textbf{j})\right]=\dfrac{1}{2}\left[\textbf{j}+\textbf{j}^T-\textbf{j}^T\cdot\textbf{j}\right]\\e_{ij}=\dfrac{1}{2}\left[\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}+\dfrac{\part{u}_k}{\part{x}_i}\dfrac{\part{u}_k}{\part{x}_j}\right]\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

### Example

For the movement in the previous example, obtain the strain tensors in the material and spatial description.

​					$[\textbf{x}]=\begin{bmatrix}X+Y^2t\\Y(1+t)\\Ze^t\end{bmatrix}$

$\textbf{F}=\begin{bmatrix}1&2Yt&0\\0&1+t&0\\0&0&e^t\end{bmatrix}$	$\textbf{F}^{-1}=\begin{bmatrix}1&-\dfrac{2yt}{(1+t)^2}&0\\0&\dfrac{1}{1+t}&0\\0&0&e^{-t}\end{bmatrix}$

The strain tensor in material description:

$\textbf{E}=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})$$=\dfrac{1}{2}\left(\begin{bmatrix}1&0&0\\2Yt&1+t&0\\0&0&e^t\end{bmatrix}\cdot\begin{bmatrix}1&2Yt&0\\0&1+t&0\\0&0&e^t\end{bmatrix}-\textbf{1}\right)=\dfrac{1}{2}\begin{bmatrix}1-1&2Yt&0\\2Yt&(2Yt)^2+(1+t)^2-1&0\\0&0&e^te^t-1\end{bmatrix}$$=\dfrac{1}{2}\begin{bmatrix}0&2Yt&0\\2Yt&(2Yt)^2+(1+t)^2-1&0\\0&0&e^{2t}-1\end{bmatrix}$

The strain tensor in spatial description:

$\textbf{e}(\textbf{x},t)=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})$$=\dfrac{1}{2}\left(\textbf{1}-\begin{bmatrix}1&0&0\\-\dfrac{2yt}{(1+t)^2}&\dfrac{1}{1+t}&0\\0&0&e^{-t}\end{bmatrix}\cdot\begin{bmatrix}1&-\dfrac{2yt}{(1+t)^2}&0\\0&\dfrac{1}{1+t}&0\\0&0&e^{-t}\end{bmatrix}\right)$$=\dfrac{1}{2}\begin{bmatrix}1-1&-\dfrac{2yt}{(1+t)^2}&0\\-\dfrac{2yt}{(1+t)^2}&\textbf{1}-\left(\left(-\dfrac{2yt}{(1+t)^2}\right)^2+\left(\dfrac{1}{1+t}\right)^2\right)&0\\0&0&\textbf{1}-e^{-t}e^{-t}\end{bmatrix}$$=\dfrac{1}{2}\begin{bmatrix}0&-\dfrac{2yt}{(1+t)^2}&0\\-\dfrac{2yt}{(1+t)^2}&\textbf{1}-\left(\left(-\dfrac{2yt}{(1+t)^2}\right)^2+\left(\dfrac{1}{1+t}\right)^2\right)&0\\0&0&\textbf{1}-e^{-2t}\end{bmatrix}$

Observe that $\textbf{E}\neq\textbf{e}$.

# Variation of Distances

* The **stretch ratio** or **stretch** is defined as:

  $\boxed{\textbf{stretch}\stackrel{def}{=}\lambda_T=\lambda_t=\dfrac{\overline{P^\prime{Q^\prime}}}{\overline{PQ}}=\dfrac{ds}{dS}\space\space\space\space{(0<\lambda<\infty)}}$

  $\textbf{T}$ is the unit vector of $\overrightarrow{PQ}$, $t$ is the unit vector of $\overrightarrow{P^\prime{Q^\prime}}$

  > ==REMARK== The sub-indexes $(\bullet)_\textbf{T}$ and $(\bullet)_\textbf{t}$ are often dropped. But one must bear in mind that stretch and unit elongation always have a particular direction associated to them.

* The **extension** or **unit elongation** is defined as:

  $\boxed{\textbf{unit elongation}\stackrel{def}{=}\varepsilon_\textbf{T}=\varepsilon_\textbf{t}=\dfrac{\Delta\overline{PQ}}{\overline{PQ}}=\dfrac{ds-dS}{dS}}$
  
  $\Delta\overline{PQ}=\overline{P^\prime{Q^\prime}}-\overline{PQ}$

## Relation between Stretch and Unit Elongation

* The **stretch** and **unit elongation** for a same point and direction are related through:

  $\varepsilon=\dfrac{ds-dS}{dS}=\underbrace{\dfrac{ds}{dS}}_{=\lambda}-1=\lambda-1$	$\Rightarrow$	$(-1<\varepsilon<\infty)$

  * If $\lambda=1$ $(\varepsilon=0)$ $\Rightarrow$ $ds=dS$: $P$ and $Q$ may have moved in time but have kept the <u>distance</u> between them <u>constant</u>.
  * If $\lambda>1$ $(\varepsilon>0)$ $\Rightarrow$ $ds>dS$: the <u>distance</u> between $P$ and $Q$ has <u>increased</u> with the deformation of the medium.
  * If $\lambda<1$ $(\varepsilon<0)$ $\Rightarrow$ $ds<dS$: the <u>distance</u> between $P$ and $Q$ has <u>decreased</u> with the deformation of the medium.

## Stretch and Unit Elongation in terms of the Strain Tensors

* Considering:

  $\begin{cases}(ds)^2-(dS)^2=2d\textbf{X}\cdot\textbf{E}\cdot{d}\textbf{X}\\(ds)^2-(dS)^2=2d\textbf{x}\cdot\textbf{e}\cdot{d}\textbf{x}\end{cases}$	$\begin{cases}d\textbf{X}=\textbf{T}dS\\d\textbf{x}=\textbf{t}dS\end{cases}$

* Then:

  $\begin{cases}(ds)^2-(dS)^2=2(dS)^2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}\space\space\space\stackrel{\cross{}^1{\mskip -5mu/\mskip -3mu}_{(dS)^2}}{\Longrightarrow}\overbrace{\left(\dfrac{ds}{dS}\right)}^{=\lambda^2}-1=2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}\\(ds)^2-(dS)^2=2(ds)^2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}\space\space\space\underset{\cross{}^1{\mskip -5mu/\mskip -3mu}_{(ds)^2}}{\Longrightarrow}1-\underbrace{\left(\dfrac{ds}{dS}\right)}_{=\left({}^1{\mskip -5mu/\mskip -3mu}_\lambda\right)^2}=2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}\end{cases}$

  $\boxed{\begin{matrix*}[l]\lambda=\sqrt{1+2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}\\\varepsilon=\lambda-1=\sqrt{1+2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}-1\end{matrix*}}$	$\boxed{\begin{matrix*}[l]\lambda=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}\\\varepsilon=\lambda-1=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}-1\end{matrix*}}$

  > ==REMARK== $\textbf{E}(\textbf{X},t)$ and $\textbf{e}(\textbf{X},t)$ contain information regarding the stretch and unit elongation for any direction in the differential neighborhood of a point.

# Variation of Angles

​	$\begin{cases}d\textbf{X}^{(1)}=\textbf{T}^{(1)}dS^{(1)}\\d\textbf{X}^{(2)}=\textbf{T}^{(2)}dS^{(2)}\end{cases}$	$\begin{cases}d\textbf{x}^{(1)}=\textbf{t}^{(1)}ds^{(1)}\\d\textbf{x}^{(2)}=\textbf{t}^{(2)}ds^{(2)}\end{cases}$

* The scalar product of the vectors $d\textbf{x}^{(1)}$ and $d\textbf{x}^{(2)}$:

  $d\textbf{x}^{(1)}\cdot{d\textbf{x}^{(2)}}=|d\textbf{x}^{(1)}|\cdot|d\textbf{x}^{(2)}|\cos{\theta}=ds^{(1)}ds^{(2)}\cos{\theta}$

$\underbrace{\underbrace{d\textbf{x}^{(1)}}_{\left[d\textbf{x}^{(1)}\right]^T}\cdot{\underbrace{d\textbf{x}^{(2)}}_{\left[d\textbf{x}^{(2)}\right]^T}}}_{\begin{CD}\\@VV \begin{cases}d\textbf{x}^{(1)}=\textbf{F}\cdot{d\textbf{X}^{(1)}}\\d\textbf{x}^{(2)}=\textbf{F}\cdot{d\textbf{X}^{(2)}}\end{cases} V\end{CD}}=\boxed{ds^{(1)}ds^{(2)}\cos{\theta}}\longrightarrow\boxed{\cos\theta=\dfrac{\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}}{\sqrt{1+2\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}}\sqrt{1+2\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}}}}$

$\begin{CD}d\textbf{x}^{(1)}\cdot{d\textbf{x}^{(2)}}=\left[\textbf{F}\cdot{d\textbf{X}^{(1)}}\right]^T\cdot\left[\textbf{F}\cdot{d\textbf{X}^{(2)}}\right]=d\textbf{X}^{(1)}\cdot\underbrace{(\textbf{F}^T\cdot\textbf{F})}_{2\textbf{E}+\textbf{1}}\cdot{d\textbf{X}^{(2)}}\\@V \begin{rcases*}d\textbf{X}^{(1)}=\textbf{T}^{(1)}dS^{(1)}\\d\textbf{X}^{(2)}=\textbf{T}^{(2)}dS^{(2)}\end{rcases*} VV\end{CD}$

$d\textbf{x}^{(1)}\cdot{d\textbf{x}^{(2)}}=\underbrace{dS^{(1)}}_{{}^{ds^{(1)}}{\mskip -5mu/\mskip -3mu}_{\lambda^{(1)}}}\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}\underbrace{dS^{(2)}}_{{}^{ds^{(2)}}{\mskip -5mu/\mskip -3mu}_{\lambda^{(2)}}}=ds^{(1)}ds^{(2)}\begin{CD}\underbrace{\left(\dfrac{1}{\lambda^{(1)}}\dfrac{1}{\lambda^{(2)}}\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}\right)}\\@VV \lambda=\sqrt{1+2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}} V\end{CD}=ds^{(1)}ds^{(2)}\cos{\theta}$

​											$\left(\dfrac{\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}}{\sqrt{1+2\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}}\sqrt{1+2\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}}}\right)$

* The scalar product of the vectors $d\textbf{X}^{(1)}$ and $d\textbf{X}^{(2)}$:

  $d\textbf{X}^{(1)}\cdot{d\textbf{X}^{(2)}}=|d\textbf{X}^{(1)}|\cdot|d\textbf{X}^{(2)}|\cos{\Theta}=dS^{(1)}dS^{(2)}\cos{\Theta}$

$\underbrace{\underbrace{d\textbf{X}^{(1)}}_{\left[d\textbf{X}^{(1)}\right]^T}\cdot{\underbrace{d\textbf{X}^{(2)}}_{\left[d\textbf{X}^{(2)}\right]^T}}}_{\begin{CD}\\@VV \begin{cases}d\textbf{X}^{(1)}=\textbf{F}^{-1}\cdot{d\textbf{x}^{(1)}}\\d\textbf{X}^{(2)}=\textbf{F}^{-1}\cdot{d\textbf{x}^{(2)}}\end{cases} V\end{CD}}=\boxed{dS^{(1)}dS^{(2)}\cos{\Theta}}\longrightarrow\boxed{\cos\Theta=\dfrac{\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}}{\sqrt{1-2\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}}\sqrt{1-2\textbf{t}^{(2)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}}}}$

$\begin{CD}d\textbf{X}^{(1)}\cdot{d\textbf{X}^{(2)}}=\left[\textbf{F}^{-1}\cdot{d\textbf{x}^{(1)}}\right]^T\cdot\left[\textbf{F}^{-1}\cdot{d\textbf{x}^{(2)}}\right]=d\textbf{x}^{(1)}\cdot\underbrace{(\textbf{F}^{-T}\cdot\textbf{F}^{-1})}_{\textbf{1}-2\textbf{e}}\cdot{d\textbf{x}^{(2)}}\\@V \begin{rcases*}d\textbf{x}^{(1)}=\textbf{t}^{(1)}ds^{(1)}\\d\textbf{x}^{(2)}=\textbf{t}^{(2)}ds^{(2)}\end{rcases*} VV\end{CD}$

$d\textbf{X}^{(1)}\cdot{d\textbf{X}^{(2)}}=\underbrace{ds^{(1)}}_{\lambda^{(1)}dS^{(1)}}\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}\underbrace{ds^{(2)}}_{\lambda^{(2)}dS^{(2)}}=dS^{(1)}dS^{(2)}\begin{CD}\underbrace{\left(\lambda^{(1)}\lambda^{(2)}\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}\right)}\\@VV \lambda=\cfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}} V\end{CD}=dS^{(1)}dS^{(2)}\cos{\Theta}$



​											$\left(\dfrac{\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}}{\sqrt{1-2\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}}\sqrt{1-2\textbf{t}^{(2)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}}}\right)$

> ==REMARK== $\textbf{E}(\textbf{X},t)$ and $\textbf{e}(\textbf{X},t)$ contain information regarding the variation in angles between segments in the differential neighborhood of a point.

### Example

Let us consider the motion of a continuum body such that the spatial description of the Cartesian components of the spatial Almansi strain tensor is given by,

$\left[{\textbf{e}(\textbf{x},t)}\right]=\begin{bmatrix}0&0&-te^{tz}\\0&0&0\\-te^{tz}&0&t(2e^{tz}-e^t)\end{bmatrix}$

Compute at time $\text{t}=0$, the length of the curve that at time $\text{t}=2$ is a straight line going from point $\text{a}(0,0,0)$ to point $\text{b}(1,1,1)$.

The length of the curve at time $\text{t}=0$ can be expressed as,

$L=\displaystyle\int_{A}^{B}{\underbrace{dS}_{=\dfrac{ds}{\lambda}}}=\displaystyle\int_{a}^{b}{\dfrac{1}{\lambda}(\textbf{x},t)ds}$

### Solution

The inverse of the stretch, at the points belonging to the straight line going from $\text{a}(0,0,0)$ to $\text{b}(1,1,1)$ along the unit vector in the direction of the straight line, is given by,

$\lambda(\textbf{x},t)=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}$	$\rightarrow$	$\lambda^{-1}(\textbf{x},t)=\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}$

Where the unit vector is given by,

$[\textbf{t}]=\dfrac{1}{\sqrt{3}}\begin{bmatrix}1\\1\\1\end{bmatrix}$

Substituting the unit vector and spatial Almansi strain tensor into the expression of the inverse of the stretching yields,

$\lambda^{-1}(\textbf{x},t)=\sqrt{1+\dfrac{2}{3}te^t}$

The inverse of the stretch, which is uniform and therefore does not depends on the spatial coordinates, at time $\text{t}=2$ reads,

$\lambda^{-1}(\textbf{x},2)=\sqrt{1+\dfrac{4}{3}e^2}$

Substituting the inverse of the stretch into the integral expression providing the length at time $\text{t}=0$ yields,

$L=\displaystyle\int_{\Gamma}{dS}=\displaystyle\int_{a}^{b}{\lambda^{-1}(\textbf{x},t)ds}$$=\displaystyle\int_{a}^{b}{\sqrt{1+\dfrac{4}{3}e^2}}ds=\sqrt{1+\dfrac{4}{3}e^2}\underbrace{\displaystyle\int_{(0,0,0)}^{(1,1,1)}{ds}}_{\mathcal{l}=\sqrt{3}}=\sqrt{3+4e^2}$

# Physical interpretation of the Strain Tensors

## Physical Interpretation of $\textbf{E}$

* Consider the components of the material strain tensor, $\textbf{E}$:

  $E=\begin{bmatrix}E_{XX}&E_{XY}&E_{XZ}\\E_{YX}&E_{YY}&E_{YZ}\\E_{ZX}&E_{ZY}&E_{ZZ}\end{bmatrix}=\begin{bmatrix}E_{11}&E_{12}&E_{13}\\E_{21}&E_{22}&E_{23}\\E_{31}&E_{32}&E_{33}\end{bmatrix}$

* For a segment parallel to the $X$-axis,

  $\textbf{T}^{(1)}=\begin{Bmatrix}1\\0\\0\end{Bmatrix}$	$d\textbf{X}=dS\textbf{T}^{(1)}=\begin{Bmatrix}dS\\0\\0\end{Bmatrix}$

  the stretch is:

  $\lambda=\sqrt{1+2\underbrace{\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}}$

​			$\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}=\underbrace{\begin{bmatrix}1&0&0\end{bmatrix}}_{\left[{\textbf{T}^{(1)}}\right]^T}\cdot\begin{bmatrix}E_{11}&E_{12}&E_{13}\\E_{21}&E_{22}&E_{23}\\E_{31}&E_{32}&E_{33}\end{bmatrix}\cdot\underbrace{\begin{bmatrix}1\\0\\0\end{bmatrix}}_{\left[{\textbf{T}^{(1)}}\right]}=E_{11}$

$\Rightarrow$	$\lambda_1=\sqrt{1+2E_{11}}$	Stretching of the material in the $X$-direction

* Similarly, the stretching of the material in the $Y$-direction and the $Z$-direction:

  $\boxed{\begin{matrix*}{\lambda_1=\sqrt{1+2E_{11}} \Rightarrow \varepsilon_X=\lambda_X-1=\sqrt{1+2E_{XX}}-1}\\{\lambda_2=\sqrt{1+2E_{22}} \Rightarrow \varepsilon_Y=\lambda_Y-1=\sqrt{1+2E_{YY}}-1}\\{\lambda_3=\sqrt{1+2E_{33}} \Rightarrow \varepsilon_Z=\lambda_Z-1=\sqrt{1+2E_{ZZ}}-1}\end{matrix*}}$

* The *longitudinal strains* contain information on the stretch and unit elongation of the segments initially oriented in the $X$, $Y$ and $Z$-directions (in the material configurations).

  $E=\begin{bmatrix}\underline{\mathbf{E_{XX}}}&E_{XY}&E_{XZ}\\E_{YX}&\underline{\mathbf{E_{YY}}}&E_{YZ}\\E_{ZX}&E_{ZY}&\underline{\mathbf{E_{ZZ}}}\end{bmatrix}$	$\begin{cases}\text{if }E_{XX}=0\space\space\space\Rightarrow\space\space\space\varepsilon_X=0\space\space\space\text{No elongation in the }X\text{-direction}\\\text{if }E_{YY}=0\space\space\space\Rightarrow\space\space\space\varepsilon_Y=0\space\space\space\text{No elongation in the }Y\text{-direction}\\\text{if }E_{ZZ}=0\space\space\space\Rightarrow\space\space\space\varepsilon_Z=0\space\space\space\text{No elongation in the }Z\text{-direction}\end{cases}$

* Consider the angle between a segment parallel to the $X$-axis and a segment parallel to the $Y$-axis,

  $\textbf{T}^{(1)}=\begin{Bmatrix}1\\0\\0\end{Bmatrix}$  $\textbf{T}^{(2)}=\begin{Bmatrix}0\\1\\0\end{Bmatrix}$	$\begin{cases}\textbf{T}^{(1)}\cdot\textbf{T}^{(2)}=0\\\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}=E_{11}\\\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}=E_{12}\\\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}=E_{22}\\\Theta_{XY}=\dfrac{\pi}{2}\end{cases}$

  the angle is:

  $\boxed{\cos\theta=\dfrac{\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}}{\sqrt{1+2\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}}\sqrt{1+2\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}}}}$	$\Rightarrow$

  $\cos\theta=\dfrac{2E_{12}}{\sqrt{1+2E_{11}}\sqrt{1+2E_{22}}}$	$\Rightarrow$

  $\theta\equiv\theta_{xy}=\arccos\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}=\dfrac{\pi}{2}-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}$

* The increment of the final angle w.r.t. its initial value:

  $\Delta\Theta_{XY}=\theta_{xy}-\underbrace{\Theta_{XY}}_{\dfrac{\pi}{2}}=-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}$

* Similarly, the increment of the final angle w.r.t its initial value for couples of segments oriented in the direction of the coordinate axes:

  $\boxed{\begin{matrix*}\Delta\Theta_{XY}=-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}\\\Delta\Theta_{XZ}=-\arcsin\dfrac{2E_{XZ}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{ZZ}}}\\\Delta\Theta_{YZ}=-\arcsin\dfrac{2E_{YZ}}{\sqrt{1+2E_{YY}}\sqrt{1+2E_{ZZ}}}\end{matrix*}}$

* The *angular strains* contain information on the variation of the angles between segments initially oriented in the $X$, $Y$ and $Z$-directions (in the material configuration).

  $E=\begin{bmatrix}E_{XX}&\underline{\mathbf{E_{XY}}}&\underline{\mathbf{E_{XZ}}}\\E_{YX}&E_{YY}&\underline{\mathbf{E_{YZ}}}\\E_{ZX}&E_{ZY}&E_{ZZ}\end{bmatrix}$

  $\begin{cases}{\text{if }E_{XY}=0\space\space\space\text{No angle variation between the }X\text{- and }Y\text{-directions}}\\{\text{if }E_{XZ}=0\space\space\space\text{No angle variation between the }X\text{- and }Z\text{-directions}}\\{\text{if }E_{YZ}=0\space\space\space\text{No angle variation between the }Y\text{- and }Z\text{-directions}}\end{cases}$

## Physical Interpretation of $\textbf{e}$

* Consider the components of the spatial strain tensor, $\textbf{e}$:

  $\textbf{e}=\begin{bmatrix}e_{xx}&e_{xy}&e_{xz}\\e_{yx}&e_{yy}&e_{yz}\\e_{zx}&e_{zy}&e_{zz}\end{bmatrix}=\begin{bmatrix}e_{11}&e_{12}&e_{13}\\e_{21}&e_{22}&e_{23}\\e_{31}&e_{32}&e_{33}\end{bmatrix}$

* For a segment parallel to the $x$-axis,

  $\textbf{t}^{(1)}=\begin{Bmatrix}1\\0\\0\end{Bmatrix}$

* the stretch is:

  $\boxed{\lambda=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}}$

  $\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}=\begin{bmatrix}1&0&0\end{bmatrix}\cdot\begin{bmatrix}e_{11}&e_{12}&e_{13}\\e_{21}&e_{22}&e_{23}\\e_{31}&e_{32}&e_{33}\end{bmatrix}\cdot\begin{bmatrix}1\\0\\0\end{bmatrix}=e_{11}$

  $\Rightarrow$	$\lambda=\dfrac{1}{\sqrt{1-2e_{11}}}$	Stretching of the material in the $x$-direction

* Similarly, the stretching of the material in the $y$-direction and the $z$-direction:

  $\boxed{\begin{matrix*}\lambda_1=\dfrac{1}{\sqrt{1-2e_{11}}}\Rightarrow\varepsilon_x=\lambda_x-1=\dfrac{1}{\sqrt{1-2e_{xx}}}-1\\\lambda_2=\dfrac{1}{\sqrt{1-2e_{22}}}\Rightarrow\varepsilon_y=\lambda_y-1=\dfrac{1}{\sqrt{1-2e_{yy}}}-1\\\lambda_3=\dfrac{1}{\sqrt{1-2e_{33}}}\Rightarrow\varepsilon_z=\lambda_z-1=\dfrac{1}{\sqrt{1-2e_{zz}}}-1\end{matrix*}}$

* The *longitudinal strains* contain information on the stretch and unit elongation of the segments oriented in the $x$, $y$ and $z$-directions (in the deformed and actual configurations).

  $\textbf{e}=\begin{bmatrix}\underline{\mathbf{e_{xx}}}&e_{xy}&e_{xz}\\e_{yx}&\underline{\mathbf{e_{yy}}}&e_{yz}\\e_{zx}&e_{zy}&\underline{\mathbf{e_{zz}}}\end{bmatrix}$

* Consider the angle between a segment parallel to the $x$-axis and a segment parallel to the $y$-axis,

  $\textbf{t}^{(1)}=\begin{Bmatrix}1\\0\\0\end{Bmatrix}$  $\textbf{t}^{(2)}=\begin{Bmatrix}0\\1\\0\end{Bmatrix}$	$\begin{cases}\textbf{t}^{(1)}\cdot\textbf{t}^{(2)}=0\\\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}=e_{11}\\\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}=e_{12}\\\textbf{t}^{(2)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}=e_{22}\\\theta_{xy}=\dfrac{\pi}{2}\end{cases}$

  the angle is:

  $\boxed{\cos\Theta=\dfrac{\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}}{\sqrt{1-2\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}}\sqrt{1-2\textbf{t}^{(2)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}}}}$	$\Rightarrow$

  $\cos\Theta=\dfrac{2e_{12}}{\sqrt{1-2e_{11}}\sqrt{1-2e_{22}}}$	$\Rightarrow$

  $\Theta\equiv\Theta_{xy}=\dfrac{\pi}{2}+\arcsin\dfrac{2e_{xy}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{yy}}}$

* The increment of the angle in the reference configuration w.r.t. its value in the deformed one:

  $\Delta\theta_{xy}=\underbrace{\theta_{xy}}_{\dfrac{\pi}{2}}-\Theta_{xy}=-\arcsin\dfrac{2e_{xy}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{yy}}}$

* Similarly, the increment of the final angle in the reference configuration w.r.t its value in the deformed one for couples of segments oriented in the direction of the coordinate axes:

  $\boxed{\begin{matrix}\Delta\theta_{xy}=\dfrac{\pi}{2}-\Theta_{XY}=-\arcsin\dfrac{2e_{xy}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{yy}}}\\\Delta\theta_{xz}=\dfrac{\pi}{2}-\Theta_{XZ}=-\arcsin\dfrac{2e_{xz}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{zz}}}\\\Delta\theta_{yz}=\dfrac{\pi}{2}-\Theta_{YZ}=-\arcsin\dfrac{2e_{yz}}{\sqrt{1-2e_{yy}}\sqrt{1-2e_{zz}}}\end{matrix}}$

* The *angular strains* contain information on the variation of the angles between segments oriented in the $x$, $y$ and $z$-directions (in the deformed or actual configuration).

  $\textbf{e}=\begin{bmatrix}e_{xx}&\underline{\mathbf{e_{xy}}}&\underline{\mathbf{e_{xz}}}\\e_{yx}&e_{yy}&\underline{\mathbf{e_{yz}}}\\e_{zx}&e_{zy}&e_{zz}\end{bmatrix}$

# Polar Decomposition

* **Polar Decomposition Theorem:**

  * "For any non-singular 2^nd^ order tensor $\textbf{F}$ there exist two unique positive-definite symmetrical 2^nd^ order tensors $\textbf{U}$ and $\textbf{V}$, and a unique orthogonal 2^nd^ order tensor $\textbf{Q}$ such that:"

    $\begin{rcases*}\textbf{U}\stackrel{not.}{=}\sqrt{\textbf{F}^T\cdot\textbf{F}}\\\textbf{V}\stackrel{not.}{=}\sqrt{\textbf{F}\cdot\textbf{F}^T}\\\textbf{Q}=\textbf{F}\cdot\textbf{U}^{-1}=\textbf{V}^{-1}\cdot\textbf{F}\end{rcases*}$	$\Rightarrow$	$\textbf{F}=\underbrace{\textbf{Q}\cdot\textbf{U}}_{\begin{matrix}\text{right polar}\\\text{decomposition}\end{matrix}}=\overbrace{\textbf{V}\cdot\textbf{Q}}^{\begin{matrix}\text{left polar}\\\text{decomposition}\end{matrix}}$

    * The decomposition is unique.
    * $\textbf{Q}$: Rotation tensor
    * $\textbf{U}$: Right or material stretch tensor
    * $\textbf{V}$: Left or spatial stretch tensor

    > ==REMARK== An orthogonal 2^nd^ order tensor verifies: 
    >
    > $\textbf{Q}^T\cdot\textbf{Q}=\textbf{Q}\cdot\textbf{Q}^T=\textbf{1}$

## Properties of an orthogonal tensor

* An **orthogonal tensor $\textbf{Q}$** when multiplied (dot product) times a vector rotates it (without changing its length): $\textbf{y}=\textbf{Q}\cdot\textbf{x}$

  * $\textbf{y}$ has the same norm as $\textbf{x}$:

    $\norm{\textbf{y}}^2=\textbf{y}\cdot\textbf{y}=[\textbf{y}]^T[\textbf{y}]=\left[\textbf{Q}\cdot\textbf{x}\right]^T\cdot\left[\textbf{Q}\cdot\textbf{x}\right]=\textbf{x}\cdot\underbrace{\textbf{Q}^T\cdot\textbf{Q}}_{1}\cdot\textbf{x}=\norm{\textbf{x}}^2$

  * when $\textbf{Q}$ is applied on two vectors $\textbf{x}^{(1)}$ and $\textbf{x}^{(2)}$, with the same origin, the original angle they form is maintained:

    $\begin{matrix*}\textbf{y}^{(1)}=\textbf{Q}\cdot\textbf{x}^{(1)}\\\textbf{y}^{(2)}=\textbf{Q}\cdot\textbf{x}^{(2)}\end{matrix*}$	$\Rightarrow$	$\dfrac{\textbf{y}^{(1)}\cdot\textbf{y}^{(2)}}{\norm{\textbf{y}^{(1)}}\norm{\textbf{y}^{(2)}}}=\dfrac{\overbrace{\textbf{x}^{(1)}\cdot\textbf{Q}^T}^{[\textbf{y}^{(1)}]^T}\cdot\overbrace{\textbf{Q}\cdot\textbf{x}^{(2)}}^{[\textbf{y}^{(2)}]^T}}{\norm{\textbf{y}^{(1)}}\norm{\textbf{y}^{(2)}}}=\dfrac{\textbf{x}^{(1)}\cdot\textbf{x}^{(2)}}{\norm{\textbf{x}^{(1)}}\norm{\textbf{x}^{(2)}}}=\cos\alpha$

* Consequently, the **rotation $\textbf{y}=\textbf{Q}\cdot\textbf{x}$ maintains angles and distances**.

## Polar Decomposition of $\textbf{F}$

* Consider the deformation gradient tensor, $\textbf{F}$:

  $\textbf{F}=\textbf{Q}\cdot\textbf{U}=\textbf{V}\cdot\textbf{Q}$	$\Rightarrow$

  $d\textbf{x}=\textbf{F}\cdot{d\textbf{X}}=(\textbf{V}\cdot\textbf{Q})\cdot{d\textbf{X}}=\overbrace{\textbf{V}\cdot\overbrace{{(\textbf{Q}\cdot{d\textbf{X}})}}^{\text{rotation}}}^{\text{stretching}}$	$\Rightarrow$	$\boxed{\textbf{F}(\bullet)=\text{stretching}\stackrel{not.}{\circ}\text{rotation}(\bullet)}$

  $d\textbf{x}=\textbf{F}\cdot{d\textbf{X}}=(\textbf{Q}\cdot\textbf{U})\cdot{d\textbf{X}}=\overbrace{\textbf{Q}\cdot\overbrace{{(\textbf{U}\cdot{d\textbf{X}})}}^{\text{stretching}}}^{\text{rotation}}$	$\Rightarrow$	$\boxed{\textbf{F}(\bullet)=\text{rotation}\stackrel{not.}{\circ}\text{stretching}(\bullet)}$

  > ==REMARK== For a rigid solid movement:
  >
  > $\textbf{U}=\textbf{V}=\textbf{1}$ and $\textbf{Q}=\textbf{F}$

# Volume Variation

## Differential Volume Ratio

* Consider the variation of a differential volume associated to a particle $\textbf{P}$:

  $dV_0=(d\textbf{X}^{(1)}\cross{d\textbf{X}^{(2)}})\cdot{d\textbf{X}^{(3)}}=$

  $=\det{\underbrace{\begin{bmatrix}dX^{(1)}_1&dX^{(1)}_2&dX^{(1)}_3\\dX^{(2)}_1&dX^{(2)}_2&dX^{(2)}_3\\dX^{(3)}_1&dX^{(3)}_2&dX^{(3)}_3\end{bmatrix}}_{[\textbf{M}]}}=|\textbf{M}|$

  $dV_t=(d\textbf{x}^{(1)}\cross{d\textbf{x}^{(2)}})\cdot{d\textbf{x}^{(3)}}=$

  $=\det{\underbrace{\begin{bmatrix}dx^{(1)}_1&dx^{(1)}_2&dx^{(1)}_3\\dx^{(2)}_1&dx^{(2)}_2&dx^{(2)}_3\\dx^{(3)}_1&dx^{(3)}_2&dx^{(3)}_3\end{bmatrix}}_{[\textbf{m}]}}=|\textbf{m}|$

  $\boxed{M_{ij}=dX^{(i)}_j\space\space\space\space\space\space\space m_{ij}=dx^{(i)}_j}$

* Consider now: $\begin{cases}d\textbf{x}^{(i)}=\textbf{F}\cdot{d\textbf{X}^{(i)}}\space\space\space\space{i\in\{1,2,3\}}\space\space\space\space\rightarrow\text{Fundamental eq. of deformation}\\dx^{(i)}_j=F_{jk}dX^{(i)}_k\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

  $M_{ij}=dX^{(i)}_j$ and $m_{ij}=dx^{(i)}_j$	$\Rightarrow$

  $m_{ij}=dx^{(i)}_j=F_{jk}dX^{(i)}_k=F_{jk}dX_{ik}=dX_{ik}F^T_{jk}$	$\Rightarrow$	$\textbf{m}=\textbf{M}\cdot\textbf{F}^T$

* Then:

  $dV_t=|\textbf{m}|=\begin{vmatrix}\textbf{M}\cdot\textbf{F}^T\end{vmatrix}=|\textbf{F}|\underbrace{|\textbf{M}|}_{dV_0}=|\textbf{F}|dV_0$	$\Rightarrow$	$\boxed{dV_t=|\textbf{F}|dV_0}$

  * And, defining $J(\textbf{X},t)$ as the jacobian of the deformation,

    $J(\textbf{X},t)=\det\textbf{F}(\textbf{X},t)>0$	$\Rightarrow$	$\boxed{dV_t=J(\textbf{X},t)\cdot{dV_0}}$

# Area Variation

## Surface Area Ratio

* Consider the variation of a differential area associated to a particle $\textbf{P}$:

  $d\textbf{A}:=dA\textbf{N}$$\rightarrow$$\text{material vector "differential of area"}$$\rightarrow$$|d\textbf{A}|=dA$

  $d\textbf{a}:=da\textbf{n}$$\rightarrow$$\text{spatial vector "differential of area"}$$\rightarrow$$|d\textbf{a}|=da$

  $dV_0=dHdA=\underbrace{d\textbf{X}^{(3)}\cdot\textbf{N}}_{dH}dA=d\textbf{X}^{(3)}\cdot\underbrace{\textbf{N}dA}_{d\textbf{A}}=d\textbf{A}\cdot{d\textbf{X}^{(3)}}$

  $dV_t=dhda=\underbrace{d\textbf{x}^{(3)}\cdot\textbf{n}}_{dh}dA=d\textbf{x}^{(3)}\cdot\underbrace{\textbf{n}da}_{d\textbf{a}}=d\textbf{a}\cdot{d\textbf{x}^{(3)}}$

* Consider now:

  $\begin{CD}dV_t=d\textbf{a}\cdot{d\textbf{x}^{(3)}}\\@VV \begin{cases}d\textbf{x}^{(3)}=\textbf{F}\cdot\textbf{X}^{(3)}\\d{V}_t=|\textbf{F}|d{V}_0\\d{V}_0=d\textbf{A}\cdot{d\textbf{X}^{(3)}}\end{cases} V\end{CD}$

  $\underbrace{dV_t}_{|\textbf{F}|d{V}_0}=|\textbf{F}|\underbrace{d\textbf{A}\cdot{\cancel{d\textbf{X}^{(3)}}}}_{d{V}_0}=\underbrace{d\textbf{a}\cdot\textbf{F}\cdot{\cancel{d\textbf{X}^{(3)}}}}_{d{V}_t}$	$\forall{d\textbf{X}^{(3)}}\Rightarrow|\textbf{F}|d\textbf{A}={d\textbf{a}\cdot\textbf{F}}$

  ​	 $\begin{CD}@VVV\end{CD}$

  $\boxed{d\textbf{a}=|\textbf{F}|\cdot\textbf{A}\cdot\textbf{F}^{-1}}$  $\underset{\begin{cases}d\textbf{A}=\textbf{N}dA\\d\textbf{a}=\textbf{n}da\end{cases}}{\longrightarrow}$  $\boxed{da\textbf{n}=|\textbf{F}|\textbf{N}\cdot\textbf{F}^{-1}dA}$ $\longrightarrow$ $\boxed{da\textbf{n}=|\textbf{F}|\norm{\textbf{N}\cdot\textbf{F}^{-1}}dA}$

# Volumetric Strain

* **Volumetric Strain**

  $\boxed{e(\textbf{X},t)\stackrel{def}{=}\dfrac{dV(\textbf{X},t)-dV(\textbf{X},t_0)}{dV(\textbf{X},t)}\stackrel{not.}{=}\dfrac{dV_t-dV_0}{dV_0}}$

  ​	$\begin{CD}@VV d{V}_t=|\textbf{F}|d{V}_0 V\end{CD}$

  $e=\dfrac{|\textbf{F}|d{V}_0-dV_0}{dV_0}$	$\longrightarrow$	$\boxed{e=|\textbf{F}|-1}$

  > ==REMARK== The incompressibility condition (null volumetric strain) takes the form
  >
  > $e=J-1=0$	$\Rightarrow$	$J=|\textbf{F}|=1$

# Infinitesimal Strain

## Infinitesimal Strain Theory

* The **infinitesimal strain theory** (also called **small strain theory**) is based on the simplifying hypotheses:

  * <u>Displacements are very small</u> w.r.t. the typical dimensions in the continuum medium,

    * As a consequence, $\norm{\textbf{u}}<<(\textit{size of }\Omega_0)$ and the **reference and deformed configurations are considered to be practically the same**, as are the material and spatial coordinates:

      $\Omega\cong\Omega_0$  and  $\begin{cases}\textbf{x}=\textbf{X}+\textbf{u}\cong\textbf{X}\\x_i=X_i+u_i\cong{X_i}\end{cases}$ $\Rightarrow$ $\begin{cases}\textbf{U}(\textbf{X},t)\stackrel{not.}{=}\textbf{u}(\textbf{X},t)\equiv\textbf{u}(\textbf{x},t)\\U_i(\textbf{X},t)\stackrel{not.}{=}u_i(\textbf{X},t)\equiv{u_i}(\textbf{x},t)\space\space\space\space{i\in\{1,2,3\}}\end{cases}$
    
  * <u>Displacement gradients are infinitesimal</u>,  $\left|\dfrac{\part{u_i}}{\part{x_j}}\right|<<1$,  $\forall{i\in\{1,2,3\}}$
  
* The material and spatial coordinates coincide, $\textbf{x}=\textbf{X}+\underset{\approx0}{\textbf{u}}\cong\textbf{X}$

  * Even though it is considered that $\textbf{u}$ cannot be neglected when calculating other properties such as the infinitesimal strain tensor $\boldsymbol{\varepsilon}$.

* There is no difference between the material and spatial differential operators:

  $\begin{cases}\overline\nabla\stackrel{symb}{=}\dfrac{\part{}}{\part{X}_i}\hat{{\textbf{e}}}_i=\dfrac{\part{}}{\part{x}_i}\hat{{\textbf{e}}}_i=\nabla\\\textbf{J}(\textbf{X},t)=\textbf{U}(\textbf{X},t)\otimes\overline\nabla=\textbf{u}(\textbf{x},t)\otimes\nabla=\textbf{U}(\textbf{X},t)\otimes\overline\nabla=\textbf{j}(\textbf{x},t)\end{cases}$

* The local an material time derivatives coincide

  $\begin{cases}\Gamma(\underbrace{\textbf{X}}_{\approx\textbf{x}},t)\approx\Gamma(\textbf{x},t)=\gamma(\textbf{x},t)=\gamma(\textbf{X},t)\\\dfrac{d\gamma}{dt}=\dfrac{\part{\gamma(\textbf{X},t)}}{\part{t}}=\dfrac{\part{\gamma(\textbf{x},t)}}{\part{t}}=\dot{\gamma}\end{cases}$

## Strain Tensors

* **Green-Lagrange strain tensor**

  $\begin{cases}\textbf{E}=\dfrac{1}{2}\left(\textbf{F}^T\textbf{F}-\textbf{1}\right)=\dfrac{1}{2}\left(\textbf{J}+\textbf{J}^T+\cancel{\textbf{J}^T\cdot\textbf{J}}\right)\\E_{ij}=\dfrac{1}{2}\left(\dfrac{\part{U}_i}{\part{X}_j}+\dfrac{\part{U}_j}{\part{X}_i}+\underbrace{\cancel{\dfrac{\part{U}_k}{\part{X}_i}\dfrac{\part{U}_k}{\part{X}_j}}}_{\left|\frac{\part{U}_k}{\part{X}_j}\right|<<1}\right)\end{cases}$ $\Rightarrow$ $\boxed{\begin{cases}\textbf{E}\cong\dfrac{1}{2}\left(\textbf{J}+\textbf{J}^T\right)=\dfrac{1}{2}\left(\textbf{j}+\textbf{j}^T\right)=\boldsymbol{\varepsilon}\\E_{ij}\cong\varepsilon_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}\right)=\varepsilon_{ij}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

* **Euler-Almansi strain tensor**

  $\begin{cases}\textbf{e}=\dfrac{1}{2}\left(\textbf{1}-\textbf{F}^{-T}\textbf{F}^{-1}\right)=\dfrac{1}{2}\left(\textbf{j}+\textbf{j}^T-\cancel{\textbf{j}^T\cdot\textbf{j}}\right)\\e_{ij}=\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}+\underbrace{\cancel{\dfrac{\part{u}_k}{\part{x}_i}\dfrac{\part{u}_k}{\part{x}_j}}}_{\left|\frac{\part{u}_k}{\part{x}_j}\right|<<1}\right)\end{cases}$ $\Rightarrow$ $\boxed{\begin{cases}\textbf{e}\cong\dfrac{1}{2}\left(\textbf{j}+\textbf{j}^T\right)=\dfrac{1}{2}\left(\textbf{J}+\textbf{J}^T\right)=\boldsymbol{\varepsilon}\\e_{ij}\cong\dfrac{1}{2}\left(\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}\right)=\varepsilon_{ij}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

* Therefore, the **infinitesimal strain tensor** is defined as:

  $\boxed{\begin{cases}\boldsymbol{\varepsilon}=\dfrac{1}{2}\left(\textbf{J}+\textbf{J}^T\right)=\dfrac{1}{2}\left(\textbf{j}+\textbf{j}^T\right)=\dfrac{1}{2}\left(\textbf{u}\otimes\nabla+\nabla\otimes\textbf{u}\right)\stackrel{not.}{=}\nabla^s\textbf{u}\\\varepsilon_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

  > ==REMARK== $\boldsymbol{\varepsilon}$ is a symmetrical tensor and its components are infinitesimal: $|\varepsilon_{ij}|<<1$, $\forall{{i,j\in\{1,2,3\}}}$

## Stretch and Unit Elongation

* Stretch in terms of the strain tensors:

  $\lambda_{\text{T}}=\sqrt{1+2\underbrace{\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}_{x}}$	$\lambda_t=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}$

  Considering that $\textbf{e}\cong\textbf{E}\cong\boldsymbol{\varepsilon}$ and that it is infinitesimal, a Taylor linear series expansion up to first order terms around $x=0$ yields:

  $\lambda_{\text{T}}=\sqrt{1+2\underbrace{\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}_{x}}\xRightarrow{\begin{matrix*}[l]\lambda(x)=\sqrt{1+2x}\\\cong\lambda(0)+\underbrace{\left.\cfrac{d\lambda}{dx}\right|_{x=0}}_{=1}x=1+x\end{matrix*}}\lambda_{\text{T}}\cong1+\textbf{T}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}$

  $\lambda_t=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}\xRightarrow{\begin{matrix*}[l]\lambda(x)=\cfrac{1}{\sqrt{1-2x}}\\\cong\lambda(0)+\underbrace{\left.\cfrac{d\lambda}{dx}\right|_{x=0}}_{=1}x=1+x\end{matrix*}}\lambda_t\cong1+\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}$

* But in infinitesimal Strain Theory, $\textbf{T}\approx\textbf{t}$. So the **linearized stretch and unit elongation** through a direction given by the unit vector $\textbf{T}\approx\textbf{t}$ are:

  $\boxed{\lambda=\dfrac{ds}{dS}\cong1+\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}\cong1+\textbf{T}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}}$	$\boxed{\varepsilon=\dfrac{ds-dS}{dS}=\lambda-1=\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}}$

## Physical Interpretation of Infinitesimal Strains

* Consider the components of the infinitesimal strain tensor, $\boldsymbol{\varepsilon}$:

  $\boldsymbol{\varepsilon}=\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&\varepsilon_{zz}\end{bmatrix}=\begin{bmatrix}\varepsilon_{11}&\varepsilon_{12}&\varepsilon_{13}\\\varepsilon_{21}&\varepsilon_{22}&\varepsilon_{23}\\\varepsilon_{31}&\varepsilon_{32}&\varepsilon_{33}\end{bmatrix}$

* For a segment parallel to the $x$-axis, the stretch and unit elongation are:

  $\textbf{T}^{(1)}\cong\textbf{t}^{(1)}\equiv\begin{Bmatrix}1\\0\\0\end{Bmatrix}$	$d\textbf{X}\cong{d\textbf{x}}\equiv\begin{Bmatrix}dS\\0\\0\end{Bmatrix}$

  $\boxed{\lambda\cong1+\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}}$

  $\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}=\begin{bmatrix}1&0&0\end{bmatrix}\cdot\begin{bmatrix}\varepsilon_{11}&\varepsilon_{12}&\varepsilon_{13}\\\varepsilon_{21}&\varepsilon_{22}&\varepsilon_{23}\\\varepsilon_{31}&\varepsilon_{32}&\varepsilon_{33}\end{bmatrix}\cdot\begin{bmatrix}1\\0\\0\end{bmatrix}=\varepsilon_{11}$

  $\lambda_1=\lambda_X=1+\varepsilon_{11}$	Stretch in the $x$-direction

  $\varepsilon_{1}=1-\lambda=\varepsilon_{11}$	Unit elongation in the $x$-direction

  $\varepsilon_{X}=1-\lambda=\varepsilon_{XX}$

* Similarly, the stretching unit elongation of the material in the $y$-direction and $z$-direction:

  $\boxed{\begin{matrix*}[l]\lambda_1=1+\varepsilon_{11}\Rightarrow\varepsilon_{x}=\lambda_x-1=\varepsilon_{xx}\\\lambda_2=1+\varepsilon_{22}\Rightarrow\varepsilon_{y}=\lambda_y-1=\varepsilon_{yy}\\\lambda_3=1+\varepsilon_{33}\Rightarrow\varepsilon_{z}=\lambda_z-1=\varepsilon_{zz}\end{matrix*}}$

* The diagonal components of the infinitesimal strain tensor are the **unit elongations** of the material when in the $x$, $y$ and $z$-directions.

  $\boldsymbol{\varepsilon}=\begin{bmatrix}\underline{\boldsymbol{\varepsilon_{xx}}}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&\underline{\boldsymbol{\varepsilon_{yy}}}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&\underline{\boldsymbol{\varepsilon_{zz}}}\end{bmatrix}$

* Consider the angle between a segment parallel to the $X$-axis and a segment parallel to the $Y$-axis, the angle is $\Theta_{XY}=\dfrac{\pi}{2}$.

* Applying: $\boxed{\theta\equiv\theta_{xy}=\dfrac{\pi}{2}-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}}$

  ​					 		$\Bigg\Downarrow$ $\begin{cases}E_{XX}=\varepsilon_{xx}\\E_{XY}=\varepsilon_{xy}\\E_{YY}=\varepsilon_{yy}\end{cases}$

  $\theta_{xy}=\dfrac{\pi}{2}-\arcsin\dfrac{2\varepsilon_{xy}}{\underbrace{{\sqrt{1+2\varepsilon_{xx}}}}_{\approx1}\underbrace{{\sqrt{1+2\varepsilon_{yy}}}}_{\approx1}}\cong\dfrac{\pi}{2}-\underbrace{\arcsin2\varepsilon_{xy}}_{\approx2\varepsilon_{xy}}=\dfrac{\pi}{2}-2\varepsilon_{xy}$

  > ==REMARK== The Taylor linear series expansion of $\arcsin$ $\text{x}$ yields
  >
  > $\arcsin(x)\cong\arcsin(0)+\left.{}\dfrac{d\arcsin}{dx}\right|_{x=0}(x)+\dots=x+O(x^2)$

  $\theta_{xy}\cong\dfrac{\pi}{2}-2\varepsilon_{xy}$

* The increment of the final angle w.r.t. its initial value:

  $\Delta\theta_{xy}=\theta_{xy}-\dfrac{\pi}{2}\cong\dfrac{\pi}{2}-2\varepsilon_{xy}-\dfrac{\pi}{2}=-2\varepsilon$

* Similarly, the increment of the final angle w.r.t. its initial value for couples of segments oriented in the direction of the coordinate axes:

  $\boxed{\begin{matrix}\varepsilon_{xy}=-\dfrac{1}{2}\Delta\theta_{xy}&;&\varepsilon_{xz}=-\dfrac{1}{2}\Delta\theta_{xz}&;\varepsilon_{yz}=-\dfrac{1}{2}\Delta\theta_{yz}\end{matrix}}$

* The non-diagonal components of the infinitesimal strain tensor are equal to the semi-decrements produced by the deformation of the angles between segments initially oriented in the $\text{x}$, $\text{y}$ and $\text{z}$-directions.

## Engineering Strains

* Using an **engineering notation**, instead of the scientific notation, the components of the infinitesimal strain tensor are

  $\boldsymbol{\varepsilon}=\overbrace{\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&\varepsilon_{zz}\end{bmatrix}}^{\text{scientific notation}}$$\equiv\overbrace{\begin{bmatrix}\varepsilon_{x}&\dfrac{1}{2}\gamma_{xy}&\dfrac{1}{2}\gamma_{xz}\\\dfrac{1}{2}\gamma_{xy}&\varepsilon_{y}&\dfrac{1}{2}\gamma_{yz}\\\dfrac{1}{2}\gamma_{xz}&\dfrac{1}{2}\gamma_{yz}&\varepsilon_{z}\end{bmatrix}}^{\text{engineering notation}}$

  where $\varepsilon_{x}$, $\varepsilon_{y}$, and $\varepsilon_{z}$ are **longitudinal strains**, $\gamma_{xy}$, $\gamma_{xz}$, and $\gamma_{yz}$ are **angular strains**.

  > ==REMARK== Positive longitudinal strains indicate increase in segment length.
  >
  > Positive angular strains indicate the corresponding angles decrease with the deformation process.

* Because of the symmetry of $\boldsymbol{\varepsilon}$, the tensor can be written as a 6-component infinitesimal strain vector, (Voigt's notation):

  $\boldsymbol{\varepsilon}\in\R^6$	$\boldsymbol{\varepsilon}\stackrel{def}{=}\begin{bmatrix}\underbrace{\varepsilon_{x},\varepsilon_{y},\varepsilon_{z},}_{\begin{matrix}\text{longitudinal}\\\text{strains}\end{matrix}}&\underbrace{\gamma_{xy},\gamma_{xz},\gamma_{yz}}_{\begin{matrix}\text{angular}\\\text{strains}\end{matrix}}\end{bmatrix}^T$

## Variation of Angles

* Consider two segments in the reference configuration with the same origin an angle $\Theta$ between them.

  $\boxed{\begin{matrix*}[l]\textbf{T}^{(1)}\approx\textbf{t}^{(1)}\\\textbf{T}^{(2)}\approx\textbf{t}^{(2)}\\\Theta\approx\theta\end{matrix*}}$

  $\boxed{\cos\theta=\dfrac{\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}}{\sqrt{1+2\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}}\sqrt{1+2\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}}}}$

  ​				$\Bigg\Downarrow$ $\begin{cases}\theta=\Theta+\Delta\theta\\\textbf{E}=\boldsymbol{\varepsilon}\end{cases}$ 

  $\cos(\Theta+\Delta\theta)=\dfrac{\textbf{T}^{(1)}\cdot[\textbf{1}+2\boldsymbol{\varepsilon}]\cdot\textbf{T}^{(2)}}{\sqrt{\underbrace{1+2\textbf{T}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(1)}}_{\approx1}}\sqrt{\underbrace{1+2\textbf{T}^{(2)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(2)}}_{\approx1}}}$

  ​							  $\Bigg\Downarrow$

  ​		  	$\cos(\Theta+\Delta\theta)=\textbf{T}^{(1)}\cdot\textbf{T}^{(2)}+2\textbf{T}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(2)}$

* $\textbf{T}^{(1)}$ and $\textbf{T}^{(2)}$ are unit vectors in the directions of the original segments, therefore, $\textbf{T}^{(1)}\cdot\textbf{T}^{(2)}=\norm{\textbf{T}^{(1)}}\norm{\textbf{T}^{(2)}}\cos\Theta=\cos\Theta$

* Also, $\cos(\Theta+\Delta\theta)=\cos\Theta\cdot\underbrace{\cos\Delta\theta}_{\approx1}-\sin\Theta\cdot\underbrace{\sin\Delta\theta}_{\approx\Delta\theta}=\cos\Theta-\sin\Theta\cdot\Delta\theta$	$\Rightarrow$

  $\cos\Theta-\sin\Theta\cdot\Delta\theta=\cos\Theta+2\textbf{T}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(2)}$	$\Rightarrow$

  $\boxed{\Delta\theta=-\dfrac{2\textbf{T}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(2)}}{\sin\Theta}=-\dfrac{2\textbf{t}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}^{(2)}}{\sin\theta}}$

  > ==REMARK== The Taylor linear series expansion of $\sin\text{x}$ and $\cos\text{x}$ yield
  >
  > $\sin(x)\cong\sin(0)+\left.{\dfrac{d\sin}{dx}}\right|_{x=0}(x)+\dots=x+O(x^2)$
  >
  > $\cos(x)\cong\cos(0)+\left.{\dfrac{d\cos}{dx}}\right|_{x=0}(x)+\dots=x+O(x^2)$

## Polar Decomposition

* **Polar decomposition** in finite-strain problems:

  $\begin{rcases*}\textbf{U}\stackrel{not.}{=}\sqrt{\textbf{F}^T\cdot\textbf{F}}\\\textbf{V}\stackrel{not.}{=}\sqrt{\textbf{F}\cdot\textbf{F}^T}\\\textbf{Q}=\textbf{F}\cdot\textbf{U}^{-1}=\textbf{V}^{-1}\cdot\textbf{F}\end{rcases*}$	$\Rightarrow$	$\textbf{F}=\underbrace{\textbf{Q}\cdot\textbf{U}}_{\begin{matrix}\text{right polar}\\\text{decomposition}\end{matrix}}=\overbrace{\textbf{V}\cdot\textbf{Q}}^{\begin{matrix}\text{left polar}\\\text{decomposition}\end{matrix}}$

  > ==REMARK== In infinitesimal Strain Theory
  >
  > $\textbf{x}\approx\textbf{X}$, therefore, $\textbf{F}=\dfrac{\part{\text{x}}}{\part{X}}\approx\textbf{1}$

* In **Infinitesimal Strain Theory**:

  $\textbf{U}=\sqrt{\textbf{F}^T\cdot\textbf{F}}=\sqrt{\left(\textbf{1}+\textbf{J}^T\right)\cdot\left(\textbf{1}+\textbf{J}\right)}=\sqrt{\textbf{1}+\textbf{J}^T+\textbf{J}+\underbrace{\textbf{J}^T\cdot\textbf{J}}_{<<\textbf{J}}}\approx\sqrt{\textbf{1}+\underbrace{\textbf{J}^T+\textbf{J}}_{=\textbf{x}}}=\textbf{1}+\underbrace{\dfrac{1}{2}(\textbf{J}^T+\textbf{J})}_{=\boldsymbol{\varepsilon}}$

  ​	$\bigg\Downarrow$

  $\boxed{\textbf{U}=\textbf{1}+\boxed{\boldsymbol{\varepsilon}}}\leftarrow(\text{infinitesimal strain tensor})$

  Similarly,

  $\textbf{U}^{-1}=(\textbf{1}+\underbrace{\varepsilon}_{=\textbf{x}})^{-1}=\textbf{1}-\boldsymbol{\varepsilon}=\textbf{1}-\underbrace{\dfrac{1}{2}(\textbf{J}^T+\textbf{J})}_{=\boldsymbol{\varepsilon}}$

  $\boxed{\textbf{U}^{-1}=\textbf{1}-\boxed{\boldsymbol{\varepsilon}}}\leftarrow(\text{infinitesimal strain tensor})$
  
  > ==REMARK== The Taylor linear series expansion of $\sqrt{1+x}$ and $(1+x)^{-1}$ yield
  >
  > $\lambda(x)=\sqrt{1+x}\cong\lambda(0)+\left.\dfrac{d\lambda}{dx}{}\right|_{x=0}x=1+\dfrac{1}{2}x+O(x^2)$
  >
  > $\lambda(x)=(1+x)^{-1}\cong\lambda(0)+\left.\dfrac{d\lambda}{dx}{}\right|_{x=0}x=1-x+O(x^2)$
  
  $\underset{\bigg\Downarrow}{\textbf{Q}=\textbf{F}\cdot\textbf{U}^{-1}}=(\textbf{1}+\textbf{J})\cdot\left[{\textbf{1}-\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)}\right]=\textbf{1}+\textbf{J}-\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)-\underbrace{\dfrac{1}{2}\textbf{J}\cdot(\textbf{J}+\textbf{J}^T)}_{<<\textbf{J}}=\textbf{1}+\underbrace{\dfrac{1}{2}(\textbf{J}-\textbf{J}^T)}_{=\Omega}$
  
  $\boxed{\textbf{Q}=\textbf{1}+\boldsymbol{\Omega}}$
  
* The **infinitesimal rotation tensor $\boldsymbol{\Omega}$** is defined:

  $\boxed{\begin{cases}\boldsymbol{\Omega}\stackrel{def}{=}\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)=\dfrac{1}{2}(\textbf{u}\otimes\nabla-\nabla\otimes\textbf{u})\stackrel{def}{=}\nabla^a\textbf{u}\\\Omega_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}}\right]<<1\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

  > ==REMARK==
  >
  > The skew-symmetrical gradient operator is defined as
  >
  > $\nabla^a(\bullet)=\dfrac{1}{2}\left[{(\bullet)\otimes\nabla-\nabla\otimes}(\bullet)\right]$

  * The diagonal terms of $\boldsymbol{\Omega}$ are zero: $[\boldsymbol{\Omega}]=\begin{bmatrix}0&\Omega_{12}&-\Omega_{31}\\-\Omega_{12}&0&\Omega_{23}\\\Omega_{31}&-\Omega_{23}&0\end{bmatrix}$

  * It can be expressed as an **infinitesimal rotation vector $\boldsymbol{\theta}_t$**

    $\boldsymbol{\theta}\equiv\begin{Bmatrix}\theta_1\\\theta_2\\\theta_3\end{Bmatrix}=\begin{Bmatrix}-\Omega_{23}\\-\Omega_{31}\\-\Omega_{12}\end{Bmatrix}=\dfrac{1}{2}\begin{Bmatrix}\dfrac{\part{u_3}}{\part{x_2}}-\dfrac{\part{u_2}}{\part{x_3}}\\\dfrac{\part{u_1}}{\part{x_3}}-\dfrac{\part{u_3}}{\part{x_1}}\\\dfrac{\part{u_2}}{\part{x_1}}-\dfrac{\part{u_1}}{\part{x_2}}\end{Bmatrix}\stackrel{def}{=}\dfrac{1}{2}\nabla\cross\textbf{u}$ (curl of $\textbf{u}$)

    > ==REMARK== $\boldsymbol{\Omega}$ is a skew-symmetric tensor and its components are infinitesimal.

* From any skew-symmetric tensor $\boldsymbol{\Omega}$, it can be extracted a vector $\boldsymbol{\theta}$ (axial vector of $\boldsymbol{\Omega}$) exhibiting the following property:

  $\boldsymbol{\theta}\cross\textbf{r}=\boldsymbol{\Omega}\cdot\textbf{r}$	$\forall\textbf{r}$

  As a consequence:

  * The resulting vector is orthogonal to $\textbf{r}$.
  * If the components of $\boldsymbol{\Omega}$ are infinitesimal, then $\boldsymbol{\theta}\cross\textbf{r}=\boldsymbol{\Omega}\cdot\textbf{r}$ is also infinitesimal
  * The vector $\textbf{r}+\boldsymbol{\Omega}\cdot\textbf{r}=\textbf{r}+\boldsymbol{\theta}\cross\textbf{r}$ can be seen as the result of applying a (infinitesimal) **rotation** (of axial vector $\boldsymbol{\theta}$) on the vector $\textbf{r}$.


**Proof of $\boldsymbol{\theta}\cross\textbf{r}=\boldsymbol{\Omega}\cdot\textbf{r}$	$\forall\textbf{r}$**

* The result of the dot product of the infinitesimal rotation tensor, $\boldsymbol{\Omega}$, and a generic vector, $\textbf{r}$, is exactly the same as the result of the cross product of the infinitesimal rotation vector, $\boldsymbol{\theta}$, and this same vector.

  $[\boldsymbol{\Omega}]=\begin{bmatrix}0&\Omega_{12}&-\Omega_{31}\\-\Omega_{12}&0&\Omega_{23}\\\Omega_{31}&-\Omega_{23}&0\end{bmatrix}$$\rightarrow$$\boldsymbol{\theta}\equiv\begin{Bmatrix}\theta_1\\\theta_2\\\theta_3\end{Bmatrix}=\begin{Bmatrix}-\Omega_{23}\\-\Omega_{31}\\-\Omega_{12}\end{Bmatrix}$$\Rightarrow$$\boldsymbol{\theta}\cross\textbf{r}=\boldsymbol{\Omega}\cdot\textbf{r}$	$\forall\textbf{r}=\begin{Bmatrix}\text{r}_1\\\text{r}_2\\\text{r}_3\end{Bmatrix}$

* Proof:

  $\boldsymbol{\theta}\cross\textbf{r}\stackrel{not.}{=}$$\begin{bmatrix}\hat{{\textbf{e}}}_1&\hat{{\textbf{e}}}_2&\hat{{\textbf{e}}}_3\\\theta_1&\theta_2&\theta_3\\\text{r}_1&\text{r}_2&\text{r}_3\end{bmatrix}=$$\begin{bmatrix}\hat{{\textbf{e}}}_1&\hat{{\textbf{e}}}_2&\hat{{\textbf{e}}}_3\\-\Omega_{23}&-\Omega_{31}&-\Omega_{12}\\\text{r}_1&\text{r}_2&\text{r}_3\end{bmatrix}=$$\begin{Bmatrix}\Omega_{12}\text{r}_2-\Omega_{31}\text{r}_3\\-\Omega_{12}\text{r}_1-\Omega_{23}\text{r}_3\\\Omega_{31}\text{r}_1-\Omega_{23}\text{r}_2\end{Bmatrix}$

  $\boldsymbol{\Omega}\cdot\textbf{r}=$$\begin{bmatrix}0&\Omega_{12}&-\Omega_{31}\\-\Omega_{12}&0&\Omega_{23}\\\Omega_{31}&-\Omega_{23}&0\end{bmatrix}\begin{Bmatrix}\text{r}_1\\\text{r}_2\\\text{r}_3\end{Bmatrix}=$$\begin{Bmatrix}\Omega_{12}\text{r}_2-\Omega_{31}\text{r}_3\\-\Omega_{12}\text{r}_1-\Omega_{23}\text{r}_3\\\Omega_{31}\text{r}_1-\Omega_{23}\text{r}_2\end{Bmatrix}$

$\blacksquare$

* Using:

  $\begin{rcases*}\textbf{J}=\textbf{F}-\textbf{1}\\\boldsymbol{\varepsilon}=\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)\\\textbf{Q}=\textbf{1}+\boldsymbol{\Omega}\end{rcases*}$ $\Rightarrow$ $\textbf{F}=\textbf{1}+\textbf{J}=$$\textbf{1}+\underbrace{\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)}_{=\boldsymbol{\varepsilon}}+\underbrace{\dfrac{1}{2}(\textbf{J}-\textbf{J}^T)}_{=\boldsymbol{\Omega}}$$\Rightarrow$$\boxed{\textbf{F}=\textbf{1}+\boldsymbol{\varepsilon}+\boldsymbol{\Omega}}$

* Consider a differential segment $d\textbf{X}$:

  $d\textbf{x}=$$\textbf{F}\cdot{d\textbf{X}}=$$(\textbf{1}+\boldsymbol{\varepsilon}+\boldsymbol{\Omega})\cdot{d\textbf{X}}=$$\overbrace{\boldsymbol{\varepsilon}\cdot{d\textbf{X}}}^{\text{stretch}}+\overbrace{(\textbf{1}+\boldsymbol{\Omega})\cdot{d\textbf{X}}}^{\text{rotation}}$	$\Rightarrow$

  $\boxed{\textbf{F}(\bull)\equiv\text{stretching}(\bull)+\text{rotation}(\bull)}$

  > ==REMARK== The infinitesimal rotation tensor characterizes the rotation and, in the small-strain context, maintains angles and distances.

## Volumetric Deformation

* The **volumetric strain**:

  $\boxed{e=|\textbf{F}|-1}$

* Considering: $\textbf{F}=\textbf{Q}\cdot\textbf{U}$ and $\textbf{U}=\textbf{1}+\boldsymbol{\varepsilon}$

  ​					   $\bigg\Downarrow$

  $|\textbf{F}|=|\textbf{Q}||\textbf{U}|=|\textbf{U}|=|\textbf{1}+\boldsymbol{\varepsilon}|=\det{\begin{vmatrix}1+\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&1+\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&1+\varepsilon_{zz}\end{vmatrix}}=$

  $=1+\underset{=Tr(\boldsymbol{\varepsilon})}{\boxed{\varepsilon_{xx}+\varepsilon_{yy}+\varepsilon_{zz}}}+O(\varepsilon^2)\approx1+Tr(\boldsymbol{\varepsilon})$

  ​							  $\bigg\Downarrow$

  ​			 			 $\boxed{e=Tr(\boldsymbol{\varepsilon})}$

# Strain Rate

## Spatial Velocity Gradient Tensor

* Consider the relative velocity between two points in space at a give (current) instant:

  $\begin{cases}\textbf{v}_{P^\prime}=\textbf{v}(\textbf{x},t)=\textbf{v}(x_1,x_2,x_3,t)\\d\textbf{v}(\textbf{x},t)=\textbf{v}_{Q^\prime}-\textbf{v}_{P^\prime}=\textbf{v}(\textbf{x}+d\textbf{x},t)-\textbf{v}(\textbf{x},t)\end{cases}$	$\Rightarrow$

  $\begin{cases}d\textbf{v}=\dfrac{\part{\textbf{v}}}{\underbrace{\part{\textbf{x}}}_{\mathbfit{l}}}\cdot{d\textbf{x}}=\mathbfit{l}\cdot{d\textbf{x}}\\d\text{v}_i=\dfrac{\part{\text{v}_i}}{\underbrace{\part{\text{x}_j}}_{\mathit{l}_{ij}}}\cdot{d\text{x}_j}=\mathit{l}_{ij}\cdot{d\text{x}_{j}}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$

  Spatial velocity gradient tensor:

  $\boxed{\begin{cases}\mathbfit{l}(\textbf{x},t)\stackrel{def}{=}\dfrac{\part\textbf{v}(\textbf{x},t)}{\part\textbf{x}}=\textbf{v}\otimes\nabla\\l_{ij}=\dfrac{\part{\text{v}_i}}{\part\text{x}_j}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

## Strain Rate and Rotation Rate (or Spin) Tensors

* The spatial velocity gradient tensor can be split into a symmetrical and a skew-symmetrical tensor:

  $\begin{cases}\mathbfit{l}(\textbf{x},t)\stackrel{def}{=}\dfrac{\part\textbf{v}(\textbf{x},t)}{\part\textbf{x}}=\textbf{v}\otimes\nabla\\l_{ij}=\dfrac{\part{\text{v}_i}}{\part\text{x}_j}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}$	$\Rightarrow$	$\boxed{\textbf{l}=\text{sym}[\textbf{l}]+\text{skew}[\textbf{l}]:=\textbf{d}+\textbf{w}}$

* **Strain Rate Tensor**

  $\textbf{d}\stackrel{def}{=}sym(\mathbfit{l})=\dfrac{1}{2}(\mathbfit{l}+\mathbfit{l}^T)=\dfrac{1}{2}(\textbf{v}\otimes\nabla+\nabla\otimes\textbf{v})\stackrel{not.}{=}\nabla^s\otimes\textbf{v}$

  $\text{d}_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{\text{v}_i}}{\part\text{x}_j}+\dfrac{\part{\text{v}_j}}{\part\text{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}$

  $[\textbf{d}]=\begin{bmatrix}\text{d}_{11}&\text{d}_{12}&\text{d}_{13}\\\text{d}_{21}&\text{d}_{22}&\text{d}_{23}\\\text{d}_{31}&\text{d}_{32}&\text{d}_{33}\end{bmatrix}$

* **Rotation Rate or Spin Tensor**

  $\textbf{w}\stackrel{def}{=}sym(\mathbfit{l})=\dfrac{1}{2}(\mathbfit{l}-\mathbfit{l}^T)=\dfrac{1}{2}(\textbf{v}\otimes\nabla-\nabla\otimes\textbf{v})\stackrel{not.}{=}\nabla^a\otimes\textbf{v}$

  $\text{w}_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{\text{v}_i}}{\part\text{x}_j}-\dfrac{\part{\text{v}_j}}{\part\text{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}$

  $[\textbf{w}]=\begin{bmatrix}0&\text{w}_{12}&-\text{w}_{31}\\-\text{w}_{12}&0&\text{w}_{23}\\\text{w}_{31}&-\text{w}_{23}&0\end{bmatrix}$

## Physical Interpretation of $\textbf{d}$

* The **strain rate** measures the rate of deformation of the square of the differential length $ds$ in the spatial configuration,

  $\dfrac{d}{dt}(ds(t))^2=$$\dfrac{d}{dt}(d\textbf{x}\cdot{d\textbf{x}})=$$\dfrac{d}{dt}(d\textbf{x})\cdot{d\textbf{x}}+d\textbf{x}\cdot\dfrac{d}{dt}(d\textbf{x})=$$d\underset{=\textbf{v}}{\left({\dfrac{d\textbf{x}}{dt}}\right)}\cdot{d\textbf{x}}+d\textbf{x}\cdot{d}\underset{=\textbf{v}}{\left({\dfrac{d\textbf{x}}{dt}}\right)}=$$d\textbf{v}\cdot{d}\textbf{x}+d\textbf{x}\cdot{d}\textbf{v}$

  ​	$\Bigg\Downarrow$ $\begin{cases}d\textbf{v}=\mathbfit{l}\cdot{d}\textbf{x}\\\textbf{d}=\dfrac{1}{2}(\mathbfit{l}+\mathbfit{l}^T)\end{cases}$

  $\dfrac{d}{dt}(ds(t))^2=$$\underbrace{({d}\textbf{x}\cdot\mathbfit{l}^T)}_{[d\textbf{v}]^T}\cdot{d}\textbf{x}+{d}\textbf{x}\cdot\underbrace{(\mathbfit{l}\cdot{d}\textbf{x})}_{[d\textbf{v}]}=$${d}\textbf{x}\cdot\underset{=2\textbf{d}}{\left[{\mathbfit{l}^T+\mathbfit{l}}\right]}\cdot{d}\textbf{x}=$$\boxed{2{d}\textbf{x}\cdot\textbf{d}\cdot{d}\textbf{x}}$

* Differentiating w.r.t. time the expression $(ds(t))^2-(dS)^2=2{d}\textbf{X}\cdot\textbf{E}\cdot{d}\textbf{X}=$

  $\dfrac{d}{dt}(\underbrace{(ds(t))^2-\underbrace{(dS)^2}_{\text{constant}}}_{2{d}\textbf{X}\cdot\textbf{E}(\textbf{X},t)\cdot{d}\textbf{X}})=$$\dfrac{d}{dt}(2{d}\textbf{X}\cdot\textbf{E}(\textbf{X},t)\cdot{d}\textbf{X})=$$\boxed{2{d}\textbf{X}\cdot\underset{\stackrel{not.}{=}\dot{\textbf{E}}}{\dfrac{d\textbf{E}}{dt}}\cdot{d}\textbf{X}}=$$\dfrac{d}{dt}((ds(t))^2)$	$\Rightarrow$

  ${d}\textbf{X}\cdot\dot{\textbf{E}}\cdot{d}\textbf{X}=$${d}\textbf{x}\cdot\textbf{d}\cdot{d}\textbf{x}$

     		$\bigg\Downarrow$ ${d}\textbf{x}=\textbf{F}\cdot{d}\textbf{X}$

  ${d}\textbf{X}\cdot\dot{\textbf{E}}\cdot{d}\textbf{X}=$${d}\textbf{x}\cdot\textbf{d}\cdot{d}\textbf{x}=$$\underset{\textbf{F}\cdot{d}\textbf{X}}{[{d}\textbf{x}]}^T[\textbf{d}]\underset{\textbf{F}\cdot{d}\textbf{X}}{[{d}\textbf{x}]}=$$\underset{[{d}\textbf{X}]^T[\textbf{F}]^T}{[\textbf{F}\cdot{d}\textbf{X}]}^T[\textbf{d}]\underset{[\textbf{F}][{d}\textbf{X}]}{[\textbf{F}\cdot{d}\textbf{X}]}=$${d}\textbf{X}\cdot(\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F})\cdot{d}\textbf{X}$

* And, rearranging terms:

  ${d}\textbf{X}\cdot\left[\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}-\dot{\textbf{E}}\right]\cdot{d}\textbf{X}=0$  $\forall{d}\textbf{X}$ $\Rightarrow$ $\left[\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}-\dot{\textbf{E}}\right]=0$ $\Rightarrow$ $\boxed{\dot{\textbf{E}}=\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}}$

  * There is a direct relation between the material derivative of the material strain tensor and the strain rate tensor but they are not the same.
  * $\dot{\textbf{E}}$ and $\textbf{d}$ will coincide when in the reference configuration $\left.{\textbf{F}}\right|_{t=0}=\textbf{1}$.

  > ==REMARK== Given a 2^nd^ order tensor $\textbf{A}$, if $\textbf{x}\cdot\textbf{A}\cdot\textbf{x}=\textbf{0}$ for any vector $\textbf{x}\neq\textbf{0}$ then $\textbf{A}=\textbf{0}$

## Physical Interpretation of $\textbf{w}$

* To determine the (skew-symmetric) rotation rate (spin) tensor only three different components are needed:

  $\text{w}_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{\text{v}_i}}{\part\text{x}_j}-\dfrac{\part{\text{v}_j}}{\part\text{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}$	$[\textbf{w}]=\begin{bmatrix}0&\text{w}_{12}&-\text{w}_{31}\\-\text{w}_{12}&0&\text{w}_{23}\\\text{w}_{31}&-\text{w}_{23}&0\end{bmatrix}$

* The **spin vector** (axial vector $[\textbf{w}]$) of can be extracted:

  $\boldsymbol{\omega}=$$\dfrac{1}{2}rot(\textbf{v})=$$\dfrac{1}{2}\nabla\cross\textbf{v}\equiv$$\dfrac{1}{2}\begin{bmatrix}\dfrac{\part{\text{v}_3}}{\part{x_2}}-\dfrac{\part{\text{v}_2}}{\part{x_3}}\\\dfrac{\part{\text{v}_1}}{\part{x_3}}-\dfrac{\part{\text{v}_3}}{\part{x_1}}\\\dfrac{\part{\text{v}_2}}{\part{x_1}}-\dfrac{\part{\text{v}_1}}{\part{x_2}}\end{bmatrix}=$$\begin{bmatrix}-\text{w}_{23}\\-\text{w}_{31}\\-\text{w}_{12}\end{bmatrix}=$$\begin{bmatrix}\omega_1\\\omega_2\\\omega_3\end{bmatrix}$	$[\textbf{w}]=\begin{bmatrix}0&-\omega_3&\omega_2\\\omega_3&0&-\omega_1\\-\omega_2&\omega_1&0\end{bmatrix}$

* The vector $2\boldsymbol{\omega}=\nabla\cross\textbf{v}$ is named **vorticity vector**.

* It can be proven that the equality $\boldsymbol{\omega}\cross\textbf{r}=\textbf{w}\cdot\textbf{r}$  $\forall\textbf{r}$ holds true.

  Therefore:

  * If $\boldsymbol{\omega}$ is the angular velocity of a rotation movement.
  * $\boldsymbol{\omega}\cross\textbf{r}=\textbf{w}\cdot\textbf{r}$ is the rotation velocity of the point that has $\textbf{r}$ as its position vector w.r.t. the rotation center.

* Consider now the relative velocity $d\textbf{v}$,

  $\begin{rcases*}d\textbf{v}=\mathbfit{l}\cdot{d}\textbf{x}\\\mathbfit{l}=\textbf{d}+\textbf{w}\end{rcases*}$	$\Rightarrow$	$\boxed{d\textbf{v}=\textbf{d}\cdot{d}\textbf{x}+\textbf{w}\cdot{d}\textbf{x}}$

  where $\textbf{d}\cdot{d}\textbf{x}$ is the **stretch velocity**, and $\textbf{w}\cdot{d}\textbf{x}$ ($=\boldsymbol{\omega}\cross{d}\textbf{x}$) is the **rotation velocity**

# Material Time Derivative

## Deformation Gradient Tensor $\textbf{F}$

* The material time derivative of the **deformation gradient tensor**,

  $F_{ij}(\textbf{X},t)=\dfrac{\part{x_{i}(\textbf{X},t)}}{\part{X}_{j}}$	$i,j\in\{1,2,3\}$

  ​			  $\bigg\Downarrow$ $\dfrac{d}{dt}$

  $\dfrac{dF_{ij}}{dt}=$$\dfrac{\part{}}{\part{t}}\dfrac{\part{x_{i}(\textbf{X},t)}}{\part{X}_{j}}=$$\dfrac{\part{}}{\part{X}_{j}}\underset{=V_i(\textbf{X},t)}{\boxed{\dfrac{\part{x_{i}(\textbf{X},t)}}{\part{t}}}}=$$\dfrac{\part{V_i(\textbf{X},t)}}{\part{X}_{j}}=$$\underset{=\mathbfit{l}_{ik}}{\boxed{\dfrac{\part{\text{v}_i(\textbf{x}(\textbf{X},t))}}{\part{x}_{k}}}}\underset{=F_{kj}}{\boxed{\dfrac{\part{\textbf{x}_k}}{\part{X_j}}}}=$$\mathbfit{l}_{ik}F_{kj}$

  ​			  $\bigg\Downarrow$

  $\boxed{\begin{cases}\dfrac{d\textbf{F}}{dt}\stackrel{not.}{=}\dot{\textbf{F}}=\mathbfit{l}\cdot\textbf{F}\\\dfrac{dF_{ij}}{dt}=\dot{F}_{ij}=\mathbfit{l}_{ik}F_{kj}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

## Inverse Deformation Gradient Tensor $\textbf{F}^{-1}$

* The material time derivative of the **inverse deformation gradient tensor**,

  $\textbf{F}\cdot\textbf{F}^{-1}=\textbf{1}$

  ​	$\bigg\Downarrow$ $\dfrac{d}{dt}$

  $\dfrac{d}{dt}(\textbf{F}\cdot\textbf{F}^{-1})=$$\dfrac{d\textbf{F}}{dt}\cdot\textbf{F}^{-1}+\textbf{F}\cdot\dfrac{d(\textbf{F}^{-1})}{dt}=\textbf{0}$

  $\Rightarrow$ $\textbf{F}\cdot\dfrac{d(\textbf{F}^{-1})}{dt}=-\dfrac{d\textbf{F}}{dt}\cdot\textbf{F}^{-1}=-\dot{\textbf{F}}\cdot\textbf{F}^{-1}$

  Rearranging terms,

  $\dfrac{d(\textbf{F}^{-1})}{dt}=$$-\textbf{F}^{-1}\cdot\underset{=\mathbfit{l}\cdot\textbf{F}}{\boxed{\dot{\textbf{F}}}}\cdot\textbf{F}^{-1}=$$-\textbf{F}^{-1}\cdot\mathbfit{l}\cdot\underset{=\textbf{1}}{\boxed{\textbf{F}\cdot\textbf{F}^{-1}}}=$$-\textbf{F}^{-1}\cdot\mathbfit{l}$

  ​	$\bigg\Downarrow$

  $\boxed{\begin{cases}\dfrac{d(\textbf{F}^{-1})}{dt}=-\textbf{F}^{-1}\cdot\mathbfit{l}\\\dfrac{dF^{-1}_{ij}}{dt}=-\textbf{F}^{-1}_{ik}\cdot\mathbfit{l}_{kj}\space\space\space\space{i,j\in\{1,2,3\}}\end{cases}}$

## Strain Tensor $\textbf{E}$

* The material time derivative of the **material strain tensor** has already been derived for the physical interpretation of the deformation rate tensor:

  $\boxed{\dot{\textbf{E}}=\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}}$

  ​	$\Bigg\Downarrow$ $\dfrac{d}{dt}$		  	$\underbrace{\begin{matrix*}[l]\dot{\textbf{F}}=\mathbfit{l}\cdot\textbf{F}\\\dot{\textbf{F}}^T=\textbf{F}^T\cdot\mathbfit{l}^T\end{matrix*}}$

  $\dfrac{d\textbf{E}}{dt}=\dot{\textbf{E}}=$$\dfrac{1}{2}\left({\dot{\textbf{F}}^T\cdot\textbf{F}+\textbf{F}^T\cdot\dot{\textbf{F}}}\right)=$$\dfrac{1}{2}\left({\textbf{F}^T\cdot\mathbfit{l}^T\cdot\textbf{F}+\textbf{F}^T\cdot\mathbfit{l}\cdot\textbf{F}}\right)=$$\textbf{F}^T\cdot\underbrace{\dfrac{1}{2}\left({\mathbfit{l}+\mathbfit{l}^T}\right)}_{\textbf{d}}\cdot\textbf{F}=$$\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}$

  ​	$\bigg\Downarrow$

  $\boxed{\dot{\textbf{E}}=\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}}$

## Strain Tensor $\textbf{e}$

* The material time derivative of **spatial strain tensor**,

  $\textbf{e}=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})$

  ​	$\bigg\Downarrow$ $\dfrac{d}{dt}$			  	$\underbrace{\begin{matrix*}[l]\dot{\textbf{F}}^{-1}=\textbf{F}^{-1}\cdot\mathbfit{l}\\\dot{\textbf{F}}^{-T}=\mathbfit{l}^{T}\cdot\textbf{F}^{-T}\end{matrix*}}$

  $\dfrac{d\textbf{e}}{dt}=\dot{\textbf{e}}=$$\dfrac{1}{2}\left({\dot{\textbf{F}}^{-T}}\cdot\textbf{F}^{-1}+\textbf{F}^{-T}\cdot\dot{\textbf{F}}^{-1}\right)=$$\dfrac{1}{2}\left({\mathbfit{l}^{T}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}+\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot\mathbfit{l}}\right)$

  ​	$\bigg\Downarrow$

  $\boxed{\dot{\textbf{e}}=\dfrac{1}{2}\left({\mathbfit{l}^{T}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}+\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot\mathbfit{l}}\right)}$

## Volume differential $dV$

* The material time derivative of the **volume differential** associated to a given particle,

  $\boxed{dV(\textbf{x}(\textbf{X},t),t)=|\textbf{F}(\textbf{X},t)|dV_0(\textbf{X})}$
  
  ​			 $\bigg\Downarrow$ $\dfrac{d}{dt}$
  
  $\dfrac{d}{dt}dV(t)=\dfrac{\part{|\textbf{F}(\textbf{X},t)|}}{\part{t}}dV_0=\dfrac{d}{dt}|\textbf{F}|dV_0$
  
  > The material time derivative of the determinant of the **deformation gradient tensor** is:
  >
  > ​	For a 2^nd^ order tensor $\textbf{A}$:
  >
  > ​	$\left[{\dfrac{d|\textbf{A}|}{d\textbf{A}}}\right]_{ij}=\dfrac{d|\textbf{A}|}{dA_{ij}}=|\textbf{A}|\cdot\textbf{A}^{-1}_{ij}$
  >
  > $\dfrac{d|\textbf{F}|}{dt}=\dfrac{d|\textbf{F}|}{dF_{ij}}\dfrac{dF_{ij}}{dt}=|\textbf{F}|F^{-1}_{ij}\underbrace{\dfrac{dF_{ij}}{dt}}_{l_{ik}F_{kj}}=|\textbf{F}|\underbrace{F_{kj}F^{-1}_{ji}}_{(\textbf{F}\cdot\textbf{F}^{-1})_{ki}-\delta_{ki}}\mathbfit{l}_{ik}$
  >
  > $=|\textbf{F}|\mathbfit{l}_{ii}=|\textbf{F}|\underbrace{\dfrac{\part{\text{v}_i}}{\part{x_i}}}_{\nabla\cdot\textbf{v}}=|\textbf{F}|\nabla\cdot\textbf{v}$ $\Rightarrow$ $\boxed{\dfrac{d|\textbf{F}|}{dt}=|\textbf{F}|\nabla\cdot\textbf{v}=(\nabla\cdot\textbf{v})|\textbf{F}|}$
  
  ​			 $\bigg\Downarrow$
  
  $\dfrac{d}{dt}(dV)=(\nabla\cdot\textbf{v})\underset{=dV}{|\textbf{F}|dV_0}$
  
  ​			 $\bigg\Downarrow$
  
  $\boxed{\dfrac{d}{dt}(dV(\textbf{x},t))=\nabla\cdot\textbf{v}(\textbf{x},t)dV(\textbf{x},t)}$
  

# Other Coordinate Systems

## Cylindrical Coordinate System

$\textbf{x}(r,\theta,z)\equiv\begin{cases}x=r\cos\theta\\y=r\sin\theta\\z=z\end{cases}$

$\dfrac{\part{\hat{{\textbf{e}}}_r}}{\part{\theta}}=\hat{{\textbf{e}}}_\theta$	$\dfrac{\part{\hat{{\textbf{e}}}_\theta}}{\part{\theta}}=\hat{{\textbf{e}}}_r$

$dV=r\space{d\theta}\space{dz}$

## Spherical Coordinate System

$\textbf{x}(r,\theta,\varphi)\equiv\begin{cases}x=r\sin\theta\cos\varphi\\y=r\sin\theta\sin\varphi\\z=\cos\theta\end{cases}$

$\dfrac{\part{\hat{{\textbf{e}}}_r}}{\part{\theta}}=\hat{{\textbf{e}}}_\theta$	$\dfrac{\part{\hat{{\textbf{e}}}_\theta}}{\part{\theta}}=-\hat{{\textbf{e}}}_r$	$\dfrac{\part{\hat{{\textbf{e}}}_\phi}}{\part{\theta}}=\textbf{0}$

$dV=r^2\sin\theta\space{dr}\space{d\theta}\space{d\phi}$







