426
離散數學（下）

\section*{布林表示式的最小化}

每個布林表示式皆可對應一邏輯網路（logic network）。一個布林表示式有許多不同的表示法，不同的表示法造成邏輯閘個數的不同，以下提供兩種簡化的方法。
\begin{itemize}
\item[（1）] 代數化簡
\item[（2）] 卡諾圖（Karnaugh Map）
\end{itemize}

\section*{二個變數}

例題（5）
求布林表示式的最佳簡化。
\begin{itemize}
\item[（1）] $E_1\left(x_1, x_2\right)=\bar{x}_1 \bar{x}_2+\bar{x}_1 x_2+x_1 x_2$ ．
\item[（2）] $A+A B$ ．
\item[（3）] $(A+B)^{\prime}\left(A^{\prime}+B^{\prime}\right)^{\prime}$ ．
\item[] 解（1）
$$
\begin{aligned}
E\left(x_1, x_2\right) & =\overline{x_1} \overline{x_2}+\overline{x_1} x_2+x_1 x_2=\overline{x_1} \overline{x_2}+\overline{x_1} x_2+\overline{x_1} x_2+x_1 x_2 \\
& =\overline{x_1}\left(\overline{x_2}+x_2\right)+\left(\overline{x_1}+x_1\right) x_2 \\
& =\overline{x_1}+x_2
\end{aligned}
$$
（2）
$$
\begin{aligned}
A+A B & =A I+A B \\
& =A(I+B) \\
& =A
\end{aligned}
$$
（3）
$$
\begin{aligned}
(A+B)^{\prime}\left(A^{\prime}+B^{\prime}\right)^{\prime} & =\left(A+B+A^{\prime}+B^{\prime}\right)^{\prime} \\
& =\left(A+A^{\prime}+B+B^{\prime}\right)^{\prime} \\
& =(I+I)^{\prime} \\
& =I^{\prime} \\
& =O .
\end{aligned}
$$
\item[] ∵ 等效律
\item[] ∵ 分配律
\item[] ∵ 補元素性質
\item[] $\because I$ 為宇上界
\item[] ∵ 分配律
\item[] $\because I$ 為宇上界
\item[] ∵ 笛摩根定律
\item[] ∵ 交換律
\item[] ∵ 補元素性質
\item[] ∵ 等效律
\item[] ∵ 補元素性質
\end{itemize}