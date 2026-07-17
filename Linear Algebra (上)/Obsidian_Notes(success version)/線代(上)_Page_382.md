## 矩陣的秩(rank)

> **定理**
>
> 對任意矩陣 $A$，$rr(A)=cr(A)$，且稱此為 $A$ 的秩，記成 $\text{rank}(A)$。

> **【證明】**
>
> 令 $A:m \times n$，由 Sylvester 定理可得，$n=\dim(\ker(A))+\dim(CS(A))$。
>
> 設 $\dim(\ker(A))=k$，則得 $cr(A)=n-k$ ……(1)
>
> 另一方面，$\dim(\ker(A))=k$，表示 $\ker(A)$ 的基底中有 $k$ 個向量，
>
> 即解 $Ax=0$ 時，$x$ 有 $k$ 個自由變數，$n-k$ 個基本變數，
>
> 即 $A$ 做列運算後，最後得 $n-k$ 個非零列，
>
> 即 $\dim(RS(A))=rr(A)=n-k$ ……(2)
>
> 比較 (1)(2)，故得 $cr(A)=rr(A)$。

> **Note**
>
> 求 $\text{rank}(A)$ 時，除了常用 $rr(A)$、$cr(A)$ 之外，最常應用的就是 **Sylvester Theorem**：
>
> 設矩陣 $A:m \times n$ 則
>
> $$n=\dim(\ker(A))+\dim(CS(A))=\dim(\ker(A))+\text{rank}(A).$$
>
> $$m=\dim(\ker(A^t))+\dim(CS(A^t))=\dim(\ker(A^t))+\text{rank}(A).$$

> **例題 1**
>
> (8%) Find the rank and nullity of the matrix
>
> $$\begin{bmatrix}1&0&1&-1&6\\2&-1&5&-1&7\\-1&1&-4&1&-3\\0&1&-3&1&1\end{bmatrix}$$
>
> 【105 政大資科甲類題、107 師大資工】

解：

$$\text{rank}\begin{bmatrix}1&0&1&-1&6\\2&-1&5&-1&7\\-1&1&-4&1&-3\\0&1&-3&1&1\end{bmatrix}=\cdots=\text{rank}\begin{bmatrix}1&0&1&-1&6\\0&1&-3&-1&5\\0&0&0&1&-2\\0&0&0&0&0\end{bmatrix}=3,$$

再由 Sylvester 定理：$\text{nullity}(A)=$ 行數 $-\text{rank}(A)=5-3=2$。