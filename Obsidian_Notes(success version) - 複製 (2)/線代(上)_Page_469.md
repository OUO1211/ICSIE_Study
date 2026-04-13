## 特殊的線性映射 — 冪等算子3(idempotent operator)與冪等矩陣(idempotent matrix)

> **定義**
>
> 若 $V$ 上的算子 $T$ 滿足 $T^2 = T$，則稱 $T$ 為一冪等算子（也稱投影算子）。
>
> 若方陣 $A$ 滿足 $A^2 = A$，則稱 $A$ 為一冪等矩陣（也稱投影矩陣）。

> **Note**
>
> (1) 例如：$A=\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$，$B=\begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$，$C=\begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$ 都是投影矩陣。
>
> (2) $T^{(v)}=T(T(v))$，表示 $T$ 與 $T$ 的合成，後面會再定義。
>
> (3) 例如，$T:R^{2\times 2}\to R^{2\times 2}$ 定義為 $T(A)=\dfrac{A+A^T}{2}$，則為 $R^{2\times 2}$ 上的一投影算子。
>
> 【證明】
>
> $$T^2(X)=T(T(X))=T\left(\dfrac{X+X^T}{2}\right)=\dfrac{1}{2}\left(\dfrac{X+X^T}{2}+\left(\dfrac{X+X^T}{2}\right)^T\right)$$
>
> $$=\dfrac{X+X^T+X^T+X}{4}=\dfrac{X+X^T}{2}=T(X)，\therefore T^2=T。$$
>
> (4) 例如：$H=I_n-\dfrac{1}{n}J_n$ 即為一冪等矩陣，其中 $J_n$ 為全 $1$ 的 $n$ 階方陣。
>
> 【101 高雄統計】