## Ch2: Deformation and Strain

$\Omega_0$: non-deformed (or reference) configuration, at reference time $t_0$.

$X$: Position vector of a particle at reference time.

$\Omega$ or $\Omega_t$: deformed (or present) configuration, at present time $t$.

$x$: Position vector of a particle at present time.

$\textbf{F}(\textbf{X},t)$: (material) deformation gradient tensor

* $[\textbf{F}]=[\textbf{x}\otimes\overline{\nabla}]=\overbrace{\begin{bmatrix}\text{x}_1\\\text{x}_2\\\text{x}_3\end{bmatrix}}^{=[\textbf{x}]}\overbrace{\begin{bmatrix}\dfrac{\partial}{\partial{X_1}}&\dfrac{\partial}{\partial{X_2}}&\dfrac{\partial}{\partial{X_3}}\end{bmatrix}}^{=[\overline{\nabla}]^T}=\begin{bmatrix}\dfrac{\part{x_1}}{\part{X_1}}&\dfrac{\part{x_1}}{\part{X_2}}&\dfrac{\part{x_1}}{\part{X_3}}\\\dfrac{\part{x_2}}{\part{X_1}}&\dfrac{\part{x_2}}{\part{X_2}}&\dfrac{\part{x_2}}{\part{X_3}}\\\dfrac{\part{x_3}}{\part{X_1}}&\dfrac{\part{x_3}}{\part{X_2}}&\dfrac{\part{x_3}}{\part{X_3}}\end{bmatrix}$
* $\textbf{x}=\textbf{F}\cdot{\textbf{X}}$

$\textbf{F}^{-1}(\textbf{x},t)$: spatial (or inverse) deformation gradient tensor

* $[\textbf{F}^{-1}]=[\textbf{X}\otimes\nabla]=\overbrace{\begin{bmatrix}\text{X}_1\\\text{X}_2\\\text{X}_3\end{bmatrix}}^{=[\textbf{X}]}\overbrace{\begin{bmatrix}\dfrac{\partial}{\partial{x_1}}&\dfrac{\partial}{\partial{x_2}}&\dfrac{\partial}{\partial{x_3}}\end{bmatrix}}^{=[\nabla]^T}=\begin{bmatrix}\dfrac{\part{X_1}}{\part{x_1}}&\dfrac{\part{X_1}}{\part{x_2}}&\dfrac{\part{X_1}}{\part{x_3}}\\\dfrac{\part{X_2}}{\part{x_1}}&\dfrac{\part{X_2}}{\part{x_2}}&\dfrac{\part{X_2}}{\part{x_3}}\\\dfrac{\part{X_3}}{\part{x_1}}&\dfrac{\part{X_3}}{\part{x_2}}&\dfrac{\part{X_3}}{\part{x_3}}\end{bmatrix}$
* $\textbf{X}=\textbf{F}^{-1}\cdot{\textbf{x}}$
* $\textbf{F}\cdot\textbf{F}^{-1}=\textbf{1}$

$\textbf{U}(\textbf{X},t)$: Material description Displacement vector

* $\textbf{U}(\textbf{X},t)=\textbf{x}(\textbf{X},t)-\textbf{X}$

$\textbf{u}(\textbf{x},t)$: Spatial description Displacement vector

* $\textbf{u}(\textbf{x},t)=\textbf{x}-\textbf{X}(\textbf{x},t)$

$\textbf{J}$: Material Displacement Gradient Tensor

* $\textbf{J}\stackrel{def}{=}\textbf{U}(\textbf{X},t)\otimes\overline\nabla=\textbf{F}-\textbf{1}$

$\textbf{j}$: Spatial Displacement Gradient Tensor

* $\textbf{j}\stackrel{def}{=}\textbf{u}(\textbf{x},t)\otimes\nabla=\textbf{1}-\textbf{F}^{-1}$

$d\textbf{X}$: difference of two points in material configuration ($\mathbf{Q}-\mathbf{P}$)

