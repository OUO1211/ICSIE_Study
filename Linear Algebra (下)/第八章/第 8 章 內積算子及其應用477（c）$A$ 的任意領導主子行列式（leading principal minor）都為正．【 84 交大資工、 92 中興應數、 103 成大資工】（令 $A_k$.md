第 8 章 內積算子及其應用
477

（c）$A$ 的任意領導主子行列式（leading principal minor）都為正．
【 84 交大資工、 92 中興應數、 103 成大資工】
（令 $A_k$ 為取 $A$ 的第1到第 $k$ 行，第1到第 $k$ 列所成矩陣，則 $\operatorname{det}\left(A_k\right)=\Delta_k(A)$ 稱為 $A$ 的領導主子行列式 $k=1,2, \ldots, n$ ．）
【證明】
（a）⇒（b）：前頁有證．
（b）$\Rightarrow(\mathrm{a})$ ：
因 $A$ 為對稱矩陣，故可正交對角化，存在正交矩陣 $P$ 使 $P^T A P=D=\operatorname{diag}\left(\lambda_1, \ldots, \lambda_n\right)$ ，其中，$\lambda_1, \ldots, \lambda_n$ 為 $A$ 的特徵根，都是正數，亦即 $A=P D P^T$ ，
$$
\forall \boldsymbol{x}=\left[\begin{array}{c}
x_1 \\
\vdots \\
x_n
\end{array}\right] \neq 0, \boldsymbol{x}^T D \boldsymbol{x}=\left[x_1 \cdots x_n\right]\left[\begin{array}{ccc}
\lambda_1 & & O \\
& \ddots & \\
O & & \lambda_n
\end{array}\right]\left[\begin{array}{c}
x_1 \\
\vdots \\
x_n
\end{array}\right]=\lambda_1 x_1^2+\cdots+\lambda_n x_n^2>0,
$$

即 $D$ 為正定矩陣，但 $A$ 與 $D$ 正交相似，故 $A$ 亦為正定矩陣，得證。
（a）⇒（c）：
對 $k=1,2, \ldots, n-1$ ，取 $\boldsymbol{y}=\left[\begin{array}{c}y_1 \\ \vdots \\ y_k\end{array}\right] \in R^{k \times 1}-\{\mathbf{0}\}$ ，並令 $\boldsymbol{x}=\left[\begin{array}{c}y_1 \\ \vdots \\ y_k \\ \hline 0 \\ \vdots \\ 0\end{array}\right]$ ，
則因為 $A$ 為正定矩陣，故 $\boldsymbol{x}^T A \boldsymbol{x}>0$ ，又 $\boldsymbol{x}^T A \boldsymbol{x}=\boldsymbol{y}^T A_k \boldsymbol{y}$ ，其中，$A_k$ 為取 $A$ 的第 1 到第 $k$ 行，第 1 到第 $k$ 列所成矩陣，故 $A_k$ 亦為正定，故 $\Delta_k(A)=\operatorname{det}\left(A_k\right)>0$ ．
對 $k=n$ 時，$\Delta_n(A)=\operatorname{det}\left(A_n\right)=\operatorname{det}(A)>0$ ，前面已證。
（c）⇒（a）
因為 $\Delta_k(A)>0, \forall k=1 \sim n$ ，且 $A$ 為對稱矩陣，故 $A$ 可做 $L D L^T$ 分解，
$$
\text { 令 } A=\left[\begin{array}{cc}
A_k & B \\
C & E
\end{array}\right], L=\left[\begin{array}{cc}
L_k & O \\
F & G
\end{array}\right], D=\left[\begin{array}{cc}
D_k & O \\
O & H
\end{array}\right] \text {, }
$$

其中，$L$ 為對角元素都是 1 的下三角矩陣，$D$ 為對角矩陣，$A_k, L_k, D_k$ 均為 $k \times k$ ，
則 $\left[\begin{array}{cc}A_k & B \\ C & E\end{array}\right]=\left[\begin{array}{cc}L_k & O \\ F & G\end{array}\right]\left[\begin{array}{cc}D_k & O \\ O & H\end{array}\right]\left[\begin{array}{cc}L_k^T & F^T \\ O & G^T\end{array}\right]=\left[\begin{array}{cc}L_k D_k L_k^T & L_k D_k F^T \\ F D_k L_k^T & F D_k F^T+G H G^T\end{array}\right]$ ，
故 $\Delta_k(A)=\operatorname{det}\left(A_k\right)=\operatorname{det}\left(L_k D_k L_k^T\right)=\operatorname{det}\left(D_k\right)$ ，
但 $\Delta_k(A)>0, \forall k=1 \sim n$ ，故 $D$ 的對角元素 $d_1, \ldots, d_n$ 都為正數，