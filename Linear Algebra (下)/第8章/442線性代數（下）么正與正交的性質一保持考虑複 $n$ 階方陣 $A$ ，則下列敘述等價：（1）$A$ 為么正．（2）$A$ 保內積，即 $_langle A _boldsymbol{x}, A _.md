442
線性代數（下）

么正與正交的性質一保持
考虑複 $n$ 階方陣 $A$ ，則下列敘述等價：
（1）$A$ 為么正．
（2）$A$ 保內積，即 $\langle A \boldsymbol{x}, A \boldsymbol{y}\rangle=<\boldsymbol{x}, \boldsymbol{y}\rangle, \forall \boldsymbol{x}, \boldsymbol{y} \in C^{n \times 1}$ 。
（3）$A$ 保長度，即 $\|A \boldsymbol{x}\|=\|\boldsymbol{x}\|, \forall \boldsymbol{x} \in C^{n \times 1}$ 。

【102交大應数】

【證明】
（1）⇒（2）
$$
\forall \boldsymbol{x}, \boldsymbol{y} \in C^{n \times 1},\langle A \boldsymbol{x}, A \boldsymbol{y}\rangle=\left\langle\boldsymbol{x}, A^H A \boldsymbol{y}\right\rangle=\langle\boldsymbol{x}, I \boldsymbol{y}\rangle=\langle\boldsymbol{x}, \boldsymbol{y}\rangle .
$$
（2）⇒（3）
$$
\forall \boldsymbol{x} \in C^{n \times 1},\|A \boldsymbol{x}\|^2=<A \boldsymbol{x}, A \boldsymbol{x}>=<\boldsymbol{x}, \boldsymbol{x}>=\|\boldsymbol{x}\|^2, \therefore\|A \boldsymbol{x}\|=\|\boldsymbol{x}\| .
$$
（3）⇒（1）
$$
\begin{aligned}
& \forall \boldsymbol{x} \in C^{n \times 1},\|A \boldsymbol{x}\|^2-\|\boldsymbol{x}\|^2=0, \\
& \therefore 0=<A \boldsymbol{x}, A \boldsymbol{x}>-<\boldsymbol{x}, \boldsymbol{x}>=<A^H A \boldsymbol{x}, \boldsymbol{x}>-<\boldsymbol{x}, \boldsymbol{x}>=<A^H A \boldsymbol{x}-\boldsymbol{x}, \boldsymbol{x}>=<\left(A^H A-I\right) \boldsymbol{x}, \boldsymbol{x}>, \\
& \therefore A^H A-I=O,
\end{aligned}
$$

故得 $A^H A=I$ ，故 $A$ 為么正．
（3）⇒（1）的推導過程有使用下列性質：
若矩陣 $A$ 滿足 $A^H=A$ ，且任何向量 $x$ 都使 $\langle A \boldsymbol{x}, \boldsymbol{x}\rangle=0$ ，則 $A$ 為零矩陣．
Pf：
$$
\begin{aligned}
\forall \boldsymbol{x}, 0 & =<A(A \boldsymbol{x}+\boldsymbol{x}),(A \boldsymbol{x}+\boldsymbol{x})>=<A(A \boldsymbol{x}), A \boldsymbol{x}>+<A \boldsymbol{x}, A \boldsymbol{x}>+<A(A \boldsymbol{x}), \boldsymbol{x}>+<A \boldsymbol{x}, \boldsymbol{x}> \\
& =0+<A \boldsymbol{x}, A \boldsymbol{x}>+<A \boldsymbol{x}, A \boldsymbol{x}>+0=2\|A \boldsymbol{x}\|^2 \Rightarrow A \boldsymbol{x}=0, \Rightarrow A=O
\end{aligned}
$$

Note
（1）考慮實方陣 $A$ ，則下列敘述等價：
（a）$A$ 為正交．
（b）$A$ 保內積，即 $\langle A \boldsymbol{x}, A \boldsymbol{y}\rangle=\langle\boldsymbol{x}, \boldsymbol{y}\rangle, \forall \boldsymbol{x}, \boldsymbol{y} \in R^{n \times 1}$ 。

【104中興資科】

（c）$A$ 保長度，即 $\|A \boldsymbol{x}\|=\|\boldsymbol{x}\|, \forall \boldsymbol{x} \in R^{n \times 1}$ 。
【證明】證明方式與前述相似。

【重要】