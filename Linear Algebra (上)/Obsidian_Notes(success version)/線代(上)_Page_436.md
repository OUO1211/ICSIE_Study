（接上頁試題 4，$R^\infty$ 為向量空間的驗證）

(3) 具向量加法反元素：

$\forall \{a_n\} \in R^\infty$，取 $-v = \{-a_n\} \in R^\infty$，則 $v + (-v) = \{0_n\} = (-v) + v$。

(4) 向量加法具交換性：

$\forall \{a_n\}, \{b_n\} \in R^\infty$，$u + v = \{a_n + b_n\} = \{b_n + a_n\} = v + u$。

(5) 純量乘積對向量加法有分配性：

$\forall \alpha \in R$，$u = \{a_n\}$，$v = \{b_n\} \in R^\infty$，$\alpha(u + v) = \{(a_n + b_n)\alpha\} = \{\alpha a_n + \alpha b_n\} = (\alpha \cdot u) + (\alpha \cdot v)$。

(6) 純量乘積對純量加法有分配性：

$\forall \alpha, \beta \in R$，$v = \{a_n\} \in R^\infty$，$(\alpha + \beta) \cdot v = \{(\alpha + \beta) a_n\} = \{\alpha a_n + \beta a_n\} = (\alpha \cdot v) + (\beta \cdot v)$。

(7) 純量乘積純量乘法具結合性：

$\forall \alpha, \beta \in R$，$\{a_n\} \in R^\infty$，$(\alpha\beta) \cdot \{a_n\} = \{(\alpha\beta) a_n\} = \alpha \cdot (\beta \cdot \{a_n\})$。

(8) 單位純量乘積的不變性：

$\forall v = \{a_n\} \in R^\infty$，$1 \cdot v = \{1 \cdot a_n\} = \{a_n\} = v$。

故 $(R^\infty, +, \cdot)$ 為佈於 $R$ 的向量空間。

> **試題 5**
>
> Let $A$ be the coefficient matrix of a homogeneous system of $m$ linear equations in $n$ unknowns $x_1, \ldots, x_n$. Show that if we include one more equation, $c_1 x_1 + \cdots + c_n x_n = 0$ in the system, the dimension of the solution space will decrease by one if the vector $(c_1, \ldots, c_n)$ cannot be spanned by the row vectors of $A$.
>
> 【106 清水進數】

解：考慮此等係數矩陣增加一列後的矩陣 $A'$，因為多增加一列（無法被前幾列線性組合），

故 $\text{rank}(A')$ 會增加 1，而由 Sylvester 定理，$\ker(A')$ 的維度就會少 1，即方程式的解空間維度少 1。

> **試題 6**
>
> Show that: Let $U$, $V$, and $W$ be subspaces of some vector space $X$ and $U$ is a subset of $W$. Then $(U + V) \cap W = U + (V \cap W)$.

解：

（$\subseteq$）：任取 $x \in (U + V) \cap W$，

則存在 $u \in U$，$v \in V$，故 $x = u + v \in U + V$，且 $x \in W$，

又 $u \in U \subseteq W$，故 $v = x - u \in W$，

$\therefore v \in V \cap W$，故 $x = u + v \in U + (V \cap W)$。

（$\supseteq$）：任取 $x \in U + (V \cap W)$，

則存在 $u \in U$，$v \in V \cap W$，故 $x = u + v$，

又 $u \in U \subseteq V$，故 $x = u + v \in U + V$，

又 $u \in U \subseteq W$，$v \in W$，故 $x = u + v \in W$，

$\therefore x \in (U + V) \cap W$。
