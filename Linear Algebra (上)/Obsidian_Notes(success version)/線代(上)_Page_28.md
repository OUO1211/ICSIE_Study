## 列展開與列切割

> **定義：列展開與列切割**
>
> 設 $A_{(i)}$ 為矩陣 $A = [a_{ij}]_{m \times n}$ 的第 $i$ 個列向量，$y$ 為列向量為 $y = [y_1 \quad y_2 \quad \cdots \quad y_m]_{1 \times m}$。
>
> **列展開寫法：**
>
> $$yA = [y_1 \quad y_2 \quad \cdots \quad y_m] \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix} = [y_1 \quad y_2 \quad \cdots \quad y_m] \begin{bmatrix} A_{(1)} \\ A_{(2)} \\ \vdots \\ A_{(m)} \end{bmatrix}$$
>
> $$= y_1 A_{(1)} + y_2 A_{(2)} + \cdots + y_m A_{(m)}$$
>
> **列切割寫法：**
>
> 設 $A = [a_{ij}]_{m \times n}$，$B = [b_{ij}]_{n \times p}$，$C = [c_{ij}]_{m \times p}$，則
>
> $AB = C$ 可寫成
>
> $$A_{(i)} B = C_{(i)}, \quad \forall i = 1, 2, \ldots, m$$
