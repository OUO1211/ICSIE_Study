510
離散數學（下）

\section*{有限狀態機的簡化}

若某一狀態非起始狀態，又没有其他狀態可抵達，則可將此狀態去掉而得化简。
【91、96清大資工】
Note
下方介紹一演算法執行有限狀態機的化簡，此處先定義相關單字。
考慮一有限狀態機：$M=\left[I, O, S, f_s, f_o\right]$ ，令狀態 $s_i, s_j \in S$ ，
\begin{itemize}
\item[（1）] 若 $f_o\left(s_i\right)=f_o\left(s_j\right)$ ，即 $s_i$ 與 $s_j$ 具有相同的 output，稱 $s_i$ 與 $s_j$ 為 0－equivalent，並記做 $s_i E_0 s_j$ 。
\item[（2）] 若 $f_o\left(s_i\right)=f_o\left(s_j\right)$ ，且 $\forall x \in I, f_s\left(s_i, x\right)$ 與 $f_s\left(s_j, x\right)$ 為 $(k-1)$－equivalent，
則稱 $s_i$ 與 $s_j$ 為 $k$－equivalent，$k=1,2, \ldots$ ，並記做 $s_i E_k s_j$ 。
\item[（3）] 若 $s_i$ 與 $s_j$ 為 $k$－equivalent，$\forall k=0,1,2, \ldots$ ，則稱 $s_i$ 與 $s_j$ 為狀態 equivalent，並記做 $s_i E s_j$ 。由以上之定義可知 $E_k$ 與 $E$ 均為等價關係，$\forall k=0,1,2, \ldots$ 。且若兩個狀態等價，則其功能必完全相同（輸出與狀態轉換均相同），可視為相同的狀態。
令 $E_k$ 所對應的分割為 $P_k, k=1,2, \ldots ; E$ 所對應的分割為 $P$ 。由以上定義可知 $P_{k+1}$ 為 $P_k$ 的細分（refinement）．
\end{itemize}

\section*{Moore State Reduction Algorithm}

已知一有限狀態機 $M$ ：
step1 ：先求 $P_0$ 。
step2：再求 $P_1, P_2, \ldots$ 直到 $P_k=P_{k+1}$ ．
step3：令 $P_k$ 對應的區塊代表新的狀態，其狀態轉換函數及輸出函數可取區塊中其中一個代表元素，得到另一個有限狀態機，稱為 $M$ 之簡化機（reduce machine）。

Note
$P_0=\left\{S_1, S_2\right\}$ 為狀態集 $S=\left\{s_1, s_2, \ldots, s_n\right\}$ 之一分割，
使 $S_1 \cup S_2=S$ ，且 $\forall s_i, s_j \in S_t, f_0\left(s_i\right)=f_o\left(s_j\right), t=1,2,1 \leq i \leq j \leq n$ 。
（即依照輸出的相同與否分成兩大子集 $S_1, S_2$ ）。