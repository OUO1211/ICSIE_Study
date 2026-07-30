第 9 章 圖論 II 169

著色多項式（chromatic polynomial）
$G=(V, E)$ 為無向圖，$P(G, k)$ 稱為 $G$ 的著色多項式，表示以 $k$ 種顏色對 $G$ 做正當著色的不同方法數。

例如，考慮 $K_{1,3}$ ，
【99 台大電機】
對 $a$ 點著色時，可用 $k$ 種顏色中的任一種，故有 $k$ 種著法，
對 $b$ 點著色時，只需避掉其鄰點 $a$ 所用過的顏色，故有 $k-1$ 種著法，對 $c$ 點著色時，只需避掉其鄰點 $a$ 所用過的顏色，故有 $k-1$ 種著法，
對 $d$ 點著色時，只需避掉其鄰點 $a$ 所用過的顏色，故有 $k-1$ 種著法，故得圖 $G$ 的著色多項式為 $P(G, k)=k(k-1)^3$ 。

例題 4
Find the chromatic polynomials of the following graph：

（1）

（2）

（3）

【99 中山電機】【89 高科電通】【92 中山電機】
解（1）$P(G, k)=\stackrel{b}{k} \times\left(k^c-1\right) \times\left(k^x-2\right) \times\left(k^a-2\right) \times\left(k^y-2\right)=k(k-1)(k-2)^3$ 。
\begin{itemize}
\item[（2）] $P(G, k)=k(k-1)(k-2)^2$ 。
\item[（3）] 若 $a$ 與 $d$ 同色，則方法數：$\stackrel{a}{k} \times \stackrel{d}{1} \times\left(k^c-1\right) \times\left(k^b-1\right)$ ；若 $a$ 與 $d$ 不同色，則方法數：$\stackrel{a}{k} \times\left(k^d-1\right) \times\left(k^c-2\right) \times\left(k^b-2\right)$ ；相加得 $P(G, k)=k^4-4 k^3+6 k^2-3 k$ 。
\end{itemize}