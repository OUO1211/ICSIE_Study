68
資料結構（含精選試題）
品

Data Structure

\section*{2－1 有序串列（Ordered List）}
\begin{itemize}
\item[] －線性串列（Linear List）
\item[] －循序串列（Sequential List）
\item[] －密集串列（Dense List）
\end{itemize}

一．為日常容易碰到的資料
例：紙牌之數字（2，3，4，5，6，7，8，9，10，J，Q，K，A）
二．以理論方面來考慮
一個串列可為：1．空串列
2．$\left(a_1, a_2, \cdots, a_n\right)$ ，$a_i$ 是某集合之元素。
三．串列上常見的動作
\begin{itemize}
\item[（一）] Length
\item[（二）] retrieve（A，i）
\item[（三）] update（A，i）
\item[（四）] Insert（i）
\item[（五）] Delete（i）
\end{itemize}

2－2 陣列（Array）
Def：為表示 List 的一種方式，佔用連續的記憶體空間，串列中元素採 Sequentialmapping 方式，對應儲存到 Array 中。
\begin{itemize}
\item[] －支援 Sequential access 及 random access。
\item[] －插入、刪除元素較不方便，須挪移其它元素。Time：O（n）
\end{itemize}

一．一維陣列
若陣列是 $\mathrm{A}(1: \mathrm{m})$ ，假設每一個 Item 佔 d 個空間，則陣列元素位址如下（假設 $\mathrm{L}_0$ 是起始位址）。
A（1）A（2）A（3）⋯⋯ A（n）
$\mathrm{L}_0 \quad \mathrm{~L}_0+1^* \mathrm{~d} \quad \mathrm{~L}_0+2^* \mathrm{~d} \quad \mathrm{~L}_0+(\mathrm{n}-1)^* \mathrm{~d}$