第13章 有限狀態機
497

\section*{13－1 有限狀態機}

\section*{有限狀態機（Finite State Machine，F．S．M．）}

一個有限狀態機為一代數系統 $M=\left[I, O, S, f_s, f_o\right]$ ，其中，
$I$ 表輸入符號集（input symbol set），
$O$ 表輸出符號集（output symbol set），
$S$ 表狀態集（state set），
$f_s: S \times I \rightarrow S$ 為一狀態轉換函數（state transition function），
$f_o: S \rightarrow O$ 為一輸出函數（output function）。
Note
\begin{itemize}
\item[（1）] 有時表達成 $M=\left[I, O, S, f_s, f_o, s_0\right]$ ，其中 $s_0$ 為給定的起始狀態（initial state）．
\item[（2）] 一般對 FSM 之定義分兩種，以上之定義為 Moore model。另一種為 Mealy model $M=\left[I, O, S, f_s, g\right]$ ，其中，
\begin{itemize}
\item[（1）] $I$ 表輸入符號集；$O$ 表輸出符號集；$S$ 表狀態集。
\item[（2）] $f_s: S \times I \rightarrow S$ 為一狀態轉換函數。
\item[（3）] $g: S \times I \rightarrow O$ 為一輸出函數。
\end{itemize}
\item[（3）] 另有一種表示法為 Finite State Automata（F．S．A．），用於認知語言和文法。
\item[（4）] FSM 表示法有兩種：狀態圖與狀態表。
\end{itemize}