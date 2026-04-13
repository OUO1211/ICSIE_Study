## 584 線性代數(上)

> **試題 11**
>
> Let $T: R^n \to R^n$ be a linear transformation with the property that $T(T(x)) = T(x)$ for every vector $x \in R^n$.
>
> (1) (5%) Write $V$ for the range of $T$, in other words, $V = \{T(x) \mid x \in R^n\}$. If $x \in V$, then what is $T(x)$?
>
> (2) (5%) If $x \in R^n$, then what is $T(x - T(x))$?
>
> (3) (5%) Let $\{v_1, \ldots, v_k\}$ be a basis for $V$, then we can add some more vectors $u_1, \ldots, u_l$ to get a basis $\beta$ for $R^n$. Show that if you replace $u_i$ with $u_i - T(u_i)$, you still have a basis.
>
> (4) (5%) In the same way, can replace each $u_i$ with $u_i - T(u_i)$. What is the matrix of $T$ with respect to the basis $\{v_1, \ldots, v_k, u_1 - T(u_1), \ldots, u_l - T(u_l)\}$?
>
> 【105 政大應數】

**解：**

$\because T^2 = T$，即 $T$ 為 idempotent，$\therefore \lambda = 0$ 或 $1$，

且 $\operatorname{Im}(T) = V(1)$，$\ker(T) = V(0)$，$R^n = \operatorname{Im}(T) \oplus \ker(T)$。

(1) $x \in V = \operatorname{Im}(T) = V(1)，\therefore T(x) = x$。

(2) $T(T(x) - x) = T(T(x)) - T(x) = T(x) - T(x) = 0$。

(3) $\{v_1, \ldots, v_k\}$ 為 $V = V(1)$ 的一組基底，

由命(2) $u_1 - T(u_1), \ldots, u_l - T(u_l)$ 為 $\ker(T) = V(0)$ 的一組基底，

再由 $R^n = \operatorname{Im}(T) \oplus \ker(T)，\therefore \{v_1, \ldots, v_k, u_1 - T(u_1), \ldots, u_l - T(u_l)\}$ 為 $R^n$ 的一組基底。

(4) $\because T(v_i) = v_i,\ \text{for } i = 1 \sim k,\ T(u_j - T(u_j)) = 0 = 0(u_j - T(u_j)),\ \text{for } j = 1 \sim l,$

$$
[T] =
\begin{bmatrix}
I_k & 0 \\
0 & O_l
\end{bmatrix}
$$