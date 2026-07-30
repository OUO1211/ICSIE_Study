第 9 章 圖論 II 131

\section*{漢米爾頓路徑（Hamilton path）與漢米爾頓環路（Hamilton cycle）}

考虑點数至少3的無向圖 $G=(V, E)$ ，
$G$ 的漢米爾頓路徑是一個經過 $G$ 的每點恰一次的路徑；
$G$ 的漢米爾頓環路是一個經過 $G$ 的每點恰一次的環路；
若 $G$ 有一個漢米爾頓環路，則稱 $G$ 稱為漢米爾頓圖（Hamiltonian graph）。
【很重要】

如右圖即為漢米爾頓圖，$a-f-o-n-m-l-k-j-i-q-r-s-t-p-g-h-b-c-d-e-a$ ，$a-f-o-n-m-l-k-j-i-q-r-s-t-p-g-h-b-c-d-e-a$ ，
為其中一漢米爾頓環路。
為其中一漢米爾頓環路。

【105 交大應數】【106、108台北資工】

Note
\begin{itemize}
\item[1．] 本問題也稱環遊世界問題。
\item[2．] 判斷是否存在漢米爾頓環路，不存在簡單且一般化的作法。
\item[3．] 點度數都很小時，可以下列步驟輔助判別漢米爾頓圖：
\begin{itemize}
\item[（1）] 必須為連通。
\item[（2）] Degree $=2$ 的點的兩邊必選。
\item[（3）] 不能提前形成 cycle。
\end{itemize}
\end{itemize}
例如下列各圖均不為漢米爾頓圖 ：

【81 成大電機】

【91 中正資工】
以 $G_1$ 為例，如存在 Hamilton cycle，則因為 $b, c, j$ 均度數2，故此 cycle 必須使用 $(b, a),(b, g)$ ，$(j, g),(j, i),(c, a),(c, i)$ ，但因為每點恰經一次，所以就不能再使用 $(a, e),(g, d),(i, h)$ ，即在外圍形成 cycle，卻無法抵達內部的點，即不存在 Hamilton cycle。