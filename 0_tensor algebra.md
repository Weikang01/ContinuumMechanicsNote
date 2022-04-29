# Concept of Tensor

> A ==TENSOR== is an algebraic entity with various components which ==generalizes the concepts== of scalar, vector and matrix.

* Many physical quantities are mathematically represented as tensors.
* Tensors are independent of any reference system but, by need, are commonly represented in one by means of their "component matrices".
* The components of a tensor will depend of the reference system chosen and will vary with it.

## Order of a Tensor

* the order of a tensor is given by the number of indexes needed to specify without ambiguity a component of a tensor
  * **scalar**: zero dimension.
  * **vector**: 1 dimension
  * **2^nd^ order**: 2 dimensions
  * **3^rd^ order**: 3 dimensions
  * **4^th^ order** ...

## Cartesian Coordinate System

* given an orthonormal basis formed by three mutually perpendicular unit vectors

  where $|\hat{e}_1|=1$, $|\hat{e}_2|=1$, $|\hat{e}_3|=1$

* note that

  $\hat{e}_i\cdot\hat{e}_j=\begin{cases}1\text{ if }i=j\\0\text{ if }i\neq{j}\end{cases}=\delta_{ij}$

## Tensor Bases - Vector

* a vector $\textrm{v}$ can be written as a unique linear combination of the three vector basis $\hat{e}_i$ for $i\in\{1,2,3\}$

  $\text{v=v}_1\hat{e}_1+\text{v}_2\hat{e}_2+\text{v}_3\hat{e}_3$

* in matrix notation:

  [v]=[v~1~  v~2~  v~3~]^T^

* in index notation:

  $\textbf{v=}\sum_i{\text{v}_i}{\hat{e}_{i}}$	tensor as a physical entity

  $[\textbf{v}]_i=\text{v}_i$	  component $i$ of the tensor in the given basis $i\in\{1,2,3\}$

## Tensor Basis - 2^nd^ Order Tensor

* a 2^nd^ order tensor $\textbf{A}$ can be written as a unique linear combination of the **nine** dyads $\hat{e}_{i}\otimes\hat{e}_{j}\equiv\hat{e}_{i}\hat{e}_{j}$ for $i,j\in\{1,2,3\}$

  $\textbf{A}$=$A_{11}(\hat{e}_{1}\otimes\hat{e}_{1})+A_{12}(\hat{e}_{1}\otimes\hat{e}_{2})+A_{13}(\hat{e}_{1}\otimes\hat{e}_{3})+$

    $+A_{21}(\hat{e}_{2}\otimes\hat{e}_{1})+A_{22}(\hat{e}_{2}\otimes\hat{e}_{2})+A_{23}(\hat{e}_{2}\otimes\hat{e}_{3})+$

    $+A_{31}(\hat{e}_{3}\otimes\hat{e}_{1})+A_{32}(\hat{e}_{3}\otimes\hat{e}_{2})+A_{33}(\hat{e}_{3}\otimes\hat{e}_{3})$

* alternatively, this could have been written as:

  $\textbf{A}$=$A_{11}\hat{e}_{1}\hat{e}_{1}+A_{12}\hat{e}_{1}\hat{e}_{2}+A_{13}\hat{e}_{1}\hat{e}_{3}+$

  $+A_{21}\hat{e}_{2}\hat{e}_{1}+A_{22}\hat{e}_{2}\hat{e}_{2}+A_{23}\hat{e}_{2}\hat{e}_{3}+$

  $+A_{31}\hat{e}_{3}\hat{e}_{1}+A_{32}\hat{e}_{3}\hat{e}_{2}+A_{33}\hat{e}_{3}\hat{e}_{3}$

* in matrix notation:

  $[\textbf{A}]=\begin{bmatrix}A_{11}&A_{12}&A_{13}\\A_{21}&A_{22}&A_{23}\\A_{31}&A_{32}&A_{33}\end{bmatrix}$

* in index notation:

  $\textbf{A}=\sum_\limits{ij}\text{A}_{ij}(\hat{e}_i\otimes\hat{e}_j)$	tensor as a physical entity

  $[\textbf{A}]_{ij}=A_{ij}$			component $ij$ of the tensor in the given basis $i,j\in\{1,2,3\}$

## Tensor Bases - 3^rd^ Order Tensor

* a 3^rd^ order tensor $\mathbfcal{A}$ can be written as a unique linear combination of the 27 triads $\hat{e}_{i}\otimes\hat{e}_{j}\otimes\hat{e}_{k}\equiv\hat{e}_{i}\hat{e}_{j}\hat{e}_{k}$ for $i,j,k\in\{1,2,3\}$

  $\mathbfcal{A}$=$\mathcal{A}_{111}(\hat{e}_{1}\otimes\hat{e}_{1}\otimes\hat{e}_{1})+\mathcal{A}_{121}(\hat{e}_{1}\otimes\hat{e}_{2}\otimes\hat{e}_{1})+\mathcal{A}_{131}(\hat{e}_{1}\otimes\hat{e}_{3}\otimes\hat{e}_{1})+$

    $\mathcal{A}_{211}(\hat{e}_{2}\otimes\hat{e}_{1}\otimes\hat{e}_{1})+\mathcal{A}_{221}(\hat{e}_{2}\otimes\hat{e}_{2}\otimes\hat{e}_{1})+\mathcal{A}_{231}(\hat{e}_{2}\otimes\hat{e}_{3}\otimes\hat{e}_{1})+$

    $\mathcal{A}_{311}(\hat{e}_{3}\otimes\hat{e}_{1}\otimes\hat{e}_{1})+\mathcal{A}_{321}(\hat{e}_{3}\otimes\hat{e}_{2}\otimes\hat{e}_{1})+\mathcal{A}_{331}(\hat{e}_{3}\otimes\hat{e}_{3}\otimes\hat{e}_{1})+$

    $\mathcal{A}_{112}(\hat{e}_{1}\otimes\hat{e}_{1}\otimes\hat{e}_{2})+\mathcal{A}_{122}(\hat{e}_{1}\otimes\hat{e}_{2}\otimes\hat{e}_{2})+\dots$

