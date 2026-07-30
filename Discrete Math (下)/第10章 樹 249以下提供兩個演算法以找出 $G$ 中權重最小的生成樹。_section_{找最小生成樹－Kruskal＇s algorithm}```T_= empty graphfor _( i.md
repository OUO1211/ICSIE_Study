第10章 樹 249

以下提供兩個演算法以找出 $G$ 中權重最小的生成樹。

\section*{找最小生成樹－Kruskal＇s algorithm}
```
T:= empty graph
for \( i = 1 \) to n - 1 \)
    e:= any edge in G with smallest weight
        that does not form a simple circuit
        when added to T
    \(\):= T \) with \( \ell \)
return T ( T is a min spanning tree of G)
```


【110 中興資科】
Note
\begin{itemize}
\item[（1）] Kruskal 演算法找出最小生成樹。
【95 交大資訊】【95 北科資工】
【證明】
由其演算法知，所得必為一生成樹，設為 $T^*$ 。
設 $w t\left(T^*\right)$ 不為最小，即另有生成樹其 weight 小於 $w t\left(T^*\right)$ 。
將 $G$ 的所有邊給編號 $e_1, e_2, \ldots$ ，
對 $G$ 的所有生成樹 $T$ ，定義 $\operatorname{index}(T)=\min \left\{i \mid e_i \in T^*-T\right\}$ ，
令 $T_{\text {max }}$ 為所有具 min weight 的樹中 index 最大的樹，且其 index 為 $k$ ，
即 $e_1, e_2, \ldots, e_{k-1} \in T^* \cap T_{\text {max }}, e_k \in T^*-T_{\text {max }}$ ，
則由換邊定理知：存在 $e_j \in T_{\text {max }}, j>k$ ，
使得 $T_1=\left\{T_{\text {max }}-e_j\right\} \bigcup\left\{e_k\right\}, T_2=\left\{T^*-e_k\right\} \bigcup\left\{e_j\right\}$ 均為生成樹。
若 $w t\left(e_j\right)<w t\left(e_k\right)$ ，則當初以此演算法找生成樹時就應先把 $e_k^{\prime}$ 選入 $T^*$ ，不合；
故知 $w t\left(e_j\right) \geq w t\left(e_k\right)$ ，所以得 $w t\left(T_1\right)=w t\left(T_{\text {max }}\right)-w t\left(e_j\right)+w t\left(e_k\right) \leq w t\left(T_{\text {max }}\right)$ ，
但 $w t\left(T_{\text {max }}\right)$ 為最小，所以 $w t\left(T_1\right)=w t\left(T_{\text {max }}\right)=$ 最小。
但此時，$e_1, e_2, \ldots, e_k \in T^* \cap T_1, \therefore \operatorname{index}\left(T_1\right)>k$ ，與當初 $T_{\text {max }}$ 的定義矛盾，
故知 $w t\left(T^*\right)$ 為最小，即 $T^*$ 為最小生成樹。
\end{itemize}