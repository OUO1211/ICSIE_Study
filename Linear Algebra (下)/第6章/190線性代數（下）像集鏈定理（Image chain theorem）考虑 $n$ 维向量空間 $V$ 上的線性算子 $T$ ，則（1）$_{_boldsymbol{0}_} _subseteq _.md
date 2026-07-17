190
線性代數（下）

像集鏈定理（Image chain theorem）
考虑 $n$ 维向量空間 $V$ 上的線性算子 $T$ ，則
（1）$\{\boldsymbol{0}\} \subseteq \cdots \subseteq \operatorname{Im}\left(T^{i+1}\right) \subseteq \operatorname{Im}\left(T^i\right) \subseteq \cdots \subseteq \operatorname{Im}\left(T^2\right) \subseteq \operatorname{Im}\left(T^1\right) \subseteq V$ ．
（2）存在最小正整数 $k$ ，使得 $\operatorname{Im}\left(T^k\right)=\operatorname{Im}\left(T^{k+1}\right)=\operatorname{Im}\left(T^{k+2}\right)=\cdots$ ．
（3）$\bigcap_{i=1}^{\infty} \operatorname{Im}\left(T^i\right)=\operatorname{Im}\left(T^k\right)$ ，其中 $k$ 為（2）所得。
（4）$W=\bigcap_{i=1}^{\infty} \operatorname{Im}\left(T^i\right)$ 為 $T$ 的最大可逆區．
【證明】
（1）明顯可得．
（2）由（1）可得 $0 \leq \cdots \leq \operatorname{dim}\left(\operatorname{Im}\left(T^2\right)\right) \leq \operatorname{dim}(\operatorname{Im}(T)) \leq \operatorname{dim}(V)=n$ ，故 $\operatorname{dim}(\operatorname{Im}(T)), \operatorname{dim}\left(\operatorname{Im}\left(T^2\right)\right), \operatorname{dim}\left(\operatorname{Im}\left(T^3\right)\right), \ldots$ ，這無限多個數字中，必存在 $k \in Z^{+}$使得 $\operatorname{dim}\left(\operatorname{Im}\left(T^k\right)\right)=\operatorname{dim}\left(\operatorname{Im}\left(T^{k+1}\right)\right)$ ，而得 $\operatorname{Im}\left(T^k\right)=\operatorname{Im}\left(T^{k+1}\right)$ ，
又，已知 $\operatorname{Im}\left(T^{k+2}\right) \subseteq \operatorname{Im}\left(T^{k+1}\right)$ ，
以下證明 $\operatorname{Im}\left(T^{k+1}\right) \subseteq \operatorname{Im}\left(T^{k+2}\right)$ ，而得 $\operatorname{Im}\left(T^{k+1}\right)=\operatorname{Im}\left(T^{k+2}\right)$ ，
$\left(\begin{array}{l}\text { 設 } \boldsymbol{v} \in \operatorname{Im}\left(T^{k+1}\right), \text { 即 } \boldsymbol{v}=T^{k+1}(\boldsymbol{u})=T\left(T^k(\boldsymbol{u})\right), \text { for some } \boldsymbol{u}, \\ \because T^k(\boldsymbol{u}) \in \operatorname{Im}\left(T^k\right), \text { 且 } \operatorname{Im}\left(T^{k+1}\right)=\operatorname{Im}\left(T^k\right), \therefore T^k(\boldsymbol{u})=T^{k+1}(\boldsymbol{w}), \text { for some } \boldsymbol{w}, \\ \therefore \boldsymbol{v}=T\left(T^{k+1}(\boldsymbol{w})\right) \in \operatorname{Im}\left(T^{k+2}\right),\end{array}\right)$
又類推可得 $\operatorname{Im}\left(T^{k+2}\right)=\operatorname{Im}\left(T^{k+3}\right), \operatorname{Im}\left(T^{k+3}\right)=\operatorname{Im}\left(T^{k+4}\right), \cdots$ ，故得證．
（3）由（1），（2）可得．
（4）先證出 $W=\bigcap_{i=1}^{\infty} \operatorname{Im}\left(T^i\right)=\operatorname{Im}\left(T^k\right)$ 為 $T$－不變子空間，（明顯可得）
再證出 $T_W$ 為可逆算子，
（因為 $T_W: W \rightarrow W$ ，且 $T$ 為映成，故 $T_W$ 可逆）
再證明 $W$ 為最大可逆區，
（令 $W^{\prime}$ 亦為 $T$ 的一個可逆區，即 $T_{W^{\prime}}$ 亦為可逆算子，則 $T_{W^{\prime}}\left(W^{\prime}\right)=W^{\prime}, \therefore T\left(W^{\prime}\right)=W^{\prime}$ ，則 $T^2\left(W^{\prime}\right)=W^{\prime}$ ，類推可得 $T^i\left(W^{\prime}\right)=W^{\prime}$ ，

又因為 $T^i\left(W^{\prime}\right) \subseteq \operatorname{Im}\left(T^i\right), \forall i, \therefore W^{\prime} \subseteq \operatorname{Im}\left(T^i\right), \therefore W^{\prime} \subseteq \bigcap_{i=1}^{\infty} \operatorname{Im}\left(T^i\right)=W, \therefore W^{\prime} \subseteq W$ ，得證．