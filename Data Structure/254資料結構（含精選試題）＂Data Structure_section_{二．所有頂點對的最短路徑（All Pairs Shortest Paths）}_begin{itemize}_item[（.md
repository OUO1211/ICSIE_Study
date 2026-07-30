254
資料結構（含精選試題）
＂

Data Structure

\section*{二．所有頂點對的最短路徑（All Pairs Shortest Paths）}
\begin{itemize}
\item[（一）] 問題敘述
\end{itemize}

所有頂點對的最短路徑問題是要找出所有成對的頂點 $\left(v_i, v_j\right), i \neq j$ 之間的最短路徑。
《方法一》
使用 Shortest Path 演算法 n 次，而每次都以 V（G）中的一個頂點為起始點；這個方法需要 $O\left(n^3\right)$ 的時間。
《方法二》
\begin{itemize}
\item[1．] 圖形 G 以成本矩陣表示，其中 $\operatorname{COST}(\mathrm{i}, \mathrm{j})=0$ ，而且，若邊 $\langle\mathrm{i}, \mathrm{j}\rangle \mathrm{i} \neq \mathrm{j}$ ，不屬於G ，則 $\operatorname{COST}(\mathrm{i}, \mathrm{j})=\infty$ 。
\item[2．] 定義 $A^k(i, j)$ 為從 i 到 j 之最短路徑的成本，且這條路徑所經過的頂點編號，不能超過 k。因此 An（i，j）即為圖形 G 中從 i 到 j 最短路徑的花費，因為 G 中沒有註標大於 n 的頂點。
\item[3．] $\mathrm{A}^0(\mathrm{i}, \mathrm{j})$ 就是 $\operatorname{COST}(\mathrm{i}, \mathrm{j})$ 。
\item[4．] 所有成對頂點的最短路徑之演算法即是依序建立矩陣：
$$
\mathrm{A}^0, \quad \mathrm{~A}^1, \cdots, \mathrm{~A}^{\mathrm{n}} .
$$
\item[5．] 從頂點 i 到頂點 $j$ 的最短路徑為下列二者中較小者：
$$
A^k(i, j)=\min \left(A^{k-1}(i, j), \quad\left(A^{k-1}(i, k)+A^{k-1}(k, j)\right), k \geq 1\right.
$$
\item[（二）] 想法
對任何一對頂點 i 和 j 而言：
\item[1．] 從 i 到 j 而不經過足標大於 k 之頂點的最短路徑不會經過足標為 k 之頂點，因此其成本為 $A^{k-1}[i, j]$ 。
\item[2．] 其最短路徑會經過頂點 k 。
必須注意的是，只有當 G 中沒有有包含頂點 k 且長度不為負數的循環時，此法才會成立；否則的話，會有不合理之錯誤發生。
\item[] 例：下圖所示為一個有向圖形及其矩陣 $\mathrm{A}^0$ ，對這個圖形而言 $\mathrm{A}^2[1,3] \neq \min \left\{\mathrm{A}^1[1\right.$ ，3］，$\left.\quad \mathrm{A}^1[1,2]+\mathrm{A}^1[2,3]\right\}=2$ 。因為路徑 $1,2,1,2,1,2, \cdots, 1,2,3$ 的長度可以變得任意地小到 $-\infty$ 。這是因為有長度為 -1 的循環121存在之故。

圖：有負長度循環之圖形
\end{itemize}