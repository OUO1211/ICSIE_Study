第12章 代數結構 447

\section*{子群（subgroup）}

設 $H$ 為群 $(G, *)$ 的一子集且滿足 $(H, *)$ 亦為一群，則稱 $(H, *)$ 為 $(G, *)$ 的一個子群。
Note
\begin{itemize}
\item[（1）] $G$ 為 $G$ 之 improper subgroup；$\{e\}$ 為 $G$ 之 trivial subgroup，其中 $e$ 為 $G$ 的單位元素。
\item[（2）] $H$ 中之單位元素與 $G$ 中之單位元素必相同。
\item[（3）] $H$ 中之運算方式與 $G$ 中之運算方式需相同，例如：（ $\{$ 偶整數 $\},+)$ 為 $(Z,+)$ 之子群，但$\left(Q^{+}, \cdot\right)$ 不為 $(R,+)$ 之子群。
\item[（4）] 設 $G$ 為一群，$H, K$ 為 $G$ 的子群，則 $H \cap K$ 亦為 $G$ 的子群。
【證明】
只需證 ：$\forall a, b \in H \cap K, a b^{-1} \in H \cap K$ 。【102 輔大資工】
取 $a, b \in H \cap K, \because a, b \in H$ ，且 $H$ 為 $G$ 之子群 $\therefore a b^{-1} \in H$ 。
同理，$\because a, b \in K$ ，且 $K$ 為 $G$ 之子群 $\therefore a b^{-1} \in K, \therefore a b^{-1} \in H \cap K$ 。
\item[（5）] 設 $G$ 為一群，$H, K$ 為 $G$ 的子群，則 $H \cup K$ 為 $G$ 的子群 $\Leftrightarrow H \subseteq K$ or $K \subseteq H$ 。
【證明】【102 輔大資工】
⇐ 若 $H \subseteq K$ 則 $H \cup K=K$ ，當然為 $G$ 的子群，
若 $K \subseteq H$ 則 $H \cup K=H$ ，當然亦為 $G$ 的子群。
⇒ 設 $H \not \subset K$ ，且 $K \not \subset H$ ，即 $\exists x \in H-K, \exists y \in K-H \therefore x, y \in H \cup K, \therefore x y \in H \cup K$ ，
但若 $x y \in H$ ，then $\because x^{-1} \in H \therefore x^{-1} x y \in H, \therefore y \in H$ ，得一矛盾。
若 $x y \in K$ ，then $\because y^{-1} \in K \quad \therefore x y y^{-1} \in K, \therefore x \in K$ ，亦得一矛盾。
故知 $H \subseteq K$ 或 $K \subseteq H$ 。
\end{itemize}