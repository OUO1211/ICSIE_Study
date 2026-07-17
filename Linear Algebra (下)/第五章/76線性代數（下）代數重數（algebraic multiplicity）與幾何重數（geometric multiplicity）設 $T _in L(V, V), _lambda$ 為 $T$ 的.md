76
線性代數（下）

代數重數（algebraic multiplicity）與幾何重數（geometric multiplicity）
設 $T \in L(V, V), \lambda$ 為 $T$ 的特微根，
（1）$\lambda$ 在 $\operatorname{char}_T(x)$ 中的個数稱為 $\lambda$ 的代数重数，又稱稱重数，記做 $m(\lambda)$ ．
（2） $\operatorname{dim}(V(\lambda))$ 稱為 $\lambda$ 的幾何重数，記做 $g m(\lambda)$ 。
例如，考慮線性映射 $T: R^2 \rightarrow R^2, T(\boldsymbol{x})=A \boldsymbol{x}, A=\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right]$ ，
則 $\operatorname{char}_T(x)=\operatorname{char}_A(x)=(1-x)^2$ ，特徵根為 1,1 ，則
1 的代數重數 $m(1)=2$ ，
1 的幾何重數 $g m(1)=\operatorname{dim}(V(1))=\operatorname{dim}(\operatorname{ker}(A-I))=2-\operatorname{rank}(A-I)=2-\operatorname{rank}\left(\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right]\right)=1$ ．

Note
（1）此處對線性算子所討論的定義與性質，對方陣討論時亦可成立。
（2）計算時常使用： $\operatorname{gm}(\lambda)=\operatorname{dim}(V(\lambda))=\operatorname{dim}(\operatorname{ker}(T-\lambda I))=n-\operatorname{rank}(T-\lambda I)$ ．
（3）對特徴根 0 的時候：$g m(0)=\operatorname{dim}(V(0))=\operatorname{dim}(\operatorname{ker}(T))=n-\operatorname{rank}(T)$ 。
（4）考慮 $n$ 維空間 $V$ 上的線性算子 $T$ ，若 $\lambda$ 為 $T$ 的一個特徵根，則 $g m(\lambda) \leq m(\lambda)$ ．
（5）若 $\lambda$ 為特徵根，則 $V(\lambda)$ 不只含 $\mathbf{0}$ ，故 $g m(\lambda)=\operatorname{dim}(V(\lambda)) \geq 1$ 。
（6）若 $\lambda$ 為特徵根，則因為 $\operatorname{deg}\left(\operatorname{char}_T(x)\right)=n$ ，故 $m(\lambda) \leq n$ ．
（7）由上述得： $1 \leq g m(\lambda) \leq m(\lambda) \leq n$ ．
（8）由上述得：若 $\operatorname{rank}(T)=k$ ，則 $T$ 的相異非零特徵根頂多 $k$ 個．

【90成大應數】