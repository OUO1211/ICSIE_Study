> **矩陣乘法滿足的性質**
>
> (1) 結合律(associative)：
>
> 對任意矩陣 $A, B, C$，$(AB)C = A(BC)$。
>
> (2) 分配律(distributive)：
>
> 對任意矩陣 $A, B, C$，$A(B+C) = AB + AC$；$(B+C)A = BA + CA$。
>
> (3) 係數與矩陣乘法運算的結合律：
>
> 對任意矩陣 $A, B$，對任意係數 $c$，$c(AB) = (cA)B = A(cB)$。
>
> (4) 由零矩陣相乘表示為零矩陣：
>
> 對任意矩陣 $A$，$A_{m \times n} O_{n \times r} = O_{m \times r}$，$O_{s \times m} A_{m \times n} = O_{s \times n}$。
>
> (5) 與單位矩陣相乘後為本身：
>
> 對任意矩陣 $A_{m \times n}$，$A_{m \times n} I_n = A_{m \times n}$；$I_m A_{m \times n} = A_{m \times n}$。
>
> (6) 指數運算：
>
> 對任意方矩陣 $A$，對任意非負整數 $r, s$，$A^r A^s = A^{r+s}$；$(A^r)^s = A^{rs}$。
>
> (7) 列矩陣與行矩陣的表達：
>
> $A_{1 \times n} B_{n \times 1} = [c_{11}]$，即 $[a_1 \quad a_2 \quad \cdots \quad a_n] \begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix} = [a_1 b_1 + a_2 b_2 + \cdots + a_n b_n]$
>
> $B_{n \times 1} A_{1 \times n} = C_{n \times n}$，即 $\begin{bmatrix} b_1 \\ b_2 \\ \vdots \\ b_n \end{bmatrix} [a_1 \quad a_2 \quad \cdots \quad a_n] = [c_{ij}]$，其中 $c_{ij} = b_i a_j$。
>
> (8) 關於上（下、對角）三角矩陣：
>
> 上（下、對角）三角矩陣相乘必為上（下、對角）三角矩陣。

【證明】以下證明(1)，其它請讀者自行練習。

(1) $\forall 1 \leq i \leq m$，$1 \leq j \leq q$

$$(ABC)_{ij} = \sum_{k=1}^{n} A_{ik}(BC)_{kj} = \sum_{k=1}^{n} A_{ik} \left[\sum_{l=1}^{p} B_{kl} C_{lj}\right] = \sum_{k=1}^{n} \sum_{l=1}^{p} A_{ik} B_{kl} C_{lj}$$

$$= \sum_{l=1}^{p} \sum_{k=1}^{n} A_{ik} B_{kl} C_{lj} = \sum_{l=1}^{p} (AB)_{il} C_{lj} = ((AB)C)_{ij}$$

故 $A(BC) = (AB)C$
