第 5 章 對角化理論

47



特徵空間（eigenspace）

設 $T \in L(V, V)$ ，純量 $\lambda$ 為 $T$ 的特徵根，則

稱 $V(\lambda)=\{\boldsymbol{v} \in V \mid T(\boldsymbol{v})=\lambda \boldsymbol{v}\}=\operatorname{ker}(T-\lambda I)$ 為 $\lambda$ 的特徵空間。

【99中正資工】

Note

（1）有些書上把 $V(\lambda)$ 記成 $E_\lambda ; V(\lambda)$ 為 $V$ 的子空間．

（2）$\lambda$ 所對應的特徵向量為 $V(\lambda)$ 中的非零向量．

（3）$V(\lambda)$ 為 $T$ 不變子空間．

【證明】

【99中正資工】

任取 $T(\boldsymbol{u}) \in T(V(\lambda))$ ，其中 $\boldsymbol{u} \in V(\lambda)$ ，即 $T(\boldsymbol{u})=\lambda \boldsymbol{u}$ ，

故 $T(T(\boldsymbol{u}))=T(\lambda \boldsymbol{u})=\lambda T(\boldsymbol{u})$ ，

$$

\begin{aligned}

& \therefore T(\boldsymbol{u}) \in V(\lambda), \\

& \therefore T(V(\lambda)) \subseteq V(\lambda),

\end{aligned}

$$



故 $V(\lambda)$ 為 $T$ 不變子空間．

（4）設 $T \in L(V, V)$ ，且 $\lambda_1, \lambda_2, \cdots, \lambda_k$ 為 $T$ 的相異特徵根，則

（a）$V\left(\lambda_1\right), V\left(\lambda_2\right), \cdots, V\left(\lambda_k\right)$ 為獨立子空間．

（b）任取對應 $\lambda_i$ 的特徵向量 $\boldsymbol{v}_i, 1 \leq i \leq k$ ，則 $\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots, \boldsymbol{v}_k$ 為線性獨立。



【重要】



【證明】（相異特徵根所對特徵向量獨立．）

induction on $k$ ，

$k=1$ 時， $\boldsymbol{v}_1$ 顯然為線性獨立，

設 $k=s-1$ 時，命題成立。

則 $k=s$ 時，

$$

\begin{equation*}

\text { 令 } \alpha_1 \boldsymbol{v}_1+\alpha_2 \boldsymbol{v}_2+\cdots+\alpha_s \boldsymbol{v}_s=\mathbf{0}, \ldots \ldots \tag{*}

\end{equation*}

$$



則 $\mathbf{0}=T(\mathbf{0})=T\left(\alpha_1 \boldsymbol{v}_1+\alpha_2 \boldsymbol{v}_2+\cdots+\alpha_s \boldsymbol{v}_s\right)$

$$

=\alpha_1 T\left(\boldsymbol{v}_1\right)+\alpha_2 T\left(\boldsymbol{v}_2\right)+\cdots+\alpha_s T\left(\boldsymbol{v}_s\right)=\alpha_1 \lambda_1 \boldsymbol{v}_1+\alpha_2 \lambda_2 \boldsymbol{v}_2+\cdots+\alpha_s \lambda_s \boldsymbol{v}_s \ldots\left({ }^{* *}\right)

$$

$(* *)-(*) \times \lambda_s$ ，可得 $\alpha_1\left(\lambda_1-\lambda_s\right) \boldsymbol{v}_1+\alpha_2\left(\lambda_2-\lambda_s\right) \boldsymbol{v}_2+\cdots+\alpha_{s-1}\left(\lambda_{s-1}-\lambda_s\right) \boldsymbol{v}_{s-1}=\mathbf{0}$ ，

而由歸納假設知， $\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots, \boldsymbol{v}_{s-1}$ 為線性獨立，

且因 $\lambda_i \neq \lambda_s, \forall i \neq s, \therefore \alpha_i=0, \forall i=1,2, \ldots, s-1$ ，

再將這些 $\alpha_i=0, \forall i=1,2, \ldots, s-1$ 代入（ $*$ ）得 $\alpha_s=0$ ，

即 $\alpha_i=0, \forall i=1,2, \ldots, s$ ，即 $\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots, \boldsymbol{v}_s$ 為線性獨立。