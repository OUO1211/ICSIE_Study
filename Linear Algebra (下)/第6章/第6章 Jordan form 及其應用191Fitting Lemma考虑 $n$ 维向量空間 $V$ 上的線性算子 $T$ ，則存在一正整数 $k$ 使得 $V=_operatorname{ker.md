第6章 Jordan form 及其應用

191



Fitting Lemma

考虑 $n$ 维向量空間 $V$ 上的線性算子 $T$ ，則存在一正整数 $k$ 使得 $V=\operatorname{ker}\left(T^k\right) \oplus \operatorname{Im}\left(T^k\right)$ ．

【95．103 台大数學、95 高師数學】

【證明】

由核集鏈定理知存在正整數 $k$ 使得 $\operatorname{ker}\left(T^k\right)=\operatorname{ker}\left(T^{k+1}\right)=\cdots=\operatorname{ker}\left(T^{2 k}\right)$ ，

任取 $\boldsymbol{v} \in \operatorname{ker}\left(T^k\right) \cap \operatorname{Im}\left(T^k\right)$ ，

即 $T^k(\boldsymbol{v})=\mathbf{0}$ ，且 $\boldsymbol{v}=T^k(\boldsymbol{u})$ ，for some $\boldsymbol{u}$ ，

$$

\begin{aligned}

& \therefore \mathbf{0}=T^k(\boldsymbol{v})=T^k\left(T^k(\boldsymbol{u})\right)=T^{2 k}(\boldsymbol{u}), \\

& \therefore \boldsymbol{u} \in \operatorname{ker}\left(T^{2 k}\right),

\end{aligned}

$$



又因為 $\operatorname{ker}\left(T^k\right)=\operatorname{ker}\left(T^{2 k}\right), \therefore T^k(\boldsymbol{u})=\mathbf{0}, \therefore \boldsymbol{v}=\mathbf{0}$ ，

得 $\operatorname{ker}\left(T^k\right) \cap \operatorname{Im}\left(T^k\right)=\{\mathbf{0}\}$ ，

再由 Sylvester 第二定理可得 $V=\operatorname{ker}\left(T^k\right) \oplus \operatorname{Im}\left(T^k\right)$ ．