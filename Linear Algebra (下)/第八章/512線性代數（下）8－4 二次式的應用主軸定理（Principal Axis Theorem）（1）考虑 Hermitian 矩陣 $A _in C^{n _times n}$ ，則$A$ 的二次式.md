512
線性代數（下）

8－4 二次式的應用

主軸定理（Principal Axis Theorem）
（1）考虑 Hermitian 矩陣 $A \in C^{n \times n}$ ，則
$A$ 的二次式 $Q(x)=x^H A x$
可以表達成 $\lambda_1\left|y_1\right|^2+\lambda_2\left|y_2\right|^2+\ldots+\lambda_n\left|y_n\right|^2=\left[y_1 \cdots y_n\right]\left[\begin{array}{lll}\lambda_1 & & O \\ & \ddots & \\ O & & \lambda_n\end{array}\right]\left[\begin{array}{c}y_1 \\ \vdots \\ y_n\end{array}\right]$ ，
其中，$\lambda_1, \lambda_2, \ldots, \lambda_n$ 為 $A$ 的特徵根， $\boldsymbol{x} \in C^{n \times 1}, y_1, y_2, \ldots, y_n \in C$ 。
（2）考慮對稱矩陣 $A \in R^{n \times n}$ ，則
$A$ 的二次式 $Q(\boldsymbol{x})=\boldsymbol{x}^T A \boldsymbol{x}$
可以表達成 $\lambda_1 y_1{ }^2+\lambda_2 y_2{ }^2+\ldots+\lambda_n y_n{ }^2=\left[y_1 \cdots y_n\right]\left[\begin{array}{lll}\lambda_1 & & O \\ & \ddots & \\ O & & \lambda_n\end{array}\right]\left[\begin{array}{c}y_1 \\ \vdots \\ y_n\end{array}\right]$ ，
其中，$\lambda_1, \lambda_2, \ldots, \lambda_n$ 為 $A$ 的特徵根，$x \in R^{n \times 1}, y_1, y_2, \ldots, y_n \in R$ 。
【證明】

【97中興統計】

（1）因為 $A$ 為 Hermitian，故 $A$ 為正規矩陣，故 $A$ 可么正對角化，
即存在么正矩陣 $P \in C^{n \times n}$ ，使得 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \lambda_2, \ldots, \lambda_n\right)$ ，即 $A=P D P^H$ ，
$$
\begin{aligned}
& \therefore Q(\boldsymbol{x})=\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H P D P^H \boldsymbol{x}=\left(P^H \boldsymbol{x}\right)^H D\left(P^H \boldsymbol{x}\right) \\
& =\boldsymbol{y}^H D \boldsymbol{y}=\lambda_1\left|y_1\right|^2+\lambda_2\left|y_2\right|^2+\ldots+\lambda_n\left|y_n\right|^2, \\
& \text { (取 } \left.\boldsymbol{y}=\left[\begin{array}{llll}
y_1 & y_2 & \cdots & y_n
\end{array}\right]^T=P^H \boldsymbol{x}\right)
\end{aligned}
$$
（2）因 $A$ 為對稱矩陣，故 $A$ 可正交對角化，
其餘與上述證明過程類似。