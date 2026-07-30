第9章 圖論11201

\section*{對偶圖 G＊（dual graph）}
$G$ 為一平面圆，則其對偶圖 $G^*$ 以下列方式建立：
先给定一個平面圆 $G$（區域的编號為 $r_1, r_2, \ldots, r_m$ ），
則 $G^*$ 中的點就编號為 $r_1, r_2, \ldots, r_m$ ，
而 $G$ 中每個邊的左右兩區域（設為 $r_i, r_j$ ），反映在 $G^*$ 中，$r_i, r_j$ 就以一邊相連。
例如 ：

Note
\begin{itemize}
\item[（1）] 在上述定義下，$G^*$ 有可能出現 loop 或多重邊。
\item[（2）] $G^*$ 亦為平面圖。
\item[（3）] 若 $G \cong G^*$ ，則 $G$ 稱為自對偶（self－dual）圖。
\item[（4）] 對平面圖 $G$ 做區域著色，相當於對 $G$ 的對偶圖 $G^*$ 做點著色。
\end{itemize}