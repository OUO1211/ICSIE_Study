第11章 二元關係及其應用
323

\section*{特殊二元關係的等價條件}

設 $R \subseteq A \times A$ 為 $A$ 上之一二元關係，則
\begin{itemize}
\item[（1）] $R$ 具反身性 $\Leftrightarrow R^0 \subseteq R$ 。
\item[（2）] $R$ 具非反身性 $\Leftrightarrow R^0 \cap R=\varnothing$ 。
\item[（3）] $R$ 具對稱性 $\Leftrightarrow R=R^{-1}$ 。
\item[（4）] $R$ 具非對稱性 $\Leftrightarrow R \cap R^{-1}=\varnothing$ 。
\item[（5）] $R$ 具反對稱性 $\Leftrightarrow R \cap R^{-1} \subseteq R^0$ 。
\item[（6）] $R$ 具遞移性 $\Leftrightarrow R^2 \subseteq R$ 。
\end{itemize}

【重要】
【證明】 $R^0=\{(x, x) \mid \forall x \in A\}$ 也稱為 $A$ 上的對角關係（diagonal relation），或相等關係。
\begin{itemize}
\item[（1）] 、（2）從定義可知。
\item[（3）] $R$ 具對稱性 ⇔ 其關係矩陣 $M_R$ 為對稱矩陣 $\Leftrightarrow M_R^T=M_R$ ，
又 $M_{R^{-1}}=M_R^T$ ，故得 $R$ 具對稱性 $\Leftrightarrow R=R^{-1}$ 。
\item[（4）]
$$
\begin{aligned}
\because(a, b) \in R \cap R^{-1} & \Leftrightarrow(a, b) \in R \text { 且 }(a, b) \in R^{-1} \\
& \Leftrightarrow(a, b) \in R \text { 且 }(b, a) \in R \Leftrightarrow R \text { 不具非對稱性。 }
\end{aligned}
$$
\item[（5）] 由反對稱性的定義與（4）可知。
\item[（6）] （⇒）設 $R$ 有遞移性，令 $(a, c) \in R^2$ ，則必存在 $b \in A$ ，使得 $(a, b) \in R,(b, c) \in R$ ，
但因為 $R$ 有遞移性，故 $(a, c) \in R$ ，所以 $R^2 \subseteq R$ 。
（⇐）設 $R^2 \subseteq R$ ，令 $(a, b) \in R,(b, c) \in R$ ，
則由 $R^2$ 的定義知 $(a, c) \in R^2$ ，但 $R^2 \subseteq R$ ，故 $(a, c) \in R$ ，故知 $R$ 有遞移性 ${ }^{\circ}$
\end{itemize}