$d\textbf{x}$: difference of two points in spatial configuration ($\mathbf{Q}^\prime-\mathbf{P}^\prime$)

$\textbf{T}$: unit direction vector of $d\textbf{X}$

$\textbf{t}$: unit direction vector of $d\textbf{x}$

$dS$: length of segment $d\textbf{X}$

* $dS=\sqrt{d\textbf{X}\cdot{d\textbf{X}}}$
* $(dS)^2=d\textbf{X}\cdot{d\textbf{X}}$
* $(dS)^2=d\textbf{x}\cdot\textbf{F}^{-T}\cdot\textbf{F}^{-1}\cdot{d\textbf{x}}$
* $d\textbf{X}=\textbf{T}dS$

$ds$: length of segment $d\textbf{x}$

* $ds=\sqrt{d\textbf{x}\cdot{d\textbf{x}}}$
* $(ds)^2=d\textbf{x}\cdot{d\textbf{x}}$
* $(ds)^2=d\textbf{X}\cdot\textbf{F}^T\cdot\textbf{F}\cdot{d\textbf{X}}$
* $d\textbf{x}=\textbf{t}ds$

$\textbf{E}(\textbf{X},t)$: Green-Lagrange (Material) Strain Tensor

* $\textbf{E}(\textbf{X},t)=\dfrac{1}{2}(\textbf{F}^T\cdot\textbf{F}-\textbf{1})$
* $(ds)^2-(dS)^2=2d\textbf{X}\cdot\textbf{E}\cdot{d\textbf{X}}$
* $\textbf{E}=\dfrac{1}{2}\left[\textbf{J}+\textbf{J}^T+\textbf{J}^T\cdot\textbf{J}\right]$$=\dfrac{1}{2}\left[{\dfrac{\part{U}_i}{\part{X}_j}+\dfrac{\part{U}_j}{\part{X}_i}+\dfrac{\part{U}_k}{\part{X}_i}\dfrac{\part{U}_k}{\part{X}_j}}\right]$

$\textbf{e}(\textbf{x},t)$: Euler-Almansi (Spatial) Strain Tensor

* $\textbf{e}(\textbf{x},t)=\dfrac{1}{2}(\textbf{1}-\textbf{F}^{-T}\cdot\textbf{F}^{-1})$
* $(ds)^2-(dS)^2=2d\textbf{x}\cdot\textbf{e}\cdot{d\textbf{x}}$
* $\textbf{e}=\dfrac{1}{2}\left[\textbf{j}+\textbf{j}^T-\textbf{j}^T\cdot\textbf{j}\right]$

$\lambda$: stretch ratio or stretch:

* $\lambda=\lambda_T=\lambda_t=\dfrac{ds}{dS}$
  * $ds=\lambda{dS}$
  * $dS=\lambda^{-1}ds$
* $\lambda=\sqrt{1+2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}$
* $\lambda=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}$
* $\lambda^{-1}(\textbf{x},t)=\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}$

$\varepsilon$: extension or unit elongation:

* $\varepsilon=\varepsilon_\textbf{T}=\varepsilon_\textbf{t}=\dfrac{ds-dS}{dS}$
* $\varepsilon=\lambda-1$
* $\varepsilon=\sqrt{1+2\textbf{T}\cdot\textbf{E}\cdot\textbf{T}}-1$
* $\varepsilon=\lambda-1=\dfrac{1}{\sqrt{1-2\textbf{t}\cdot\textbf{e}\cdot\textbf{t}}}-1$

$\cos\Theta$: angle between particle ($\mathbf{P}$) and other two particles ($\mathbf{Q}$ and $\mathbf{R}$) in initial state

* $\cos\theta=\dfrac{\textbf{T}^{(1)}\cdot(\textbf{1}+2\textbf{E})\cdot\textbf{T}^{(2)}}{\sqrt{1+2\textbf{T}^{(1)}\cdot\textbf{E}\cdot\textbf{T}^{(1)}}\sqrt{1+2\textbf{T}^{(2)}\cdot\textbf{E}\cdot\textbf{T}^{(2)}}}$

