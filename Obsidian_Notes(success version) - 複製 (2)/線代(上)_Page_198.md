### 行列式性質－轉置與相乘

> **定義** 考慮 $n$ 階方陣 $A, B$：
>
> (1) $\det(A^T) = \det(A)$ 【重要】
>
> (2) $\det(AB) = \det(A)\det(B)$ 【重要】【102 成大數學】

【證明】

(1) 對 $n$ 做歸納法，$n = 1$ 時，顯然成立。

設所有 $A \in F^{(n-1)\times(n-1)}$，均使 $\det(A^T) = \det(A)$，

則對 $A \in F^{n \times n}$ 時，$\because \det(A) = \sum_{j=1}^{n} (-1)^{1+j} a_{1j} \det(M_{1j})$，

其中，而 $M_{1j}$ 為 $A$ 去第 1 列第 $j$ 行所得 $(n-1)$ 階矩陣，

由歸納假設知 $\det(M_{1j}) = \det(M_{1j}^T)$，

而 $M_{1j}^T$ 為 $A^T$ 去第 1 行第 $j$ 列所得 $(n-1)$ 階矩陣，

$\therefore \sum_{j=1}^{n}(-1)^{1+j} a_{1j} \det(M_{1j}^T) = \det(A^T)$，故得 $\det(A) = \det(A^T)$。

(2) 若 $B$ 不可逆，即 $\det(B) = 0$，若存在非零向量 $x$ 使 $Bx = 0$，

則 $A(Bx) = A0 = 0$，即 $(AB)x = 0$ 有非零解，故 $\det(AB) = 0$，

故 $\det(AB) = \det(A)\det(B)$。

若 $B$ 可逆，則 $B$ 可表為若干初等基本矩陣的乘積，設 $B = E_1 E_2 \cdots E_k$，

則 $\det(AB) = \det(AE_1 E_2 \cdots E_k) = \det(AE_1 E_2 \cdots E_{k-1})\det(E_k)$

$= \cdots = \det(A)\det(E_1)\det(E_2)\cdots\det(E_k)$

$= \det(A)\det(E_1 E_2 \cdots E_k) = \det(A)\det(B)$

> **Note**
>
> (1) $\det(\bar{A}) = \overline{\det(A)}$；$\det(A^H) = \overline{\det(A)}$。【108 台大資工】
>
> (2) $\det(AA^T) = [\det(A)]^2$；$\det(AA^H) = |\det(A)|^2$。
>
> (3) $\det(A^{-1}) = \dfrac{1}{\det(A)}$。
>
> 【95 台大資工、103,106 中央資工、110 交大資工、110 台科資工】
>
> (4) $\det(A^k) = \det(A)^k$。【100 交大資工、103 中央資工、105 台大資工、110 台科資工】
>
> (5) $\det(AB) = \det(BA)$（只在 $A, B$ 都為方陣時）【很重要】
>
> (6) $\det(A \pm B) \neq \det(A) \pm \det(B)$ 不恆成立。【很重要】
>
> (7) $A$ 為 $n$ 階**斜對稱方陣**且 $n$ 為奇數，則 $\det(A) = 0$。【98 雲科資工、107 交大應數】
