444
離散數學（下）

\section*{群的性質}

設 $\left(G,{ }^*\right)$ 為單位元素 $e$ 的一個群，則
\begin{itemize}
\item[（1）] $G \neq \varnothing$ 。
\item[（2）] 單位元素存在且唯一。
\end{itemize}

【90 中興資科】【90 南師資教】
\begin{itemize}
\item[（3）] $\forall a \in G, a$ 之反元素存在且唯一。
\item[（4）] $\forall a \in G,\left(a^{-1}\right)^{-1}=a$ ．
\item[（5）] $\forall a, b \in G,\left(a^* b\right)^{-1}=b^{-1} * a^{-1}$ ．
\item[（6）] $\forall a_1, a_2, \ldots, a_k \in G,\left(a_1{ }^* a_2{ }^* \ldots{ }^* a_k\right)^{-1}=a_k{ }^{-1} * \ldots * a_2{ }^{-1} * a_1{ }^{-1}$ ．
\item[（7）] $G$ 具有消去性。（反之未必成立）
\end{itemize}

【107暨南資工】
\begin{itemize}
\item[（8）] 若 $|G|$ 為偶數，則存在非單位元素 $a, a^2=e$ 。
\end{itemize}

【91 成大電機】
【證明】
\begin{itemize}
\item[（1）] 必有單位元素。
\item[（2）] 、（3）存在性是定義；唯一性之前證過了。
\item[（4）] $\because a^* a^{-1}=e=a^{-1} \cdot a, \therefore a$ 是 $a^{-1}$ 的反元素，即 $a=\left(a^{-1}\right)^{-1}$ 。
\item[（5）] $\because\left(a^* b\right)^*\left(b^{-1} * a^{-1}\right)=a * b^* b^{-1} * a^{-1}=a * e^* a^{-1}=e$ ，
且 $\left(b^{-1} * a^{-1}\right) *\left(a^* b\right)=b^{-1} * a^{-1} * a^* b=b^{-1} * e^* b=e$ ，
$\therefore b^{-1} * a^{-1}$ 是 $a * b$ 的反元素，即 $b^{-1} * a^{-1}=(a * b)^{-1}$ 。
\item[（6）] 對 $k$ 作歸納法可得。
\item[（7）] $\forall a, b, c \in G$ ，
$a * b=a * c \Rightarrow a^{-1} *(a * b)=a^{-1} *(a * c) \Rightarrow b=c$ ，所以有左消去性。
$b^* a=c^* a \Rightarrow\left(b^* a\right)^* a^{-1}=\left(c^* a\right)^* a^{-1} \Rightarrow b=c$ ，所以有右消去性。
（但反之不成立。ex：自由半群 $\left(\Sigma^{+}, \circ\right)$ 。）
\end{itemize}

Note
由群 $G$ 具有消去性，可得知群的二元運算表中每行每列之元素不重複。
\begin{itemize}
\item[（8）] 此結論即是指必存在一非單位元素 $a, a=a^{-1}$（即自身為自身之反元素）。反之，若每個$G$ 中的非單位元素都不是自己的反元素的話，因為反元素具有唯一性，則每個 $G$ 中的非單位元素都可找到另一個 $G$ 中的非單位元素，彼此為彼此的反元素。再加上單位元素，則 $G$ 共有奇數個元素。得一矛盾。
\end{itemize}