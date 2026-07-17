第 5 章 對角化理論
121

完全投影集（complete set of projections）
（1）考虑 $V$ 上的投影算子 $T_1, \ldots, T_k$ ，若滿足
（i）$T_i T_j=O, \forall i \neq j$ ，且（ii）$T_1+\ldots+T_k=I$ ，
则稱 $\left\{T_1, \ldots, T_k\right\}$ 为 $V$ 上的一组完全投影集。
（2）考慮 $F^{n \times n}$ 上的投影矩陣 $A_1, \ldots, A_k$ ，若滿足
（i）$A_i A_j=O, \forall i \neq j$ ，且（ii）$A_1+\ldots+A_k=I$ ，
则稱 $\left\{A_1, \ldots, A_k\right\}$ 为 $F^{n \times n}$ 上的一组完全投影集。
Note
例如：若 $T^2=T$ ，則 $\{T, I-T\}$ 即為 $V$ 上的一組完全投影集。
光譜分解（spectral decomposition）
設 $T \in L(V, V)$ ，且 $T$ 有相異特徵根 $\lambda_1, \ldots, \lambda_2$ ，
若 $T$ 可到角化，則
存在一完全投影集 $\left\{T_1, \ldots, T_k\right\}$ 使 $T=\lambda_1 T_1+\ldots+\lambda_k T_k$ 。
Note
（1）此稱為 $T$ 的光譜分解．
（2）影方陣 $A$ 亦有類似結論。
（3）做光譜分解的方法：
設矩陣 $A$ 可對角化且有相異特徵根：$\lambda_1, \ldots, \lambda_k$ ，設各重根數為 $m_i$ ，
令可逆矩陣 $P$ 使得 $P^{-1} A P=D=\left[\begin{array}{ccc}\lambda_1 I_{m_1} & & O \\ & \ddots & \\ O & & \lambda_k I_{m_k}\end{array}\right]$ ，
則 $A=P D P^{-1}=P\left(\lambda_1\left[\begin{array}{llll}I_{m_1} & & & O \\ & O & & \\ O & & & O\end{array}\right]+\cdots+\lambda_k\left[\begin{array}{llll}O & & & O \\ & \ddots & & \\ O & & & O \\ & & & I_{m_k}\end{array}\right]\right) P^{-1} =\lambda_1 P\left[\begin{array}{llll}I_{m_1} & & & O \\ & O & & \\ & & \ddots & \\ O & & & O\end{array}\right] P^{-1}+\cdots+\lambda_k P \underbrace{\left[\begin{array}{llll}O & & & O \\ & \ddots & & \\ & & O & \\ O & & & I_{m_k}\end{array}\right]}_{A_k} P^{-1}=\lambda_1 A_1+\cdots+\lambda_k A_k$