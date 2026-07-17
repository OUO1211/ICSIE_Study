第6章 Jordan form 及其應用
187

6－1 循環分解定理

冪

零（nilpotent）與指標（index）
（1）對線性算子 $T$ ，若存在正整数 $k$ 使得 $T^k=O$ ，則稱 $T$ 為一冪零算子，並稱使 $T^k=O$ 成立的最小正整数 $k$ 為 $T$ 的指標（index）．
（2）對矩陣 $A$ ，若存在正整数 $k$ 使得 $A^k=O$ ，則稱 $A$ 為一冪零矩陣，並稱使 $A^k=O$ 成立的最小正整数 $k$ 為 $A$ 的指標（index）．

例如：零矩陣是冪零矩陣，指標為 1 ；嚴格上（下）三角也是冪零矩陣。

Note
（1）以下性質對矩陣或算子都有類似討論。
（2）若 $T$ 為向量空間 $V$ 上的冪零算子，則
$\operatorname{index}(T)=k \Leftrightarrow \operatorname{ker}\left(T^k\right)=V$ 且 $\operatorname{ker}\left(T^{k-1}\right) \neq V$ ．
（3）若 $T$ 為向量空間 $V$ 上的算子，且 $W$ 為 $T$ 不變子空間，$T_W$ 為限制在 $W$ 上的函數，則
（a）若 $T_W$ 為冪零算子，稱 $T$ 在 $W$ 上局部冪零（locally nilpotent on $W$ ）．
（b）若 $T_W$ 為可逆算子，稱 $T$ 在 $W$ 上局部可逆（locally invertible on $W$ ）．
（c）若 $W$ 為使 $T_W$ 為冪零算子的最大不變子空間，則稱 $W$ 為最大冪零區．
（d）若 $W$ 為使 $T_W$ 為可逆算子的最大不變子空間，則稱 $W$ 為最大可逆區．
（4）考慮 $n$ 維向量空間 $V$ 上的冪零算子 $T$ ，則
（a）$T$ 的特徵根均為 0 ．
（b） $\operatorname{char}_T(x)=(-x)^n$ ．
（c）$T^n=O$ ．

【91．92 台大數學】

（d） $\operatorname{det}(T)=0$ ．
（e）$T$ 不可逆．