* in index notation

  $\mathbfcal{A}=\sum_\limits{ijk}(\hat{e}_{i}\otimes\hat{e}_{j}\otimes\hat{e}_{k})=$

  $=\mathcal{A}_{ijk}(\hat{e}_{i}\otimes\hat{e}_{j}\otimes\hat{e}_{k})\equiv\mathcal{A}_{ijk}\hat{e}_{i}\hat{e}_{j}\hat{e}_{k}$	tensor as a physical entity

  $[\mathbfcal{A}]=\mathcal{A}_{ijk}$						component $ijk$ of the tensor in the given basis $i,j,k\in\{1,2,3\}$

## Repeated-index (or Einstein's) Notation

* the ==Einstein Summation Convention==: repeated Roman indices are summed over.

   $a_ib_i=\sum^\limits{3}_{i=1}a_ib_i=a_1b_1+a_2b_2+a_3b_3$	where ==$i$== is a **mute index**

  $A_{ij}b_j=\sum^\limits{3}_{j=1}A_{ij}b_j=A_{i1}b_1+A_{i2}b_2+A_{i3}b_3$	where ==$i$== is a **talking index** and ==$j$== is a **mute index**

* a "==MUTE=="(or **Dummy**) INDEX is an index that does not appear in a monomial after the summation is carried out (it can be arbitrarily changed of "name").

* a "==TALKING==" INDEX is an index that is not repeated in the same monomial and is transmitted outside of it (it cannot be arbitrarily changed of "name").

  > ==REMARK==: an index can only appear up to two times in a monomial

RULES of this notation:

1. sum over all repeated indices.

2. increment all unique indices fully at least once, covering all combinations.

3. increment repeated indices first.

4. a comma indicates differentiation, with respect to coordinate $x_i$.

   $u_{i,i}=\dfrac{\partial{u_i}}{\partial{x_i}}=\sum^\limits{3}_{i=1}\dfrac{\partial{u_i}}{\partial{x_i}}$

   $u_{i,jj}=\dfrac{\partial^2{u_i}}{\partial{x_j}\partial{x_j}}=\sum^\limits{3}_{j=1}\dfrac{\partial^2{u_i}}{\partial{x^2_j}}$

   $A_{ij,j}=\dfrac{\partial{A_{ij}}}{\partial{x_j}}=\sum^\limits{3}_{j=1}\dfrac{\partial{A_{ij}}}{\partial{x_j}}$

5. the number of talking indices indicates the order of the tensor result

## Kronecker Delta $\delta$

* the Kronecker delta $\delta_{ij}$ is defined as:

  $\delta_{ij}=\begin{cases}1\text{ if } i=j\\0\text{ if }i\neq{j}\end{cases}$

* both $i$ and $j$ may take on any value in $\{1,2,3\}$

* only for the three possible cases where $i=j$ is $\delta_{ij}$ non-zero:

  $\delta_{ij}=\begin{cases}1\text{ if } i=j\text{  }(\delta_{11}=\delta_{22}=\delta_{33}=1)\\0\text{ if }i\neq{j}\text{  }(\delta_{12}=\delta_{13}=\delta_{21}=\dots=0)\end{cases}$

* $\delta_{ij}=\delta_{ji}$

> ==REMARK== following Einstein's notation: $\delta_{ii}=\delta_{11}+\delta_{22}+\delta_{33}=3$
>
> Kronecker delta serves as a replacement operator:
>
> $\delta_{ij}u_j=u_i$, $\delta_{ij}A_{jk}=A_{ik}$

## Levi-Civita Epsilon (permutation) $\varepsilon$

* the Levi-Civita epsilon $e_{ijk}$ is defined as:

  $e_{ijk}=\begin{cases}0\text{ if there is a repeated index}\\+1\text{ if }ijk=123,231\text{ or }312\\-1\text{ if }ijk=213,132\text{ or }321\end{cases}$

* 3 indices $\Rightarrow$ 27 possible combinations.

* $e_{ijk}=-e_{ikj}$

  > ==REMARK== The Levi-Civita symbol is also named permutation or alternating symbol.

**Example**

prove the following expression is true:

$e_{ijk}e_{ijk}=6$

> remember: $e_{ijk}$ is 0 if there is a **repeated index**

$e_{111}e_{111}=e_{112}e_{112}=e_{113}e_{113}=e_{121}e_{121}=e_{122}e_{122}=$

$e_{131}e_{131}=e_{133}e_{133}=e_{211}e_{211}=e_{212}e_{212}=e_{221}e_{221}=$

$e_{222}e_{222}=e_{223}e_{223}=e_{311}e_{311}=e_{313}e_{313}=e_{322}e_{322}=$

$e_{323}e_{323}=e_{331}e_{331}=e_{332}e_{332}=e_{333}e_{333}=0\times0=0$

> $e_{ijk}$ is +1 if $ijk$ is 123, 231 or 312

$e_{123}e_{123}=e_{231}e_{231}=e_{312}e_{312}=1\times1=1$

> $e_{ijk}$ is -1 if $ijk$ is 213, 132 or 321

