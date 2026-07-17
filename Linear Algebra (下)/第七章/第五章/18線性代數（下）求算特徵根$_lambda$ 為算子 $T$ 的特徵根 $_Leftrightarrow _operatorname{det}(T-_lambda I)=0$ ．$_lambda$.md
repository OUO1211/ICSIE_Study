18
線性代數（下）

求算特徵根
$\lambda$ 為算子 $T$ 的特徵根 $\Leftrightarrow \operatorname{det}(T-\lambda I)=0$ ．
$\lambda$ 為方陣 $A$ 的特徵根 $\Leftrightarrow \operatorname{det}(A-\lambda I)=0$ ．
【證明】
以下為對算子 $T$ 的證明，對方陣 $A$ 的討論雷同：
$\lambda$ 為 $T$ 的特徵根 ⇔ 存在 $\boldsymbol{v} \neq \mathbf{0}$ 使得 $T \boldsymbol{v}=\lambda \boldsymbol{v}$
$$
\begin{aligned}
& \Leftrightarrow \text { 存在 } \boldsymbol{v} \neq \mathbf{0} \text { 使得 } T \boldsymbol{v}-\lambda \boldsymbol{v}=\mathbf{0} \\
& \Leftrightarrow \text { 存在 } \boldsymbol{v} \neq \mathbf{0} \text { 使得 }(T-\lambda I) \boldsymbol{v}=\mathbf{0} \\
& \Leftrightarrow T-\lambda I \text { 不可逆 } \\
& \Leftrightarrow \operatorname{det}(T-\lambda I)=0 .
\end{aligned}
$$

例題 4
Find the eigenvalues for the following matrix：
$$
\begin{aligned}
& A=\left[\begin{array}{ll}
2 & 2 \\
1 & 3
\end{array}\right] . \\
& B=\left[\begin{array}{lll}
1 & 0 & 0 \\
5 & 1 & 1 \\
7 & 3 & 3
\end{array}\right] . \\
& C=\left[\begin{array}{ccc}
-1 & 1 & 0 \\
0 & -1 & 1 \\
-1 & 1 & 0
\end{array}\right] .
\end{aligned}
$$

【107 台大電機】

【109 台大流預】

【110 台科資工】

解 $\operatorname{det}(A-x I)=\left|\begin{array}{cc}2-x & 2 \\ 1 & 3-x\end{array}\right|=x^2-5 x+4=(x-1)(x-4)$ ，
得特徴根1，4．
$$
\operatorname{det}(B-x I)=\operatorname{det}\left(\left[\begin{array}{ccc}
1-x & 0 & 0 \\
5 & 1-x & 1 \\
7 & 3 & 3-x
\end{array}\right]\right)=(1-x)((1-x)(3-x)-3)=(1-x)\left(x^2-4 x\right),
$$

得特徴根 0，1，4．
$$
\operatorname{det}(C-x I)=\operatorname{det}\left(\left[\begin{array}{ccc}
-1-x & 1 & 0 \\
0 & -1-x & 1 \\
-1 & 1 & 0-x
\end{array}\right]\right)=(0-x)(0-x)(-2-x),
$$

得特徵根 $0,0,-2$ 。