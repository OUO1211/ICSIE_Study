536
離散數學（下）

\section*{13－3 自動狀態機}

\section*{自動狀態機（Finite State Automaton）}

一個自動狀態機 $M$ 為一個代數系統：$\left[I, S, f_s, A, S_0\right]$ ，其中，
$I$ ：輸入符號集；
$S$ ：狀態集；
$f_s: S \times I \rightarrow S$ 之狀態轉換函數；
$A \subseteq S$ ：為接受狀態集（accept state set）；
$S_0$ ：初始狀態（initial state）；
若 $I *$ 中的字串 $\alpha$ ，滿足從 $S_0$ 出發後停在接受狀態 $S_i \in A$ ，則稱為 $M$ 之接受字串（acceptstring）。若停在拒絕狀態 $S_j \notin A$ ，則稱為 $M$ 之拒絕字串（reject string）。

Note
設 $M$ 為一自動狀態機，$L=\{\alpha \mid \alpha$ 為 $M$ 中的接受字串 $\}$ ，則稱 $\boldsymbol{M}$ 認知 $\boldsymbol{L}$（ $M$ recognizes $L$ ），且稱 $L$ 為有限狀態語言（Finite State Language）或正規語言（regular language）。【90成大工科】

例題 1
Consider the finite state machine $M=\left(S, I, f, s_0, F\right)$ ，where the states set $S=\left\{s_0, s_1, s_2\right\}$ ，input set $I=\{a, b\}$ ，transition function $f$ defined as table， initial state $s_0$ ，finial state set $F=\left\{s_1\right\}$ ．
\begin{itemize}
\item[（a）] Does $M$ accept string abbabb？
\item[（b）] Find all string accepted by $M$ ．
\end{itemize}

\begin{tabular}{|l|l|}
\hline state & input $a \quad b$ \\
\hline $s_0$ & $s_0 s_1$ \\
\hline $s_1$ & $s_1 s_2$ \\
\hline $\boldsymbol{s}_{\mathbf{2}}$ & $s_2 s_0$ \\
\hline
\end{tabular}

解（1）yes．輸入後的狀態轉移如下圖。
$$
s_0 \xrightarrow{a} s_0 \xrightarrow{b} s_1 \xrightarrow{b} s_2 \xrightarrow{a} s_2 \xrightarrow{b} s_0 \xrightarrow{b} s_1
$$
\begin{itemize}
\item[（2）] 所有含 $3 k+1$ 個 $b$ 的字串，$k \geq 0$ 。
\end{itemize}