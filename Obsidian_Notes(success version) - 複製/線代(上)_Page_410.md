解：由題意 $\ker(A) = \{0\}$，故由 Sylvester 定理 $n = \dim(\ker(A)) + \text{rank}(A)$，

得 $\text{rank}(A) = n$。

(1) 若增廣矩陣 $[A|b]$ 的 rank 大於等於 $n+1$，則 $Ax = b$ 無解，inconsistent。

(2) 必恰一解，證明如下：

設 $x, y$ 均為 $Ax = b$ consistent 的解，

則 $A(x - y) = 0$，故 $x - y \in \ker(A)$，得 $x - y = 0$，矛盾。

故 $x = y$，均為 $Ax = b$ 恰一解。

5. (10%) Let $A$ be a $3 \times 5$ matrix. The linear system $Ax = b$ is consistent for every $b \in R^3$.

(1) Find $\dim(RS(A))$. (2) Find $\dim(N(A))$. (3) If $A = [a_1, a_2, a_3, a_4, a_5]$ and $y = [1, 2, 3]^T$, then what is the dimension of $\text{span}(a_1, a_2, a_3, a_4, a_5, y)$?

【101 交大進數】

解：(1) 3. (2) 2. (3) 3.

6. Each row of the given table below summarizes data collected for some matrix $A$ and the corresponding transformation. The "always solvable" column refers to whether $Ax = b$ is solvable for all $b$. The "unique solution" refers to whether or not there will be at most one solution. If the data is inconsistent, write "impossible."

| size | always solvable | unique solution | dim of image | dim of nullspace | rank |
|------|----------------|----------------|--------------|-----------------|------|
| $4 \times 3$ | yes | | | | |
| $4 \times 5$ | yes | | | | |
| $5 \times 5$ | | | | 2 | |
| $4 \times 4$ | | | | | |
| $3 \times 2$ | | yes | | | |
| $5 \times 4$ | no | | | | 3 |

解：

| size | always solvable | unique solution | dim of image | dim of nullspace | rank |
|------|----------------|----------------|--------------|-----------------|------|
| $4 \times 3$ | impossible | impossible | impossible | impossible | impossible |
| $4 \times 5$ | | no | 4 | 1 | 4 |
| $5 \times 5$ | no | no | 3 | 2 | 3 |
| $4 \times 4$ | yes | yes | 4 | 0 | 4 |
| $3 \times 2$ | no | | 2 | 0 | 2 |
| $5 \times 4$ | | no | 3 | 1 | 3 |
