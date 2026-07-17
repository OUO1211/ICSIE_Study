第 6 章 Jordan form 及其應用

205



找可逆矩陣 $Q$ 使 $Q^{-1} A Q=J_A$

設 $A$ 有特徵多項式 $\operatorname{char}_A(\lambda)=(\alpha-\lambda)^5(\beta-\lambda)^4$ ，且點圖分別為：

$$

\lambda=\alpha: \quad \bullet \quad \bullet ; \lambda=\beta:

$$

－

（1）由 $\lambda=\alpha$ 的點圖的第一列找 3 個向量： $\boldsymbol{v}_1, \boldsymbol{v}_2, \boldsymbol{v}_3$ ，第二列找 2 個向量： $\boldsymbol{v}_4, \boldsymbol{v}_5$ ．

其中， $\boldsymbol{v}_1 \in \operatorname{ker}(A-\alpha I)^3-\operatorname{ker}(A-\alpha I)^2, \boldsymbol{v}_2=(A-\alpha I) \boldsymbol{v}_1, \boldsymbol{v}_3=(A-\alpha I) \boldsymbol{v}_2=(A-\alpha I)^2 \boldsymbol{v}_1$ ， $\boldsymbol{v}_4 \in \operatorname{ker}(A-\alpha I)^2-\operatorname{ker}(A-\alpha I)$ 且與 $\boldsymbol{v}_2$ 線性獨立， $\boldsymbol{v}_5=(A-\alpha I) \boldsymbol{v}_4$ ．

$$

\begin{array}{lll}

v_1 & v_2=(A-\alpha I) v_1 & v_3=(A-\alpha I)^2 v_1

\end{array}

$$



如圖：

$$

\boldsymbol{v}_4 \quad \boldsymbol{v}_5=(A-\alpha \boldsymbol{I}) \boldsymbol{v}_4

$$

（2）由 $\lambda=\beta$ 的點圖的第一列找 2 個向量： $\boldsymbol{u}_1, \boldsymbol{u}_2$ ，

第二列找 1 個向量： $\boldsymbol{u}_3$ ，第三列找 1 個向量 $\boldsymbol{u}_4$ ．

其中， $\boldsymbol{u}_1 \in \operatorname{ker}(A-\beta I)^2-\operatorname{ker}(A-\beta I), \boldsymbol{u}_2=(A-\beta I) \boldsymbol{u}_1$ ，

$\boldsymbol{u}_3 \in \operatorname{ker}(A-\beta I)$ ，且與 $\boldsymbol{u}_2$ 線性獨立，

$\boldsymbol{u}_4 \in \operatorname{ker}(A-\beta I)$ ，且與 $\boldsymbol{u}_2, \boldsymbol{u}_3$ 線性獨立。

$$

\boldsymbol{u}_1 \quad \boldsymbol{u}_2=(A-\beta I) \boldsymbol{u}_1

$$



如圖：

$$

\boldsymbol{u}_3

$$

$$

\boldsymbol{u}_4

$$

（3）則 $Q$ 為以 $\left[\boldsymbol{v}_1, \boldsymbol{v}_2, \boldsymbol{v}_3, \boldsymbol{v}_4, \boldsymbol{v}_5, \boldsymbol{u}_1, \boldsymbol{u}_2, \boldsymbol{u}_3, \boldsymbol{u}_4\right]$ 為行向量的矩陣，可使 $Q^{-1} A Q=J_A$ ．

（4）若取 $Q=\left[\boldsymbol{v}_3, \boldsymbol{v}_2, \boldsymbol{v}_1, \boldsymbol{v}_5, \boldsymbol{v}_4, \boldsymbol{u}_2, \boldsymbol{u}_1, \boldsymbol{u}_3, \boldsymbol{u}_4\right]$ 為行向量的矩陣，則 $Q^{-1} A Q$ 所得為上移型的 Jordan form．