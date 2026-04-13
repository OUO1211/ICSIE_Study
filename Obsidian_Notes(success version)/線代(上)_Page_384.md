> **例題 3**
>
> (5%) Let $A$ be an $m \times n$ matrix whose null space has dimension $k$. Which conclusion is correct?
>
> (1) The dimension of $\text{Null}(A^T)$ is $k$.
>
> (2) The dimension of row space of $A$ is $m - k$.
>
> (3) The dimension of column space of $A$ is $m - k$.
>
> (4) The dimension of row space of $A$ is $n - k$.
>
> (5) The dimension of column space of $A$ is $n - k$.
>
> 【101 交大資工】

解：(4), (5)。

由 Sylvester 定理：

- $n = \dim(N(A)) + \text{rank}(A) = k + \text{rank}(A)$
- $m = \dim(N(A^T)) + \text{rank}(A^T) = \dim(N(A^T)) + \text{rank}(A) = \dim(N(A^T)) + n - k$
- $\therefore \dim(N(A^T)) = m - n + k$
- $\dim(RS(A)) = \text{rank}(A) = n - k$
- $\dim(CS(A)) = \text{rank}(A) = n - k$

> **例題 4**
>
> (5%) Let $A \in R^{5 \times 3}$ and $\text{nullity}(A)$ denote the dimension of $N(A)$. Suppose $\text{nullity}(A) = 2$. Which of the following statements are true?
>
> (1) $\text{rank}(A^T) = 3$.
>
> (2) $\text{nullity}(A^T) = 4$.
>
> (3) Let $A = [a_1, a_2, a_3]$. Then $a_1$ and $a_2$ are linearly dependent.
>
> (4) The linear equation $Ax = 0$ has infinitely many solutions.
>
> (5) The linear equation $A^T y = d$ cannot have a unique solution for any $d \in R^3$.
>
> 【110 中山電機】

解：

(1) False. $\text{rank}(A^T) = \text{rank}(A) = 3 - \text{nullity}(A) = 3 - 2 = 1$。

(2) True. $A^T : 3 \times 5$，$\text{nullity}(A^T) = 5 - \text{rank}(A^T) = 5 - 1 = 4$。

(3) True. 因為 $\text{rank}(A) = 1$。

(4) True. 因為 $\dim(\text{Null}(A)) = \text{nullity}(A) = 3 - \text{rank}(A) = 2$。

(5) True. 因為 $\text{rank}(A^T) = 1$ 小於 $A^T$ 的行數，故若 $A^T y = d$ 有解，則解不唯一。