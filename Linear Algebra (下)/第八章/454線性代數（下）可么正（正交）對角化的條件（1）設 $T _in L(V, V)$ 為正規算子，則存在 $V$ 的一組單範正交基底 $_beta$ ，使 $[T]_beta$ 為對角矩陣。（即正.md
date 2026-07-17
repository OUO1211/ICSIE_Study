454
線性代數（下）

可么正（正交）對角化的條件
（1）設 $T \in L(V, V)$ 為正規算子，則
存在 $V$ 的一組單範正交基底 $\beta$ ，使 $[T]_\beta$ 為對角矩陣。
（即正規算子 $T$ 可么正對角化）
（2）若 $A \in C^{n \times n}$ ，則
$A$ 為正規且為上三角矩陣 $\Leftrightarrow A$ 為對角矩陣。

【91清大應数】

（3）若 $A \in R^{n \times n}$ ，則
$A$ 為對稱且為上三角矩陣 $\Leftrightarrow A$ 為對角矩陣。
（4）若 $A \in C^{n \times n}$ ，則
$\underline{A \text { 為正規矩陣 } \Leftrightarrow A \text { 可么正對角化．}}$
（5）若 $A \in R^{n \times n}$ ，則
$\underline{A \text { 為對稱矩陣 } \Leftrightarrow A \text { 可正交對角化．}}$
【96台大数學、99交大資工】
【證明】
（1）因 $\operatorname{char}_T(x)$ 在 $C$ 中可分解，故由 Schur 定理得：
存在 $V$ 的一單範正交基底 $\beta=\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_n\right\}$ 使 $[T]_\beta$ 為一上三角矩陣，設為 $A$ ，其中 $n=\operatorname{dim}(V)$ ，
由對 $n$ 做歸納法以證明：＂$v_1, \ldots, v_n$ 均為 $T$ 的特徵向量＂， $n=1$ 時，$R$ 為 $1 \times 1$ 矩陣，$T\left(v_1\right)=R v_1$ ，明顯成立。
設 $v_1, \ldots, v_{k-1}$ 都是 $T$ 的特徵向量，欲證明 $v_k$ 亦為 $T$ 的特徵向量：
令 $A=\left[\begin{array}{ll}B & C \\ O & E\end{array}\right]$ ，則 $A^H=\left[\begin{array}{cc}B^H & O \\ C^H & E^H\end{array}\right]$ ，其中，$B:(k-1) \times(k-1)$ 的對角矩陣，
又因 $A$ 為上三角矩陣，故 $(A)_{i k}=0, \forall i>k$ ，
又 $A^H=\left([T]_\beta\right)^H=\left[T^*\right]_\beta$ ，且 $T$ ：normal， $\boldsymbol{v}_1, \ldots, \boldsymbol{v}_{k-1}$ 都是 $T^*$ 的特徴向量，
故 $C^H=O$ ，而得 $\left(A^H\right)_{i k}=0, \forall i<k$ ，得 $(A)_{i k}=0, \forall i<k$ ，故 $\boldsymbol{v}_k$ 為 $T$ 的特徵向量，
故由歸納法得證 $\boldsymbol{v}_1, \ldots, \boldsymbol{v}_n$ 均為 $T$ 的特徵向量，故 $T$ 可么正對角化．
（2）$(\Rightarrow) \because A$ 為正規，$\therefore A^H A=A A^H$ ，故 $\forall i=1 \sim n,\left(A^H A\right)_{i i}=\left(A A^H\right)_{i i}$ ，
$$
\text { 即 } \sum_{k=1}^n\left(A^H\right)_{i k}(A)_{k i}=\sum_{k=1}^n(A)_{i k}\left(A^H\right)_{k i} \therefore \sum_{k=1}^n \overline{(A)_{k i}}(A)_{k i}=\sum_{k=1}^n(A)_{i k} \overline{(A)_{i k}}
$$