則 $AB = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$，$\text{tr}(A)\text{tr}(B) = 1 \times 1 \neq \text{tr}(AB)$。

(6) 例如取 $A = \begin{bmatrix} 1 & 1 \\ 1 & 0 \end{bmatrix}$，

則 $A^2 = \begin{bmatrix} 2 & 1 \\ 1 & 1 \end{bmatrix}$，故 $\text{tr}(A^2) = 3$，但 $(\text{tr}(A))^2 = 1$。

(7) $\because (A^T A)_{jj} = \sum_{i=1}^{m} (A^T)_{ji} A_{ij} = \sum_{i=1}^{m} A_{ij} A_{ij} = \sum_{i=1}^{m} (A_{ij})^2$，

$\therefore \text{tr}(A^T A) = \sum_{j=1}^{n} (A^T A)_{jj} = \sum_{j=1}^{n} \sum_{i=1}^{m} (A_{ij})^2 = \sum_{i,j} (A_{ij})^2$。

> **例題 9**
>
> 證明：不存在方陣 $A$，$B$ 使 $AB - BA = I$。
>
> 〔95 彰師資工、100 中興應數、101 中山電機、103 高師應數、109 交大應數〕
>
> **解：**
>
> 若存在 $n$ 階方陣 $A$，$B$ 使 $AB - BA = I_n$，則 $\text{tr}(AB - BA) = \text{tr}(I_n)$，
>
> 等號左邊 $= \text{tr}(AB) - \text{tr}(BA) = 0$，
>
> 但等號右邊 $\text{tr}(I_n) = n$，得一矛盾。