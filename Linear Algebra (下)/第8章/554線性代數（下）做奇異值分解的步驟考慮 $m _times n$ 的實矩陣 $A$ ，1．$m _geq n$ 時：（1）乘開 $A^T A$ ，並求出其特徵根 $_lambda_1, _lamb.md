554
線性代數（下）

做奇異值分解的步驟
考慮 $m \times n$ 的實矩陣 $A$ ，
1．$m \geq n$ 時：
（1）乘開 $A^T A$ ，並求出其特徵根 $\lambda_1, \lambda_2, \cdots$ ，與特徵向量 $v_1, v_2, \cdots$ ．
（2）令 $\sigma_i=\sqrt{\lambda_i}$ ，並由大到小依序放在 $(\Sigma)_{i i}$ ，其餘位置放 0 。
（3）對 $\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots\right\}$ 作單範正交化，組成 $V$ 的行向量：$V^{(1)}, \ldots, V^{(n)}$ 。
（4）取 $\boldsymbol{u}_i=\frac{1}{\sigma_i} A V^{(i)}$ ，即得 $\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \cdots\right\}$ 成 $U$ 的行向量．
（若不夠組成 $U$ ，則從 $N\left(A^T\right)$ 的單範正交基底中找）。
2．$m \leq n$ 時：
方法一：
令 $B=A^T$ ，執行上述步驟得 $B=U \Sigma V^T$ ，則 $A=\left(U \Sigma V^T\right)^T=V \Sigma^T U^T$ ．
方法二：
（1）乘出 $A A^T$ ，並求出其特徵根 $\lambda_1, \lambda_2, \cdots$ ，與特徵向量 $\boldsymbol{u}_1, \boldsymbol{u}_2, \cdots$ ．
（2）令 $\sigma_i=\sqrt{\lambda_i}$ ，並由大到小依序放在 $(\Sigma)_{i i}$ ，其餘位置放 0 。
（3）對 $\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \cdots\right\}$ 作單範正交化，組成 $U$ 的行向量 $U^{(1)}, \ldots, U^{(m)}$ 。
（4）取 $\boldsymbol{v}_i=\frac{1}{\sigma_i} A^{\mathrm{H}} U^{(i)}$ ，即得 $\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots\right\}$ 組成 $V$ 的行向量．
（若不夠組成 $V$ ，則從 $N(A)$ 的單範正交基底中找）