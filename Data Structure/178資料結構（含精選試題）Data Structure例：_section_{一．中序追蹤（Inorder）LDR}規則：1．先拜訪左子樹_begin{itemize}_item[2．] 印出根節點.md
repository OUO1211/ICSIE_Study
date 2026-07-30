178
資料結構（含精選試題）
Data Structure

例：

\section*{一．中序追蹤（Inorder）LDR}

規則：1．先拜訪左子樹
\begin{itemize}
\item[2．] 印出根節點內容
\item[3．] 再拜訪右子樹
\end{itemize}

遞迴演算法：
Procedure inorder（currentnode ：treepointer）；
｛Currentnode is a pointer to a root in a binary tree．\}
begin
if currentnode＜＞nil then
begin
inorder（currentnode ↑ ．leftchild）；
write（currentnode ↑ ．data）；
inorder（currentnode ↑ ．rightchild）；
end
end；｛of inorder\}
結果：A＊B＋C＊＊D－E

\section*{二．前序追蹤（Preorder）DLR}

規則：1．印出樹根資料內容
\begin{itemize}
\item[2．] 先拜訪左子樹
\item[3．] 再拜訪右子樹
\end{itemize}