## 546 線性代數(上)

> **例題 6**
>
> (10%) Define $T(A) = \dfrac{A + A^T}{2}$, where $A$ is a $n \times n$ matrix. Then
>
> (1) $\ker(T) = (\ )$
>
> (2) $\text{nullity}(T) = (\ )$
>
> 【101 整南資工、103 成大應數、103 中正數學、106 高鐵所統計、102 台大資工】

**解**

(1) $\ker(T) = \{A \in R^{n \times n} \mid T(A) = 0\}$

$$= \{A \in R^{n \times n} \mid A + A^T = 0\} = \{A : A \text{ 為斜對稱矩陣}\}$$

(2) 取 $\{E_{ij} - E_{ji} : i > j\}$ 作為基底，共 $\dfrac{n(n-1)}{2}$ 個。

故 $\text{rank}(T) = \dim(R^{n \times n}) - \text{nullity}(T) = n^2 - \dfrac{n(n-1)}{2} = \dfrac{n(n+1)}{2}$。

> **例題 7**
>
> Let $T: R_3[x] \to R$ be the linear transformation defined by $T(P(x)) = \int_0^1 P(x)\,dx$.
>
> (1) Find a basis for $\ker(T)$. (2) Find a basis for $\text{Im}(T)$.
>
> 【94 整南資工、90 中山系統工程】

**解**

(1) $\ker(T) = \left\{P \in R_3[x] \mid \int_0^1 P(x)\,dx = 0\right\}$

令 $P(x) = a + bx + cx^2$，則 $\int_0^1 P\,dx = a + \dfrac{1}{2}b + \dfrac{1}{3}c = 0$，

故 $a = -\dfrac{1}{2}b - \dfrac{1}{3}c$。

$\therefore P(x) = \left(-\dfrac{1}{2}b - \dfrac{1}{3}c\right) + bx + cx^2 = b\left(-\dfrac{1}{2} + x\right) + c\left(-\dfrac{1}{3} + x^2\right)$

故可取 $\left\{\left(-\dfrac{1}{2} + x\right),\left(-\dfrac{1}{3} + x^2\right)\right\}$ 為 $\ker(T)$ 的一組基底。

(2) $\because \dim(\ker(T)) = 2$，$\dim(R_3[x]) = 3$，故 $\dim(\text{Im}(T)) = \dim(R_3[x]) - \dim(\ker(T)) = 3 - 2 = 1$，

且 $\text{Im}(T) \subseteq R$，又 $T(1) = 1 \in \text{Im}(T)$，故 $\text{Im}(T) = R$，

故可取 $R$ 的標準基底 $\{1\}$ 為 $\text{Im}(T)$ 的基底。
