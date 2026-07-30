第10章 樹 239

\section*{生成樹個數－其他計算法－遞迴}

Let $G=(V, E)$ be the undirected connected ladder graph shown in the following figure．For $n \geq 0$ ，let $a_n$ be the number of spanning trees of $G$ ，where as $b_n$ is the number of spanning trees that contain the edge $\left\{x_1, y_1\right\}$ ．
\begin{itemize}
\item[（1）] Find an equation that expresses $a_n$ in terms of $a_{n-1}$ and $b_n$ ．
\item[（2）] Find another equation that expresses $b_n$ in terms of $a_{n-1}$ and $b_{n-1}$ ．
\item[（3）] Use the result in part（1）＆（2）to set up and solve a recurrence relation for $a_n$ ．
【85 成大電機】 86 台大資工】
\end{itemize}

解 $a_n$ 可計算如下：
\begin{itemize}
\begin{itemize}
\item[（i）] 必選 $x_1 y_1$ 邊，即 $b_n$ 之定義；
\item[（ii）] 必不選 $x_1 y_1$ 邊，即考慮 $G-\left\{x_1, y_1\right\}$ 之 spanning tree，再加上邊 $x_1 x_2$ 與邊 $y_1 y_2$ ，即 $a_{n-1}$ ， $\therefore a_n=b_n+a_{n-1}$ 。
\item[] $b_n$ 可計算如下：
\item[（i）] 必選 $x_1 x_2$ 不選 $y_1 y_2$ ，即先考慮 $G-\left\{x_1, y_1\right\}$ 之 spanning tree，再加上邊 $x_1 x_2$ 與邊 $x_1 y_1$ ，故為 $a_{n-1}$ ；
\item[（ii）] 必選 $y_1 y_2$ 不選 $x_1 x_2$ ，即先考慮 $G-\left\{x_1, y_1\right\}$ 之 spanning tree 再加上邊 $y_1 y_2$ 與邊 $x_1 y_1$ ，故為 $a_{n-1}$ ；
\item[（iii）] 必選 $x_1 x_2$ 必選 $y_1 y_2$ ，即必選 $x_2-x_1-y_1-y_2$ 此path，因此若在 $G$ 中把此 path看成一邊，即等同於在 $G-\left\{x_1, y_1\right\}$ 中找必含 $x_2 y_2$ 邊之 spanning tree，故為 $b_{n-1}$ ；
$$
\therefore b_n=b_{n-1}+2 a_{n-1} .
$$
考慮 $n=1$ 時得初值條件 $a_1=1, b_1=1$ ，
故得遞迴關係式：$a_1=1, b_1=1$ ，且對於 $n \geq 2,\left\{\begin{array}{l}a_n=b_n+a_{n-1} \\ b_n=b_{n-1}+2 a_{n-1}\end{array}\right.$ ，
代入消去，再用特徵多項式法，可解得
$$
a_n=\frac{1}{2 \sqrt{3}}\left((2+\sqrt{3})^n-(2-\sqrt{3})^n\right), \quad n \geq 1 .
$$
\end{itemize}
\end{itemize}