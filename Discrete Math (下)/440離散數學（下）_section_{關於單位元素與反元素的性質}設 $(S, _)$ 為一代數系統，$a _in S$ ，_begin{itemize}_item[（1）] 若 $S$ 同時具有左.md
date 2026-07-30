440
離散數學（下）

\section*{關於單位元素與反元素的性質}

設 $(S, *)$ 為一代數系統，$a \in S$ ，
\begin{itemize}
\item[（1）] 若 $S$ 同時具有左單位元素 $e_l$ 與右單位元素 $e_r$ ，則 $e_l=e_r$ 。
\end{itemize}

【91 交大資科】
\begin{itemize}
\item[（2）] 若 $S$ 具有結合性與單位元素 $e$ ，且 $a$ 具有左反元素 $b_l$ 及右反元数 $b_r$ ，則 $b_l=b_r{ }^{\circ}$
\end{itemize}

\section*{證明}
\begin{itemize}
\item[（1）] $\because e_r$ 是右單位元素 $\therefore e_l \cdot e_r=e_l$ ，
$\because e_l$ 是左單位元素 $\therefore e_l \cdot e_r=e_r$ ，
$\therefore e_r=e_l$ ．
\item[（2）] $\because b_r$ 是 $a$ 的右反元素 $\therefore a \cdot b_r=e$ ，
$\because b_l$ 是 $a$ 的左反元素 $\therefore b_l \cdot a=e$ ，
$\therefore b_r=e \cdot b_r=\left(b_l \cdot a\right) \cdot b_r=b_l \cdot\left(a \cdot b_r\right)=b_l \cdot e=b_l$ ．
\end{itemize}

Note
上述（2）的結合性條件若去掉了，則結論不見得成立。例如右列之代數系統，$a$ 的左反元素可為 $a$ 與 $b$ 。

\begin{tabular}{|l|l|l|l|}
\hline ＊ & $e$ & $a$ & $b$ \\
\hline $e$ & $e$ & $a$ & $b$ \\
\hline $a$ & a & $e$ & $e$ \\
\hline $b$ & b & $e$ & $e$ \\
\hline
\end{tabular}

\section*{半群（semi group）與單群（monoid）}

若 $(S, *)$ 為一具有封閉性與結合性之代數系統，則稱 $(S, *)$ 為一半群。
若 $(S, *)$ 為一具有封閉性，結合性與單位元素之代數系統，則稱 $(S, *)$ 為一單群。
\begin{itemize}
\item[] Note
（1）令 $\Sigma=\left\{x_1, x_2, \ldots, x_n\right\}$ 為一非空集合，$\Sigma^{+}$表示選取 $\Sigma$ 中的元素所形成之所有有限長度的字串集，定義連接（catenation）運算＊為 $\alpha=a_1 a_2 \ldots a_h, \beta=b_1 b_2 \ldots b_k$ ，
$\alpha^* \beta=a_1 a_2 \ldots a_h b_1 b_2 \ldots b_k$ ，則此運算滿足封閉性與結合性，稱 $\left(\Sigma^{+} *\right)$ 為半群（又稱自由半群）。
【92清大資工】
\begin{itemize}
\item[（2）] 若上述 $\left(\Sigma^{+},{ }^*\right)$ 再加入空字串 $\lambda$ ，則稱為自由單群。
\end{itemize}
\end{itemize}