$\cos\theta$: angle between particle ($\mathbf{P}^\prime$) and other two particles ($\mathbf{Q}^\prime$ and $\mathbf{R}^\prime$) in time $t$

* $\cos\Theta=\dfrac{\textbf{t}^{(1)}\cdot(\textbf{1}-2\textbf{e})\cdot\textbf{t}^{(2)}}{\sqrt{1-2\textbf{t}^{(1)}\cdot\textbf{e}\cdot\textbf{t}^{(1)}}\sqrt{1-2\textbf{t}^{(2)}\cdot\textbf{e}\cdot\textbf{t}^{(2)}}}$

Physical Interpretation of $\textbf{E}(\textbf{X},t)$:

* $\lambda_X$ (stretch in $X$-direction): $\lambda_X=\sqrt{1+2E_{XX}}$
* $\lambda_Y$ (stretch in $Y$-direction): $\lambda_Y=\sqrt{1+2E_{YY}}$
* $\lambda_Z$ (stretch in $Z$-direction): $\lambda_Z=\sqrt{1+2E_{ZZ}}$
* $\varepsilon_X$ (unit elongation in $X$-direction): $\varepsilon_X=\lambda_X-1=\sqrt{1+2E_{XX}}-1$
* $\varepsilon_Y$ (unit elongation in $Y$-direction): $\varepsilon_Y=\lambda_Y-1=\sqrt{1+2E_{YY}}-1$
* $\varepsilon_Z$ (unit elongation in $Z$-direction): $\varepsilon_Z=\lambda_Z-1=\sqrt{1+2E_{ZZ}}-1$
* $\theta_{xy}$ (angle between the $X$- and $Y$-directions at time $t$): $\theta_{xy}=\dfrac{\pi}{2}-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}$
* $\theta_{xz}$ (angle between the $X$- and $Z$-directions at time $t$): $\theta_{xz}=\dfrac{\pi}{2}-\arcsin\dfrac{2E_{XZ}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{ZZ}}}$
* $\theta_{yz}$ (angle between the $Y$- and $Z$-directions at time $t$): $\theta_{yz}=\dfrac{\pi}{2}-\arcsin\dfrac{2E_{YZ}}{\sqrt{1+2E_{YY}}\sqrt{1+2E_{ZZ}}}$
* $\Delta\Theta_{XY}$ (the increment of the final angle w.r.t its initial value in the $X$- and $Y$-directions): $\Delta\Theta_{XY}=-\arcsin\dfrac{2E_{XY}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{YY}}}$
* $\Delta\Theta_{XZ}$ (the increment of the final angle w.r.t its initial value in the $X$- and $Z$-directions): $\Delta\Theta_{XZ}=-\arcsin\dfrac{2E_{XZ}}{\sqrt{1+2E_{XX}}\sqrt{1+2E_{ZZ}}}$
* $\Delta\Theta_{YZ}$ (the increment of the final angle w.r.t its initial value in the $Y$- and $Z$-directions): $\Delta\Theta_{YZ}=-\arcsin\dfrac{2E_{YZ}}{\sqrt{1+2E_{YY}}\sqrt{1+2E_{ZZ}}}$

Physical Interpretation of $\textbf{e}(\textbf{x},t)$:

