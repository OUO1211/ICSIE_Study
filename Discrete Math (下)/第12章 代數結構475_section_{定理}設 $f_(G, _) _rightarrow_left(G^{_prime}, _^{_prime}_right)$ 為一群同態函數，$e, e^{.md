第12章 代數結構
475

\section*{定理}

設 $f:(G, *) \rightarrow\left(G^{\prime}, *^{\prime}\right)$ 為一群同態函數，$e, e^{\prime}$ 分別為 $G, G^{\prime}$ 的單位元素，則
\begin{itemize}
\item[（1）] $f(e)=e^{\prime}$ ．
\item[（2）] $f\left(a^{-1}\right)=f(a)^{-1}, \forall a \in G$ 。
\item[（3）] 若 $H$ 為 $G$ 的子群，則 $f(H)$ 亦為 $G^{\prime}$ 的子群。
\end{itemize}

\section*{【證明】}
\begin{itemize}
\item[（1）] $\because e^{\prime *} f(e)=f(e)=f\left(e^* e\right)=f(e)^{*^{\prime}} f(e)$ ，且 $G^{\prime}$ 為群，＊＇有消去性，$\therefore e^{\prime}=f(e)$ 。
\item[（2）] $\because f(a)^{*^{\prime}} f\left(a^{-1}\right)=f\left(a^* a^{-1}\right)=f(e)=e^{\prime}$ ，同理 $f\left(a^{-1}\right)^{*^{\prime}} f(a)=e^{\prime}, \therefore f(a)^{-1}=f\left(a^{-1}\right)$ 。
\item[（3）] 很明顯 $f(H)$ 為 $G^{\prime}$ 的非空子集合，
對任意 $y_1, y_2 \in f(H)$ ，存在 $x_1, x_2 \in H$ ，s．t．$f\left(x_1\right)=y_1, f\left(x_2\right)=y_2$ ，
$\therefore y_1{ }^* y_2{ }^{-1}=f\left(x_1\right) *^{\prime} f\left(x_2\right)^{-1}=f\left(x_1\right)^{*^{\prime}} f\left(x_2{ }^{-1}\right)=f\left(x_1{ }^* x_2{ }^{-1}\right) \in f(H)$ 。
$\left(\because x_1 * x_2{ }^{-1} \in H\right)$
\end{itemize}