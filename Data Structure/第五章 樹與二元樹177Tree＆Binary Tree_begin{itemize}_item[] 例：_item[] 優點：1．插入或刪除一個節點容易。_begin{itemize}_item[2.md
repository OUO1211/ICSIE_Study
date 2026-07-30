第五章 樹與二元樹
177
Tree＆Binary Tree
\begin{itemize}
\item[] 例：
\item[] 優點：1．插入或刪除一個節點容易。
\begin{itemize}
\item[2．] 對 Skewed Binary Tree 的表示較 Array 節省空間。
\end{itemize}
\item[] 缺點：1．很難找到該節點的 Parent
改善方式：可再加入一個 Parent 欄位，用以指向父親節點。
\begin{itemize}
\item[2．] 仍有一半的 Link 空間未使用。
\end{itemize}
\item[] 證明：假設一個二元樹有 n 個節點，故總共有 2 n 個 Link 欄，但只有 n－1 個 Link 欄用到，因此，浪費了 $2 n-(n-1)=n+1$ 個 Link 欄的空間。
\end{itemize}

\section*{5－5 二元樹的走訪、追蹤（Traversal）【非常重要】}
\begin{itemize}
\item[] －定義：走訪每一個節點一次。
\item[] －如果 L：表示拜訪左子樹。
\begin{itemize}
\item[] D：表印出節點資料。
\item[] R：表示拜訪右子樹。
\end{itemize}
\end{itemize}

那麼就有六種可能的走訪順序：LDR，LRD，DLR，DRL，RDL，RLD，若我們限制左子樹必在右子樹的之前走訪，那只有三種順序：LDR，LRD 及 DLR 等。其中 LDR：表示中序（Inorder）走訪
\begin{itemize}
\begin{itemize}
\item[] LRD：表後序（Postorder）走訪
\item[] DLR：表前序（Preorder）走訪
\end{itemize}
\end{itemize}