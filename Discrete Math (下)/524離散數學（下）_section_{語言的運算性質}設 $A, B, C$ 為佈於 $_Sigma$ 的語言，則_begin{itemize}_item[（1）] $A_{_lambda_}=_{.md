524
離散數學（下）

\section*{語言的運算性質}

設 $A, B, C$ 為佈於 $\Sigma$ 的語言，則
\begin{itemize}
\item[（1）] $A\{\lambda\}=\{\lambda\} A=A$ ．
\item[（2）] $(A B) C=A(B C)$ ．
\end{itemize}

【101 成大資工】
\begin{itemize}
\item[（3）] $A(B \cup C)=A B \cup A C ;(B \cup C) A=B A \cup C A$ ．
\item[（4）] $A(B \cap C) \subseteq A B \cap A C ;(B \cap C) A \subseteq B A \cap C A$ ．
\end{itemize}

【93 中興資科】【96 政大資科】【97 高雄資工】【101 成大資工】
\begin{itemize}
\item[（5）] $A \subseteq B \Rightarrow A^{+} \subseteq B^{+} ; \quad A \subseteq B \Rightarrow A^* \subseteq B^*$ ．
\item[（6）] $A A^*=A^* A=A^{+}$．
\item[（7）] $A^* A^*=A^*=\left(A^{+}\right)^*=\left(A^*\right)^{+}$．
\end{itemize}

【96政大資科】【101 成大資工】
\begin{itemize}
\item[（8）] $(A \cup B)^*=\left(A^* \cup B^*\right)^*=\left(A^* B^*\right)^*$ ．
\end{itemize}

【101 成大資工】
【證明】
以下為（4），（8）的證明，其他請讀者自行推導。
\begin{itemize}
\item[（4）] 設 $x y \in(B \cap C) A$ ，即 $x \in(B \cap C)$ ，且 $y \in A$ ，
故 $(x \in B$ 且 $y \in A)$ 且 $(x \in C$ 且 $y \in A)$ ，即 $x y \in B A \cap C A$ ，所以 $(B \cap C) A \subseteq B A \cap C A$ 。
\item[（8）]
$$
\begin{align*}
& \because A \subseteq A^*, B \subseteq B^*, \therefore A \cup B \subseteq A^* \cup B^*, \therefore(A \cup B)^* \subseteq\left(A^* \cup B^*\right)^*  \tag{1}\\
& \because A, B \subseteq A \cup B, \therefore A^* \subseteq(A \cup B)^*, B^* \subseteq(A \cup B)^* \\
& \therefore A^* \cup B^* \subseteq(A \cup B)^*, \therefore\left(A^* \cup B^*\right)^* \subseteq(A \cup B)^* \ldots \ldots . .(2) \tag{2}
\end{align*}
$$
由（1）（2）知 $\left(A^* \cup B^*\right)^*=(A \cup B)^*$ 。
$\because A^* \subseteq A^* B^*, \quad B^* \subseteq A^* B^*, \quad \therefore A^* \cup B^* \subseteq\left(A^* B^*\right), \quad \therefore\left(A^* \cup B^*\right)^* \subseteq\left(A^* B^*\right)^*$
任取 $x y \in A^* B^*$ ，即 $x \in A^*, y \in B^*, \therefore x, y \in A^* \cup B^*, \therefore x y \in\left(A^* \cup B^*\right)^*$ ，
$\therefore\left(A^* B^*\right) \subseteq\left(A^* \cup B^*\right)^*, \therefore\left(A^* B^*\right)^* \subseteq\left(\left(A^* \cup B^*\right)^*\right)^*=\left(A^* \cup B^*\right)^*$
由（3）（4）知 $\therefore\left(A^* B^*\right)^*=\left(A^* \cup B^*\right)^*$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 有的書上以＋表達 。 。
\item[（2）] $A B$ 不一定等於 $B A ; ~|A B|$ 不一定等於 $|B A| ; ~|A B|$ 不一定等於 $|B| \cdot|A|$ 。
例如 ：取 $\Sigma=\{a, b, c\}, A=\{a, a b, c\}, B=\{\lambda, b\}$ ，則
$A B=\{a, a b, c, a b b, c b\}, B A=\{a, a b, c, b a, b a b, b c\} \circ$
\item[（3）] $A B \cap A C \subseteq A(B \cap C)$ 末必成立：取 $A=\{1,11\}, B=\{1, \lambda\}, C=\{11, \lambda\}$ ，則
$A B=\{1,11,111\}, A C=\{1,11,111,1111\}$ ，但 $A(B \cap C)=\{1,11\}$ 。
\end{itemize}