* $\lambda_x$ (stretch in $x$-direction): $\lambda_x=\dfrac{1}{\sqrt{1-2e_{xx}}}$
* $\lambda_y$ (stretch in $y$-direction): $\lambda_y=\dfrac{1}{\sqrt{1-2e_{yy}}}$
* $\lambda_z$ (stretch in $z$-direction): $\lambda_z=\dfrac{1}{\sqrt{1-2e_{zz}}}$
* $\varepsilon_x$ (unit elongation in $x$-direction): $\varepsilon_x=\dfrac{1}{\sqrt{1-2e_{xx}}}-1$
* $\varepsilon_y$ (unit elongation in $y$-direction): $\varepsilon_y=\dfrac{1}{\sqrt{1-2e_{yy}}}-1$
* $\varepsilon_z$ (unit elongation in $z$-direction): $\varepsilon_z=\dfrac{1}{\sqrt{1-2e_{zz}}}-1$
* $\Theta_{xy}$ (angle between the $x$- and $y$-directions at time 0): $\Theta_{xy}=\dfrac{\pi}{2}+\arcsin\dfrac{2e_{xy}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{yy}}}$
* $\Theta_{xz}$ (angle between the $x$- and $z$-directions at time 0): $\Theta_{xz}=\dfrac{\pi}{2}+\arcsin\dfrac{2e_{xz}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{zz}}}$
* $\Theta_{yz}$ (angle between the $y$- and $z$-directions at time 0): $\Theta_{yz}=\dfrac{\pi}{2}+\arcsin\dfrac{2e_{yz}}{\sqrt{1-2e_{yy}}\sqrt{1-2e_{zz}}}$
* $\Delta\theta_{xy}$ (the increment of the final angle w.r.t its initial value in the $x$- and $y$-directions): $\Delta\theta_{xy}=-\arcsin\dfrac{2e_{xy}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{yy}}}$
* $\Delta\theta_{xz}$ (the increment of the final angle w.r.t its initial value in the $x$- and $z$-directions): $\Delta\theta_{xz}=-\arcsin\dfrac{2e_{xz}}{\sqrt{1-2e_{xx}}\sqrt{1-2e_{zz}}}$
* $\Delta\theta_{yz}$ (the increment of the final angle w.r.t its initial value in the $y$- and $z$-directions): $\Delta\theta_{yz}=-\arcsin\dfrac{2e_{yz}}{\sqrt{1-2e_{yy}}\sqrt{1-2e_{zz}}}$

Polar Decomposition

* $\textbf{Q}$: Rotation tensor
  * $\textbf{Q}=\textbf{F}\cdot\textbf{U}^{-1}=\textbf{V}^{-1}\cdot\textbf{F}$
* $\textbf{U}$: Right or material stretch tensor
  * $\textbf{U}\stackrel{not.}{=}\sqrt{\textbf{F}^T\cdot\textbf{F}}$
* $\textbf{V}$: Left or spatial stretch tensor
  * $\textbf{V}\stackrel{not.}{=}\sqrt{\textbf{F}\cdot\textbf{F}^T}$

Polar Decomposition of $\textbf{F}$

* $\textbf{F}=\textbf{Q}\cdot\textbf{U}=\textbf{V}\cdot\textbf{Q}$

$dV_0$: volume associated to a particle $\textbf{P}$ at time 0

* $dV_0=(d\textbf{X}^{(1)}\cross{d\textbf{X}^{(2)}})\cdot{d\textbf{X}^{(3)}}=\det{\underbrace{\begin{bmatrix}dX^{(1)}_1&dX^{(1)}_2&dX^{(1)}_3\\dX^{(2)}_1&dX^{(2)}_2&dX^{(2)}_3\\dX^{(3)}_1&dX^{(3)}_2&dX^{(3)}_3\end{bmatrix}}_{[\textbf{M}]}}=|\textbf{M}|$

$dV_t$: volume associated to a particle $\textbf{P}$ at time $t$

* $dV_t=(d\textbf{x}^{(1)}\cross{d\textbf{x}^{(2)}})\cdot{d\textbf{x}^{(3)}}=\det{\underbrace{\begin{bmatrix}dx^{(1)}_1&dx^{(1)}_2&dx^{(1)}_3\\dx^{(2)}_1&dx^{(2)}_2&dx^{(2)}_3\\dx^{(3)}_1&dx^{(3)}_2&dx^{(3)}_3\end{bmatrix}}_{[\textbf{m}]}}=|\textbf{m}|$
* $\textbf{m}=\textbf{M}\cdot\textbf{F}^T$
* $dV_t=|\textbf{F}|dV_0$
* defining $J(\textbf{X},t)$ as the jacobian of the deformation, $J(\textbf{X},t)=\det\textbf{F}(\textbf{X},t)$
  * $dV_t=J(\textbf{X},t)\cdot{dV_0}$

