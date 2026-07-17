36
線性代數（下）

特徵多項式展開
考虑 $n$ 階方陣 $A$ ，
則 $\operatorname{char}_A(x)=(-x)^n+\operatorname{tr}_1(A)(-x)^{n-1}+\operatorname{tr}_2(A)(-x)^{n-2}+\cdots+\operatorname{tr}_{n-1}(A)(-x)+\operatorname{tr}_n(A)$ ，
其中， $\operatorname{tr}_i(A)$ 表 $A$ 中，所有恰含 $i$ 個對角項的 $i$ 階子行列式的和。
【95台大電機、99清大統計】
Note
（1） $\operatorname{tr}_1(A)=a_{11}+a_{22}+\cdots+a_{n n}=\operatorname{tr}(A)$ ．
（2） $\operatorname{tr}_n(A)=\operatorname{det}(A)$ ．

【95台大電機】

（3）$A$ 為 $2 \times 2$ 方陣時， $\operatorname{char}_A(\lambda)=x^2-\operatorname{tr}(A) x+\operatorname{det}(A)$ 。
（4）另外，令 $A$ 的特徵根是 $\lambda_1, \ldots, \lambda_n$ 則
$$
\begin{aligned}
\operatorname{char}_A(x) & =\left(\lambda_1-x\right)\left(\lambda_2-x\right) \cdots\left(\lambda_n-x\right) \\
& =(-x)^n+\left(\lambda_1+\lambda_2+\cdots+\lambda_n\right)(-x)^{n-1}+\cdots+\left(\lambda_1 \lambda_2 \cdots \lambda_n\right), \text { 故 }
\end{aligned}
$$
（a） $\operatorname{det}(A)=\lambda_1 \lambda_2 \cdots \lambda_n$ ．
【每年必考】
（b） $\operatorname{tr}(A)=\lambda_1+\lambda_2+\cdots+\lambda_n$ ．
【每年必考】
（c）$A$ 可逆 $\Leftrightarrow A$ 的所有特徵根均不為 0 ．
【每年必考】

例如
若 $A=\left[\begin{array}{llll}1 & 8 & 1 & 2 \\ 2 & 7 & 4 & 3 \\ 3 & 6 & 5 & 6 \\ 4 & 5 & 8 & 7\end{array}\right]$ 的特徵根是 $\lambda_1, \ldots, \lambda_4$ ，則

【清大統計】

$\operatorname{char}_A(x)=\operatorname{det}(A-x I)=\left(x-\lambda_1\right)\left(x-\lambda_2\right)\left(x-\lambda_3\right)\left(x-\lambda_4\right)$
$$
\begin{aligned}
= & x^4-\left(\lambda_1+\lambda_2+\lambda_3+\lambda_4\right) x^3+\left(\lambda_1 \lambda_2+\lambda_1 \lambda_3+\lambda_1 \lambda_4+\lambda_2 \lambda_3+\lambda_2 \lambda_4+\lambda_3 \lambda_4\right) x^2 \\
& -\left(\lambda_1 \lambda_2 \lambda_3+\lambda_1 \lambda_2 \lambda_4+\lambda_1 \lambda_3 \lambda_4+\lambda_2 \lambda_3 \lambda_4\right) x+\lambda_1 \lambda_2 \lambda_3 \lambda_4,
\end{aligned}
$$
$$
\begin{aligned}
\operatorname{tr}_1(A) & =1+7+5+7=20 \\
\operatorname{tr}_2(A) & =\lambda_1 \lambda_2+\lambda_1 \lambda_3+\lambda_1 \lambda_4+\lambda_2 \lambda_3+\lambda_2 \lambda_4+\lambda_3 \lambda_4 \\
& =\left|\begin{array}{ll}
1 & 8 \\
2 & 7
\end{array}\right|+\left|\begin{array}{ll}
1 & 1 \\
3 & 5
\end{array}\right|+\left|\begin{array}{ll}
1 & 2 \\
4 & 7
\end{array}\right|+\left|\begin{array}{ll}
7 & 4 \\
6 & 5
\end{array}\right|+\left|\begin{array}{ll}
7 & 3 \\
5 & 7
\end{array}\right|+\left|\begin{array}{ll}
5 & 6 \\
8 & 7
\end{array}\right|=24 . \\
\operatorname{tr}_3(A) & =\left|\begin{array}{lll}
1 & 8 & 1 \\
2 & 7 & 4 \\
3 & 6 & 5
\end{array}\right|+\left|\begin{array}{lll}
1 & 8 & 2 \\
2 & 7 & 3 \\
4 & 5 & 7
\end{array}\right|+\left|\begin{array}{lll}
1 & 1 & 2 \\
3 & 5 & 6 \\
4 & 8 & 7
\end{array}\right|+\left|\begin{array}{ccc}
7 & 4 & 3 \\
6 & 5 & 6 \\
5 & 8 & 7
\end{array}\right| . \\
\operatorname{tr}_4(A) & =\operatorname{det}(A) .
\end{aligned}
$$