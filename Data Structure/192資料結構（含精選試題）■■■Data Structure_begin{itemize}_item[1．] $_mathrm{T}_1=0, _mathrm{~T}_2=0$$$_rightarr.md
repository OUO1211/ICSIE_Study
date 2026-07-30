192
資料結構（含精選試題）
■■■

Data Structure
\begin{itemize}
\item[1．] $\mathrm{T}_1=0, \mathrm{~T}_2=0$
$$
\rightarrow \quad \begin{array}{ll}
\text { Inorder } & \text { 順序 : N } \\
\text { Preorder } & \text { 順序 : N }
\end{array}
$$
\item[2．] $\mathrm{T}_1=0, \mathrm{~T}_2 \neq 0$
$$
\begin{array}{lll}
\rightarrow & \text { Inorder } & \text { 順序: } \mathrm{NT}_2^{\prime} \\
& \text { Preorder } & \text { 順序: } \mathrm{NT}_2 *
\end{array}
$$
\item[3．] $\mathrm{T}_1 \neq 0, \mathrm{~T}_2=0$
$$
\rightarrow \quad \begin{array}{ll}
\text { Inorder } & \text { 順序: } \mathrm{T}_1^{\prime} \mathrm{N} \\
& \text { Preorder }
\end{array} \quad \text { 順序: } \mathrm{NT}_1^* *
$$
\item[4．] $\mathrm{T}_1 \neq 0, \mathrm{~T}_2 \neq 0$
$$
\rightarrow \quad \begin{array}{ll}
\text { Inorder } & \text { 順序: } \mathrm{T}_1^{\prime} \mathrm{NT}_2^{\prime} \\
& \text { Preorder }
\end{array} \quad \text { 順序: } \mathrm{NT}_1 * \mathrm{~T}_2 *
$$
由1～4知，其 Inorder 及 Preorder 的配對順序在1～4中皆不相同，因此給予一個二元樹必能產生一個唯一的配對（Inorder，Preorder），故給予一個配對（Inorder，Preorder）可決定一個唯一的二元樹。
\end{itemize}

\section*{例題 5－1}

給予一前序（Preorder）順序：ABCDEFGHI、中序（Inorder）順序：BCAEDGHFI 試推出其二元樹為何？

解 前序（DLR）
中序（LDR）
$$
\rightarrow \quad \mathrm{BC}
$$
\begin{itemize}
\item[] →先考慮 BC
\begin{itemize}
\item[] ∵ 在前序時是 BC，中序也是 BC
\item[] $\therefore \quad \mathrm{DLR}=\mathrm{LDR}$ ，且要有 D 存在
\item[] $\therefore \quad \mathrm{DR}$
\item[] 因此
\end{itemize}
\end{itemize}