反之，若 $A = O$，則 $\text{tr}(A^T A) = 0$。

若為複數則矩陣則為不成立。

例如考慮 $A = \begin{bmatrix} i & 0 \\ 0 & 1 \end{bmatrix} \neq O$，但 $\text{tr}(A^T A) = \text{tr}\left(\begin{bmatrix} i & 0 \\ 0 & 1 \end{bmatrix}^T \begin{bmatrix} i & 0 \\ 0 & 1 \end{bmatrix}\right) = \text{tr}\left(\begin{bmatrix} -1 & 0 \\ 0 & 1 \end{bmatrix}\right) = 0$。

> **例題**
>
> (10%) Let $A = [a_{ij}]$ be a $3 \times 2$ matrix, where $a_{ij}$ are real-valued. If the sum of diagonal elements of $A^T A$ is 0, find $A$.
>
> 〔105 交大統計〕
>
> **解：**
>
> $$0 = \text{tr}(A^T A) = \sum_{i=1}^{2} (A^T A)_{ii} = \sum_{i=1}^{2} \sum_{k=1}^{3} (A^T)_{ik} [A]_{ki} = \sum_{i=1}^{2} \sum_{k=1}^{3} a_{ki}^2$$
>
> 得 $a_{ki} = 0$，$\forall k = 1 \sim 3$，$i = 1 \sim 2$，$\therefore A = O_{3 \times 2}$。
>
> 也可以另外假設 $A = \begin{bmatrix} a & b \\ c & d \\ e & f \end{bmatrix}$，則 $\text{tr}(A^T A) = a^2 + b^2 + c^2 + d^2 + e^2 + f^2 = 0$。
>
> 解得 $a = b = c = d = e = f = 0$。
