第9章 圖論11
147

\section*{雙分圖與漢米爾頓問題}

設 $G=(A \cup B, E)$ 為一連通隻分圖，
\begin{itemize}
\item[（1）] 若 $G$ 有 Hamilton cycle，則 $|A|=|B|$ 。
（亦即：若 $|A| \neq|B|$ ，則 $G$ 沒有 Hamilton cycle。）
【89 成大電機】
\item[（2）] 若 $G$ 有 Hamilton path，則 $||A|-|B|| \leq 1$ ，
（亦即：若 $\|A|-| B\| \geq 2$ ，則 $G$ 没有 Hamilton path。）【88成大應數】【100台科資工】
\end{itemize}

\section*{【證明】}
\begin{itemize}
\item[（1）] 因為是雙分圖，故其環路上的點必是 $A, B$ 交錯，一去一回，故 $|A|=|B|$ 。
\item[（2）] 因為是雙分圖，故其路徑的點必 $A, B$ 交錯，則此路徑之點數若為偶數，必是 $|A|=|B|$ ，若為奇數，則起終點同為 $A$（或 $B$ ）的點，故 $|A|-|B|=1$（或 $|B|-|A|=1$ ）。
\end{itemize}

\section*{Note}

由上述定理知，判斷是否存在 Hamilton 問題時，若所討論的圖為雙分圖，且剛好兩側點數不同，則必不存在 Hamilton cycle，如 $G_1$ ；同理，若兩側點數超過1，則必不存在 Hamilton path，如 $G_2$ 。

\section*{基礎類題}
\begin{itemize}
\item[1．] Is there any Hamilton path in the graphs below？

（1）

（2）

（3）

（4）

【80 交大資科】【89 清大資工】【90 北科資工】【100 成大電機】【 105 嘉義資工】
\end{itemize}