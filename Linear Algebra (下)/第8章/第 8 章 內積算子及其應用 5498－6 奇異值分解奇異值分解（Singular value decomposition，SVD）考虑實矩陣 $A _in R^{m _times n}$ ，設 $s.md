第 8 章 內積算子及其應用 549

8－6 奇異值分解

奇異值分解（Singular value decomposition，SVD）
考虑實矩陣 $A \in R^{m \times n}$ ，設 $s=\min \{m, n\}$ ，若存在正交矩陣 $U \in R^{m \times m}$ ，正交矩陣 $V \in R^{n \times n}, ~ \sum \in R^{m \times n}$ ，使得 $A=U \sum V^T$ ，其中，$\Sigma$ 的元素滿足 $(\Sigma)_{i j}=\left\{\begin{array}{l}0, \forall i \neq j \\ \sigma_i, i=j\end{array}\right.$ 且 $\sigma_1 \geq \sigma_2 \geq \cdots \geq \sigma_s$ ，
則稱此為 $A$ 的一種奇異值分解，並稱 $\sigma_i$ 為 $A$ 的奇異值．
Note
（1）實矩陣的奇異值分解：
考慮複矩陣 $A \in C^{m \times n}$ ，設 $s=\min \{m, n\}$ ，
若存在么正矩陣 $U \in C^{m \times m}$ ，么正矩陣 $V \in C^{n \times n}, ~ \Sigma \in C^{m \times n}$ ，使得 $A=U \Sigma V^H$ ，
其中，$\Sigma$ 的元素滿足 $(\Sigma)_{i j}=\left\{\begin{array}{l}0, \forall i \neq j \\ \sigma_i, i=j\end{array}\right.$ 且 $\sigma_1 \geq \sigma_2 \geq \cdots \geq \sigma_s$,
則稱此為 $A$ 的一種奇異值分解，並稱 $\sigma_i$ 為 $A$ 的奇異值．
（2）任意矩陣的奇異值分解均存在．
（3）設 $A=U \sum V^H$ 為 $A$ 的奇異值分解，$\lambda_1, \lambda_2, \ldots, \lambda_n$ 為 $A^H A$ 的特徵根，則
（a）$A^H A$ 必為正半定，故 $\lambda_i$ 均為非負實數，而 $A$ 的奇異值 $\sigma_i=\sqrt{\lambda_i} \in R, \forall i$ ．
（b）$A^H A=\left(U \Sigma V^H\right)^H\left(U \Sigma V^H\right)=V \Sigma^H \Sigma V^H, \therefore\left(A^H A\right) V=V\left(\Sigma^H \Sigma\right)$ ，
$V$ 的行向量 $v_1, v_2, \ldots, v_n$ 為 $A^H A$ 的特徵向量（稱 $A$ 的右奇異向量），且形成單範正交集．
（c）$A A^H=\left(U \Sigma V^H\right)\left(U \Sigma V^H\right)^H=U \Sigma \Sigma^H U^H, \therefore\left(A A^H\right) U=U\left(\Sigma \Sigma^H\right)$ ，
$U$ 的行向量 $\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_m$ 為 $A A^H$ 的特徵向量（稱 $A$ 的左奇異向量），且形成單範正交集．
（d）若 $\operatorname{rank}(A)=r$ ，則 $\operatorname{rank}\left(A^H A\right)=r$ ，得 $A^H A$ 有 $r$ 個非零特徵根，設為 $\lambda_1, \ldots, \lambda_r$ ，
則由 $A=U \Sigma V^H, \therefore A V=U \Sigma$ ，得 $A \boldsymbol{v}_i=\left\{\begin{array}{l}\sigma_i \boldsymbol{u}_i, \text { for } 1 \leq i \leq r \\ \mathbf{0}, \text { for } r+1 \leq i \leq n\end{array}\right.$ ，
又由 $A^H=V \Sigma^H U^H, \therefore A^H U=V \Sigma^H$ 得 $A^H \boldsymbol{u}_i=\left\{\begin{array}{l}\sigma_i \boldsymbol{v}_i, \text { for } 1 \leq i \leq r \\ \mathbf{0}, \text { for } r+1 \leq i \leq m\end{array}\right.$ ；且
（i） $\boldsymbol{v}_1, \ldots, \boldsymbol{v}_r$ 形成 $R\left(A^H\right)$ 的單範正交基底， $\boldsymbol{v}_{r+1}, \ldots, \boldsymbol{v}_n$ 形成 $N(A)$ 的單範正交基底．
（ii） $\boldsymbol{u}_1, \ldots, \boldsymbol{u}_r$ 形成 $R(A)$ 的單範正交基底， $\boldsymbol{u}_{r+1}, \ldots, \boldsymbol{u}_m$ 形成 $N\left(A^H\right)$ 的單範正交基底。