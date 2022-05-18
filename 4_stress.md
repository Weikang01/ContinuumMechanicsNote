# Forces Acting on a Continuum Body

Forces acting on a continuum body:

* **Body forces.**

  * Act on the elements of volume or mass **inside** the body.

  * "Action-at-a-distance" force.

  * E.g.: gravity, electrostatic forces, magnetic forces

    $\mathbf{f}_V=$$\displaystyle\int_{V}^{}{\rho\mathbf{b}(\mathbf{x},t)dV}$	where $\mathbf{b}$ is the body force per unit (**specific boy forces**)

* **Surface forces.**

  * **Contact forces** acting on the body at its **boundary** surface.

  * E.g.: contact forces between bodies, applied point or distributed loads on the surface of a body

    $\mathbf{f}_S=$$\displaystyle\int_{\part{V}}^{}{\textbf{t}(\textbf{x},t)dS}$	where $\textbf{t}$ is the surface force per unit surface (**traction vector**)

# Cauchy’s Postulates

1. **Cauchy’s 1^st^ Postulates**

   The traction vector $\textbf{t}$ remains unchanged for all surfaces passing through the point $P$ and having the same normal vector $\textbf{n}$ at $P$.

   $\boxed{\textbf{t}=\textbf{t}(P,\textbf{n})}$

   > ==REMARK== The traction vector (generalized to internal points) is not influenced by the curvature of the internal surfaces.

