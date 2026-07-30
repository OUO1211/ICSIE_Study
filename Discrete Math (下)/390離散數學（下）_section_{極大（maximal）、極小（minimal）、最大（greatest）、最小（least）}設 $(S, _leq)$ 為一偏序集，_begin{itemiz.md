390
離散數學（下）

\section*{極大（maximal）、極小（minimal）、最大（greatest）、最小（least）}

設 $(S, \leq)$ 為一偏序集，
\begin{itemize}
\item[（1）] 稱 $M \in S$ 為 $S$ 之極大元素，如果不存在其他 $S$ 中的元素 $x$ ，使 $M \leq x$ 。
\item[（2）] 稱 $m \in S$ 為 $S$ 之極小元素，如果不存在其他 $S$ 中的元素 $x$ ，使 $x \leq m 。$
\item[（3）] 稱 $I \in S$ 為 $S$ 之最大元素，如果對 $S$ 中的任意元素 $x$ ，均有 $x \leq I$ 。
\item[（4）] 稱 $O \in S$ 為 $S$ 之最小元素，如果對 $S$ 中的任意元素 $x$ ，均有 $O \leq x$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 極大（極小）元素不一定存在（例如 $S$ 為無限集時）；但若存在，也不一定唯一。其實，極大（極小）元素就是 Hasse 圖的頂層（底層）的元素。
\item[（2）] 最大（最小）元素不一定存在；但若存在，必定唯一（即至多 1 個）。其實當 Hasse 圖的頂層（底層）的元素只一個時，那就是最大（最小）元素。
\item[（3）] 設（ $S, \leq$ ）為一偏序集，$S \neq \varnothing$ 為有限集，則 $S$ 的極大（極小）元素必存在。
【108 台大電機】
\end{itemize}

\section*{上界（upper bound）、下界（lower bound）}

設 $(S, \leq)$ 為一偏序集，$A$ 為 $S$ 的一個子集，
\begin{itemize}
\item[（1）] 稱 $u \in S$ 為 $A$ 之上界，如果 $\forall x \in A, x \leq u$ 。
\item[（2）] 稱 $u \in S$ 為 $A$ 之最小上界（least upper bound，lub），
如果 $u$ 為 $A$ 之上界且對 $A$ 的其他上界 $u^{\prime}$ ，均有 $u \leq u^{\prime}$ 。
\item[（3）] 稱 $l \in S$ 為 $A$ 之下界，如果 $\forall x \in A, l \leq x$ 。
\item[（4）] 稱 $l \in S$ 為 $A$ 之最大下界（greatest lower bound，glb），
如果 $l$ 為 $A$ 之下界且對 $A$ 的其他下界 $l^{\prime}$ ，均有 $l^{\prime} \leq l$ 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] $S$ 的最大下界又稱 $S$ 的宇下界，也記為 $O$ ；（2）$S$ 的最小上界又稱 $S$ 的宇上界，也記為 $I$ ．
\item[（3）] $\forall A \subseteq S$ ，頂多只有一個 $\operatorname{lub}(\boldsymbol{A})$ 與 $\operatorname{glb}(\boldsymbol{A})$ ，但 $\operatorname{lub}(\boldsymbol{A})$ 與 $\operatorname{glb}(\boldsymbol{A})$ 不一定 $\in A$ 。
\item[（4）] 此處採用 Grimaldi 書上的定義方式，讀者請注意在劉炯郎教授書上的定義方式：
$u \in S$ 為 $A$ 之 lub，若 $u$ 為 $A$ 之上界且找不到其他的上界 $u^{\prime}$ 使 $u^{\prime} \leq u$ 。
$l \in S$ 為 $A$ 之 glb，若 $l$ 為 $A$ 之下界且找不到其他的下界 $l^{\prime}$ 使 $l \leq l^{\prime}$ 。
此兩種不同定義有時會造成答案不相同。
\item[（5）] 有時 glb又記為 inf（infimum）；lub 又記為 sup（supremum）。
\end{itemize}