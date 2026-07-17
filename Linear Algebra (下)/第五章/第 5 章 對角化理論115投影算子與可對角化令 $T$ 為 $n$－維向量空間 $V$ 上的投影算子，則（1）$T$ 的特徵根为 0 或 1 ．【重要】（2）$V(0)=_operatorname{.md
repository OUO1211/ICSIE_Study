第 5 章 對角化理論
115

投影算子與可對角化
令 $T$ 為 $n$－維向量空間 $V$ 上的投影算子，則
（1）$T$ 的特徵根为 0 或 1 ．

【重要】

（2）$V(0)=\operatorname{ker}(T), \quad V(1)=\operatorname{Im}(T)$ ．

【106 交大應数】

（3）$T$ 必可對角化．

【重要】

（4）存在 $V$ 的一组基底 $\beta$ 使得 $[T]_\beta=\left[\begin{array}{cc}I_r & O \\ O & O_{n-r}\end{array}\right]$ ，其中 $r=\operatorname{rank}(T)=\operatorname{tr}(T)$ ．
【97交大應数】
【證明】
【92中正統計、107中央統計、 88.108 成大統計】
（1）設 $\lambda$ 為 $T$ 的特徵根，
即存在非零向量 $\boldsymbol{v}$ ，使 $T(\boldsymbol{v})=\lambda \boldsymbol{v}$ ，
則 $\lambda \boldsymbol{v}=T(\boldsymbol{v})=T^2(\boldsymbol{v})=T(T(\boldsymbol{v}))=T(\lambda \boldsymbol{v})=\lambda T(\boldsymbol{v})=\lambda^2 \boldsymbol{v}$ ，
即 $\left(\lambda^2-\lambda\right) \boldsymbol{v}=\mathbf{0}$ ，得 $\lambda^2-\lambda=0$ ，
得 $\lambda=1$ 或 0 ．
（2）$V(0)=\{\boldsymbol{v} \in V \mid T(\boldsymbol{v})=0 \boldsymbol{v}\}=\operatorname{ker}(T)$ ．
$$
\begin{aligned}
& V(1)=\{\boldsymbol{v} \in V \mid T(\boldsymbol{v})=1 \boldsymbol{v}\}=\{\boldsymbol{v} \in V \mid \boldsymbol{v}=T(\boldsymbol{v})\} . \\
& \because T \in L(V, V), \therefore V(1) \subseteq \operatorname{Im}(T),
\end{aligned}
$$

又，取 $\boldsymbol{v} \in \operatorname{Im}(T)$ ，則存在 $\boldsymbol{u} \in V$ ，使得 $\boldsymbol{v}=T(\boldsymbol{u})$ ，
因 $T$ 為投影算子，故 $\boldsymbol{v}=T(\boldsymbol{u})=T^2(\boldsymbol{u})=T(T(\boldsymbol{u}))=T(\boldsymbol{v})$ ，所以 $\boldsymbol{v} \in V(1)$ ，
所以 $\operatorname{Im}(T) \subseteq V(1)$ ，得 $V(1)=\operatorname{Im}(T)$ ．
（3）$\because T$ 為為投影算子，由第四章中的討論得 $V=\operatorname{Im}(T) \oplus \operatorname{ker}(T)$ ，
再由（2）得：$V=V(0) \oplus V(1)$ ，且因 $T$ 之特徵根為 0 或 1 ，
故 $T$ 可對角化．
（4）令 $\beta_1, \beta_2$ 分別為 $V(0), V(1)$ 的基底，取 $\beta=\beta_1 \cup \beta_2$ 為 $V$ 的基底，且 $[T]_\beta=\left[\begin{array}{cc}I_r & O \\ O & O_{n-r}\end{array}\right]$ ，其中，$r=\operatorname{dim}(V(1))=\operatorname{dim}(\operatorname{Im}(T))=\operatorname{rank}(T)$ ，另一方面 $\operatorname{tr}(T)=\operatorname{tr}\left([T]_\beta\right)=r$ ，故得 $\operatorname{rank}(T)=\operatorname{tr}(T)$ ．