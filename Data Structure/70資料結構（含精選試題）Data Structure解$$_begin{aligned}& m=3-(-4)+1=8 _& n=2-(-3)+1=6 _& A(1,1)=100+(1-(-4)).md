70
資料結構（含精選試題）
Data Structure

解
$$
\begin{aligned}
& m=3-(-4)+1=8 \\
& n=2-(-3)+1=6 \\
& A(1,1)=100+(1-(-4)) \cdot 6 \cdot 1+(1-(-3)) \cdot 1=134
\end{aligned}
$$

例題 2－3
—Array 被以横列為主的順序放在 Memory 內，每個元素佔用4個單位的 Memory，若起始位址是100，則下列宣告的元素存放的位址為何？
\begin{itemize}
\item[（1）] Var A：array $[-100 \cdots 1,1 \cdots 100]$ 求 $\mathrm{A}[1,12]$ ？
\item[（2）] Var A：array $[5 \cdots 10,-10 \cdots 20]$ 求 A［5，－5］？
\end{itemize}

【高考、研究所常考題型】
解（1）40544（2）120

【題型二】給予二個已知位址量，自行判斷 Row－major 或 Column－major，並求 A［i，j］之Location 。
$$
\text { Note: 判斷 }\left\{\begin{array}{cl}
\text { Row }- \text { major } & \Rightarrow \text { 求出 } \ell_0 \text { 及行數(但列數不知) } \\
\text { Column }- \text { major } & \Rightarrow \text { 求出 } \ell_0 \text { 及列數(但行數不知) }
\end{array}\right.
$$

例題 2－4
A 為一二維陣列，若 $\mathrm{A}(3,2)$ is 1110 and $\mathrm{A}(2,3)$ is 1115 。假設元素大小為 1 則 $\mathrm{A}(5,4)$ 之位址為何？A（1，4）位址？

解 $\mathrm{A}(1,4)=1120$
$A(5,4)=$ ？（同學自行練習）
例題 2－5
若 $\mathrm{A}(1,1)$ 與 $\mathrm{A}(3,3)$ 位址分別 1204 與 1244 ，則 $\mathrm{A}(4,4)$ 的位址為何？
假設 $(\mathrm{d}=1)$ 。
解 因本題 A（i，j），i＝j，故用 Row－Major 或 Column－Major 皆相同算法。
$$
\begin{aligned}
& A(3,3)=A(1,1)+(3-1) \times 1 \times n+(3-1) \times 1 \\
& 1244=1204+2 n+2 \\
& \begin{aligned}
40=2 n & +2 \quad n=19 \\
A(4,4) & =A(1,1)+(4-1) \times 1 \times 19+(4-7) \times 1=1204+57+3 \\
& =1264
\end{aligned}
\end{aligned}
$$