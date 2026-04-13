## 576 線性代數(上)

## 4-6 進階試題練習

> **試題 1**
>
> (12%) Let $V$ and $W$ be vector spaces over a field $F$. Let $T: V \to W$ be a function satisfying $T(x + y) = T(x) + T(y)$. If $F$ is the set of rational numbers, then prove or disprove that $T$ is a linear transformation from $V$ to $W$.
>
> 【101 交大應數】

**解**

只需再證明 $T$ 滿足保持係數：

$\forall c \in \mathbb{Q}$（有理數集），$\forall x \in V$，$T(cx) = cT(x)$：

若若 $c = 0$，則明顯成立。

否則，令 $c = \dfrac{q}{p}$，其中 $p, q \in \mathbb{Z}$，

則
$$
T(cx)=T\left(\frac{q}{p}x\right)=T\left(\frac{x}{p}+\cdots+\frac{x}{p}\right)=T\left(\frac{x}{p}\right)+\cdots+T\left(\frac{x}{p}\right)=qT\left(\frac{x}{p}\right),
$$

$\therefore T(x)=T\left(p\cdot \dfrac{x}{p}\right)=pT\left(\dfrac{x}{p}\right)$，即 $\dfrac{1}{p}T(x)=T\left(\dfrac{x}{p}\right)$，

$\therefore T(cx)=T\left(\dfrac{q}{p}x\right)=q \cdot T\left(\dfrac{x}{p}\right)=q \cdot \dfrac{1}{p}T(x)=cT(x)$。

> **試題 2**
>
> (10%) Let $W_1$, $W_2$ be subspaces of $R^3$, where $W_1 = \text{span}\{(1,0,0), (1,0,1)\}$ and $W_2 = \text{span}\{(1,1,1)\}$. Let $T: R^3 \to R^3$ be the projection on $W_1$ along $W_2$. Let $\beta$ be the standard ordered basis for $R^3$. Find the matrix representation $[T]_\beta$ for $T$.
>
> 【107 政大應數】

**解**

$(1,0,0) = 1 \cdot (1,0,0) + 0 \cdot (1,0,1) + 0 \cdot (1,1,1)$，

$(0,1,0) = 0 \cdot (1,0,0) - 1 \cdot (1,0,1) + 1 \cdot (1,1,1)$，

$(0,0,1) = -1 \cdot (1,0,0) + 1 \cdot (1,0,1) + 0 \cdot (1,1,1)$，

$T(1,0,0) = (1,0,0) = 1 \cdot (1,0,0) + 0 \cdot (0,1,0) + 0 \cdot (0,0,1)$，

$T(0,1,0) = (-1,0,-1) = -1 \cdot (1,0,0) + 0 \cdot (0,1,0) - 1 \cdot (0,0,1)$，

$T(0,0,1) = (0,0,1) = 0 \cdot (1,0,0) + 0 \cdot (0,1,0) + 1 \cdot (0,0,1)$，

$$
\therefore [T]_\beta =
\begin{bmatrix}
1 & -1 & 0 \\
0 & 0 & 0 \\
0 & -1 & 1
\end{bmatrix}.
$$