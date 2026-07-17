第 5 章 對角化理論
35

特徵多項式（characteristic polynomial）
定義方陣 $A$ 的特徵多項式 $c h a r_A(x)=\operatorname{det}(A-x I)$ ，其中 $I$ 為單位矩陣。
Note
（1）有時也把 $\operatorname{char}_A(x)$ 定義成 $\operatorname{det}(x I-A)$ ，而只是與上述有 $(-1)^n$ 倍的差別，不影響特徵根，其中 $A$ 為 $n \times n$ ．
（2）同理可以定義 $\operatorname{char}_T(x)=\operatorname{det}(T-x I)$ ，其中 $T$ 為 $V$ 上的線性映射，$I$ 為 $V$ 上的單位映射。
（3）考慮方陣 $A, B$ ，若 $A$ 與 $B$ 相似，則其特徵多項式相同。

【重要】

【證明】
設 $B=P^{-1} A P$ ，其中 $P$ 為可逆矩陣，則
$$
\begin{aligned}
\operatorname{char}_B(x) & =\operatorname{det}(B-x I)=\operatorname{det}\left(P^{-1} A P-P^{-1} x I P\right)=\operatorname{det}\left(P^{-1}(A-x I) P\right) \\
& =\operatorname{det}\left(P^{-1}\right) \operatorname{det}(A-x I) \operatorname{det}(P)=\operatorname{det}(A-x I)=\operatorname{char}_A(x)
\end{aligned}
$$
（4）若矩陣 $A, B$ 的特徵多項式相同，則有仍可能 $A$ 與 $B$ 不相似．
例如 $\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right]$ 與 $\left[\begin{array}{ll}1 & 1 \\ 0 & 1\end{array}\right]$ 的特徵式都是 $(1-x)^2$ ，但卻不相似。
（5）考慮方陣 $A$ 與 $B$ ，則 $A B$ 與 $B A$ 的特徵多項式相同。
【證明】
【89中央數學、90彰師數學、92台大數學】
$$
\because\left[\begin{array}{cc}
I & B \\
O & I
\end{array}\right]\left[\begin{array}{cc}
O & O \\
A & A B
\end{array}\right]\left[\begin{array}{cc}
I & -B \\
O & I
\end{array}\right]=\left[\begin{array}{cc}
B A & O \\
A & O
\end{array}\right],
$$

取 $X=\left[\begin{array}{cc}O & O \\ A & A B\end{array}\right], Y=\left[\begin{array}{cc}B A & O \\ A & O\end{array}\right], P=\left[\begin{array}{cc}I & B \\ O & I\end{array}\right]$ ，則 $P^{-1}=\left[\begin{array}{cc}I & -B \\ O & I\end{array}\right]$ ，而得 $X$ 與 $Y$ 相似，
故得 $\operatorname{char}_X(x)=\operatorname{char}_Y(x)$ ，即 $\operatorname{det}\left[\begin{array}{cc}-x I & O \\ A & A B-x I\end{array}\right]=\operatorname{det}\left[\begin{array}{cc}B A-x I & O \\ A & -x I\end{array}\right]$ ，
$$
\begin{aligned}
& \therefore \operatorname{det}(-x I) \operatorname{det}(A B-x I)=\operatorname{det}(B A-x I) \operatorname{det}(-x I), \\
& \therefore \operatorname{det}(A B-x I)=\operatorname{det}(B A-x I), \text { 即 } \operatorname{char}_{A B}(x)=\operatorname{char}_{B A}(x) .
\end{aligned}
$$