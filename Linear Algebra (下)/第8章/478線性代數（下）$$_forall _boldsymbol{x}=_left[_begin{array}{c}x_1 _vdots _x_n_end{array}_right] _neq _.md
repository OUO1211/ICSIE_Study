478
線性代數（下）
$$
\forall \boldsymbol{x}=\left[\begin{array}{c}
x_1 \\
\vdots \\
x_n
\end{array}\right] \neq \mathbf{0}, \text { 令 } \boldsymbol{y}=\left[\begin{array}{c}
y_1 \\
\vdots \\
y_n
\end{array}\right]=L^T \boldsymbol{x} \neq \mathbf{0},
$$

則 $\boldsymbol{x}^T A \boldsymbol{x}=\boldsymbol{x}^T\left(L D L^T\right) \boldsymbol{x}=\left(L^T \boldsymbol{x}\right)^T D\left(L^T \boldsymbol{x}\right)=\boldsymbol{y}^T D \boldsymbol{y}=d_1 y_1^2+\ldots+d_n y_n^2>0$ ，
而得 $A$ 為正定矩陣。
（3）性質（2）對複數矩陣亦成立。
（4）判斷正定矩陣常用方法：
（a）在元素有複數時，＂特徵根都是正數⇔為正定矩陣＂。
（b）對實數對稱矩陣：＂特徵根都是正數⇔為正定矩陣＂．
（c）若實數矩陣 $A$ 並非對稱矩陣，則取 $B=\frac{A+A^T}{2}$ 為對稱矩陣，可使對任何向量 $\boldsymbol{x}$ ， $\boldsymbol{x}^T A \boldsymbol{x}=\boldsymbol{x}^T B \boldsymbol{x}$ ，然後判斷 $B$ 的正定性即可．
（d）依定義，用配方法．