110

線性代數（下）



同步對角化（simultaneously diagonalizable）

（1）考虑 $V$ 上的算子 $T, U$ ，若存在 $V$ 的基底 $\beta$ 使得 $[T]_\beta=D_1,[U]_\beta=D_2$ 都是對角矩陣，则構 $T, U$ 可同步社角化．

（2）考感方伴 $A, B$ ，若存在可逆矩倳 $P$ 使得 $P^{-1} A P=D_1, P^{-1} B P=D_2$ 都是對角矩陣，則稱 $A, B$ 可同步對角化．



例如：考慮矩陣 $A=\left[\begin{array}{cc}2 & 1 \\ 1 & 2\end{array}\right], B=\left[\begin{array}{cc}3 & -1 \\ -1 & 3\end{array}\right]$ ，則

$\operatorname{char}_A(x)=\operatorname{det}\left(\left[\begin{array}{cc}2-x & 1 \\ 1 & 2-x\end{array}\right]\right)=(x-1)(x-3)$ ，得特徵根 1，3，

$$

\begin{aligned}

& \left.V(1)=\operatorname{ker}(A-I)=\operatorname{ker}\left(\left[\begin{array}{ll}

1 & 1 \\

1 & 1

\end{array}\right]\right)=\operatorname{span}\left\{\begin{array}{c}

-1 \\

1

\end{array}\right]\right\}, \\

& V(3)=\operatorname{ker}(A-3 I)=\operatorname{ker}\left(\left[\begin{array}{cc}

-1 & 1 \\

1 & -1

\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{l}

1 \\

1

\end{array}\right]\right\},

\end{aligned}

$$



故取 $P=\left[\begin{array}{cc}-1 & 1 \\ 1 & 1\end{array}\right]$ ，則 $P^{-1} A P=D_1=\left[\begin{array}{ll}1 & 0 \\ 0 & 3\end{array}\right]$ ，

又因 $B\left[\begin{array}{c}-1 \\ 1\end{array}\right]=\left[\begin{array}{c}-4 \\ 4\end{array}\right]=4\left[\begin{array}{c}-1 \\ 1\end{array}\right], B\left[\begin{array}{l}1 \\ 1\end{array}\right]=\left[\begin{array}{l}2 \\ 2\end{array}\right]=2\left[\begin{array}{l}1 \\ 1\end{array}\right]$ ，

（即 4,2 為其特徵根且對應特徵向量分別為 $\left[\begin{array}{c}-1 \\ 1\end{array}\right],\left[\begin{array}{l}1 \\ 1\end{array}\right]$ ）

故 $B P=P\left[\begin{array}{ll}4 & 0 \\ 0 & 2\end{array}\right]$ ，即 $P^{-1} B P=D_2=\left[\begin{array}{ll}4 & 0 \\ 0 & 2\end{array}\right]$ ．



Note

（1）設 $T, U \in L(V, V)$ ，若 $T, U$ 都可對角化，則 $T, U$ 可同步對角化 $\Leftrightarrow T U=U T$ ．

【證明】



【90中興應數、 94 成大應數、 99 政大應數、 100 師大數學】



設 $\operatorname{dim}(V)=n$ ，

⇒ 若 $T, U$ 可同步對角化，

令 $V$ 的基底 $\beta=\left\{\boldsymbol{b}_1, \boldsymbol{b}_2, \ldots, \boldsymbol{b}_n\right\}$ 使得 $[T]_\beta=D_1,[U]_\beta=D_2$ 都是對角矩陣，

則 $[T U]_\beta=[T]_\beta[U]_\beta=D_1 D_2=D_2 D_1=[U]_\beta[T]_\beta=[U T]_\beta$ ，

則 $(T U)\left(\boldsymbol{b}_i\right)=(U T)\left(\boldsymbol{b}_i\right), \quad \forall i=1,2, \ldots, n$ ，

即 $\forall x \in V, T U(x)=U T(x)$ ，即 $T U=U T$ ．