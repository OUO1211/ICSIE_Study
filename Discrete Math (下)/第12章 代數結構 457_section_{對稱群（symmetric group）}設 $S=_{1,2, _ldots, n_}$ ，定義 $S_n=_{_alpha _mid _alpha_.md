第12章 代數結構 457

\section*{對稱群（symmetric group）}

設 $S=\{1,2, \ldots, n\}$ ，定義 $S_n=\{\alpha \mid \alpha: S \xrightarrow[1-1, \text { onto }]{ } S\}$ ，
則 $\left(S_n\right.$, 。）為一群，稱為對稱群，其中。為函數之合成。
Note
\begin{itemize}
\item[（1）] $\forall \alpha \in S_n$ ，稱 $a$ 為 $S$ 上之一重排（permutation、也稱排列）。
\item[（2）] 對任何 $S_n$ 上之子群 $G$ ，都稱 $G$ 為 $S$ 上的排列群（permutation group on $S$ ）°
\item[（3）] 此處表達函數時通常用兩列表達法：
例如，考慮函數 $f:\{1,2,3\} \rightarrow\{1,2,3\}$ 定義成 $f(1)=3, f(2)=1, f(3)=2$ ，則記錄成 $f=\left(\begin{array}{lll}1 & 2 & 3 \\ 3 & 1 & 2\end{array}\right)$ ，上方放定義域、下方放對應的值。兩列表達法的合成方式如下：
例如，$p \circ q=\left(\begin{array}{llll}1 & 2 & 3 & 4 \\ 2 & 4 & 1 & 3\end{array}\right) \circ\left(\begin{array}{llll}1 & 2 & 3 & 4 \\ 2 & 3 & 1 & 4\end{array}\right)=\left(\begin{array}{llll}1 & 2 & 3 & 4 \\ 4 & 1 & 2 & 3\end{array}\right)$ ，由 $q$ 的 1 到下方的 2 ，再由 $p$ 的 2 到下方的 4 ，故合成後 1 下方為 4 ；由 $q$ 的 2 到下方的 3 ，再由 $p$ 的 3 到下方的 1 ，故合成後 2 下方為 1 ；由 $q$ 的 3 到下方的 1 ，再由 $p$ 的 1 到下方的 2 ，故合成後 3 下方為 2 ；由 $q$ 的 4 到下方的 4 ，再由 $p$ 的 4 到下方的 3 ，故合成後 4 下方為 3 。
\item[（4）] 本處之合成運算是以右運算方式：$(\alpha \circ \beta)(x)=\alpha(\beta(x)) \ldots$ 。
\item[（5）] 單位元素為 $e=\left(\begin{array}{llllll}1 & 2 & 3 & \ldots & n-1 & n \\ 1 & 2 & 3 & \ldots & n-1 & n\end{array}\right)$ ，即 $f(x)=x$ 。
\item[（6）] 若 $\alpha=\left(\begin{array}{cccccc}1 & 2 & 3 & \ldots & n-1 & n \\ \alpha(1) & \alpha(2) & \alpha(3) & \ldots & \alpha(n-1) & \alpha(n)\end{array}\right)$ ，則 $\alpha^{-1}=\left(\begin{array}{cccccc}\alpha(1) & \alpha(2) & \alpha(3) & \ldots & \alpha(n-1) & \alpha(n) \\ 1 & 2 & 3 & \ldots & n-1 & n\end{array}\right)$ 。
\item[（7）] 當 $n \geq 3$ 時，$S_n$ 為非交換群。
【證明】
$$
n=3 \text { 時, }\left(\begin{array}{lll}
1 & 2 & 3 \\
2 & 1 & 3
\end{array}\right)\left(\begin{array}{lll}
1 & 2 & 3 \\
1 & 3 & 2
\end{array}\right)=\left(\begin{array}{lll}
1 & 2 & 3 \\
2 & 3 & 1
\end{array}\right) \text {, 但 }\left(\begin{array}{lll}
1 & 2 & 3 \\
1 & 3 & 2
\end{array}\right)\left(\begin{array}{lll}
1 & 2 & 3 \\
2 & 1 & 3
\end{array}\right)=\left(\begin{array}{lll}
1 & 2 & 3 \\
3 & 1 & 2
\end{array}\right) \text { 。 }
$$
$n \geq 4$ 時，取含有上述兩個 cycle 的 permutation 即可。
例如，
$$
\left(\begin{array}{llll}
1 & 2 & 3 & 4 \\
2 & 1 & 3 & 4
\end{array}\right)\left(\begin{array}{llll}
1 & 2 & 3 & 4 \\
1 & 3 & 2 & 4
\end{array}\right) \neq\left(\begin{array}{llll}
1 & 2 & 3 & 4 \\
1 & 3 & 2 & 4
\end{array}\right)\left(\begin{array}{llll}
1 & 2 & 3 & 4 \\
2 & 1 & 3 & 4
\end{array}\right) .
$$
\end{itemize}