$e_{213}e_{213}=e_{132}e_{132}=e_{321}e_{321}=-1\times-1=1$

therefore,

$e_{ijk}e_{ijk}=\sum^\limits{3}_{i=1}\sum^\limits{3}_{j=1}\sum^\limits{3}_{k=1}e_{ijk}e_{ijk}=$

$e_{123}e_{123}+e_{231}e_{231}+e_{312}e_{312}+e_{213}e_{213}+e_{132}e_{132}+e_{321}e_{321}=6$

## Vector Operations

* **sum and subtraction. parallelogram law.**

  $\textbf{a}+\textbf{b}=\textbf{b}+\textbf{a}=c\Rightarrow c_i=a_i+b_i$

  $\textbf{a}-\textbf{b}=\textbf{d}$       $\Rightarrow d_i=a_i-b_i$

* **scalar multiplication**

  $\alpha\textbf{a}=\textbf{b}=\alpha a_1\hat{\textbf{e}}_1+\alpha a_2\hat{\textbf{e}}_2+\alpha a_3\hat{\textbf{e}}_3$    $\Rightarrow b_i=\alpha a_i$

* **scalar or dot product** yields a scalar

  $\textbf{u}\cdot{\textbf{v}}=|\textbf{u}||\textbf{v}|\text{cos}(\theta)$, where $\theta$ is the angle between the vectors $\textbf{u}$ and $\textbf{v}$

  * in index notation:

    $\textbf{u}\cdot{\textbf{v}}=u_i\hat{\textbf{e}}_i\cdot{\text{v}_j\hat{\textbf{e}}_j}=u_i\text{v}_j\hat{\textbf{e}}_i\cdot\hat{\textbf{e}}_j=u_i\text{v}_j\delta_{ij}=u_i\text{v}_i\left(=\sum^\limits{i=3}_{i=1}u_i\text{v}_i\right)=[\textbf{u}]^T[\textbf{v}]$

* **norm of a vector**

  $\norm{\textbf{u}}=(\textbf{u}\cdot\textbf{u})^{\dfrac{1}{2}}=(u_iu_i)^{\dfrac{1}{2}}$

  $\Rightarrow\norm{\textbf{u}}^2=\textbf{u}\cdot\textbf{u}=u_i\hat{\textbf{e}}_i\cdot u_j\hat{\textbf{e}}_j=u_iu_j\delta{ij}=u_iu_i$

  * some **properties** of the **scalar or dot product**

    $\textbf{u}\cdot\textbf{v}=\textbf{v}\cdot\textbf{u}$

    $\textbf{u}\cdot\textbf{0}=0$

    $\textbf{u}\cdot(\alpha\textbf{v}+\beta\textbf{w})=\alpha(\textbf{u}\cdot\textbf{v})+\beta(\textbf{u}\cdot\textbf{w})$	(linear operator)

    $\textbf{u}\cdot\textbf{u}>0\iff\textbf{u}\neq\textbf{0}$

    $\textbf{u}\cdot\textbf{u}=0\iff\textbf{u}=\textbf{0}$

    $\textbf{u}\cdot\textbf{v}=0, \textbf{u}\neq\textbf{0}, \textbf{v}\neq\textbf{0}\iff\textbf{u}\perp\textbf{v}$

* **vector product (or cross product)** yields another vector

  $\textbf{c}=\textbf{a}\cross\textbf{b}=-\textbf{b}\cross\textbf{a}$

  $|\textbf{c}|=|\textbf{a}||\textbf{b}|\text{sin}(\theta)$	where $\theta$ is the angle between the vectors $\textbf{a}$ and $\textbf{b}$ ($0\leq\theta\leq\pi$)

  * in index notation:

    $\textbf{c}=c_i\hat{\textbf{e}}_i=e_{ijk}a_jb_k\hat{\textbf{e}}_i$    $\Rightarrow c_i=e_{ijk}a_jb_k$  $i\in\{1,2,3\}$

    $\textbf{c}=(a_2b_3-a_3b_2)\hat{\textbf{e}}_1+(a_3b_1-a_1b_3)\hat{\textbf{e}}_2+(a_1b_2-a_2b_1)\hat{\textbf{e}}_3$  $\stackrel{symb}{=}$ $\text{det}\begin{bmatrix}\hat{\textbf{e}}_1&\hat{\textbf{e}}_2&\hat{\textbf{e}}_3\\a_1&a_2&a_3\\b_1&b_2&b_3\end{bmatrix}$

  * some **properties** of the **vector or cross product**

    $\textbf{u}\cross\textbf{v}=-(\textbf{v}\cross\textbf{u})$

    $\textbf{u}\cross\textbf{v}=\textbf{0},\textbf{u}\neq\textbf{0},\textbf{v}\neq\textbf{0}$ $\iff$ $\textbf{u}\parallel\textbf{v}$

    $\textbf{u}\cross(a\textbf{v}+b\textbf{w})=a(\textbf{u}\cross\textbf{v})+b(\textbf{u}\cross\textbf{w})$	(linear operator)

