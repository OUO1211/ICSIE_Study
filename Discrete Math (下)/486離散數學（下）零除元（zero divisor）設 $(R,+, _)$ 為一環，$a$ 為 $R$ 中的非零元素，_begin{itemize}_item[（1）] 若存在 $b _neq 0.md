486
離散數學（下）

零除元（zero divisor）
設 $(R,+, *)$ 為一環，$a$ 為 $R$ 中的非零元素，
\begin{itemize}
\item[（1）] 若存在 $b \neq 0$ ，使得 $a * b=0$ ，則稱 $a$ 為左零除元。
\item[（2）] 若存在 $b \neq 0$ ，使得 $b * a=0$ ，則稱 $a$ 為右零除元。
\item[（3）] 若存在 $b \neq 0$ ，使得 $a * b=b * a=0$ ，則稱 $a$ 為零除元。
\end{itemize}

Note
（1）例如 $:\left(Z_6,+_6,{ }_6\right)$ 中，$\because 2 \neq 0$ ，但 $3 .{ }_6 2=0, \therefore 2$ 即為零除元（當然 3 亦為零除元）。
\begin{itemize}
\item[（2）] 設 $(R,+, *)$ 為一個環，則
$R$ 不具左及右零除元 $\Leftrightarrow \forall a, b, c \in R$ ，若 $a b=a c$ 且 $b a=c a$ ，where $a \neq 0$ ，則 $b=c \circ$（即 $R$ 不具左及右零除元 $\Leftrightarrow R-\{0\}$ 中，＊具有消去性）
【證明】
⇐ 若存在零除元 $a$ ，即存在非零元素 $b$ ，使得 $a * b=b^* a=0$ ，
但 $0=a * 0$ ，故由消去性得 $b=0$ ，矛盾。
$\Rightarrow \forall a \in R-\{0\}$ ，若 $a b=a c$ ，則 $a b-a c=0, \therefore a *(b-c)=0 \therefore b-c=0 \therefore b=c$ ；
又 $b a=c a$ ，則 $b a-c a=0, \therefore(b-c) * a=0, b-c=0, \therefore b=c$ 。
\item[（3）] 若 $a$ 為環的 unit（即具有乘法反元素），則 $a$ 必不為零除元。
【93 暨南資工】
\end{itemize}