314

線性代數（下）



歐式空間下求正交投影的方式

考虑 $R^{m \times 1}$ 的一子空間 $W, \boldsymbol{b}$ 為 $R^{m \times 1}$ 的某一向量，若 $W=C S(A)$ ，則

（1）正規方程（normal equation）$A^T A \boldsymbol{x}=A^T \boldsymbol{b}$ 必有解．



【重要】



（2）令 $\boldsymbol{x}$ 為正規方程的解，則 $p r o j_W \boldsymbol{b}=A \boldsymbol{x}$ 。

（3）若 $A$ 為行獨立矩陣，則 $\operatorname{proj}_W \boldsymbol{b}=A\left(A^T A\right)^{-1} A^T \boldsymbol{b}$ 。



【重要】



【證明】

（1）任取 $\boldsymbol{y} \in C S\left(A^T A\right)$ ，則存在 $\boldsymbol{x} \in R^{n \times 1}$ 使 $\boldsymbol{y}=\left(A^T A\right) \boldsymbol{x}=A^T(A \boldsymbol{x}) \in C S\left(A^T\right)$ ，故 $C S\left(A^T A\right) \subseteq C s\left(A^T\right)$ ，又因 $\operatorname{rank}\left(A^T A\right)=\operatorname{rank}\left(A^T\right)$ ，使得 $C S\left(A^T A\right)=C S\left(A^T\right)$ ．任取 $\boldsymbol{b} \in R^{m \times 1}, A^T \boldsymbol{b} \in C S\left(A^T\right)=C S\left(A^T A\right)$ ，即存在 $\boldsymbol{x}_0 \in R^{n \times 1}$ 使得 $A^T \boldsymbol{b}=A^T A \boldsymbol{x}_0$ ．

（2）

$$

\begin{aligned}

A \boldsymbol{x}=\operatorname{proj}_W \boldsymbol{b} & \Leftrightarrow<\boldsymbol{b}-A \boldsymbol{x}, \boldsymbol{w}>=0, \forall \boldsymbol{w} \in W \\

& \Leftrightarrow<\boldsymbol{b}-A \boldsymbol{x}, A \boldsymbol{y}>=0, \boldsymbol{w}=A \boldsymbol{y}, \\

& \Leftrightarrow<A^T \boldsymbol{b}-A^T A \boldsymbol{x}, \boldsymbol{y}>=0, \\

& \Leftrightarrow A^T \boldsymbol{b}-A^T A \boldsymbol{x}=\mathbf{0} \\

& \Leftrightarrow A^T \boldsymbol{b}=A^T A \boldsymbol{x} .

\end{aligned}

$$

（3）若 $A$ 行獨立，則 $A^T A$ 可逆，

故正規方程 $A^T A \boldsymbol{x}=A^T \boldsymbol{b}$ 的解為 $\boldsymbol{x}=\left(A^T A\right)^{-1} A^T \boldsymbol{b}$ ，

再根據（2），

$$

\therefore \operatorname{proj}_W \boldsymbol{b}=A \boldsymbol{x}=A\left(A^T A\right)^{-1} A^T \boldsymbol{b} .

$$



也可另外以定義如下確認：

$$

A\left(A^T A\right)^{-1} A^T \boldsymbol{b}=A\left[\left(A^T A\right)^{-1} A^T \boldsymbol{b}\right] \in C S(A)=W,

$$

$\therefore \forall \boldsymbol{w} \in W$ ，存在 $\boldsymbol{x}$ 使得 $\boldsymbol{w}=A \boldsymbol{x}$ ，

$$

\begin{aligned}

\therefore\left\langle\boldsymbol{b}-A\left(A^T A\right)^{-1} A^T \boldsymbol{b}, \boldsymbol{w}\right\rangle & =\left\langle\boldsymbol{b}-A\left(A^T A\right)^{-1} A^T \boldsymbol{b}, A \boldsymbol{x}\right\rangle=\left\langle A^T\left(\boldsymbol{b}-A\left(A^T A\right)^{-1} A^T \boldsymbol{b}\right), \boldsymbol{x}\right\rangle \\

& =\left\langle A^T \boldsymbol{b}-A^T A\left(A^T A\right)^{-1} A^T \boldsymbol{b}, \boldsymbol{x}\right\rangle=\left\langle A^T \boldsymbol{b}-A^T \boldsymbol{b}, \boldsymbol{x}\right\rangle=0, \\

\therefore \operatorname{proj}_W \boldsymbol{b}=A\left(A^T A\right)^{-1} A^T \boldsymbol{b} . &

\end{aligned}

$$



Note

（1）此處所用的內積為標準內積．

（2）正規方程的解不一定唯一。

（3）把轉置換成共軛轉置，實矩陣換成複矩陣，則上述討論結果均成立。

（4）若 $A$ 沒有行獨立，則可先將 $A$ 作行運算，挑出最大行獨立集形成矩陣 $B$ ，再用 $B$ 代入（3）即可求出正交投影向量．