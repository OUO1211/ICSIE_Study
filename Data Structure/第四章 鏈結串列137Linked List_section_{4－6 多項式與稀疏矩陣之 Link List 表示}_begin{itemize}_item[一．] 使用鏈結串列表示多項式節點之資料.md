第四章 鏈結串列
137
Linked List

\section*{4－6 多項式與稀疏矩陣之 Link List 表示}
\begin{itemize}
\item[一．] 使用鏈結串列表示多項式
節點之資料結構設計如下：

\begin{tabular}{|l|l|l|l|}
\hline & COEF & EXP & LINK \\
\hline type & polypointer＝↑ polynode； polynode＝record coef ：integer；｛儲存 Cofficient \} exp ：integer；｛儲存 Exponent \} link：polypointer；｛指向下一個節點\} end； & & \\
\hline
\end{tabular}
\end{itemize}

例題 4－4
多項 $\mathrm{a}=3 \mathrm{x}^{14}+2 \mathrm{x}^8+1$ 之表示方式如下：
多項式 $\mathrm{b}=8 \mathrm{x}^{14}-3 \mathrm{x}^{10}+10 \mathrm{x}^6$ 之表示方式如下：

例題 4－5
若是有兩個變數的多項式時，每一項次使用下列之結構：

\begin{tabular}{|l|l|l|l|}
\hline COEF & EXP－X & EXP－Y & LINK \\
\hline
\end{tabular}
$$
f(x, y)=3 x^3 y^3+2 x^2 y-4 x y^2+5
$$