522
線性代數（下）

Rayleigh 法則（Rayleigh principle）
考虑 Hermitian 矩陣 $A \in C^{n \times n}$ ，且 $\lambda_1 \leq \lambda_2 \leq \ldots \leq \lambda_n$ 為 $A$ 的特徵根，則
（1）$\lambda_1 \leq \rho(\boldsymbol{x}) \leq \lambda_n$ ．
（2） $\max _{x \neq 0} \rho(\boldsymbol{x})=\lambda_n$ ．
（3） $\min _{x \neq 0} \rho(\boldsymbol{x})=\lambda_1$ ．

【證明】
【 80.87 .95 中央統計、 80.96 清大統計、 88 成大統計、 81.93 清大應數、 96 中央數學、 99 高雄統計、100政大應數、100中山通訊】
（1）因 $A$ 為 Hermitian 故 $A$ 可么正對角化，
即存一么正矩陣 $P$ 使 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \lambda_2, \ldots, \lambda_n\right)$ ，即 $A=P D P^H$ ，
$$
\begin{aligned}
\therefore Q(\boldsymbol{x}) & =\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H P D P^H \boldsymbol{x}=\left(P^H \boldsymbol{x}\right)^H D\left(P^H \boldsymbol{x}\right)=\boldsymbol{y}^H D \boldsymbol{y} \\
& =\lambda_1\left|y_1\right|^2+\lambda_2\left|y_2\right|^2+\ldots+\lambda_n\left|y_n\right|^2,\left(\text { 取 } \boldsymbol{y}=\left[\begin{array}{llll}
y_1 & y_2 & \cdots & y_n
\end{array}\right]^T=P^H \boldsymbol{x}\right)
\end{aligned}
$$

則 $\boldsymbol{x}^H \boldsymbol{x}=(P \boldsymbol{y})^H(P \boldsymbol{y})=\boldsymbol{y}^H P^H P \boldsymbol{y}=\boldsymbol{y}^H \boldsymbol{y}=\sum_{i=1}^n\left|y_i\right|^2$ ，
$$
\begin{aligned}
& \therefore \rho(\boldsymbol{x})=\frac{Q(\boldsymbol{x})}{\boldsymbol{x}^H \boldsymbol{x}}=\frac{\sum_{i=1}^n \lambda_i\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2}, \\
& \text { 又 } \because \lambda_1=\frac{\lambda_1 \sum_{i=1}^n\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2}=\frac{\sum_{i=1}^n \lambda_1\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2} \leq \frac{\sum_{i=1}^n \lambda_i\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2} \leq \frac{\sum_{i=1}^n \lambda_n\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2}=\lambda_n \frac{\sum_{i=1}^n\left|y_i\right|^2}{\sum_{i=1}^n\left|y_i\right|^2}=\lambda_n, \\
& \therefore \lambda_1 \leq \rho(\boldsymbol{x}) \leq \lambda_n, \forall \boldsymbol{x} \neq \mathbf{0} .
\end{aligned}
$$
（2）取 $\boldsymbol{x}_n$ 為 $A$ 相對於 $\lambda_n$ 的特徵向量，則由前一頁討論可得 $\rho\left(\boldsymbol{x}_n\right)=\lambda_n$ ，即 $\max _{x \neq 0} \rho(\boldsymbol{x})=\lambda_n$ ．
（3）取 $\boldsymbol{x}_1$ 為 $A$ 相對於 $\lambda_1$ 的特徵向量，則由前一頁討論可得 $\rho\left(\boldsymbol{x}_1\right)=\lambda_1$ ，即 $\min _{x \neq 0} \rho(\boldsymbol{x})=\lambda_1$ ．

Note
（1）$A$ 為實對稱矩陣時，上述結果亦成立。
【87．90 政大應數、87 中央統計、88．92 成大統計】
（2）由證明的過程可得： $\boldsymbol{x}$ 取 $\lambda_1\left(\lambda_n\right)$ 所對的特徵向量可使 $\rho(\boldsymbol{x})$ 為最小（大）值．

【88 成大統計】