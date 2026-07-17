210
線性代數（下）

相似與喬丹型
若 $J_A$ 為 $A$ 的 Jordan form，$J_B$ 為 $B$ 的 Jordan form，則
$A$ 與 $B$ 相似 $\Leftrightarrow J_A=J_B$ 。
（此處不計較 Jordan form 的排序方式）

例題 7
$(10 \%)$ Suppose that $A$ has the Jordan form $J_A=\left[\begin{array}{ccccc}-1 & 1 & 0 & 0 & 0 \\ 0 & -1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 0 & 1\end{array}\right]$ ．Find the Jordan form of $A^2$ ．

【99交大應数】

解 令可逆矩陣 $P$ 使得 $A=P J_A P^{-1}$ ，
則 $A^2=P\left(J_A\right)^2 P^{-1}$ ，其中 $\left(J_A\right)^2=\left[\begin{array}{ccccc}1 & -2 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 0 & 1 & 2 \\ 0 & 0 & 0 & 0 & 1\end{array}\right]$（令為 $B$ ），
則因 $B$ 有特徵根 1，1，1，1，0，

且 $\operatorname{dim}(\operatorname{ker}(B-I))=5-\operatorname{rank}(B-I)=5-2=3$ ，所以 $\lambda=1$ 的點圖是

另外，$\lambda=0$ 的點圖是 $\bullet$ ，
故 $B$ 的 Jordan form 為 $J_B=\left[\begin{array}{cc|c|c|c}1 & 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 0 \\ \hline 0 & 0 & 1 & 0 & 0 \\ \hline 0 & 0 & 0 & 1 & 0 \\ \hline 0 & 0 & 0 & 0 & 0\end{array}\right]$ ，
又因 $A^2$ 與 $B$ 相似，故 $A^2$ 的 Jordan form 也為 $J_B$ ．