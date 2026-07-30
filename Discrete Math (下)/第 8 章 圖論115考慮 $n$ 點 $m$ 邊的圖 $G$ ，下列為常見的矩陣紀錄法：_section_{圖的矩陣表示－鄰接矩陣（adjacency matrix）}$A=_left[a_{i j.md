第 8 章 圖論1
15

考慮 $n$ 點 $m$ 邊的圖 $G$ ，下列為常見的矩陣紀錄法：

\section*{圖的矩陣表示－鄰接矩陣（adjacency matrix）}
$A=\left[a_{i j}\right]_{n \times n}$ ：纪錄 $G$ 中點與點的連接情形。
\begin{itemize}
\item[（1）] $G$ 為無向圖時，$a_{i j}=v_i$ 與 $v_j$ 之間的邊數。
此時 $A$ 為對稱矩陣；若 $G$ 為簡單圖，則 $A$ 為零壹矩陣；對角項記錄 loop 個數（Rosen）。（有些書上把一個 loop 算成2）
\item[（2）] $G$ 為有向圖時，$a_{i j}=v_i$ 指向 $v_j$ 的邊数。
此時，第 $i$ 直行的和 $=\operatorname{indeg}\left(v_i\right)$ ；第 $i$ 横列的和 $=\operatorname{outdeg}\left(v_i\right)$ 。
例如：上圖中，$A(G)=\begin{gathered}a \\ b \\ c \\ d \\ e \\ f\left[\begin{array}{llllll}0 & 0 & 0 & 0 & 0 & 0 \\ 0 & 0 & 2 & 1 & 0 & 1 \\ 0 & 2 & 1 & 0 & 0 & 0 \\ 0 & 1 & 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 1 & 0 & 0 \\ 0 & 1 & 0 & 1 & 0 & 0\end{array}\right]\end{gathered}$
$$
A(H)=\begin{gathered}
a \\
b \\
c \\
d \\
e
\end{gathered}\left[\begin{array}{lllll}
0 & 0 & 0 & 0 & 0 \\
1 & 0 & 1 & 0 & 0 \\
0 & 0 & 0 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 \\
0 & 1 & 0 & 0 & 0
\end{array}\right] \text {. }
$$
\end{itemize}