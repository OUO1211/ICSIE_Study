# 第 1 章 矩陣

15

> **例** 3
>
> Let $A=\begin{bmatrix}1 & 1 & 1 \\ 0 & 1 & 1 \\ 0 & 0 & 1\end{bmatrix}$. Guess a general formula for $A^n$ and prove it by induction.
>
> $[106\ \text{成大統計}]$

解　猜測
$$
A^n=\begin{bmatrix}1 & n & 1+2+\cdots+n \\ 0 & 1 & n \\ 0 & 0 & 1\end{bmatrix}。
$$

$n=1$ 時，明顯成立，

假設 $n=k\geq 1$ 時此猜測正確，

則 $n=k+1$ 時，
$$
A^{k+1}=AA^k=\begin{bmatrix}1 & 1 & 1 \\ 0 & 1 & 1 \\ 0 & 0 & 1\end{bmatrix}\begin{bmatrix}1 & k & 1+2+\cdots+k \\ 0 & 1 & k \\ 0 & 0 & 1\end{bmatrix}=\begin{bmatrix}1 & k+1 & 1+2+\cdots+k+(k+1) \\ 0 & 1 & k+1 \\ 0 & 0 & 1\end{bmatrix}。
$$

故如此猜測正確

> **例** 4
>
> $(10\%)$ Show that $H=I_p-\dfrac{1}{p}J_p$ is idempotent（冪等，滿足 $H^2=H$），where $J_p$ is a matrix of ones with order $p\times p$.
>
> $[101\ \text{高雄統計}、102\ \text{中正統計}、102\ \text{中央統計}]$

解
$$
H^2=\left(I_p-\frac{1}{p}J_p\right)\left(I_p-\frac{1}{p}J_p\right)
$$
$$
=I_p-\frac{1}{p}J_p-\frac{1}{p}J_p+\frac{1}{p^2}J_pJ_p
$$
$$
=I_p-\frac{2}{p}J_p+\frac{p}{p^2}J_p，\ \text{其中，}\ J_pJ_p=pJ_p，
$$
$$
=I_p-\frac{1}{p}J_p=H
$$

故 $H$ 為冪等矩陣