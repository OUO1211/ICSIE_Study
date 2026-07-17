第 5 章 對角化理論

137



對角化應用－求極限 $\lim A^n$

考虑方陣所形成的序列 $A_1, A_2, \ldots$ ，

若 $\lim _{k \rightarrow \infty}\left(A_k\right)_{i j}=(L)_{i j}, \forall i, j$ ，其中 $L$ 為一方陣，

則稱矩陣序列 $\left\{A_1, A_2, \ldots,\right\}$ 的矩陣極限存在並收敛到 $L$ ，記作 $\lim _{k \rightarrow \infty} A_k=L$ ．

Note

（1）考慮方陣 $A$ ，可逆矩陣 $P$ ，若 $\lim _{k \rightarrow \infty} A^k=L$ ，則 $\lim _{k \rightarrow \infty}\left(P A P^{-1}\right)^k=P L P^{-1}$ ．

（2）考慮對角化矩陣 $A$ 且 $A$ 的特徵根滿足 $|\lambda|<1$ 或 $\lambda=1$ ，則 $\lim _{k \rightarrow \infty} A^k$ 收斂。



例題

（15\％）Let $A=\left[\begin{array}{cc}1 & -1 \\ 1 & -3 / 2\end{array}\right]$ ．

（1）$(7 \%)$ Compute eigenvalues and the corresponding eigenvectors of $A$ ．

（2）$(8 \%)$ Compute $\lim _{n \rightarrow \infty} A^{2 n}$ ．

【93．94．97．100 台科資工、93 中央資工、98．99 彰師統計類題、99 台科資工】

解 $\operatorname{char}_A(x)=\operatorname{det}(A-x I)=x^2+0.5 x-0.5=(x-0.5)(x+1)$ ，

解得 $A$ 的特徵根 $0.5,-1$ ，

$$

\begin{aligned}

& V(0.5)=\operatorname{ker}(A-0.5 I)=\operatorname{ker}\left(\left[\begin{array}{cc}

0.5 & -1 \\

1 & -2

\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{l}

2 \\

1

\end{array}\right]\right\}, \\

& V(-1)=\operatorname{ker}(A+I)=\operatorname{ker}\left(\left[\begin{array}{cc}

2 & -1 \\

1 & -0.5

\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{l}

1 \\

2

\end{array}\right]\right\},

\end{aligned}

$$



取對應的特徵向量為 $\left[\begin{array}{l}2 \\ 1\end{array}\right],\left[\begin{array}{l}1 \\ 2\end{array}\right]$ ，

令 $P=\left[\begin{array}{ll}2 & 1 \\ 1 & 2\end{array}\right]$ ，則得 $P^{-1} A P=D=\left[\begin{array}{cc}0.5 & 0 \\ 0 & -1\end{array}\right]$ ，

$$

\begin{aligned}

& \therefore A^{2 n}=P D^{2 n} P^{-1}=\left[\begin{array}{ll}

2 & 1 \\

1 & 2

\end{array}\right]\left[\begin{array}{cc}

(0.5)^{2 n} & 0 \\

0 & (-1)^{2 n}

\end{array}\right]\left[\begin{array}{cc}

\frac{2}{3} & \frac{-1}{3} \\

\frac{-1}{3} & \frac{2}{3}

\end{array}\right], \\

& \therefore \lim _{n \rightarrow \infty} A^{2 n}=\left[\begin{array}{ll}

2 & 1 \\

1 & 2

\end{array}\right]\left(\lim _{n \rightarrow \infty}\left[\begin{array}{cc}

(0.5)^{2 n} & 0 \\

0 & (-1)^{2 n}

\end{array}\right]\right)\left[\begin{array}{cc}

\frac{2}{3} & \frac{-1}{3} \\

\frac{-1}{3} & \frac{2}{3}

\end{array}\right]=\left[\begin{array}{ll}

2 & 1 \\

1 & 2

\end{array}\right]\left[\begin{array}{cc}

0 & 0 \\

0 & 1

\end{array}\right]\left[\begin{array}{cc}

\frac{2}{3} & \frac{-1}{3} \\

\frac{-1}{3} & \frac{2}{3}

\end{array}\right]=\left[\begin{array}{cc}

\frac{-1}{3} & \frac{2}{3} \\

\frac{-2}{3} & \frac{4}{3}

\end{array}\right] .

\end{aligned}

$$