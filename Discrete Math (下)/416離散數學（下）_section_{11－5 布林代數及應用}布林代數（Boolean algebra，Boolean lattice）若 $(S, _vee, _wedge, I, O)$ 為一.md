416
離散數學（下）

\section*{11－5 布林代數及應用}

布林代數（Boolean algebra，Boolean lattice）
若 $(S, \vee, \wedge, I, O)$ 為一有界、分配且互補的絡，
則稱 $(S, \vee, \wedge, I, O)$ 為一布林絡或布林代數，記為 $(B, \vee, \wedge, I, O,-)$ 。
Note
布林代數（ $B, \vee, \wedge, I, O,-$ ）具有性質：
\begin{itemize}
\item[（1）] 若 $B$ 有 $n$ 原子（宇下界往上一層的元素），則又記成 $B_n$ 。且由後面的同構證明可得，$B_n$中有 $2^n$ 個元素。
\item[（2）] 對偶性質（dual principle）：設 $S$ 為 $B$ 中恆為真的敘述，則其對偶敘述 $S^d$ 仍恆真。（ $S^d$ 是將 $S$ 中的 $\vee$ 換成 $\wedge ; \wedge$ 換成 $\vee, I$ 換成 $O, O$ 換成 $I$ 而得的敘述）
\item[（3）] 笛摩根定律（De－Morgan＇law）$\forall a, b \in B, \overline{a \vee b}=\bar{a} \wedge \bar{b} ; \overline{a \wedge b}=\bar{a} \vee \bar{b}$ ．
【證明】
$$
\begin{aligned}
& (a \vee b) \wedge(\bar{a} \wedge \bar{b})=[(a \wedge \bar{a}) \vee(b \wedge \bar{a})] \wedge \bar{b}=(b \wedge \bar{a}) \wedge \bar{b}=O \wedge \bar{a}=O, \\
& (a \vee b) \vee(\bar{a} \wedge \bar{b})=a \vee[(b \vee \bar{a}) \wedge(b \vee \bar{b})]=a \vee(b \vee \bar{a})=b \vee I=I,
\end{aligned}
$$
$\therefore \overline{a \vee b}=\bar{a} \wedge \bar{b}$ ，再由對偶性質可得 $: \overline{a \wedge b}=\bar{a} \vee \bar{b}$ 。
\end{itemize}