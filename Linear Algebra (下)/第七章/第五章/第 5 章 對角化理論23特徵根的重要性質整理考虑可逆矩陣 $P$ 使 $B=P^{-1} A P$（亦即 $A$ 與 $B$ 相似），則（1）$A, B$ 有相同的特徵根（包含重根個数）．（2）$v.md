第 5 章 對角化理論
23

特徵根的重要性質整理
考虑可逆矩陣 $P$ 使 $B=P^{-1} A P$（亦即 $A$ 與 $B$ 相似），則
（1）$A, B$ 有相同的特徵根（包含重根個数）．
（2）$v$ 為 $A$ 相對於 $\lambda$ 的特徵向量 $\Leftrightarrow P^{-1} v$ 為 $B$ 相對於 $\lambda$ 的特徵向量。
（3）$A B$ 與 $B A$ 有相同特徵根．
（4）$A$ 與 $A^T$ 有相同特徵根。
（5）若 $A$ 各行（列）元素和均為 $c$ ，則 $c$ 為 $A$ 的一個特徵根．
（6）$A$ 可逆 $\Leftrightarrow 0$ 不為 $A$ 的一個特徵根。
$\lambda$ 為 $A$ 相對於 $\boldsymbol{v}$ 的一個特徵根，則
（7）$\lambda^{-1}$ 為 $A^{-1}$ 相對於 $\boldsymbol{v}$ 的一個特徵根．（需 $A$ 可逆）
（8）$\lambda^k$ 為 $A^k$ 相對於 $\boldsymbol{v}$ 的一個特徵根。（ $k$ 為任意正整数）
（9）$f(\lambda)$ 為 $f(A)$ 相對於 $\boldsymbol{v}$ 的一個特徵根。（ $f$ 為多項式）
【證明】
【以上都超重要】
（1）方法一：
$c$ 為 $B$ 的特徵根
$$
\begin{aligned}
& \Leftrightarrow \operatorname{det}(B-c I)=0 \Leftrightarrow \operatorname{det}\left(P^{-1} A P-P^{-1} c I P\right)=0 \Leftrightarrow \operatorname{det}\left(P^{-1}(A-c I) P\right)=0 \\
& \Leftrightarrow \operatorname{det}\left(P^{-1}\right) \operatorname{det}(A-c I) \operatorname{det}(P)=0 \Leftrightarrow \operatorname{det}(A-c I)=0
\end{aligned}
$$
$\Leftrightarrow \lambda$ 為 $A$ 的特徵根．
方法二：
$\lambda$ 為 $A$ 相對於 $\boldsymbol{v}$ 的特徵根
$$
\begin{aligned}
& \Leftrightarrow A \boldsymbol{v}=\lambda \boldsymbol{v}, \boldsymbol{v} \neq \mathbf{0} \\
& \Leftrightarrow P B P^{-1} \boldsymbol{v}=\lambda \boldsymbol{v}, \boldsymbol{v} \neq \mathbf{0} \\
& \Leftrightarrow B P^{-1} \boldsymbol{v}=P^{-1} \lambda \boldsymbol{v}, \boldsymbol{v} \neq \mathbf{0} \\
& \Leftrightarrow B \boldsymbol{u}=\lambda \boldsymbol{u}, \boldsymbol{u}=P^{-1} \boldsymbol{v} \neq \mathbf{0},\left(\because P^{-1} \text { 可逆 }\right)
\end{aligned}
$$
$\Leftrightarrow \lambda$ 為 $B$ 相對於 $\boldsymbol{u}=P^{-1} \boldsymbol{v}$ 的特徵根．
（2）由（1）的證明可得．
（3）令 $\lambda$ 為 $A B$ 的特徵根，
（i）若 $\lambda=0$ ，則
$$
\operatorname{det}(A B-0 I)=0 \Leftrightarrow \operatorname{det}(A B)=0 \Leftrightarrow \operatorname{det}(B A)=0 \Leftrightarrow \operatorname{det}(B A-0 I)=0,
$$
$\therefore 0$ 亦為 $A B$ 的特徵根．
（ii）若 $\lambda \neq 0$ ，則