150
資料結構（含精選試題）
■■

Data Structure
果串列長度 $\mathrm{n} \geq 1$ ，則 $\alpha$ 稱為 A 的頭（Head），而（ $\alpha_2, \cdots, \alpha_{\mathrm{a}}$ ）為 A 的尾（Tail）。

\section*{二．例子}
\begin{itemize}
\item[（一）] $\mathrm{D}=()$
空串列（Empty or null list）：長度為 0
\item[（二）] $\mathrm{A}=(\mathrm{a},(\mathrm{b}, \mathrm{c}))$
長度等於2 之串列，其第一個元素為基本單位＇a＇，而第二個元素為一子串列（b，c）。
\item[（三）] $\mathrm{B}=(\mathrm{A}, \mathrm{A},())$
一長度為3的串列，其前兩個元素為串列 A，而第三個元素為空串列。
\item[（四）] $\mathrm{C}=(\mathrm{a}, \mathrm{C})$
一長度為2的遞迴串列。
\end{itemize}

從串列的定義中我們得到兩個重要的結果：
\begin{itemize}
\item[（一）] 串列可以給其他串列共用，如上例（三）之 B 串列中，兩個 A 串列變成 B 的子串列。
\item[（二）] 串列可以是遞迴的，如上例（四）之 C 串列。
\end{itemize}

\section*{三．一般串列在多項式表達方面之作法}
\begin{itemize}
\item[（一）] 假設有一多項式
$$
P=x^{10} y^3 z^2+2 x^8 y^3 z^2+3 x^8 y^2 z^2+x^4 y^4 z+6 x^3 y^4 z+2 y z
$$
則可用（法 1）來表示如下：
\end{itemize}

【法1】
項次節點結構

\begin{tabular}{|l|l|l|}
\hline coef & $\exp \mathrm{x}$ & exp y \\
\hline exp z & \multicolumn{2}{|c|}{link} \\
\hline
\end{tabular}
缺點：若多項次之變數很多且各不相同，則節點 size 會變大，而浪費空間。
【法2】
節點結構

\begin{tabular}{|l|l|l|l|}
\hline trio & dlink & exp & link \\
\hline & & & \\
\hline
\end{tabular}

其中 trio 可能為 $\left[\begin{array}{ll}\text { variable ：vble } \\ \text { ptr } \quad \text { ：dlink } \\ \text { no } \quad \text { ：coef }\end{array}\right.$