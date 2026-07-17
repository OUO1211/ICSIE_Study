114

線性代數（下）



5－4 投影算子與特徵根



投影算子與投影矩陣

若向量空間 $V$ 上線性算子 $T$ 滿足 $T^2=T$ ，

則稱 $T$ 為 $V$ 上的一投影算子（或冪等（idempotent）算子）．

若方陣 $A$ 滿足 $A^2=A$ ，

則稱 $A$ 為一投影矩陣（或冪等（idempotent）矩陣）。

Note

（1）本小節在線性算子上的定義與性質，對矩陣也有類似性質成立。

（2）若 $T \in L(V, V)$ 為投影算子，則

（a） $\operatorname{Im}\left(T^2\right)=\operatorname{Im}(T)$ ．

（b） $\operatorname{rank}\left(T^2\right)=\operatorname{rank}(T)$ ．

（c） $\operatorname{ker}\left(T^2\right)=\operatorname{ker}(T)$ ．

（d） $\operatorname{nullity}\left(T^2\right)=\operatorname{nullity}(T)$ ．

（e） $\operatorname{ker}(T) \cap \operatorname{Im}(T)=\{\boldsymbol{0}\}$ ．

（f）$V=\operatorname{ker}(T) \oplus \operatorname{Im}(T)$ ．

（g） $\operatorname{det}(T)=0$ 或 1 ．

（以上性質在第四章都有給證明了）