第五章 樹與二元樹
193

Tree＆Binary Tree
→ 根據 Preorder 得知 D 為右樹的根，而在 Inorder 中，D 的左邊是 E 右邊是 GHFI。故

→ 其他依此類推，最後可得：
（二）一對中序順序（Inorder）及後序順序（Postorder）可決定一個唯一的二元樹。例：同上述之證明。
（三）一對前序順序（Preorder）及後序順序（Postorder）無法決定一個唯一的二元樹說明：假設一二元樹如下：

探討下列四種情況：
1． $\mathrm{T}_1=0, \mathrm{~T}_2=0$
$$
\begin{array}{ll}
\text { Preorder } & \text { : N } \\
\text { Postorder } & \text { : N }
\end{array}
$$

2． $\mathrm{T}_1=0, \mathrm{~T}_2 \neq 0$
$$
\begin{array}{ll}
\text { Preorder } & : \mathrm{NT}_2^{\prime} \\
\text { Postorder } & : \mathrm{T}_2 * \mathrm{~N}
\end{array}
$$

3． $\mathrm{T}_1 \neq 0, \mathrm{~T}_2=0$
$$
\begin{array}{ll}
\text { Preorder } & : \mathrm{NT}_1{ }^{\prime} \\
\text { Postorder } & : \mathrm{T}_1 * \mathrm{~N}
\end{array}
$$