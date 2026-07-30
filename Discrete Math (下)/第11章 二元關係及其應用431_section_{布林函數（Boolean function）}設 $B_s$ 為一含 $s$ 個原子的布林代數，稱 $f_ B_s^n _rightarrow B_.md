第11章 二元關係及其應用
431

\section*{布林函數（Boolean function）}

設 $B_s$ 為一含 $s$ 個原子的布林代數，稱 $f: B_s^n \rightarrow B_s$ 為一具有 $n$ 個變數的布林函數。
Note
\begin{itemize}
\item[（1）] 在 $B_s$ 中，$n$ 個變數的布林函數有 $\left(2^s\right)^{2^{n s}}$ 種。
解 $\because\left|B_s\right|=2^s, \therefore\left|B_s^n\right|=2^{n s}$ ，即定義域中有 $2^{n s}$ 個元素，對應域中有 $2^s$ 個元素，故得證。
\item[（2）] 當 $s=1$ 時，$B_s$ 記做 $B=\{I, O\}=\{1,0\}, f: B^n \rightarrow B$ 稱為一開關函數。
\item[（3）] 每個標準布林表示式皆可用布林函數表示。
\item[（4）] 但並非每個布林函數皆可找到一布林表示式與之對應。
\item[（5）] 只在 $s=1$ 時，每個布林函數皆可找到一布林表示式與之對應，即開關函數。
\end{itemize}