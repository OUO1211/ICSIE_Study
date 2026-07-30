第11章 二元關係及其應用
339

\section*{計算特殊的二元關係個數}

若 $|A|=n$ ，則 $A$ 上共有 $2^{n^2}$ 種二元關係，其中
\begin{itemize}
\item[（1）] 具有反身性的有 $2^{n^2-n}$ 種。
\item[（2）] 具有非反身性的有 $2^{n^2-n}$ 種。
\item[（3）] 具有對稱性的有 $2^{\left(n+n^2\right) / 2}$ 種。
\item[（4）] 具有非對稱性的有 $3^{1+2+\ldots+(n-1)}$ 種。
\item[（5）] 具有反對稱性的有 $2^n \cdot 3^{1+2+\ldots+(n-1)}$ 種。
\end{itemize}

【很重要】
【證明】以對應的關係矩陣來看：
\begin{itemize}
\item[（1）] 反身性：
$a_{i i}=1, \forall i=1 \sim n$ 且 $\forall i \neq j, a_{i j}$（共 $n^2-n$ 個）可 0 或 1 ，故有 $2^{n^2-n}$ 種。
\item[（2）] 非反身性：
$a_{i i}=0, \forall i=1 \sim n$ 且 $\forall i \neq j, a_{i j}$（共 $n^2-n$ 個）可 0 或 1 ，故有 $2^{n^2-n}$ 種。
\item[（3）] 對稱性：
$\forall i=1 \sim n, a_{i i}$ 可 0 或 1 （有 $n$ 個位置）；
$\forall i \neq j$ ，每一組對稱位置 $\left(a_{i j}, a_{j i}\right)$ 只為 $(0,0)$ 或 $(1,1)$ ，（共 $\frac{n^2-n}{2}$ 組對稱位置），
故共有 $2^{n+\frac{\left(n^2-n\right)}{2}}=2^{\frac{n^2+n}{2}}$ 種。
\item[（4）] 非對稱性：
$a_{i i}=0, \quad \forall i=1 \sim n ;$
$\forall i \neq j$ ，每一組對稱位置 $\left(a_{i j}, a_{j i}\right)$ 只為 $(0,0),(1,0)$ 或 $(0,1)$ ，
$\left(\right.$ 共 $1+2+\ldots+(n-1)=\frac{n^2-n}{2}$ 組對稱位置）
故共有 $3^{\frac{n^2-n}{2}}$ 種。
\item[（5）] 反對稱性：
$\forall i=1 \sim n, a_{i i}$ 可0或1（有 $n$ 個位置）；
$\forall i \neq j$ ，每一組對稱位置 $\left(a_{i j}, a_{j i}\right)$ 只為 $(0,0),(1,0)$ 或 $(0,1)$ ，
（共 $1+2+\ldots+(n-1)=\frac{n^2-n}{2}$ 組對稱位置），
故共有 $2^n \cdot 3^{\frac{n^2-n}{2}}$ 種。
\end{itemize}