68
線性代數（下）
$$
\Leftrightarrow A \boldsymbol{v}_i=\lambda_i \boldsymbol{v}_i, \forall i=1,2, \ldots, n,
$$
$\Leftrightarrow \boldsymbol{v}_i$ 為相對 $\lambda_i$ 的特徵向量，$\forall i=1,2, \ldots, n$ ．
（3）由（2）知：$n$ 階方陣 $A$ 可對角化 $\Leftrightarrow A$ 有 $n$ 個線性獨立的特徵向量．
【重要】
（4）由（1）知：$n$ 維空間上的線性算子 $T$ 可對角化 $\Leftrightarrow T$ 有 $n$ 個線性獨立的特徵向量．
（5）若 $n$ 階方陣 $A$ 有 $n$ 個相異的特徵根，則 $A$ 有 $n$ 個線性獨立的特徵向量，故 $A$ 可對角化；但可對角化的矩陣也可能有重複的特徵根。

【很重要】

（6）若 $A$ 可對角化，則 $A^T, A^{-1}$（若 $A$ 可逆），$A^k\left(k \in Z^{+}\right), f(A)$ 都可對角化．
【證明】

【重要】

因 $A$ 可對角化，存在某對角方陣 $D$ ，使 $A$ 與 $D$ 相似，
（1）故 $A^T$ 亦與 $D^T$ 相似，而 $D^T$ 亦為對角矩陣，故 $A^T$ 亦可對角化．
（2）故 $A^{-1}$ 亦與 $D^{-1}$ 相似，而 $D^{-1}$ 亦為對角矩陣，故 $A^{-1}$ 亦可對角化．
（3）故 $A^k$ 與 $D^k$ 相似，又因 $D^k$ 亦為對角矩陣，故 $A^k$ 可對角化．
（4）故 $f(A)$ 與 $f(D)$ 相似，又因 $f(D)$ 亦為對角矩陣，故 $f(A)$ 可對角化．
（7）線性算子 $T$ 亦有以上的性質。
（8）方陣 $A$ 是否可對角化與 $A$ 是否可逆不相關．

【重要】

例如，$A=\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right]$ 可逆但不可對角化；$B=\left[\begin{array}{ll}1 & 0 \\ 0 & 0\end{array}\right]$ 不可逆但可對角化．
$C=\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right]$ 可逆也可對角化；$D=\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right]$ 不可逆也不可對角化．