$d\textbf{A}$: material vector "differential of area"

* $d\textbf{A}=dA\textbf{N}$ where $|d\textbf{A}|=dA$
* $dV_0=d\textbf{A}\cdot{d\textbf{X}^{(3)}}$

$d\textbf{a}$: spatial vector "differential of area"

* $d\textbf{a}=da\textbf{n}$ where $|d\textbf{a}|=da$
* $dV_t=d\textbf{a}\cdot{d\textbf{x}^{(3)}}$
* $d\textbf{a}=|\textbf{F}|\cdot\textbf{A}\cdot\textbf{F}^{-1}$
* $da\textbf{n}=|\textbf{F}|\textbf{N}\cdot\textbf{F}^{-1}dA$
* $da\textbf{n}=|\textbf{F}|\norm{\textbf{N}\cdot\textbf{F}^{-1}}dA$

$e(\textbf{X},t)$: Volumetric Strain

* $e(\textbf{X},t)=\dfrac{dV_t-dV_0}{dV_0}$
* $e=|\textbf{F}|-1$

Infinitesimal Strain

$\boldsymbol{\varepsilon}$: infinitesimal strain tensor

* $\boldsymbol{\varepsilon}=\dfrac{1}{2}\left(\textbf{J}+\textbf{J}^T\right)=$$\dfrac{1}{2}\left({\dfrac{\part{u}_i}{\part{x}_j}+\dfrac{\part{u}_j}{\part{x}_i}}\right)=$$\dfrac{1}{2}\left(\textbf{j}+\textbf{j}^T\right)=\dfrac{1}{2}\left(\textbf{u}\otimes\nabla+\nabla\otimes\textbf{u}\right)\stackrel{not.}{=}\nabla^s\textbf{u}$
* $\textbf{e}\cong\textbf{E}\cong\boldsymbol{\varepsilon}$, $\textbf{T}\approx\textbf{t}$
  * $\lambda_{\text{T}}\cong1+\textbf{T}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}$
  * $\lambda_t\cong1+\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}$
  * $\lambda=\dfrac{ds}{dS}\cong1+\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}\cong1+\textbf{T}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}$
  * $\varepsilon=\dfrac{ds-dS}{dS}=\lambda-1=\textbf{t}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}$
* $\boldsymbol{\varepsilon}=\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&\varepsilon_{zz}\end{bmatrix}=\begin{bmatrix}\varepsilon_{11}&\varepsilon_{12}&\varepsilon_{13}\\\varepsilon_{21}&\varepsilon_{22}&\varepsilon_{23}\\\varepsilon_{31}&\varepsilon_{32}&\varepsilon_{33}\end{bmatrix}$
  * $\begin{matrix*}[l]\lambda_1=1+\varepsilon_{11}\Rightarrow\varepsilon_{x}=\lambda_x-1=\varepsilon_{xx}\\\lambda_2=1+\varepsilon_{22}\Rightarrow\varepsilon_{y}=\lambda_y-1=\varepsilon_{yy}\\\lambda_3=1+\varepsilon_{33}\Rightarrow\varepsilon_{z}=\lambda_z-1=\varepsilon_{zz}\end{matrix*}$
  * $\theta_{xy}\cong\dfrac{\pi}{2}-2\varepsilon_{xy}$
  * $\begin{matrix*}[l]\Delta\theta_{xy}=-2\varepsilon_{xy}\\\Delta\theta_{xz}=-2\varepsilon_{xz}\\\Delta\theta_{yz}=-2\varepsilon_{yz}\end{matrix*}$
* $\Delta\theta=-\dfrac{2\textbf{T}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{T}^{(2)}}{\sin\Theta}=-\dfrac{2\textbf{t}^{(1)}\cdot\boldsymbol{\varepsilon}\cdot\textbf{t}^{(2)}}{\sin\theta}$

