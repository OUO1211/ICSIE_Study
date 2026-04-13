# 3-4 矩陣的秩

本節討論一個矩陣的重要參數 rank，但需先借用第四章的結果 Sylvester 定理：
$$
n=\dim(CS(A))+\dim(\ker(A)),
$$
其中 $A$ 為 $m\times n$ 矩陣。目前先享用這個定理帶來的好處，將來認識了線性映射後會嚴謹地證明此定理。

## 列秩(row rank)與行秩(column rank)

> **定義**
>
> 考慮矩陣 $A$，
>
> (1) $\dim(RS(A))$ 稱為 $A$ 的列秩，記做 $rr(A)$。
>
> (2) $\dim(CS(A))$ 稱為 $A$ 的行秩，記做 $cr(A)$。

> **Note**
>
> (1) 對 $A$ 做列運算化成列梯形矩陣後所得非零列數即為 $rr(A)$。
>
> (2) 對 $A$ 做行運算化成行梯形矩陣後所得非零行數即為 $cr(A)$。
>
> (3) $A$ 中各列向量線性獨立 $\Leftrightarrow rr(A)=m$。
>
> (4) $A$ 中各行向量線性獨立 $\Leftrightarrow cr(A)=n$。

例如：

(1) $A=\begin{bmatrix}1&2&3\\-1&2&1\\3&1&2\end{bmatrix}\rightarrow\begin{bmatrix}1&0&0\\-1&4&4\\3&-5&-7\end{bmatrix}$，三個非零行，故 column rank$(A)=3$。

(2) $A=\begin{bmatrix}1&2&3\\-1&2&1\\3&1&2\end{bmatrix}\rightarrow\begin{bmatrix}1&2&3\\0&4&4\\0&-5&-7\end{bmatrix}\rightarrow\begin{bmatrix}1&2&3\\0&4&4\\0&0&-2\end{bmatrix}$，三個非零列，故 row rank$(A)=3$。

(3) The row rank of $\begin{bmatrix}1&3&4\\2&-1&1\\3&2&5\\5&15&20\end{bmatrix}$ is 2. 【99 中興資料】

(4) The row rank of $\begin{bmatrix}1&2&1&3\\2&3&-1&-6\\3&-2&-4&-2\end{bmatrix}$ is 3. 【99 中興資料】