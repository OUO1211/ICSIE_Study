第五章 樹與二元樹 179
Tree＆Binary Tree

演算法 ：
```
procedure preorder(currentnode : treepointer);
    {Currentnode is a pointer to a root in a binary tree.}
begin
    if currentnode <> nil then
        begin
            write(currentnode ↑ .data);
            preorder(currentnode ↑ .lefchild);
            preorder(currentnode ↑ .rightchild);
        end
    end; {of perorder}
```


結果：－＋＊＊CDE

\section*{三．後序追縱（Postorder）LRD}

規則：1．先拜訪左子樹
\begin{itemize}
\item[2．] 再拜訪右子樹
\item[3．] 印出樹根資料內容
\end{itemize}

演算法 ：
```
procedure postorder(currentnode : treepointer);
        {Currentnode is a pointer to root in a binary tree.}
begin
    if currentnode <> nil then
        begin
            postorder(currentnode ↑ .leftchild);
            postorder(currentnode ↑ .righchild);
            write(currentnode ↑ .data);
        end
    end; {of postorder}
```


結果 ：AB＊CD＊＊＋E－