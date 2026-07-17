192
線性代數（下）

循環子空間（cyclic subspace）
考虑向量空間 $V$ 上的線性算子 $T, \boldsymbol{v}$ 為 $V$ 上任一向量， $W=\operatorname{span}\left\{\boldsymbol{v}, T(\boldsymbol{v}), T^2(\boldsymbol{v}), \ldots, T^k(\boldsymbol{v}), \ldots\right\}$ 稱為由 $\boldsymbol{v}$ 生成的 $T$－循環子空間，記作 $C_{\boldsymbol{v}}(T)$ 。

Note
（1）$C_v(T)$ 為 $V$ 的 $T$ 不變子空間．
（2）考慮向量空間 $V$ 上指標 $k$ 的幂零算子 $T$ ，則存在 $V$ 中的非零向量 $v$ 使得 $\left\{\boldsymbol{v}, T(\boldsymbol{v}), T^2(\boldsymbol{v}), \ldots, T^{k-1}(\boldsymbol{v})\right\}$ 為線性獨立集合。
（3）考慮向量空間 $V$ 上的線性算子 $T$ ，若非零向量 $v \in \operatorname{ker}\left(T^k\right)-\operatorname{ker}\left(T^{k-1}\right)$ ，則 $\beta=\left\{\boldsymbol{v}, T(\boldsymbol{v}), T^2(\boldsymbol{v}), \ldots, T^{k-1}(\boldsymbol{v})\right\}$ 為 $W=C_{\boldsymbol{v}}(T)$ 的一組基底（稱循環基底），且
$$
\left[T_W\right]_\beta=\left[\begin{array}{cccc}
0 & & & O \\
1 & 0 & & \\
& \ddots & \ddots & \\
O & & 1 & 0
\end{array}\right] .
$$
（4）考慮向量空間 $V$ 上的線性算子 $T, \boldsymbol{v}$ 為非零向量，$W=C_{\boldsymbol{v}}(T)$ 為由 $\boldsymbol{v}$ 生成的 $T$－循環子空間，若 $\operatorname{dim}(W)=k$ ，則 $\beta=\left\{\boldsymbol{v}, T(\boldsymbol{v}), T^2(\boldsymbol{v}), \ldots, T^{k-1}(\boldsymbol{v})\right\}$ 為 $W$ 的一組基底。【108政大應數】
（5）設 $T^k(\boldsymbol{v})=-a_0 \boldsymbol{v}-a_1 T(\boldsymbol{v})-a_2 T^2(\boldsymbol{v})-\ldots-a_{k-1} T^{k-1}(\boldsymbol{v})$ ，則 $\left[T_W\right]_\beta=\left[\begin{array}{ccccc}0 & 0 & \cdots & 0 & -a_0 \\ 1 & 0 & \cdots & 0 & -a_1 \\ 0 & 1 & \cdots & 0 & -a_2 \\ \vdots & \vdots & \ddots & \vdots & \vdots \\ 0 & 0 & \cdots & 1 & -a_{k-1}\end{array}\right]$稱具有特徵式 $(-1)^k\left(a_0+a_1 x+\ldots+a_{k-1} x^{k-1}+x^k\right)$ 的友矩陣（companion matrix）．

【107台大資工】

（6）任給多項式 $p(x)=x^n+a_1 x^{n-1}+\ldots+a_{n-1} x+a_n$ ，則存在矩陣 $A$ ，使得 $p(x)$ 為 $A$ 的極小多項式．

【90台大數學】

（7）設 $v \in V$ ，則 $C_v(T)$ 維度為 1 若且唯若 $v$ 為 $T$ 的特徵向量．
（8）循環分解定理（Cyclic Decomposition Theorem）：
考慮向量空間 $V$ 上的冪零算子 $T$ ，且 $\operatorname{index}(T)=k$ ，則唯一存在 $\boldsymbol{v}_1, \boldsymbol{v}_2, \cdots, \boldsymbol{v}_r \in V$ 使得 $V=C_{\boldsymbol{v}_1}(T) \oplus C_{\boldsymbol{v}_2}(T) \oplus \cdots \oplus C_{\boldsymbol{v}_r}(T), \quad r=\operatorname{dim}(\operatorname{ker}(T))$ ．
其中，$k=\operatorname{dim}\left(C_{v_1}(T)\right)=n_1 \geq \cdots \geq \operatorname{dim}\left(C_{v_r}(T)\right)=n_r, v_i \in \operatorname{ker}\left(T^{n_i}\right)-\operatorname{ker}\left(T^{n_i-1}\right)$ ．