Polar Decomposition in infinitesimal Strain Theory

* $\textbf{U}=\textbf{1}+\boldsymbol{\varepsilon}$
* $\textbf{U}^{-1}=\textbf{1}-\boldsymbol{\varepsilon}$

$\boldsymbol{\Omega}$: infinitesimal rotation tensor

* $\textbf{Q}=\textbf{1}+\boldsymbol{\Omega}$
* $\boldsymbol{\Omega}\stackrel{def}{=}\dfrac{1}{2}(\textbf{J}+\textbf{J}^T)=\dfrac{1}{2}(\textbf{u}\otimes\nabla-\nabla\otimes\textbf{u})\stackrel{def}{=}\nabla^a\textbf{u}$
* $\Omega_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{u}_i}{\part{x}_j}-\dfrac{\part{u}_j}{\part{x}_i}}\right]<<1\space\space\space\space{i,j\in\{1,2,3\}}$
* $[\boldsymbol{\Omega}]=\begin{bmatrix}0&\Omega_{12}&-\Omega_{31}\\-\Omega_{12}&0&\Omega_{23}\\\Omega_{31}&-\Omega_{23}&0\end{bmatrix}$

$\boldsymbol{\theta}_t$: infinitesimal rotation vector

* $\boldsymbol{\theta}\equiv\begin{Bmatrix}\theta_1\\\theta_2\\\theta_3\end{Bmatrix}=$$\begin{Bmatrix}-\Omega_{23}\\-\Omega_{31}\\-\Omega_{12}\end{Bmatrix}=$$\dfrac{1}{2}\begin{Bmatrix}\dfrac{\part{u_3}}{\part{x_2}}-\dfrac{\part{u_2}}{\part{x_3}}\\\dfrac{\part{u_1}}{\part{x_3}}-\dfrac{\part{u_3}}{\part{x_1}}\\\dfrac{\part{u_2}}{\part{x_1}}-\dfrac{\part{u_1}}{\part{x_2}}\end{Bmatrix}$$\stackrel{def}{=}\dfrac{1}{2}\nabla\cross\textbf{u}$
* $\boldsymbol{\theta}\cross\textbf{r}=\boldsymbol{\Omega}\cdot\textbf{r}$    $\forall\textbf{r}$

$\textbf{F}$ in infinitesimal theory

* $\textbf{F}=\textbf{1}+\boldsymbol{\varepsilon}+\boldsymbol{\Omega}$	$\textbf{F}(\bull)\equiv\text{stretching}(\bull)+\text{rotation}(\bull)$

volumetric strain $e$ in infinitesimal theory

* $e=Tr(\boldsymbol{\varepsilon})$

$\mathbfit{l}(\textbf{x},t)$: Spatial velocity gradient tensor

* $d\textbf{v}=\mathbfit{l}\cdot{d\textbf{x}}$
* $\mathbfit{l}(\textbf{x},t)\stackrel{def}{=}\dfrac{\part\textbf{v}(\textbf{x},t)}{\part\textbf{x}}=\textbf{v}\otimes\nabla$
* $\textbf{l}=\text{sym}[\textbf{l}]+\text{skew}[\textbf{l}]:=\textbf{d}+\textbf{w}$

$\textbf{d}$: Strain Rate Tensor