* **==tensor product== (or open or dyadic product) of two vectors**:

  $\textbf{A}=\textbf{u}\otimes\textbf{v}\equiv\textbf{u}\textbf{v}$

  also known as the dyad of the vectors $\textbf{u}$ and $\textbf{v}$, which results in a 2^nd^ order tensor $\textbf{A}$

  * deriving the tensor product along an orthogonal basis $\{\hat{\textbf{e}}_i\}$:

    $\textbf{A}=(\textbf{u}\otimes\textbf{v})=(u_i\hat{\textbf{e}}_i)\otimes(v_j\hat{\textbf{e}}_j)=u_iv_j(\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j)=A_{ij}(\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j)$

  $[\textbf{A}]_{ij}=A_{ij}=[\textbf{u}\otimes\textbf{v}]_{ij}=u_iv_j$  $i,j\in\{1,2,3\}$

  * in matrix notation:

    $[\textbf{u}\otimes\textbf{v}]=[\textbf{u}][\textbf{v}]^T=\begin{bmatrix}u_1\\u_2\\u_3\end{bmatrix}\begin{bmatrix}\text{v}_1&\text{v}_2&\text{v}_3\end{bmatrix}=\begin{bmatrix}u_1\text{v}_1&u_1\text{v}_2&u_1\text{v}_3\\u_2\text{v}_1&u_2\text{v}_2&u_2\text{v}_3\\u_3\text{v}_1&u_3\text{v}_2&u_3\text{v}_3\end{bmatrix}=\begin{bmatrix}A_{11}&A_{12}&A_{13}\\A_{21}&A_{22}&A_{23}\\A_{31}&A_{32}&A_{33}\end{bmatrix}$

  * some **properties** of the **open product**:

    $(\textbf{u}\otimes\textbf{v})\neq(\textbf{v}\otimes\textbf{u})$

    $(\textbf{u}\otimes\textbf{v})\cdot\textbf{w}=\textbf{u}\otimes(\textbf{v}\cdot\textbf{w})=\textbf{u}(\textbf{v}\cdot\textbf{w})=(\textbf{v}\cdot\textbf{w})\textbf{u}$

    $\textbf{u}\otimes(\alpha\textbf{v}+\beta\textbf{w})=\alpha\textbf{u}\otimes\textbf{v}+\beta\textbf{u}\otimes\textbf{w}$	$\Rightarrow$ linear operator

    $(\textbf{u}\otimes\textbf{v})(\textbf{w}\otimes\textbf{x})=(\textbf{u}\otimes\textbf{x})(\textbf{v}\cdot\textbf{w})$

    $\textbf{u}\cdot(\textbf{v}\otimes\textbf{w})=(\textbf{u}\cdot\textbf{v})\otimes\textbf{w}=(\textbf{u}\cdot\textbf{v})\textbf{w}=\textbf{w}(\textbf{u}\cdot\textbf{v})$

example

* prove the following property of the tensor product is true:

  $\textbf{u}\cdot(\textbf{v}\otimes\textbf{w})=(\textbf{u}\cdot\textbf{v})\otimes\textbf{w}$

## Tensor Operations

* **summation (only for equal order tensors)**

  $\textbf{A}+\textbf{B}=\textbf{B}+\textbf{A}=\textbf{C}$	$\Rightarrow$	$C_{ij}=A_{ij}+B_{ij}$

* **scalar multiplication (scalar times tensor)**

  $\alpha\textbf{A}=\textbf{C}$	$\Rightarrow$	$C_{ij}=\alpha A_{ij}$

