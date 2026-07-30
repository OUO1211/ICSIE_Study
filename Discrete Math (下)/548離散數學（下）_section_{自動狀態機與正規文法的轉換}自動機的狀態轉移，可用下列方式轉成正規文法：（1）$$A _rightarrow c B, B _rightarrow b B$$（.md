548
離散數學（下）

\section*{自動狀態機與正規文法的轉換}

自動機的狀態轉移，可用下列方式轉成正規文法：

（1）
$$
A \rightarrow c B, B \rightarrow b B
$$

（2）
$$
\text { ⟶ }{ }^b
$$
$$
A \rightarrow c B, B \rightarrow b B, A \rightarrow c, B \rightarrow b .
$$
$$
B \rightarrow \lambda, B \rightarrow b B .
$$

\section*{例題－ 5}

Please construct a grammar that specifies the language accepted by the following finite state machine．

【93 北科資工】【94 清大資應】
解 考慮文法 $G=(S, N, T, P)$ ，起始符號 $S=\{A\}$ ，
非終端符號 $N=\{A, B, C, D, E\}$ ，終端符號 $T=\{0,1\}$ ，
推演法則 $P=\{A \rightarrow 1 A|0 B, B \rightarrow 0 B| 1 C, C \rightarrow 0 B|1 D| 1, D \rightarrow 1 A|0 E| 0, E \rightarrow 1 C|0 D| 0\}$ 。