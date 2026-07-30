452
離散數學（下）

\section*{12－3 各種群及其特性}

\section*{模 $n$ 同餘群（group of congruence modulo $n$ ）}

在 $Z$ 上定義一個二元關係 $\equiv_n$ 為 $\forall a, b \in Z, a \equiv_n b \Leftrightarrow n \mid a-b$（同餘關係），則 $\equiv_n$ 為一等價關係，且對應的等價類有 $n$ 個：$[0],[1], \ldots,[n-1]$ 。
令 $Z_n=\{[0],[1], \ldots,[n-1]\}$ ，並定義二元運算 $+_n: \forall[a],[b] \in Z_n$ ，$[a]+{ }_n[b]=[a+b]$ ，
則 $\left(Z_n,+{ }_n\right)$ 為一群，稱為模 $n$ 同餘群。
【證明】
令 $[a],[b],[c] \in Z_n$ ，
封閉性：$[a]+{ }_n[b]=[a+b] \in Z_n$ 。
結合性：$\left([a]+{ }_n[b]\right)+{ }_n[c]=[a+b]+{ }_n[c]=[a+b+c]=[a]+{ }_n[b+c]=[a]+{ }_n\left([b]+{ }_n[c]\right)$ 。
單位元素為 $[0]: \because[0]+{ }_n[a]=[0+a]=[a]=[a+0]=[a]+{ }_n[0]$ 。
反元素性質 ：$[a]^{-1}=[n-a], \because[n-a]+{ }_n[a]=[n-a+a]=[n]=[0]=[a]+{ }_n[n-a]$ 。
交換性：$\because[a]+{ }_n[b]=[a+b]=[b+a]=[b]+{ }_n[a]$ 。

例如：

\begin{tabular}{|l|l|l|l|l|l|l|l|l|l|l|l|}
\hline \multirow{2}{*}{} & $+_4$ & 0 & 1 & 2 & 3 & \multicolumn{2}{|r|}{\multirow[t]{2}{*}{5}} & \multirow{2}{*}{} & 2 & 3 & 4 \\
\hline & 0 & 0 & 1 & 2 & 3 & & & & & & \\
\hline $\left(Z_4,+_4\right)$ ： & 1 & 1 & 2 & 3 & 0 & $\left(Z_5-\{0\}, \cdot_5\right):$ & ： 2 & 2 & 4 & 1 & 3 \\
\hline & 2 & 2 & 3 & 0 & 1 & & 3 & 3 & 1 & 4 & 2 \\
\hline & 3 & 3 & 0 & 1 & 2 & & 4 & 4 & 3 & 2 & 1 \\
\hline
\end{tabular}

Note
\begin{itemize}
\item[（1）] 有時直接以 $0,1, \ldots, n-1$ 來表示［0］，［1］，．．，，$[n-1]$ 。
\item[（2）] （ $Z_n,+_n$ ）為一交換群。
\item[（3）] （ $Z_n-\{0\}, \cdot{ }_n$ ）為群 $\Leftrightarrow n$ 為質數，其中，${ }_n$ 定義為 $a \cdot{ }_n b \equiv a b \bmod n$ 。（此為乘法模同餘詳）【證明】
（⇐）對任意 $a, b, c \in Z_n-\{0\}$ ，
封閉性：由定義知 $a \cdot{ }_n b \in Z_n$ ，而如果 $a \cdot{ }_n b=0_n$ ，則 $n \mid a b$ ，但 $n$ 為質數，故 $n \mid a$ 或 $\left.n\right|^b$即 $a \equiv 0 \bmod n$ 或 $b \equiv 0 \bmod n$ ，矛盾。 $\therefore a \cdot{ }_n b \in Z_n-\{0\}$ 。
結合性：$\because\left(a \cdot{ }_n b\right) \cdot{ }_n c=(a b) \cdot{ }_n c=a b c=a \cdot{ }_n(b c)=a \cdot{ }_n\left(b \cdot{ }_n c\right) \bmod n$ 。
\end{itemize}