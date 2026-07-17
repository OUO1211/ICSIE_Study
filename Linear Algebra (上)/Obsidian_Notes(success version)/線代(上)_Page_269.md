## 判斷矩陣空間的子空間

> **例題 3**
>
> 判斷下列集合是否為 $R^{n \times n}$ 的子空間：
>
> (1) $W_1 = \{A \mid A^T = A\}$。 【100 中台資工、103 政大應數、105 成大資工、110 台大電信】
>
> (2) $W_2 = \{A \mid A^T = -A\}$。 【109 台積電機難、110 台大電信】
>
> (3) $W_3 = \{A \mid A$ 為上三角矩陣 $\}$。 【96 暨南應數、105 交大資工、105 成大資工】
>
> (4) $W_4 = \{A \mid A$ 為上三角矩陣 $\}$。
>
> (5) $W_5 = \{A \mid \det(A) = 0\}$。 【105 成大資工、105 成大資工】
>
> (6) $W_6 = \{A \mid \det(A) \neq 0\}$。
>
> (7) $W_7 = \{A \mid A$ 不含零向量 $\}$。
>
> (8) $W_8 = \{X \mid AX = XA\}$，where $A$ is a fixed matrix.

**解** (1) True.

$\because O_n \in W_1$，$\therefore W_1 \neq \varnothing$。

任取 $A, B \in W_1$，$a \in R$，

則 $(aA + B)^T = aA^T + B^T = aA + B$，故 $aA + B \in W_1$，

即滿足向量加法和純量積的封閉性，故 $W_1$ 為 $V$ 的子空間。

(2)$\sim$(5) True. 同理由(1)的方法，請讀者自行演練。

(6) False.

反例可取 $A = \begin{bmatrix} 1 & 0 \\ 0 & 0 \end{bmatrix} \in W_6$，$B = \begin{bmatrix} 0 & 0 \\ 0 & 1 \end{bmatrix} \in W_6$，$A + B = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} \notin W_6$。

(7) False.

因為 $W_7$ 不含零矩陣。

(8) True.

$\because O_n \in W_8$，$\therefore W_8 \neq \varnothing$。

任取 $A, B \in W_8$，$a \in R$，

$(aA + B)X = aAX + BX = aXA + XB = X(aA + B)$，故 $aA + B \in W_8$，

即滿足向量加法和純量積的封閉性，故 $W_8$ 為 $V$ 的子空間。