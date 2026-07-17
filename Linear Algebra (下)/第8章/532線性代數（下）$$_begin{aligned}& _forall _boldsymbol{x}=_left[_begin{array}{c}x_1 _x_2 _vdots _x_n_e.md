532
線性代數（下）
$$
\begin{aligned}
& \forall \boldsymbol{x}=\left[\begin{array}{c}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{array}\right],\|A \boldsymbol{x}\|_{\infty}=\left\|\left[\begin{array}{c}
\sum_{j=1}^n a_{1 j} x_j \\
\sum_{j=1}^n a_{2 j} x_j \\
\vdots \\
\sum_{j=1}^n a_{m j} x_j
\end{array}\right]\right\|_{\infty}=\max _{1 \leq i \leq m}\left\{\left|\sum_{j=1}^n a_{i j} x_j\right|\right\} \leq \max _i\left\{\sum_{j=1}^n\left|a_{i j} \| x_j\right|\right\} \\
& \leq\left(\max _i\left\{\sum_{j=1}^n\left|a_{i j}\right|\right\}\right)\left(\max _j\left\{\left|x_j\right|\right\}\right)=M\|\boldsymbol{x}\|_{\infty},\left(\text { 令 } M=\max _i\left\{\sum_{j=1}^n \mid a_{i j}\right\}\right) \\
& \therefore \forall \boldsymbol{x} \neq \mathbf{0}, \frac{\|A \boldsymbol{x}\|_{\infty}}{\|\boldsymbol{x}\|_{\infty}} \leq M, \therefore\|A \boldsymbol{x}\|_{\infty}=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_{\infty}}{\|\boldsymbol{x}\|_{\infty}}\right\} \leq M,
\end{aligned}
$$

欲使等號成立，
設 $k \in\{1,2, \ldots, m\}$ 使 $\sum_{j=1}^n\left|a_{k j}\right|=\max _i\left\{\sum_{j=1}^n\left|a_{i j}\right|\right\}=M$ ，
取 $\boldsymbol{x}=\left[\begin{array}{c}x_1 \\ x_2 \\ \vdots \\ x_n\end{array}\right] \in F^{n \times 1}$ ，其中 $x_j=\left\{\begin{array}{cc}1 & \text { if } a_{k j} \geq 0 \\ -1 & \text { if } a_{k j}<0\end{array}, \forall 1 \leq j \leq n\right.$ ，則 $\boldsymbol{x} \neq \mathbf{0}$ ，且 $\|\boldsymbol{x}\|_{\infty}=1$ ，
且 $\left|(A \boldsymbol{x})_{(k)}\right|=\left|\sum_{j=1}^n a_{k j} x_j\right|=\left|\sum_{j=1}^n\right| a_{k j}| |=\sum_{j=1}^n\left|a_{k j}\right|=M, \therefore\|A \boldsymbol{x}\|_{\infty}=M$ ．
例如：考慮 $A=\left[\begin{array}{ll}4 & 0 \\ 1 & 3\end{array}\right]$ ，則
∵ 第一行的元素的絕對值的和為 $|4|+|1|=5$ ，
∵ 第二行的元素的絕對值的和為 $|0|+|3|=3, \therefore\|A\|_1=5$ ．
∵ 第一列的元素的絕對值的和為 $|4|+|0|=4$ ，
∵ 第二列的元素的絕對值的和為 $|1|+|3|=4, \therefore\|A\|_{\infty}=4$ ．
$\because A^T A=\left[\begin{array}{cc}17 & 3 \\ 3 & 9\end{array}\right]$ ，得特徵根 $18,8, \therefore\|A\|_2=\sqrt{\lambda_{\text {max }}\left(A^T A\right)}=\sqrt{18}$ ．

Note
（1）注意證明過程中 $\boldsymbol{x}$ 的取法．
（2）設 $A \in R^{n \times n}$ ，則（a）
（a）$\left\|A^T\right\|_2=\|A\|_2$ ．
（b）$\left\|A^T A\right\|_2=\|A\|_2^2$ ．