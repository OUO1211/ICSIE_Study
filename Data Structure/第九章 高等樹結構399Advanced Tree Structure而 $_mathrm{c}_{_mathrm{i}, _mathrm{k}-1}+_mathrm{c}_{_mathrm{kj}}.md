第九章 高等樹結構
399
Advanced Tree Structure

而 $\mathrm{c}_{\mathrm{i}, \mathrm{k}-1}+\mathrm{c}_{\mathrm{kj}}=\min _{\mathrm{i}<1 \leq \mathrm{j}}\left\{\mathrm{c}_{\mathrm{i}, 1-1}+\mathrm{c}_{1, \mathrm{i}}\right\}$
【例題 2 】
假設 $\mathrm{n}=4, ~\left(\mathrm{a}_1, \mathrm{a}_2, \mathrm{a}_3, \mathrm{a}_4\right)=\{$ do，if，read，while $\}$ ，
又設 $\left(\mathrm{p}_1, \mathrm{p}_2, \mathrm{p}_3, \mathrm{p}_4\right)=(3,3,1,1)$
且 $\left(\mathrm{q}_0, \mathrm{q}_1, \mathrm{q}_2, \mathrm{q}_3, \mathrm{q}_4\right)=(2,3,1,1,1)$
$\mathrm{w}_{01}=\mathrm{p}_1+\mathrm{w}_{00}+\mathrm{w}_{11}=\mathrm{p}_1+\mathrm{q}_1+\mathrm{w}_{00}=8$
$\mathrm{c}_{01}=\mathrm{w}_{01}+\min \left\{\mathrm{c}_{00}+\mathrm{c}_{11}\right\}=8$
$\mathrm{r}_{01}=1$
$\mathrm{w}_{12}=\mathrm{p}_2+\mathrm{w}_{22}=\mathrm{p}_2+\mathrm{q}_2+\mathrm{w}_{11}=7$
$\mathrm{c}_{12}=\mathrm{w}_{12}+\min \quad\left\{\mathrm{c}_{11}+\mathrm{c}_{22}\right\}=7$
$\mathrm{r}_{12}=2$
$\mathrm{w}_{23}=\mathrm{p}_3+\mathrm{w}_{22}+\mathrm{w}_{33}=\mathrm{p}_3+\mathrm{q}_3+\mathrm{w}_{22}=3$
$c_{23}=w_{23}+\min \left\{c_{22}+c_{33}\right\}=3$
$\mathbf{r}_{23}=3$
$\mathrm{w}_{34}=\mathrm{p}_4+\mathrm{w}_{33}+\mathrm{w}_{44}=\mathrm{p}_4+\mathrm{q}_4+\mathrm{w}_{33}=3$
$c_{34}=w_{34}+\min \left\{c_{33}+c_{44}\right\}=3$
$\mathbf{r}_{34}=4$
⋮
《圖示》計算 $\mathrm{c}_{04}$ 和 $\mathrm{r}_{04}$ ，此計算從列 0 到 4 逐列完成

\begin{tabular}{|l|l|l|l|l|l|}
\hline & 0 & 1 & 2 & 3 & 4 \\
\hline 0 & \begin{tabular}{l}
$$
w_{00}=2
$$ \\
$\mathrm{c}_{00}=0$ \\
$\mathrm{r}_{00}=0$
\end{tabular} & \begin{tabular}{l}
$$
w_{11}=3
$$ \\
$\mathrm{c}_{11}=0$ \\
$\mathrm{r}_{11}=0$
\end{tabular} & \begin{tabular}{l}
$$
w_{22}=1
$$ \\
$\mathrm{c}_{22}=0$ \\
$\mathrm{r}_{22}=0$
\end{tabular} & \begin{tabular}{l}
$$
w_{33}=1
$$ \\
$\mathrm{c}_{33}=0$ \\
$\mathrm{r}_{33}=0$
\end{tabular} & \begin{tabular}{l}
$$
w_{44}=1
$$ \\
$\mathrm{c}_{44}=0$ \\
$\mathrm{r}_{44}=0$
\end{tabular} \\
\hline 1 & \begin{tabular}{l}
$$
w_{01}=8
$$ \\
$\mathrm{c}_{01}=8$ \\
$\mathrm{r}_{01}=1$
\end{tabular} & \begin{tabular}{l}
$$
w_{12}=7
$$ \\
$\mathrm{c}_{12}=7$ \\
$\mathrm{r}_{12}=2$
\end{tabular} & \begin{tabular}{l}
$$
w_{23}=3
$$ \\
$\mathrm{c}_{23}=3$ \\
$\mathrm{r}_{23}=3$
\end{tabular} & \begin{tabular}{l}
$$
w_{34}=3
$$ \\
$\mathrm{c}_{34}=3$ \\
$\mathrm{r}_{34}=4$
\end{tabular} & \\
\hline 2 & \begin{tabular}{l}
$$
w_{02}=12
$$ \\
$\mathrm{c}_{02}=19$ \\
$\mathrm{r}_{02}=1$
\end{tabular} & \begin{tabular}{l}
$$
w_{13}=9
$$ \\
$\mathrm{c}_{13}=12$ \\
$\mathrm{r}_{13}=2$
\end{tabular} & \begin{tabular}{l}
$$
w_{24}=5
$$ \\
$\mathrm{c}_{24}=8$ \\
$\mathrm{r}_{24}=3$ or 4
\end{tabular} & & \\
\hline
\end{tabular}