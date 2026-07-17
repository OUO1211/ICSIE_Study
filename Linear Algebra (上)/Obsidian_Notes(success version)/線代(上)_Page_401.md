## 特殊矩陣的 rank－AB=O

> **定理**
>
> If matrices $A_{m \times n}$, $B_{n \times p}$ satisfies $AB = O$, prove that $\text{rank}(A) + \text{rank}(B) \leq n$.
>
> 【87、101 交大、94 清大、99 淡大數學、100 成大統計、108 中山資所】

解：

任取 $x \in CS(B)$，

則存在 $y$ 使 $x = By$，即 $Ax = A(By) = (AB)y = Oy = 0$，

故 $CS(B) \subseteq \ker(A)$，

故 $\text{rank}(B) \leq \text{nullity}(A)$，

由 $\text{rank}(B) \leq \text{nullity}(A) = n - \text{rank}(A)$，

故得 $\text{rank}(A) + \text{rank}(B) \leq n$。
