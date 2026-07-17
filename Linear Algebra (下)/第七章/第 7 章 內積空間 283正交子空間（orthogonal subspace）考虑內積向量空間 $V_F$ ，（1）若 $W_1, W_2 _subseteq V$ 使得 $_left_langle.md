第 7 章 內積空間 283

正交子空間（orthogonal subspace）
考虑內積向量空間 $V_F$ ，
（1）若 $W_1, W_2 \subseteq V$ 使得 $\left\langle\boldsymbol{w}_1, \boldsymbol{w}_2\right\rangle=0, \forall \boldsymbol{w}_1 \in W_1, \boldsymbol{w}_2 \in W_2$ ，
則稱 $W_1, W_2$ 為正交子空間，記做 $W_1 \perp W_2$ ．
（2）若 $W_1, W_2, \cdots, W_k \subseteq V$ 使得 $W_i \perp W_j, \forall i \neq j$ ，
則稱 $W_1, W_2, \cdots, W_k$ 為正交子空間．
例如：
考慮 $V=R^3$ ，
$W_1=\{(a, 0,0) \mid a \in R\}$ ，即 $x-$ 軸；
$W_2=\{(0, b, 0) \mid b \in R\}$ ，即 $y$－軸；
$W_3=\{(0,0, c) \mid c \in R\}$ ，即 $z$－軸；
$W_4=\{(a, b, 0) \mid a, b \in R\}$ ，即 $x y$ 平面，
則
（1）$W_4 \perp W_3, W_1 \perp W_2, W_1 \perp W_3, W_2 \perp W_3$ ，
（2）$W_1, W_2, W_3$ 形成正交子空間．

Note
若 $W_1, W_2, \cdots, W_k$ 為正交子空間，則 $W_1, W_2, \cdots, W_k$ 為獨立子空間．
【證明】
設 $\boldsymbol{w}_1+\boldsymbol{w}_2+\ldots+\boldsymbol{w}_k=\mathbf{0}$ ，其中 $\boldsymbol{w}_i \in W_i, \forall i=1,2 \ldots, k$ ．
則 $\forall i=1,2 \ldots, k$ ，
$$
\begin{aligned}
0 & =<\boldsymbol{w}_i, \mathbf{0}> \\
& =<\boldsymbol{w}_i, \boldsymbol{w}_1+\boldsymbol{w}_2+\ldots+\boldsymbol{w}_k> \\
& =<\boldsymbol{w}_i, \boldsymbol{w}_1>+<\boldsymbol{w}_i, \boldsymbol{w}_2>+\ldots+<\boldsymbol{w}_i, \boldsymbol{w}_k> \\
& =0+0+\ldots+<\boldsymbol{w}_i, \boldsymbol{w}_i>+\ldots+0 \\
& =<\boldsymbol{w}_i, \boldsymbol{w}_i>
\end{aligned}
$$

故得 $\boldsymbol{w}_i=\mathbf{0}$ ，故 $W_1, W_2, \ldots, W_k$ 為獨立子空間．