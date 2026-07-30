406
離散數學（下）

\section*{11－4 絡}

絡（lattice）
若偏序集 $(S, \leq)$ 滿足任意元素 $a 、 b$ ，
\begin{itemize}
\item[（1）] $\operatorname{lub}\{a, b\}$ 存在（並記作 $a \vee b$ ，讀作 $a$ 與 $b$ 的 joint），
\item[（2）] glb $\{a, b\}$ 存在（並記作 $a \wedge b$ ，讀作 $a$ 與 $b$ 的 meet），
\end{itemize}

則稱 $(S, \leq)$ 為一個絡，並記成 $(S, \vee, \wedge)$ 。
【 99 高雄資工】
例如，
\begin{itemize}
\item[（1）] $(N, \leq)$ 中，$a \vee b=\max \{a, b\}, ~ a \wedge b=\min \{a, b\}$ 均存在，故為絡，記成 $(N, \max , \min )$ 。
\item[（2）] $(P(A), \subseteq)$ 中，$a \vee b=a \bigcup b, a \wedge b=a \cap b$ 均存在，故為絡，記成 $(P(A), \cup, \cap)$ 。
\item[（3）] $\left(D_m, \mid\right)$ 中，$a \vee b=\operatorname{lcm}(a, b)$（最小公倍數），$a \wedge b=\operatorname{gcd}(a, b)$（最大公因數）均存在，故為絡，記成 $\left(D_m, 1 \mathrm{~cm}, \mathrm{gcd}\right)$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 此處採用 Grimaldi 書上的定義方式，讀者請注意在劉炯郎教授書上的定義方式：設 $(S, \leq)$ 為偏序集，且滿足 $\forall a, b \in S$ ，
\begin{itemize}
\item[（i）] $\operatorname{lub}\{a, b\}$ 存在且唯一（並記作 $a \vee b$ ，讀作 $a$ 與 $b$ 的 join），
\item[（ii）] $\operatorname{gcd}\{a, b\}$ 存在且唯一（並記作 $a \wedge b$ ，讀作 $a$ 與 $b$ 的 meet），
\end{itemize}
\end{itemize}

則稱 $(S, \leq)$ 為一個絡，此時並記成 $(S, \vee, \wedge)$ 。
此兩種定義雖不同，但因當初定義 lub（還有 glb）的不同，所以此兩種關於絡的定義，最後所得結論是相同的。
\begin{itemize}
\item[（2）] 特別記住一個不是絡的例子：
\item[（3）] 子絡（sublattice）：設 $(S, \vee, \wedge)$ 為一絡，$S^{\prime}$ 為 $S$ 之一子集，且 $\left(S^{\prime}, \vee^{\prime}, \wedge^{\prime}\right)$ 亦為一絡，則稱 $\left(S^{\prime}, \vee^{\prime}, \wedge\right)$ 為 $(S, \vee, \wedge)$之子絡，其中 $\vee^{\prime}=\left.\vee\right|_{S^{\prime}}$ ：為 $\vee$ 限制在 $S^{\prime}$ 下的運算結果；$\wedge^{\prime}=\left.\wedge\right|_{S^{\prime}}$ ：為 $\wedge$ 限制在 $S^{\prime}$ 下的運算結果。
\end{itemize}