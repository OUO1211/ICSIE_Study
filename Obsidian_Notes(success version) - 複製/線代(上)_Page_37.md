## 方陣的跡數 (trace)

> **定義：跡數 (trace)**
>
> 方陣 $A$ 的跡數 $\text{trace}(A)$ 定義為 $A$ 的對角項之和。 〔108 中正應數〕

**Note**

(1) $\text{trace}(A)$ 有時也記成 $\text{tr}(A)$。

(2) $\text{tr}(I_n)=n$。

例如：

$A=\begin{bmatrix} 1 & 4 \\ 2 & 3 \end{bmatrix}$，則 $\text{trace}(A)=1+3=4$；

$B=\begin{bmatrix} 9 & -1 & 2 & 3 \\ -4 & 5 & 3 & 2 \\ 1 & 6 & -7 & 2 \\ 3 & 9 & 2 & 1 \end{bmatrix}$，則 $\text{trace}(B)=9+5-7+1=8$。

## 跡數的性質

> **定理：跡數的性質**
>
> 若實係數 $n$ 階方陣 $A,B$，與純量係數 $\alpha,\beta$ 則
>
> (1) $\text{tr}(\alpha A+\beta B)=\alpha \text{tr}(A)+\beta \text{tr}(B)$。即 $\text{tr}(\cdot)$ 為一線性函數。
>
> (2) $\text{tr}(A^T)=\text{tr}(A)$。
>
> (3) $\text{tr}(A^H)=\overline{\text{tr}(A)}$。
>
> (4) $\text{tr}(AB)=\text{tr}(BA)$。 【重要】
>
> (5) $\text{tr}(AB)=\text{tr}(A)\text{tr}(B)$ 不恆成立。 〔105 台大資工、108 清大統計〕
>
> (6) $\text{tr}(A^n)=(\text{tr}(A))^n$ 不恆成立。
>
> (7) $\text{tr}(A^T A)=A$ 的各元素的平方和。

**【證明】**

從定義可看出 (1)-(3) 明顯成立。

(4) 設 $A=[a_{ij}]_{m\times n}$、$B=[b_{ij}]_{n\times m}$、$C=[c_{ij}]_{m\times m}=AB$、$D=[d_{ij}]_{n\times n}=BA$，

$$
\text{tr}(AB)=\text{tr}(C)=\sum_{i=1}^{m} c_{ii}=\sum_{i=1}^{m}\sum_{k=1}^{n} a_{ik}b_{ki}=\sum_{i=1}^{m}\sum_{k=1}^{n} b_{ki}a_{ik}=\sum_{k=1}^{n} d_{kk}=\text{tr}(D).
$$

(5) 例如取 $A=\begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix}$，$B=\begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix}$，