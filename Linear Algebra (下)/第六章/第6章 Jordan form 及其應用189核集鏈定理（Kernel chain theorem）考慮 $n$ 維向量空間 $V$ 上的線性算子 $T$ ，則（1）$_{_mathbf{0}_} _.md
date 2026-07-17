第6章 Jordan form 及其應用
189

核集鏈定理（Kernel chain theorem）
考慮 $n$ 維向量空間 $V$ 上的線性算子 $T$ ，則
（1）$\{\mathbf{0}\} \subseteq \operatorname{ker}(T) \subseteq \operatorname{ker}\left(T^2\right) \subseteq \cdots \subseteq \operatorname{ker}\left(T^i\right) \subseteq \operatorname{ker}\left(T^{i+1}\right) \subseteq \cdots \subseteq V$ ．
（2）存在最小正整数 $k$ ，使得 $\operatorname{ker}\left(T^k\right)=\operatorname{ker}\left(T^{k+1}\right)=\operatorname{ker}\left(T^{k+2}\right)=\cdots$ ．

【95高師数學】

（3）$\bigcup_{i=1}^{\infty} \operatorname{ker}\left(T^i\right)=\operatorname{ker}\left(T^k\right)$ ，其中 $k$ 為（2）所得．
（4）$W=\bigcup_{i=1}^{\infty} \operatorname{ker}\left(T^i\right)$ 為 $T$ 的最大雾零區，且 $\operatorname{index}\left(T_W\right)=k$ ．
【證明】
（1）明顯可得．
（2）由（1）可得 $0 \leq \operatorname{dim}(\operatorname{ker}(T)) \leq \operatorname{dim}\left(\operatorname{ker}\left(T^2\right)\right) \leq \cdots \leq \operatorname{dim}(V)=n$ ，故 $\operatorname{dim}(\operatorname{ker}(T)), \operatorname{dim}\left(\operatorname{ker}\left(T^2\right)\right), \operatorname{dim}\left(\operatorname{ker}\left(T^3\right)\right), \ldots$ ，這無限多個數字中，必存在 $k \in Z^{+}$使得 $\operatorname{ker}\left(T^k\right)=\operatorname{ker}\left(T^{k+1}\right)$ ，
又，已知 $\operatorname{ker}\left(T^{k+1}\right) \subseteq \operatorname{ker}\left(T^{k+2}\right)$ ，
以下證明 $\operatorname{ker}\left(T^{k+2}\right) \subseteq \operatorname{ker}\left(T^{k+1}\right)$ ，而得 $\operatorname{ker}\left(T^{k+1}\right)=\operatorname{ker}\left(T^{k+2}\right)$ ， $\binom{\text { 設 } \boldsymbol{v} \in \operatorname{ker}\left(T^{k+2}\right), ~ \text { 即 } T^{k+2}(\boldsymbol{v})=\mathbf{0}, \therefore T^{k+1}(T(\boldsymbol{v}))=\mathbf{0}, \therefore T(\boldsymbol{v}) \in \operatorname{ker}\left(T^{k+1}\right),}{\text { 但 } \operatorname{ker}\left(T^{k+1}\right)=\operatorname{ker}\left(T^k\right), \therefore T^k(T(\boldsymbol{v}))=\mathbf{0}, \therefore T^{k+1}(\boldsymbol{v})=\mathbf{0}, \therefore \boldsymbol{v} \in \operatorname{ker}\left(T^{k+1}\right)}$
又類推可得 $\operatorname{ker}\left(T^{k+2}\right)=\operatorname{ker}\left(T^{k+3}\right), \operatorname{ker}\left(T^{k+3}\right)=\operatorname{ker}\left(T^{k+4}\right), \cdots$ ，故得證．
（3）由（1），（2）可得．
（4）先證出 $W=\bigcup_{i=1}^{\infty} \operatorname{ker}\left(T^i\right)=\operatorname{ker}\left(T^k\right)$ 為 $T$ — 不變子空間（明顯可得）
再證出 $T_W$ 為冪零算子，
（for $\boldsymbol{v} \in W=\operatorname{ker}\left(T^k\right), T^k(\boldsymbol{v})=\mathbf{0}, \therefore T_W$ 為冪零算子．）
再證明 $W$ 為最大冪零區，
$\binom{\text { 令 } W^{\prime} \text { 亦為 } T \text { 的一個幂零區，即 } T_{W^{\prime}} \text { 亦為幕零算子，設 } \operatorname{index}\left(T_{W^{\prime}}\right)=t,}{\text { 則 } \forall v \in W^{\prime}, T^{\prime}(v)=\mathbf{0}, \therefore v \in \operatorname{ker}\left(T^{\prime}\right) \text { ，但 } \operatorname{ker}\left(T^{\prime}\right) \subseteq \bigcup_{i=1}^{\infty} \operatorname{ker}\left(T^i\right)=W, \therefore v \in W, \therefore W^{\prime} \subseteq W, \text { 得證．}}$
最後得 $\operatorname{index}\left(T_W\right)=k$ ：
$\binom{\because W=\operatorname{ker}\left(T^k\right), \therefore T^k(W)=\{\boldsymbol{0}\}, \text { 即 }\left(T_W\right)^k=O,}{\text { 又因为 } k \text { 为為最小正整數，故得證．}}$