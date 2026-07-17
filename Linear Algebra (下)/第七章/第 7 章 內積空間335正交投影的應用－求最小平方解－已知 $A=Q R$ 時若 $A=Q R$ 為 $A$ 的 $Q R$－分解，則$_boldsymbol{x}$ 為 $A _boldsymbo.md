第 7 章 內積空間
335

正交投影的應用－求最小平方解－已知 $A=Q R$ 時
若 $A=Q R$ 為 $A$ 的 $Q R$－分解，則
$\boldsymbol{x}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的最小平方解 $\Leftrightarrow \boldsymbol{x}$ 滿足 $R \boldsymbol{x}=Q^T \boldsymbol{b}$ ．
【93．101 中央資工】
【證明】
$\boldsymbol{x}$ 使 $\|\boldsymbol{A} \boldsymbol{x}-\boldsymbol{b}\|$ 為最小
$$
\begin{aligned}
& \Leftrightarrow A^T A \boldsymbol{x}=A^T \boldsymbol{b}, \\
& \Leftrightarrow(Q R)^T(Q R) \boldsymbol{x}=(Q R)^T \boldsymbol{b}, \\
& \Leftrightarrow R^T Q^T Q R \boldsymbol{x}=R^T Q^T \boldsymbol{b}, \\
& \Leftrightarrow R^T R \boldsymbol{x}=R^T Q^T \boldsymbol{b},\left(\because Q \text { 行向量形成單範正交, } \therefore Q^T Q=I\right) \\
& \Leftrightarrow R \boldsymbol{x}=Q^T \boldsymbol{b},
\end{aligned}
$$
＂＊＂證明如下：
若 $R \boldsymbol{x}=Q^T \boldsymbol{b}$ ，當然 $R^T R \boldsymbol{x}=R^T Q^T \boldsymbol{b}$ ．
若 $R^T R \boldsymbol{x}=R^T Q^T \boldsymbol{b}$ ，則 $R R^T R \boldsymbol{x}=R R^T Q^T \boldsymbol{b}$ ，因 $R$ 列獨立，故 $R R^T$ 可逆，故得 $R \boldsymbol{x}=Q^T \boldsymbol{b}$ ．