2. **Cauchy's fundamental lemma** (Cauchy reciprocal theorem)

   The traction vectors acting at point $P$ on opposite sides of the same surface are equal in magnitude and opposite in direction.

   $\boxed{\textbf{t}(P,\textbf{n})=-\textbf{t}(P,-\textbf{n})}$

   > ==REMARK== Cauchy's fundamental lemma is equivalent to Newton's 3^rd^ law (action and reaction).

   # Stress Tensor
   
   * The areas of the faces of the tetrahedron are:
   
     $\begin{cases}S_1=n_1S\\S_2=n_2S\\S_3=n_3S\end{cases}$	with	$\textbf{n}\equiv\left\{\text{n}_1,\text{n}_2,\text{n}_3\right\}^\text{T}$
   
   * The "mean" stress vectors acting on these faces are
   
     $\begin{cases}\textbf{t}^\ast=\textbf{t}(\textbf{x}^\ast_S),-\textbf{t}^{(1)^\ast}=\textbf{t}(\textbf{x}^\ast_{S_1},\hat{{\textbf{e}}}_1),-\textbf{t}^{(2)^\ast}=\textbf{t}(\textbf{x}^\ast_{S_2},\hat{{\textbf{e}}}_2),-\textbf{t}^{(3)^\ast}=\textbf{t}(\textbf{x}^\ast_{S_3},\hat{{\textbf{e}}}_3)\\\textbf{x}^\ast_{S_i}\in{S_i}\space\space{i}=1,2,3;\textbf{x}^\ast_S\in{S}\rightarrow\text{mean value theorem}\end{cases}$
   
     * *the surface normal vectors of the planes perpendicular to the axes* are
   
       $\textbf{n}_1=-\hat{\textbf{e}}_1$ $;$	$\textbf{n}_2=-\hat{\textbf{e}}_2$ $;$	$\textbf{n}_3=-\hat{\textbf{e}}_3$
   
     * Following Cauchy's fundamental lemma:
   
       $\textbf{t}(\textbf{x},\hat{{\textbf{e}}}_i)=$$-\textbf{t}(\textbf{x},\hat{{\textbf{e}}}_i)\stackrel{not.}{=}$$-\textbf{t}^{(\text{i})}(\textbf{x})$	$\text{i}\in\{1,2,3\}$
   
     > ==REMARK== The asterisk indicates an mean value the area.
   
   > **Mean Value Theorem**
   >
   >    * Let $f:[\text{a,b}]\rightarrow\R$ be a continuous function on the closed interval $\text{[a,b]}$, and differentiable on the open interval $\text{(a,b)}$, where $\text{a<b}$. Then there exists some $x^\ast$ in $\text{(a,b)}$ such that:
   >    
   >      $f(x^\ast)=\dfrac{1}{\Upomega}\displaystyle\int_{\Upomega}^{}{}f(x)d\Upomega$
   >    
   >    * i.e.: $f:[\text{a,b}]\rightarrow\R$ gets its "mean value" $f\left(x^\ast\right)$ at the interior of $\text{[a,b]}$
   
   * From equilibrium of forces, i.e. Newton's 2^nd^ law of motion:
   
     $\textbf{R}=$$\displaystyle\sum^{}_{i}{\textbf{f}_i}=$$\displaystyle\sum^{}_{i}{m_i\textbf{a}_i}$	$\Rightarrow$	$\displaystyle\int_{V}^{}{\rho\textbf{b}dV}+$$\displaystyle\int_{\part{V}}^{}{\textbf{t}dS}=$$\displaystyle\int_{V}^{}{\textbf{a}\underbrace{\rho{dV}}_{dm}}=$$\displaystyle\int_{V}^{}{\rho\textbf{a}dV}$
   
     $\underset{\begin{matrix}\text{resultant}\\\text{body forces}\end{matrix}}{\boxed{\displaystyle\int_{V}^{}{\rho\textbf{b}dV}}}+$$\underset{\begin{matrix}\text{resultant}\\\text{surface forces}\end{matrix}}{\boxed{\displaystyle\int_{S}^{}{\textbf{t}dS}+\displaystyle\int_{S_1}^{}{-\textbf{t}^{(1)}dS}+\displaystyle\int_{S_2}^{}{-\textbf{t}^{(2)}dS}+\displaystyle\int_{S_3}^{}{-\textbf{t}^{(3)}dS}}}=\displaystyle\int_{V}^{}{\rho\textbf{a}dV}$
   
   * Considering the mean value theorem,
   
     $(\rho\textbf{b})^\ast\text{V}+$$\textbf{t}^\ast\text{S}-$$\textbf{t}^{{(1)}^\ast}\text{S}_1-$$\textbf{t}^{{(2)}^\ast}\text{S}_2-$$\textbf{t}^{{(3)}^\ast}\text{S}_3=$$(\rho\textbf{a})^\ast\text{V}$
   
   * Introducing $S_i=n_iS$ $i\in\{1,2,3\}$ and $V=\dfrac{1}{3}Sh$,
   
     $\dfrac{1}{3}(\rho\textbf{b})^\ast{h}\bcancel{S}+$$\textbf{t}^\ast\bcancel{S}-$$\textbf{t}^{(1)^\ast}n_1\bcancel{S}-$$\textbf{t}^{(2)^\ast}n_2\bcancel{S}-$$\textbf{t}^{(3)^\ast}n_3\bcancel{S}=$$\dfrac{1}{3}(\rho\textbf{a})^\ast{h}\bcancel{S}$
   
   * If the tetrahedron shrinks to point $O$, $(\text{h}\rightarrow\text{0})$
   
     $\textbf{x}^\ast_{\text{S}_\text{i}}\rightarrow\textbf{x}_O$ $\Rightarrow$ $\displaystyle\lim_{\text{h}\rightarrow0}\left[\textbf{t}^{(\text{i})^\ast}\left(\textbf{x}^\ast_{\text{S}_\text{i}}\right)\right]=$$\textbf{t}^{(\text{i})}\left(O,\hat{{\textbf{e}}}_i\right)$	$i\in\{1,2,3\}$
   
     $\textbf{x}^\ast_{\text{S}}\rightarrow\textbf{x}_O$ $\Rightarrow$ $\displaystyle\lim_{\text{h}\rightarrow0}\left[\textbf{t}^\ast\left(\textbf{x}^\ast_\text{S},\textbf{n}\right)\right]=$$\textbf{t}(O,\textbf{n})$
   
     $\displaystyle\lim_{\text{h}\rightarrow0}\left(\dfrac{1}{3}(\rho\space\space\textbf{b})^\ast\space{h}\right)=$$\displaystyle\lim_{\text{h}\rightarrow0}\left(\dfrac{1}{3}(\rho\textbf{a})^\ast\space{h}\right)=$$\textbf{0}$
   
   * The limit of the expression for the equilibrium of forces becomes,
   
     $\cancel{\dfrac{1}{3}(\rho\textbf{b})^\ast{h}}+$$\underset{=\textbf{t}(O,\textbf{n})}{\boxed{\textbf{t}^\ast}}-$$\overset{=\textbf{t}^{(\text{1})}}{\boxed{\textbf{t}^{(\text{1})^\ast}}}n_1-$$\overset{=\textbf{t}^{(\text{2})}}{\boxed{\textbf{t}^{(\text{2})^\ast}}}n_2-$$\overset{=\textbf{t}^{(\text{3})}}{\boxed{\textbf{t}^{(\text{3})^\ast}}}n_3=$$\cancel{\dfrac{1}{3}(\rho\textbf{a})^\ast{h}}$ $\Rightarrow$ $\boxed{\textbf{t}(O,\textbf{n})-\textbf{t}^{(\text{i})}n_i=\textbf{0}}$



