* **dot product ($\cdot$) or single index contraction product**

  dot product between 2^nd^ order tensor $\textbf{A}$ and 1^st^ order tensor $\textbf{b}$ yields a 1^st^ order tensor $\textbf{c}$

  $\textbf{A}\cdot\textbf{b}=\textbf{c}$	$\Rightarrow$	$c_i=A_{ij}b_j$	$\Rightarrow$	index "j" disappears (index contraction)

  dot product between 3^rd^ order tensor $\mathbfcal{A}$ and 1^st^ order tensor $\textbf{b}$ yields a 2^nd^ order tensor $\textbf{C}$

  $\mathbfcal{A}\cdot\textbf{b}=\textbf{C}$	$\Rightarrow$	$C_{ij}=\mathcal{A}_{ijk}b_k$	$\Rightarrow$	index "k" disappears (index contraction)

  dot product between 2^nd^ order tensor $\textbf{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a 2^nd^ order tensor $\textbf{C}$

  $\textbf{A}\cdot\textbf{B}=\textbf{C}$	$\Rightarrow$	$C_{ik}=A_{ij}B_{jk}$	$\Rightarrow$	index "j" disappears (index contraction)

  > $\textbf{A}\cdot\textbf{B}\neq\textbf{B}\cdot\textbf{A}$
  >
  > ==REMARK== $\textbf{A}\cdot\textbf{A}=\textbf{A}^2$

* some **properties**:

  $\textbf{A}\cdot(\alpha\textbf{b}+\beta\textbf{c})=\alpha\textbf{A}\cdot\textbf{b}+\beta\textbf{A}\cdot\textbf{c}$	$\Rightarrow$	Linear operator

* **2^nd^ order unit** (or **identity**) **tensor**

  $\textbf{1}\cdot\textbf{u}=\textbf{u}\cdot\textbf{1}=\textbf{u}$

  $\begin{cases}\textbf{1}=\delta_{ij}\textbf{e}_i\otimes\textbf{e}_j=\textbf{e}_i\otimes\textbf{e}_i\\1_{ij}=\delta_{ij}\end{cases}$			$[\textbf{1}]=\begin{bmatrix}1&0&0\\0&1&0\\0&0&1\end{bmatrix}$

* some **properties**:

  $\textbf{1}\cdot\textbf{A}=\textbf{A}=\textbf{A}\cdot\textbf{1}$

  $\textbf{A}\cdot(\textbf{B}+\textbf{C})=\textbf{A}\cdot\textbf{B}+\textbf{A}\cdot\textbf{C}$

  $\textbf{A}\cdot(\textbf{B}\cdot\textbf{C})=(\textbf{A}\cdot\textbf{B})\cdot\textbf{C}=\textbf{A}\cdot\textbf{B}\cdot\textbf{C}$

  $\textbf{A}\cdot\textbf{B}\neq\textbf{B}\cdot\textbf{A}$

Example

when does the relation $\textbf{n}\cdot\textbf{T}=\textbf{T}\cdot\textbf{n}$ hold true?

* **transpose**

  $[\textbf{A}]=\begin{bmatrix}A_{11}&A_{12}&A_{13}\\A_{21}&A_{22}&A_{23}\\A_{31}&A_{32}&A_{33}\end{bmatrix}$	$\Rightarrow[\textbf{A}^T]=\begin{bmatrix}A_{11}&A_{21}&A_{31}\\A_{12}&A_{22}&A_{32}\\A_{13}&A_{23}&A_{33}\end{bmatrix}$

  $[\textbf{A}^T]_{ij}=\textbf{A}_{ij}$

  $\begin{cases}(\textbf{A}^T)^T=\textbf{A}\\(\textbf{A}\cdot\textbf{B})^T=\textbf{B}^T\cdot\textbf{A}^T\\(\textbf{u}\otimes\textbf{v})^T=\textbf{v}\otimes\textbf{u}\\(\alpha\textbf{A}+\beta\textbf{B})^T=\alpha\textbf{A}^T+\beta\textbf{B}^T\end{cases}$

* **trace**  yields a scalar

  $Tr(\textbf{A})=A_{ii}(=A_{11}+A_{22}+A_{33})$

  $Tr(\textbf{A}\otimes\textbf{B})=Tr[a_ib_j]=a_ib_i=\textbf{a}\cdot\textbf{b}$

  * some **properties**:

    $Tr\textbf{A}^T=Tr\textbf{A}$

    $Tr(\alpha\textbf{A})=\alpha Tr\textbf{A}$

    $Tr(\textbf{A}+\textbf{B})=Tr\textbf{A}+Tr\textbf{B}$

    $Tr(\textbf{A}\cdot\textbf{B})=Tr(\textbf{B}\cdot\textbf{A})$

* **double index contraction** or ==double (vertical) dot product== (:)

  double dot product between 2^nd^ order tensor $\textbf{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a zero order tensor (scalar) $c$

  $\textbf{A}:\textbf{B}=c$	$\Rightarrow c=A_{ij}B_{ij}$	$\Rightarrow$ indices "i,j" disappear (double index contraction)

  double dot product between 3^rd^ order tensor $\mathbfcal{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a 1^st^ order tensor $\textbf{c}$

  $\mathbfcal{A}:\textbf{B}=\textbf{c}$	$\Rightarrow\textbf{c}_{i}=\mathbfcal{A}_{ijk}\textbf{B}_{jk}$	$\Rightarrow$ indices "j,k" disappear (double index contraction)

  double dot product between 4^th^ order tensor $\mathbb{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a 2^nd^ order tensor $\textbf{C}$

  $\mathbb{A}:\textbf{B}=\textbf{C}$	$\Rightarrow\textbf{C}_{ij}=\mathbb{A}_{ijkl}\textbf{B}_{kl}$	$\Rightarrow$ indices "k,l" disappear (double index contraction)

  * **indices contiguous to the double-dot** (:) operator get vertically repeated (contraction) and they **disappear** in the resulting tensor (4 order reduction of the sum of orders).

  * **some properties**

    $\textbf{A}:\textbf{B}=Tr(\textbf{A}^T\cdot\textbf{B})=Tr(\textbf{B}^T\cdot\textbf{A})=Tr(\textbf{A}\cdot\textbf{B}^T)=Tr(\textbf{B}\cdot\textbf{A}^T)=\textbf{B}:\textbf{A}$

    $\textbf{1}:\textbf{A}=Tr\textbf{A}=\textbf{A}:\textbf{1}$

    $\textbf{A}:(\textbf{B}\cdot\textbf{C})=(\textbf{B}^T\cdot\textbf{A}):\textbf{C}=(\textbf{A}\cdot\textbf{C}^T):\textbf{B}$

    $\textbf{A}:(\textbf{u}\otimes\textbf{v})=\textbf{u}\cdot(\textbf{A}\cdot\textbf{v})$

    $(\textbf{u}\otimes\textbf{v}):(\textbf{w}\otimes\textbf{x})=(\textbf{u}\cdot\textbf{w})\cdot(\textbf{v}\cdot\textbf{w})$

    > ==REMARK== $\textbf{A}:\textbf{B}=\textbf{C}:\textbf{B}\not\Rightarrow\textbf{A}=\textbf{C}$

* **double index contraction** or ==double (horizontal) dot product== ($\cdot\cdot$)

  double dot product between 2^nd^ order tensor $\textbf{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a zero order tensor (scalar) $c$

  $\textbf{A}\cdot\cdot\textbf{B}=c$	$\Rightarrow$ $c=A_{ij}B_{ji}$ $\Rightarrow$ indices "i,j" disappear (double index contraction)

  double dot product between 3^rd^ order tensor $\mathbfcal{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a 1^st^ order tensor $\textbf{c}$

  $\mathbfcal{A}\cdot\cdot\textbf{B}=\textbf{c}$	$\Rightarrow$ $\textbf{c}_i=\mathcal{A}_{ijk}B_{kj}$ $\Rightarrow$  indices "j,k" disappear (double index contraction)

  double dot product between 4^th^ order tensor $\mathbb{A}$ and 2^nd^ order tensor $\textbf{B}$ yields a 2^nd^ order tensor $\textbf{C}$

  $\mathbb{A}\cdot\cdot\textbf{B}=\textbf{C}$	$\Rightarrow$ $\textbf{C}_{ij}=\mathbb{A}_{ijkl}B_{lk}$ $\Rightarrow$ indices "k,l" disappear (double index contraction)

  * **indices contiguous to the double-dot** ($\cdot\cdot$) operator get horizontally repeated (contraction) and they **disappear** in the resulting tensor (4 orders reduction of the sum of orders)

* ==**norm**== of a tensor is a non-negative real number defined by

  $\norm{\textbf{A}}=(\textbf{A}:\textbf{A})^\dfrac{1}{2}=(A_{ij}A_{ij})^\dfrac{1}{2}\ge0$

  $\textbf{A}\cdot\cdot\textbf{B}=Tr(\textbf{A}\cdot\textbf{B})=Tr(\textbf{B}\cdot\textbf{A})=\textbf{B}\cdot\cdot\textbf{A}$

  $\textbf{1}\cdot\cdot\textbf{A}=Tr\textbf{A}=\textbf{A}\cdot\cdot\textbf{1}$

  > ==REMARK== $\textbf{A}:\textbf{B}\neq\textbf{A}\cdot\cdot\textbf{B}$
  >
  > unless one of the two tensors is symmetric

example

prove that:

$\textbf{A}:\textbf{B}=Tr(\textbf{A}^T\cdot\textbf{B})$

$\textbf{A}\cdot\cdot\textbf{B}=Tr(\textbf{A}\cdot\textbf{B})$

* **determinant**	yields a scalar

  $\det\textbf{A}=\det[\textbf{A}]=\det\begin{bmatrix}A_{11}&A_{12}&A_{13}\\A_{21}&A_{22}&A_{23}\\A_{31}&A_{32}&A_{33}\end{bmatrix}=\varepsilon_{ijk}A_{1i}A_{2j}A_{3k}=\dfrac{1}{6}\varepsilon_{ijk}\varepsilon_{pqr}A_{pi}A_{qj}A_{rk}$

  * some **properties**:

    $\det(\textbf{A}\cdot\textbf{B})=\det\textbf{A}\cdot\det{\textbf{B}}$

    $\det\textbf{A}^T=\det\textbf{A}$

    $\det(\alpha\textbf{A})=\alpha^3\det\textbf{A}$

    > the tensor $\textbf{A}$ is **SINGULAR** if and only if $\det\textbf{A}=0$
    >
    > $\textbf{A}$ is **NONSINGULAR** if $\det\textbf{A}\neq0$.

* **inverse**

  there exists a **unique inverse** $\textbf{A}^{-1}$ of $\textbf{A}$ when $\textbf{A}$ is nonsingular, which satisfies the reciprocal relation:

  $\begin{cases}\textbf{A}\cdot\textbf{A}^{-1}=\textbf{1}=\textbf{A}^{-1}\cdot\textbf{A}\\A_{ik}A^{-1}_{kj}=A^{-1}_{ik}A_{kj}=\delta_{ij}\space\space\space i,j,k\in\{1,2,3\}\end{cases}$

### Differential operator

a **differential operator** is a mapping that transforms a field $\textbf{v(x)}$, $\textbf{A(x)}\dots$ into another fields by means of partial derivatives.

* the mapping is typically understood to be linear.
* examples:
  * Nabla operator
  * gradient
  * divergence
  * rotation
  * ...

* the **Nabla operator** $\nabla$ is a differential operator "symbolically" defined as:

  $\nabla\stackrel{symbolic}{=}\dfrac{\partial}{\partial\textbf{x}}\stackrel{symb.}{=}\dfrac{\partial}{\partial{x_i}}\hat{\textbf{e}_i}$

* in Cartesian coordinates, it can be used as a (symbolic) vector on its own:

  $[\nabla]\stackrel{symb.}{=}\begin{bmatrix}\dfrac{\partial}{\partial{x_1}}\\\dfrac{\partial}{\partial{x_2}}\\\dfrac{\partial}{\partial{x_3}}\end{bmatrix}$

#### Gradient

the **gradient** (or **open product of Nabla**) is a differential operator defined as:

* gradient of a scalar field $\Phi(\mathbf{x})$:

  * yields a vector

  $[\nabla\Phi]_i=[\nabla\otimes\Phi]_i=[\nabla]_i\Phi\stackrel{symb.}{=}\dfrac{\partial}{\partial{x_i}}\Phi=\dfrac{\partial\Phi}{\partial{x_i}}$  $i\in\{1,2,3\}$

  $\nabla\Phi=[\nabla\Phi]_i\hat{\mathbf{e}}_i=\dfrac{\part\Phi}{\part x_i}\hat{\mathbf{e}}_i$

  > $\nabla\Phi=\dfrac{\part\Phi}{\part x_i}\hat{\mathbf{e}}_i$

* gradient of a vector field $\mathbf{v(x)}$:

  * yields a 2^nd^ order tensor

  $[\nabla\otimes\mathbf{v}]_{ij}=[\nabla]_i[\mathbf{v}]_j\stackrel{symb.}{=}\dfrac{\part}{\part{x_i}}\text{v}_j=\dfrac{\part{\text{v}_j}}{\part{x_i}}$    $i,j\in\{1,2,3\}$
  
  $\nabla\textbf{v}=\nabla\otimes\textbf{v}=[\nabla\otimes\textbf{v}]_{ij}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j=\dfrac{\part\text{v}_j}{\part{x}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j$
  
  >$\nabla\textbf{v}=\dfrac{\part\text{v}_j}{\part{x}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j$
  
* gradient of a 3^nd^ order tensor field $\textbf{A(x)}$:

  * yields a 3^rd^ order tensor

  $[\nabla\textbf{A}]_{ijk}=[\nabla\otimes\textbf{A}]_{ijk}=[\nabla]_i[\textbf{A}]_{jk}\stackrel{symb.}{=}\dfrac{\part}{\part{x_i}}\text{A}_{jk}=\dfrac{\part{\text{A}_{jk}}}{\part{x_i}}$    $i,j,k\in\{1,2,3\}$

  $\nabla\textbf{A}=\nabla\otimes\textbf{A}=[\nabla\otimes\textbf{A}]_{ijk}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j\otimes\hat{\textbf{e}}_k=\dfrac{\part{\text{A}_{jk}}}{\part{x_i}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j\otimes\hat{\textbf{e}}_k$

  > $\nabla\textbf{A}=\dfrac{\part{\text{A}_{jk}}}{\part{x_i}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j\otimes\hat{\textbf{e}}_k$

#### Divergence

the **divergence** (or **dot product of Nabla**) is a differential operator defined as:

* divergence of a vector field $\textbf{v(x)}$:

  * yields a scalar

  $\nabla\cdot\textbf{v}=[\nabla]_i[\textbf{v}]_i\stackrel{symb.}{=}\dfrac{\part}{\part{x_i}}\text{v}_i=\dfrac{\part{\text{v}_i}}{\part{x_i}}$

  >$\nabla\cdot\textbf{v}=\dfrac{\part{\text{v}_i}}{\part{x_i}}$

* divergence of a 2^nd^ order tensor $\textbf{A(x)}$:

  * yields a vector

  $[\nabla\cdot\textbf{A}]_j=[\nabla]_i[\textbf{A}]_{ij}\stackrel{symb.}{=}\dfrac{\part}{\part{x_i}}\text{A}_{ij}=\dfrac{\part{\text{A}_{ij}}}{\part{x_i}}$

  $\nabla\cdot\textbf{A}=[\nabla\cdot\textbf{A}]_j\hat{\textbf{e}}_j=\dfrac{\part{\text{A}_{ij}}}{\part{x_i}}\hat{\textbf{e}}_j$

  > $\nabla\cdot\textbf{A}=\dfrac{\part{\text{A}_{ij}}}{\part{x_i}}\hat{\textbf{e}}_j$

* the divergence can only be performed on tensors of order 1 or higher.

* if $\nabla\cdot\textbf{v}=0$, the vector field $\textbf{v(x)}$ is said to be **solenoid** (or **divergence-free**)

#### Rotation

the **rotation** or **curl** (**or vector product of Nabla**) is a differential operator defined as:

* rotation of a vector field $\textbf{v(x)}$:

  * yields a vector

  $[\nabla\cross\textbf{v}]_i\stackrel{symb.}{=}\varepsilon_{ijk}[\nabla]_j[\textbf{v}]_k\stackrel{symb.}{=}\varepsilon_{ijk}\dfrac{\part}{\part{x_j}}\text{v}_k=\varepsilon_{ijk}\dfrac{\part\text{v}_k}{\part{x_j}}$    $i\in\{1,2,3\}$

  $\nabla\cross\textbf{v}=[\nabla\cross\textbf{v}]_i\hat{\textbf{e}}_i=\varepsilon_{ijk}\dfrac{\part\text{v}_k}{\part{x_j}}\hat{\textbf{e}}_i$

  > $\nabla\cross\textbf{v}=\varepsilon_{ijk}\dfrac{\part\text{v}_k}{\part{x_j}}\hat{\textbf{e}}_i$

* rotation of a 2^nd^ order tensor $\textbf{A(x)}$:

  * yields a $2^nd^ order tensor

  $[\nabla\cross\textbf{A}]_{il}\stackrel{symb.}{=}\varepsilon_{ijk}\dfrac{\part}{\part{x_j}}\text{A}_{kl}=\varepsilon_{ijk}\dfrac{\part\text{A}_{kl}}{\part{x_j}}$    $i,j,k\in\{1,2,3\}$

  $\nabla\cross\textbf{A}=[\nabla\cross\textbf{A}]_{il}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j=\varepsilon_{ijk}\dfrac{\part\text{A}_{kl}}{\part{x_j}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j$

  > $\nabla\cross\textbf{A}=\varepsilon_{ijk}\dfrac{\part\text{A}_{kl}}{\part{x_j}}\hat{\textbf{e}}_i\otimes\hat{\textbf{e}}_j$

* the rotation can only be performed on tensors of order 1 or higher

* if $\nabla\cross\textbf{v}=0$, the vector field $\textbf{v(x)}$ is said to be **irrotational** (or **curl-free**)

|                | **scalar field** $\Phi(\textbf{x})$                          | **vector field** $\textbf{v(x)}$                             | **2^nd^ order tensor** $\textbf{A(x)}$                       |
| -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **GRADIENT**   | $[\nabla\otimes\Phi]_i=\\=[\nabla\Phi]_i=\dfrac{\part{\Phi}}{\part{x_i}}$ | $[\nabla\otimes\mathbf{v}]_{ij}=\\=[\nabla\mathbf{v}]_{ij}=\dfrac{\part{\text{v}_j}}{\part{x_i}}$ | $[\nabla\otimes\textbf{A}]_{ijk}=\\=[\nabla\textbf{A}]_{ijk}=\dfrac{\part{\text{A}_{jk}}}{\part{x_i}}$ |
| **DIVERGENCE** |                                                              | $\nabla\cdot\textbf{v}=\dfrac{\part{\text{v}_i}}{\part{x_i}}$ | $[\nabla\cdot\textbf{A}]_j=\dfrac{\part{\text{A}_{ij}}}{\part{x_i}}$ |
| **ROTATION**   |                                                              | $\nabla\cross\textbf{v}=\varepsilon_{ijk}\dfrac{\part\text{v}_k}{\part{x_j}}$ | $\nabla\cross\textbf{A}=\varepsilon_{ijk}\dfrac{\part\text{A}_{kl}}{\part{x_j}}$ |

example

given the vector $\textbf{v}=\textbf{v(x)}=x_1x_2x_3\hat{\textbf{e}}_1+x_1x_2\hat{\textbf{e}}_2+x_1\hat{\textbf{e}}_3$, determine $\nabla\cdot\textbf{v}$, $\nabla\cross\textbf{v}$, and $\nabla\textbf{v}$.

$\textbf{v}=\begin{bmatrix}\text{v}_1\\\text{v}_2\\\text{v}_3\end{bmatrix}=\begin{bmatrix}x_1x_2x_3\\x_1x_2\\x_1\end{bmatrix}$

$\Rightarrow$ $\nabla\cdot\textbf{v}=\dfrac{\part{\text{v}_1}}{\part{x_1}}+\dfrac{\part{\text{v}_2}}{\part{x_2}}+\dfrac{\part{\text{v}_3}}{\part{x_3}}\\=x_2x_3+x_1$

$\Rightarrow$ $\nabla\cross\textbf{v}=\hat{\textbf{e}}_1\dfrac{\part{\text{v}_3}}{\part{x_2}}+\hat{\textbf{e}}_2\dfrac{\part{\text{v}_1}}{\part{x_3}}+\hat{\textbf{e}}_3\dfrac{\part{\text{v}_2}}{\part{x_1}}-\hat{\textbf{e}}_3\dfrac{\part{\text{v}_1}}{\part{x_2}}-\hat{\textbf{e}}_2\dfrac{\part{\text{v}_3}}{\part{x_1}}-\hat{\textbf{e}}_1\dfrac{\part{\text{v}_2}}{\part{x_3}}=\\=(x_1x_2-1)\hat{\textbf{e}}_2+(x_2-x_1x_3)\hat{\textbf{e}}_3$

$\Rightarrow$ $\nabla\textbf{v}=\begin{bmatrix}\dfrac{\part{\text{v}_1}}{\part{x_1}}&\dfrac{\part{\text{v}_2}}{\part{x_1}}&\dfrac{\part{\text{v}_3}}{\part{x_1}}\\\dfrac{\part{\text{v}_1}}{\part{x_2}}&\dfrac{\part{\text{v}_2}}{\part{x_2}}&\dfrac{\part{\text{v}_3}}{\part{x_2}}\\\dfrac{\part{\text{v}_1}}{\part{x_3}}&\dfrac{\part{\text{v}_2}}{\part{x_3}}&\dfrac{\part{\text{v}_3}}{\part{x_3}}\end{bmatrix}=$

$= \begin{bmatrix}x_2x_3&x_2&1\\x_1x_3&x_1&0\\x_1x_2&0&0\end{bmatrix}$

## Integral Theorems

### Divergence or Gauss Theorem

* given a field $\textbf{A}$ in a volume $V$ with closed boundary surface $\part{V}$ and unit **outward** normal to the boundary $\textbf{n}$, the **Divergence** (or **Gauss**) **Theorem** states:

  > $\int_V{\nabla\cdot\textbf{A }dV}=\int_{\part{V}}{\textbf{n}\cdot\textbf{A }dS}$
  >
  > $\int_V{\textbf{A}\cdot\nabla\space{dV}}=\int_{\part{V}}{\textbf{A}\cdot\textbf{n}\space{dS}}$

  where:

* $\textbf{A}$ represents either a vector field ($\textbf{v(x)}$) or a tensor field ($\textbf{A(x)}$). 

### Generalized Divergence Theorem

* given a field $\textbf{A}$ in a volume $V$ with closed boundary surface $\part{V}$ and unit outward normal to the boundary $\textbf{n}$, the **Generalized Divergence Theorem** states:

  > $\int_V{\nabla\ast\textbf{A }dV}=\int_{\part{V}}{\textbf{n}\ast\textbf{A }dS}$
  >
  > $\int_V{\textbf{A}\ast\nabla\space{dV}}=\int_{\part{V}}{\textbf{A}\ast\textbf{n}\space{dS}}$

  where:

* $\ast$ represents either the dot product ($\cdot$), the cross product ($\cross$) or the tensor product ($\otimes$).

* $\textbf{A}$ represents either a scalar field ($\phi(\textbf{x})$), a vector field ($\textbf{v(x)}$) or a tensor field ($\textbf{A(x)}$).

example

use the Generalized Divergence Theorem to show that

$$\int_S{x_in_jdS}=V\delta_{ij}$$

where $x_i$ is the position vector of $n_j$.

>$\int_{\part{V}}{\textbf{A}\ast\textbf{n}\space{dS}}=\int_V{\textbf{A}\ast\nabla\space{dV}}$

### Curl or Stokes Theorem

* given a vector field $\textbf{u}$ in a surface $S$ with closed boundary surface $\part{\text{S}}$ and unit outward normal to the boundary $\textbf{n}$, the **Curl** (or **Stokes**) **Theorem** states:

  $\int_S{(\nabla\cross\textbf{u})\cdot{\textbf{n }}dV}=\int_{\part{S}}{\textbf{u}\cdot d\textbf{r}}$

  where the curve of the line integral must have positive orientation, such that $d\textbf{r}$ points counter-clockwise when the unit normal points to the viewer, following the right-hand rule.
