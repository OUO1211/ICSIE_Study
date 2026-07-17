第 8 章 內積算子及其魔用
531

矩陣長度的性質
設 $A=\left[a_{i j}\right] \in F^{m \times n}$ ，則
（1）$\|A\|_1=\max _{1 \leq j \leq n} \sum_{i=1}^m\left|a_{i j}\right|$ 。（即各行元素的絕對值的和的最大值）
（2）$\|A\|_2=\sqrt{\lambda_{\text {max }}\left(A^H A\right)}$ ．
（3）$\|A\|_{\infty}=\max _{1 \leq i \leq n} \sum_{j=1}^n\left|a_{i j}\right|$ 。（即各列元素的絕對值的和的最大值）
【證明】
（1）令第 $k$ 個行的和（設為 $\alpha$ ）為所有行和中最大的，即 $\alpha=\max _{1 \leq j \leq n} \sum_{i=1}^m\left|a_{i j}\right|=\sum_{i=1}^m\left|a_{i k}\right|$ ，
$$
\begin{aligned}
& \text { 則 } \forall \boldsymbol{x}=\left[\begin{array}{c}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{array}\right],\|A \boldsymbol{x}\|_1=\left\|\left[\begin{array}{c}
\sum_{j=1}^n a_{1 j} x_j \\
\sum_{j=1}^n a_{2 j} x_j \\
\vdots \\
\sum_{j=1}^n a_{m j} x_j
\end{array}\right]\right\|_1=\sum_{i=1}^m\left(\left|\sum_{j=1}^n a_{i j} x_j\right|\right) \leq \sum_{i=1}^m \sum_{j=1}^n\left|a_{i j} x_j\right|=\sum_{j=1}^n\left|x_j\right| \sum_{i=1}^m\left|a_{i j}\right| \\
& \leq \alpha \sum_{j=1}^n\left|x_j\right|=\alpha\|\boldsymbol{x}\|_1, \text { 故得 } \frac{\|A \boldsymbol{x}\|_1}{\|\boldsymbol{x}\|_1} \leq \alpha, \\
& \therefore \forall \boldsymbol{x} \in F^{n \times 1}-\{\mathbf{0}\},\|A\|_1=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_1}{\|\boldsymbol{x}\|_1}\right\} \leq \alpha,
\end{aligned}
$$

而取 $\boldsymbol{x}=\boldsymbol{e}_k$ 則可使等號成立，$\therefore\|A\|_1=\alpha=\max _{1 \leq j \leq n} \sum_{i=1}^m\left|a_{i j}\right|$ 。
（2）$\|A\|_2^2=\left(\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_2}{\|\boldsymbol{x}\|_2}\right\}\right)^2=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_2^2}{\|\boldsymbol{x}\|_2^2}\right\}$ ，
又 $\frac{\|A \boldsymbol{x}\|_2^2}{\|\boldsymbol{x}\|_2^2}=\frac{\langle A \boldsymbol{x}, A \boldsymbol{x}\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}=\frac{\left\langle A^H A \boldsymbol{x}, \boldsymbol{x}\right\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}=\rho(\boldsymbol{x})$（ $A^H A$ 的 Rayleight 商式）
$$
\leq \lambda_{\max }\left(A^H A\right),\left(\because A^H A \text { 為 Hermitian }\right)
$$

又取 $\boldsymbol{x}$ 為 $\lambda_{\text {max }}\left(A^H A\right)$ 所對的特徵向量可使等號成立，
$$
\therefore\|A\|_2^2=\max _{x \neq 0} \rho(\boldsymbol{x})=\lambda_{\max }\left(A^H A\right), \therefore\|A\|_2=\sqrt{\lambda_{\max }\left(A^H A\right)} .
$$