* $\textbf{d}\stackrel{def}{=}sym(\mathbfit{l})=\dfrac{1}{2}(\mathbfit{l}+\mathbfit{l}^T)=\dfrac{1}{2}(\textbf{v}\otimes\nabla+\nabla\otimes\textbf{v})\stackrel{not.}{=}\nabla^s\otimes\textbf{v}$
* $\text{d}_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{\text{v}_i}}{\part\text{x}_j}+\dfrac{\part{\text{v}_j}}{\part\text{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}$
* $[\textbf{d}]=\begin{bmatrix}\text{d}_{11}&\text{d}_{12}&\text{d}_{13}\\\text{d}_{21}&\text{d}_{22}&\text{d}_{23}\\\text{d}_{31}&\text{d}_{32}&\text{d}_{33}\end{bmatrix}$
* $\dfrac{d}{dt}(ds(t))^2=2{d}\textbf{x}\cdot\textbf{d}\cdot{d}\textbf{x}$

$\dot{\textbf{E}}$: material derivative of the material strain tensor ($\textbf{E}$)

* $\dot{\textbf{E}}=\dfrac{d\textbf{E}}{dt}$
* $\dfrac{d}{dt}((ds(t))^2-(dS)^2)=\dfrac{d}{dt}((ds(t))^2)=2{d}\textbf{X}\cdot\dot{\textbf{E}}\cdot{d}\textbf{X}$
* $\dot{\textbf{E}}=\textbf{F}^T\cdot\textbf{d}\cdot\textbf{F}$

$\textbf{w}$: Rotation Rate or Spin Tensor

* $\textbf{w}\stackrel{def}{=}sym(\mathbfit{l})=\dfrac{1}{2}(\mathbfit{l}-\mathbfit{l}^T)=\dfrac{1}{2}(\textbf{v}\otimes\nabla-\nabla\otimes\textbf{v})\stackrel{not.}{=}\nabla^a\otimes\textbf{v}$
* $\text{w}_{ij}=\dfrac{1}{2}\left[{\dfrac{\part{\text{v}_i}}{\part\text{x}_j}-\dfrac{\part{\text{v}_j}}{\part\text{x}_i}}\right]\space\space\space\space{i,j\in\{1,2,3\}}$
* $[\textbf{w}]=\begin{bmatrix}0&\text{w}_{12}&-\text{w}_{31}\\-\text{w}_{12}&0&\text{w}_{23}\\\text{w}_{31}&-\text{w}_{23}&0\end{bmatrix}$

$\boldsymbol{\omega}$: spin vector (axial vector $[\textbf{w}]$)

* $\boldsymbol{\omega}=$$\dfrac{1}{2}rot(\textbf{v})=$$\dfrac{1}{2}\nabla\cross\textbf{v}\equiv$$\dfrac{1}{2}\begin{bmatrix}\dfrac{\part{\text{v}_3}}{\part{x_2}}-\dfrac{\part{\text{v}_2}}{\part{x_3}}\\\dfrac{\part{\text{v}_1}}{\part{x_3}}-\dfrac{\part{\text{v}_3}}{\part{x_1}}\\\dfrac{\part{\text{v}_2}}{\part{x_1}}-\dfrac{\part{\text{v}_1}}{\part{x_2}}\end{bmatrix}=$$\begin{bmatrix}-\text{w}_{23}\\-\text{w}_{31}\\-\text{w}_{12}\end{bmatrix}=$$\begin{bmatrix}\omega_1\\\omega_2\\\omega_3\end{bmatrix}$
* $[\textbf{w}]=\begin{bmatrix}0&-\omega_3&\omega_2\\\omega_3&0&-\omega_1\\-\omega_2&\omega_1&0\end{bmatrix}$

* The vector $2\boldsymbol{\omega}=\nabla\cross\textbf{v}$ is named **vorticity vector**
* $\boldsymbol{\omega}\cross\textbf{r}=\textbf{w}\cdot\textbf{r}$  $\forall\textbf{r}$

for relative velocity $d\textbf{v}$

* $d\textbf{v}=\textbf{d}\cdot{d}\textbf{x}+\textbf{w}\cdot{d}\textbf{x}$

$\dot{\textbf{F}}$: The material time derivative of the **deformation gradient tensor**

* $\dfrac{d\textbf{F}}{dt}\stackrel{not.}{=}\dot{\textbf{F}}=\mathbfit{l}\cdot\textbf{F}$
* $\dfrac{dF_{ij}}{dt}=\dot{F}_{ij}=\mathbfit{l}_{ik}F_{kj}\space\space\space\space{i,j\in\{1,2,3\}}$

## Ch3: Compatibility Equations

Considering $\boldsymbol{\varepsilon}\stackrel{def}{=}\begin{bmatrix}\varepsilon_{xx}&\varepsilon_{xy}&\varepsilon_{xz}\\\varepsilon_{yx}&\varepsilon_{yy}&\varepsilon_{yz}\\\varepsilon_{zx}&\varepsilon_{zy}&\varepsilon_{zz}\end{bmatrix}=\begin{bmatrix}\varepsilon_{11}&\varepsilon_{12}&\varepsilon_{13}\\\varepsilon_{21}&\varepsilon_{22}&\varepsilon_{23}\\\varepsilon_{31}&\varepsilon_{32}&\varepsilon_{33}\end{bmatrix}$, $\textbf{x}\stackrel{def}{=}\begin{bmatrix}x_1\\x_2\\x_3\end{bmatrix}$ and $\textbf{u}\stackrel{def}{=}\begin{bmatrix}u_1\\u_2\\u_3\end{bmatrix}$:

$\dfrac{\part{\theta_1}}{\part{x_1}}=\dfrac{\part\varepsilon_{13}}{\part{x}_2}-\dfrac{\part\varepsilon_{12}}{\part{x}_3}$	$\dfrac{\part{\theta_1}}{\part{x_2}}=\dfrac{\part\varepsilon_{23}}{\part{x}_2}-\dfrac{\part\varepsilon_{22}}{\part{x}_3}$	$\dfrac{\part{\theta_1}}{\part{x_3}}=\dfrac{\part\varepsilon_{33}}{\part{x}_2}-\dfrac{\part\varepsilon_{23}}{\part{x}_3}$

$\dfrac{\part{\theta_2}}{\part{x_1}}=\dfrac{\part\varepsilon_{11}}{\part{x}_3}-\dfrac{\part\varepsilon_{13}}{\part{x}_1}$	$\dfrac{\part{\theta_2}}{\part{x_2}}=\dfrac{\part\varepsilon_{12}}{\part{x}_3}-\dfrac{\part\varepsilon_{23}}{\part{x}_1}$	$\dfrac{\part{\theta_2}}{\part{x_3}}=\dfrac{\part\varepsilon_{13}}{\part{x}_3}-\dfrac{\part\varepsilon_{33}}{\part{x}_1}$

$\dfrac{\part{\theta_3}}{\part{x_1}}=\dfrac{\part\varepsilon_{12}}{\part{x}_1}-\dfrac{\part\varepsilon_{11}}{\part{x}_2}$	$\dfrac{\part{\theta_3}}{\part{x_2}}=\dfrac{\part\varepsilon_{22}}{\part{x}_1}-\dfrac{\part\varepsilon_{12}}{\part{x}_2}$	$\dfrac{\part{\theta_3}}{\part{x_3}}=\dfrac{\part\varepsilon_{23}}{\part{x}_1}-\dfrac{\part\varepsilon_{13}}{\part{x}_2}$

$\dfrac{\part{u_1}}{\part{x_1}}=$$\varepsilon_{11}$			 $\dfrac{\part{u_1}}{\part{x_2}}=$$\varepsilon_{12}-\theta_3$		 $\dfrac{\part{u_1}}{\part{x_3}}=$$\varepsilon_{13}+\theta_2$

$\dfrac{\part{u_2}}{\part{x_1}}=$$\varepsilon_{12}+\theta_3$		 $\dfrac{\part{u_2}}{\part{x_2}}=$$\varepsilon_{22}$			 $\dfrac{\part{u_2}}{\part{x_3}}=$$\varepsilon_{23}-\theta_1$

$\dfrac{\part{u_3}}{\part{x_1}}=$$\varepsilon_{13}-\theta_2$		 $\dfrac{\part{u_3}}{\part{x_2}}=$$\varepsilon_{23}+\theta_1$		 $\dfrac{\part{u_3}}{\part{x_3}}=$$\varepsilon_{33}$























