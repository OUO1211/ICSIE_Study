## 第 4 章 線性映射 567

## 兩向量空間的同構(isomorphic)

> **定義**
>
> 若兩向量空間 $F$ 中的 $V$ 與 $V'$ 間存在一線性映射，使得 $T: V \to V'$，且 $T$ 為 1-1 onto，則稱 $V$ 與 $V'$ 同構，記為 $V \cong V'$，也稱 $T$ 為同構映射。

例如：

(1) $R^{2 \times 2} \cong R^4$，

可取函數 $f: R^{2 \times 2} \to R^4$，其中 $f\begin{pmatrix}\begin{bmatrix}a&b\\c&d\end{bmatrix}\end{pmatrix} = \begin{pmatrix}a\\b\\c\\d\end{pmatrix}$，

明顯可得 $f$ 為一線性映射且為 1-1, onto。

(2) $R^{m \times n} \cong R^{mn}$，

可取函數 $f: R^{m \times n} \to R^{mn}$，其中 $\begin{pmatrix}a\\b+ax+cx^2\end{pmatrix}$，

明顯可得 $f$ 為一線性映射且為 1-1, onto。

> **Note** 座標同構映射(coordinate isomorphism)
>
> 令 $\beta$ 為向量空間 $V$ 的一有序基底，定義 $\phi_\beta: V \to F^n$ 為 $\phi_\beta(v) = [v]_\beta$，$\forall v \in V$。
>
> (a) $\phi_\beta$ 為線性映射。 【101 成大應數】
>
> (b) $(v_1, \ldots, v_k)$ 線性獨立 $\Leftrightarrow$ $(\phi_\beta(v_1), \ldots, \phi_\beta(v_k))$ 線性獨立。
>
> (c) 考慮有限維向量空間 $V, V'$，則 $V \cong V' \Leftrightarrow \dim(V) = \dim(V')$。 【矩陣"同構"】【100 交大資工、103 加拿大通訊】
>
> (2) 若 $\dim(V) = \dim(V')$，在有限維的情況下，$T: V \to V'$ 滿足 $T(A) = \dim(T)$，得知 $T$ 為 1-1 onto。
>
> $\because \dim(V) = n$，令 $\{A_1, A_k\}$ 分別為 $V$ 與 $V'$ 的基底，
>
> 且 $\text{Im}(T) = \text{span}(T(A_1), \ldots, T(A_k))$，將其擴充成 $V'$ 的一組基底，
>
> 又因 $\dim(\text{Im}(T)) = \dim(V') = n$，故 $T$ 為 onto，
>
> 又因 $\dim(\ker(T)) = \dim(V) - \dim(\text{Im}(T)) = n - n = 0$，故 $T$ 為 1-1。
>
> 故得 $V \cong V'$。
