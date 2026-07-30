第11章 二元關係及其應用 307

\section*{關係的運算一反關係（inverse）}

令 $R: A \rightarrow B$ 為一關係，則 $R$ 之反關係 $R^{-1}: B \rightarrow A$ 定義為
$R^{-1}=\{(b, a) \mid(a, b) \in R\}$ ，即 $\forall a \in A, b \in B, a R b \Leftrightarrow b R^{-1} a$ 。
Note
\begin{itemize}
\item[（1）] $\left(R^{-1}\right)^{-1}=R$ ，即反關係的反關係為本身。
\item[（2）] $M_{R^{-1}}=\left(M_R\right)^T$ ，即反關係的關係矩陣，為原關係的關係矩陣作轉置（transpose）。
\end{itemize}

例如：令 $A=\{1,2,3,4\}, B=\{a, b, c\}$ ，
取 $R=\{(1, a),(1, b),(2, a),(3, a)\}$ ，
則 $R$ 之反關係，$R^{-1}=\{(a, 1),(b, 1),(a, 2),(a, 3)\}$ ，
其關係矩陣 ：$M_{R^{-1}}=\underset{b}{a}\left[\begin{array}{llll}1 & 2 & 3 & 4 \\ b & 1 & 1 & 0 \\ 1 & 0 & 0 & 0 \\ 0 & 0 & 0 & 0\end{array}\right]$ ，關係圖形：