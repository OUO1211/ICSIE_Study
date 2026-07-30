第10章 樹 237

\section*{生成樹個數－其他計算法}

另外，關於完全圖 $K_n$ 這個結構性相當特殊的圖，也有許多方式來探討其相異生成樹個數，除了可以 Kirchhoff 矩陣計算法計算之外（如下），後面也提供另外雨種看法供讀者参考：一是用 Prüfer code 編號法；另一是使用遞迴關係式（但不容易求通解，須用生成函数，計算繁瑣）。

矩陣法求 $\tau\left(K_n\right)$
考慮 $K_n$ 的 Laplace matrix ：$\left[\begin{array}{ccccc}n-1 & -1 & -1 & \cdots & -1 \\ -1 & n-1 & -1 & \cdots & -1 \\ -1 & -1 & n-1 & \cdots & -1 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ -1 & -1 & -1 & \cdots & n-1\end{array}\right]_{n \times n}$ ，
則 $\tau\left(K_n\right)=\left|\begin{array}{ccccc}n-1 & -1 & -1 & \cdots & -1 \\ -1 & n-1 & -1 & \cdots & -1 \\ -1 & -1 & n-1 & \cdots & -1 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ -1 & -1 & -1 & \cdots & n-1\end{array}\right|_{(n-1) \times(n-1)}$
$$
\stackrel{\text { 把 } 2 \sim n-1 \text { 列 }}{\text { 加到第一列 }}=\left|\begin{array}{ccccc}
1 & 1 & 1 & \cdots & 1 \\
-1 & n-1 & -1 & \cdots & -1 \\
-1 & -1 & n-1 & \cdots & -1 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
-1 & -1 & -1 & \cdots & n-1
\end{array}\right|_{(n-1) \times(n-1)} \stackrel{\text { 把第一列 }}{=}\left|\begin{array}{ccccc}
1 & 1 & 1 & \cdots & 1 \\
0 & n & 0 & \cdots & 0 \\
0 & 0 & n & \cdots & 0 \\
\vdots & \vdots & \vdots & \ddots & \vdots \\
0 & 0 & 0 & \cdots & n
\end{array}\right|_{(n-1) \times(n-1)}=n^{n-2} .
$$

Note
\begin{itemize}
\item[（1）] 此時的 $K_n$ 視為 $n$ 個經過標號的不同點的完全圖（labeled graph）。
\item[（2）] 而結果均可得 $\tau\left(K_n\right)=n^{n-2}$ ，稱之為 Cayley＇s formula。
\end{itemize}

【94 中山電機】
\begin{itemize}
\item[（3）] 例如：$\tau\left(K_4\right)=16, \tau\left(K_5\right)=125, \tau\left(K_6\right)=6^4$ 。
\end{itemize}

【83台大資工】【92中正資工】【98清大資應】
\begin{itemize}
\item[（4）] 此結果亦可解釋為點集合為 $\{1,2, \ldots, n\}$ 的樹共有 $n^{n-2}$ 個。
\end{itemize}