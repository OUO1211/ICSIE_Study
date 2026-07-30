190
資料結構（含精選試題）
Data Structure

\section*{5－11 集合的表示法－樹的應用之一}
\begin{itemize}
\item[（一）] 假設集合中的元素為 $1,2,3, \cdots, n$ ，且當兩集合是為互斥的，即 $\mathrm{S}_{\mathrm{i}}$ 與 $\mathrm{S}_{\mathrm{j}}$ 的交集為空集合，而這些集合便可使用樹來表示。
\item[（二）] 假設 $\mathrm{S}_1=\{1,7,8,9\}$
$$
\begin{aligned}
& S_2=\{2,5,10\} \\
& S_3=\{3,4,6\}
\end{aligned}
$$
以樹表示如下：
\item[（三）] 此時的 Node Structure 如下：

\begin{tabular}{|l|l|}
\hline Data & Parent \\
\hline
\end{tabular}
其中 Data：儲存元素值。
Parent：指向父親節點的指標
此外，每個樹根皆會指到集合名稱所在之處，例如下圖：
\item[（四）] 集合上的運算：聯集（Union）與找尋（Find）
\begin{itemize}
\item[1．] 聯集（Union）
作法：執行兩集合之聯集所要做的事情就是將其中一棵樹之樹根的父親欄設定為另一棵樹之樹根。
\item[] 例：
或
\end{itemize}
\end{itemize}