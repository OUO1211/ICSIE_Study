16
離散數學（下）

\section*{圖的矩陣表示－接合矩陣（incidency matrix）}
$M=\left[a_{i j}\right]_{n \times m}$ 紀錄 $G$ 中點與邊的連接情形。
（1）$G$ 為無向圖時，$a_{i j}= \begin{cases}0 & \text { else } \\ 1 & \text { 若邊 } e_j \text { 與點 } v_i \text { 相接 } \\ 2 & \text { 若 } e_j \text { 為點 } v_i \text { 上的loop }\end{cases}$
Rosen 的書上把 loop 記成1。
（2）$G$ 為有向圖沒 loop 時，$a_{i j}= \begin{cases}1 & \text { 若邊 } e_j \text { 指向點 } v_i \\ -1 & \text { 若邊 } e_j \text { 指出點 } v_i \\ 0 & \text { else }\end{cases}$也有些書與上述 1 與 -1 的定法互換；$M$ 的第 $i$ 横列的 +1 的個數 $=\operatorname{indeg}\left(v_i\right) 、 M$ 的第$i$ 横列的 -1 的個數 $=\operatorname{outdeg}\left(v_i\right)$ 。
例如：上圖中，
$$
\left.M(G)=\begin{array}{c} 
\\
a \\
b \\
c \\
d \\
e \\
f
\end{array}\left[\begin{array}{ccccccc}
e_1 & e_2 & e_3 & e_4 & e_5 & e_6 & e_7 \\
1 & 0 & 0 & 1 & 1 & 1 & 0 \\
0 & 0 & 0 & 0 & 1 & 1 & 1 \\
0 & 1 & 1 & 1 & 0 & 0 & 0 \\
0 & 0 & 1 & 0 & 0 & 0 & 0 \\
1 & 1 & 0 & 0 & 0 & 0 & 0
\end{array}\right] ; M(H)=\begin{array}{c}
a \\
b \\
c \\
d \\
e
\end{array} \begin{array}{ccccc}
e_1 & e_2 & e_3 & e_4 & e_5 \\
{\left[\begin{array}{c}
1 \\
-1 \\
0 \\
0 \\
0
\end{array}\right.} & \begin{array}{c}
0 \\
0 \\
0
\end{array} & \begin{array}{c}
1 \\
0 \\
0 \\
0
\end{array} & \begin{array}{c}
0 \\
0 \\
0
\end{array} & \begin{array}{c}
-1 \\
0 \\
1
\end{array} \\
0
\end{array}\right]
$$