第 8 章 圖論1 89

\section*{8－7 同構}

\section*{圖形的同構（isomorphic）}

考虑圖 $G_1=\left(V_1, E_1\right), G_2=\left(V_2, E_2\right)$ ，若存在一函数 $f: V_1 \xrightarrow{1-1, \text { onto }} V_2$ 滿足：
$\forall a, b \in V,(a, b) \in E_1 \Leftrightarrow(f(a), f(b)) \in E_2$ ，則稱 $f$ 為一同構函數（isomorphism），
且稱 $G_1$ 與 $G_2$ 為同構，記為 $G_1 \cong G_2$ 。
例如：
下列左邊兩圖雖然形狀不盡相同，但構造相同；右邊兩圖也是構造相同。

Note
\begin{itemize}
\item[（1）] 判斷不同構的簡單方法：
\begin{itemize}
\item[（1）] 點數不同。
\item[（2）] 邊數不同。
\item[（3）] 連通性不同。
\item[（4）] 度數序列不同。但是，度數序列相同不一定同構。
\item[（5）] 特定子圖：（如 $C_n$ 或 $K_n$ ）。
\item[（6）] 特定點之距離。
\item[（7）] 檢查各自的補圖。
\end{itemize}
\item[（2）] $G_1, G_2$ 為無向無迴圈圖，則 $G_1 \cong G_2 \Leftrightarrow \overline{G_1} \cong \overline{G_2}$ 。
【證明】
若 $G_1 \cong G_2$ ，
即 $\exists f: V\left(G_1\right) \xrightarrow{1-1, \text { onto }} V\left(G_2\right)$ ，s．t．$(a, b) \in E\left(G_1\right) \Leftrightarrow(f(a), f(b)) \in E\left(G_2\right)$
即 $\exists f: V\left(G_1\right) \xrightarrow{1-1, \text { onto }} V\left(G_2\right)$ ，s．t．$(a, b) \notin E\left(G_1\right) \Leftrightarrow(f(a), f(b)) \notin E\left(G_2\right)$
即 $\exists f: V\left(\overline{G_1}\right) \xrightarrow{1-1, \text { onto }} V\left(\overline{G_2}\right)$ ，s．t．$(a, b) \in E\left(\overline{G_1}\right) \Leftrightarrow(f(a), f(b)) \in E\left(\overline{G_2}\right)$
即 $\overline{G_1} \cong \overline{G_2}$ 。
\end{itemize}