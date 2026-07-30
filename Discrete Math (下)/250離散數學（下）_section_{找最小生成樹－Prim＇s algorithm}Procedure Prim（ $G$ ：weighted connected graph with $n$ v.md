250
離散數學（下）

\section*{找最小生成樹－Prim＇s algorithm}

Procedure Prim（ $G$ ：weighted connected graph with $n$ vertices）
$$
\begin{aligned}
& V:=\left\{v_1, \ldots, v_n\right\} \\
& P:=\left\{v_1\right\} \\
& N:=V-P \\
& T:=\text { empty graph } \\
& \text { for } i=1 \text { to } n-1 \\
& \quad e:=\text { any edge between } P \text { and } N \text { of minimum weight } \\
& \quad \text { let } e=(x, y), x \text { in } P, y \text { in } N \\
& \qquad P:=P \text { with } y \text { added } \\
& \quad N:=N \text { with } y \text { deleted } \\
& \text { return } T\{T \text { is a min spanning tree of } G\}
\end{aligned}
$$

Note
\begin{itemize}
\item[（1）] Prim 演算法找出最小生成樹。【95 交大資訊】【95 北科資工】
\end{itemize}

【證明】
假設執行 Prim 演算法形成生成樹 $T_P$ ，且依序選出的邊編號為 $e_1 \sim e_{n-1}$ ，其中 $n=|V(G)|$ 。令由 $e_1, e_2, \ldots, e_k$ 形成的子圖為 $S_k$ ，
定義集合 $W$ ，收集圖 $G$ 的所有最小成本生成樹。
若 $T_P$ 不在 $W$ 中，則找出 $W$ 中最像 $T$ 的最小生成樹 $T_{\text {max }}$（即此生成樹包含的 $S_k$ 有最大$k$ ），即 $e_1 \sim e_k$ 屬於 $T_{\text {max }}$ ，但 $e_{k+1}$ 不屬於 $T_{\text {max }}$ 。
則由換邊定理可知，存在 $G$ 的某邊 $e_x$ ，使 $T_1=\left(T_{\text {max }} \cup\left\{e_{k+1}\right\}\right)-\left\{e_x\right\}$ 亦為 $G$ 的生成樹。而由Prim 演算法取邊的方式知，此 $e_x$ 不在 $e_1 \sim e_k$ 中，故 $T_1$ 包含 $e_1 \sim e_{k+1}$ 。同時，造 $S_k$ 並往外延伸後會選擇取 $e_{k+1}$ ，那表示 $e_{k+1}$ 的成本 $\leq e_x$ 的成本，故 $T_1$ 也是最小生成樹。
但因此時 $T_1$ 包含了 $S_{k+1}$ 而成為比 $T_{\max }$ 更像 $T_P$ 的最小生成樹，與 $T_{\max }$ 的定義不合。故知$T_P$ 必存在 $W$ 中，即 $T_P$ 為 $G$ 的一最小生成樹。