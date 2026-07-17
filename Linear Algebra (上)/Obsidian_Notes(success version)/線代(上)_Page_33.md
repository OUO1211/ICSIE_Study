## 轉置與共軛轉置的運算性質

> **定理：轉置與共軛轉置的運算性質**
>
> 考慮 $n$ 階方矩陣 $A$，純量（體數）$k$，
>
> (1) $(A^T)^T = A$；$(A^H)^H = A$。
>
> (2) $(A + B)^T = A^T + B^T$；$(A + B)^H = A^H + B^H$。
>
> (3) $(kA)^T = kA^T$；$(kA)^H = \bar{k}A^H$。
>
> (4) $(AB)^T = B^T A^T$；$(AB)^H = B^H A^H$，其中 $A$，$B$ 為 $m \times n$，$n \times m$。
>
> 〔99 雲科資工〕

**【證明】**

性質 (1)-(3) 可由定義明顯得知，以下證明 (4)：

令 $A: m \times n$，$B: n \times m$，則

$$((AB)^T)_{ij} = (AB)_{ji} = \sum_{k=1}^{n} A_{jk} B_{ki} = \sum_{k=1}^{n} (B^T)_{ik} (A^T)_{kj} = (B^T A^T)_{ij}, \quad \forall i, j$$

故得 $(AB)^T = B^T A^T$。

另外：

$$(AB)^H = \overline{(AB)^T} = \overline{B^T A^T} = \overline{B^T} \cdot \overline{A^T} = B^H A^H$$
