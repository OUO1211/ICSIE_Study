188
資料結構（含精選試題）
Data Structure

\section*{5－9 森林（Forest）化為二元樹的方法}

一．觀念作法
\begin{itemize}
\item[（一）] 將森林的各樹表示成二元樹。
\item[（二）] 將所有二元樹的樹根以 Sibling 的方式連結起來。
\item[（三）] 各 Root 順時針轉 45 度。
\end{itemize}

二．例子

5－10 森林的追蹤

一．森林的追蹤
\begin{itemize}
\item[（一）] 中序
\item[1．] 如果 F 為空的，那就直接返回。
\item[2．] 依樹中序走訪第一棵樹的各子樹。
\end{itemize}