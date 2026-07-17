第 5 章 對角化理論

67



5－3 對角化的定義、判別與做法



可對角化（diagonalizable）的定義

（1）考虑向量空間 $V$ 上的線性算子 $T$ ，若存在 $V$ 的基底 $\beta$ 使得 $[T]_\beta$ 為對角矩陣，則稱 $T$ 可對角化。

（2）考虑方陣 $A$ ，若存在可逆矩陣 $P$ 使得 $P^{-1} A P=D$ 為對角矩陣，則稱 $A$ 可對角化。

（亦即 $A$ 可與某對角矩陣 $D$ 相似）

Note

（1）考慮 $n$ 維向量空間 $V$ 上的線性算子 $T, \beta$ 為 $V$ 的一組基底，則 $[T]_\beta=D$ 為對角矩陣 $\Leftrightarrow \beta$ 中的向量均為 $T$ 的特徵向量．



【重要】



【證明】

令 $\beta=\left\{\boldsymbol{b}_1, \boldsymbol{b}_2, \ldots, \boldsymbol{b}_n\right\}$ 為 $V$ 的基底，（故 $\boldsymbol{b}_i \neq \mathbf{0}, \forall i$ ），則

$$

\begin{aligned}

& {[T]_\beta=D=\left[\begin{array}{cccc}

\lambda_1 & & & O \\

& \lambda_2 & & \\

& & \ddots & \\

O & & & \lambda_n

\end{array}\right]} \\

& \Leftrightarrow T\left(\boldsymbol{b}_1\right)=\lambda_1 \boldsymbol{b}_1, T\left(\boldsymbol{b}_2\right)=\lambda_2 \boldsymbol{b}_2, \ldots, T\left(\boldsymbol{b}_n\right)=\lambda_n \boldsymbol{b}_n, \\

& \Leftrightarrow \boldsymbol{b}_i \text { 為相對於 } \lambda_i \text { 特徵向量, } \forall i=1,2, \ldots, n .

\end{aligned}

$$

（2）考慮 $n$ 階方陣 $A$ ，可逆方陣 $P$ ，則

$P^{-1} A P=D$ 為對角方陣 $\Leftrightarrow P$ 的行向量都是 $A$ 的特徵向量．



【重要】



【證明】

令 $P$ 的行向量依序為 $\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n$ ，（則因 $P$ 可逆，故 $\boldsymbol{v}_i \neq \mathbf{0}, \forall i$ ），則

$$

\begin{aligned}

& P^{-1} A P=D=\left[\begin{array}{llll}

\lambda_1 & & & O \\

& \lambda_2 & & \\

& & \ddots & \\

O & & & \lambda_n

\end{array}\right] \\

& \Leftrightarrow A P=P D \\

& \Leftrightarrow A\left[\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n\right]=\left[\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n\right]\left[\begin{array}{llll}

\lambda_1 & & & O \\

& \lambda_2 & & \\

& & \ddots & \\

O & & & \lambda_n

\end{array}\right]

\end{aligned}

$$