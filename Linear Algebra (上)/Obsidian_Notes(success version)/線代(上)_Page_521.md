## 530 線性代數(上)

## 線性映射的核空間(kernel)與值域(range)

> **定義**
>
> 令 $T$ 為向量空間 $V$ 至 $V'$ 的一線性映射。
>
> 定義 $\ker(T) = \{v \in V\mid T(v) = 0\} = \{A \in \ker(T)\}$ 稱為 $T$ 的核空間，也記為 $\text{Null}(T)$，$N(T)$。
>
> 定義 $\text{Im}(T) = \{T(v) \mid v \in V\}$ 稱為 $T$ 的值域，也記為 $\text{Range}(T)$，$R(T)$。

例如：

$T: R^2 \to R^2$，定義為 $T\begin{pmatrix}x\\y\end{pmatrix} = \begin{bmatrix}1\\0\end{bmatrix}$

$\ker(T) = \text{Range}(T) = \text{span}\begin{pmatrix}0\\1\end{pmatrix}$，$\ker(T) = \text{Null}(T) = \text{span}\begin{pmatrix}0\\1\end{pmatrix}$

> **Note**
>
> (1) $\ker(T)$ 為 $V$ 的子空間，目維度也記為 $\text{nullity}(T)$。
>
> 【101 成大應數 105 台大資工】
>
> (2) $\text{Im}(T)$ 為 $V'$ 的子空間，且 $\dim(\text{Im}(T)) = \text{rank}(T)$，$\dim(\text{ker}(T)) = \text{nullity}(T)$。
>
> (3) **Sylvester 維度定理**：令 $T$ 為有限維向量空間 $V$ 至 $V'$ 的一線性映射，則 $\text{rank}(T) + \text{nullity}(T) = \dim(\text{ker}(T)) + \dim(\text{Im}(T)) = \dim(V)$

> **【證明】**
>
> 設 $\dim(V) = r$，$\{u_1, \ldots, u_k\}$ 為 $\ker(T)$ 的一組基底，$\{w_1, \ldots, w_r\}$ 為 $V$ 的某組基底，且 $15 \le r$。
>
> 故由 $\{u_1, \ldots, u_k, w_1, \ldots, w_{r-k}\}$ 為 $V$ 的一組基底。
>
> 使用 $T(v) = a_1 u_1 + a_2 u_2 + \cdots + \sum a_i u_i = T(v) = \sum \left(\sum a_i\right) T(v_i)$，
>
> 即存在 $T(w_1), \ldots, T(w_r) \in T(S)$，任何零等於的純量 $\alpha_1, \ldots, \alpha_r$，故 $\sum \alpha_i T(v_i) = 0$，
>
> 故 $T(v) = \sum \alpha_i w_i \in \ker(T)$，即可得 $\sum \alpha_i w_i = \sum \alpha_j u_j$，
>
> 所以存在純量 $\mu_1, \ldots, \mu_r$，以使得 $\sum \alpha_i u_i = 0$，即 $\alpha_i = 0$，$\forall i$。
