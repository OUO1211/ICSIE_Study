542
離散數學（下）

\section*{正規表示式（regular expression）}

設 $I$ 為輸入集，一個正規表示式可遞迴的定義為：
法則 $1: \lambda$ 為正規表示式，
法則 2 ：$\forall i \in I, i$ 為正規表示式，
法則3：若 $A, B$ 為正規表示式，則 $A \vee B, A B, A^*$ 亦為正規表示式。
（ $A \vee B$ 有時記做 $A \mid B$ 或 $A+B$ ）。
例如： $0 *,(0+1) *$ 均為正規表示式。

\section*{正規集（regular set）}

每一正規表示式均對應一集合稱為正規集，對應方式如下：
\begin{itemize}
\item[（1）] 正規表示式 $\varnothing$ 及 $\lambda$ 分別對應到 $\varnothing$ 及 $\{\lambda\}$ 。
\item[（2）] $\forall i \in I$ ，正規表示式 $i$ 對應到 $\{i\}$ 。
\item[（3）] 若正規表示式 $A, B$ 分別對應的正規集為 $A^{\prime}, B^{\prime}$ ，則正規表示式 $A \vee B, A B, A^*$ 對應的正規集為 $A^{\prime} \cup B^{\prime}, A^{\prime} B^{\prime},\left(A^{\prime}\right)^*$ ．
\end{itemize}

Note
\begin{itemize}
\item[（1）] 例如 ： $0^*,(0+1) *$ 所對應的正規表示集分別為：
$\{\lambda, 0,00, \ldots\}=\left\{0^k \mid k \geq 0\right\}$ 與 $\{\lambda, 0,1,00,01,10,11, \ldots\} 。$
\item[（2）] Kleene＇s 定理：設 $L$ 為一正規集，則存在一自動狀態機 $M$ 認知 $L$ 。【 90 成大工科】
\item[（3）] If $A$ is a regular，then the set $A^R$ consisting of the reverse of all strings in $A$ is also regular．
【 93 成大工科】
\end{itemize}

\section*{例題 2}

Use regular expression to show the set of strings accepted by the following finite－state machine．
【94 中正資工】
解 $00^* 1(0 \vee 1)^* \vee 11^* \vee 11^* 00^* 1(0 \vee 1)^*$ ．