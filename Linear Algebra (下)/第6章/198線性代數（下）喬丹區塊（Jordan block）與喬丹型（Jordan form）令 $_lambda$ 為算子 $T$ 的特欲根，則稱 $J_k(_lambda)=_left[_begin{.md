198
線性代數（下）

喬丹區塊（Jordan block）與喬丹型（Jordan form）
令 $\lambda$ 為算子 $T$ 的特徵根，則稱 $J_k(\lambda)=\left[\begin{array}{ccccc}\lambda & & & & \\ 1 & \lambda & & O & \\ & 1 & \lambda & & \\ & & \ddots & \ddots & \\ O & & & 1 & \lambda\end{array}\right]_{k \times k}$ 为 $k$ 階的喬丹區塊。
Note
（1）又稱作 Jordan 基本矩陣（Jordan fundamental matrix）．
（2）上述定義方式為下移型的 Jordan 基本矩陣，而其轉置稱上移型 Jordan 基本矩陣。例如：
$J_2(4)=\left[\begin{array}{ll}4 & 0 \\ 1 & 4\end{array}\right], J_3(0)=\left[\begin{array}{lll}0 & 0 & 0 \\ 1 & 0 & 0 \\ 0 & 1 & 0\end{array}\right], J_4(1)\left[\begin{array}{llll}1 & 0 & 0 & 0 \\ 1 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 1 & 1\end{array}\right]$ ，均為下移型；
$J_2(3)=\left[\begin{array}{ll}3 & 1 \\ 0 & 3\end{array}\right], J_3(-1)=\left[\begin{array}{ccc}-1 & 1 & 0 \\ 0 & -1 & 1 \\ 0 & 0 & -1\end{array}\right], J_4(1)\left[\begin{array}{cccc}1 & 1 & 0 & 0 \\ 0 & 1 & 1 & 0 \\ 0 & 0 & 1 & 1 \\ 0 & 0 & 0 & 1\end{array}\right]$ ，均為上移型．
（3）設 $T \in L(V, V), \operatorname{dim}(V)=n, \lambda_1, \lambda_2, \ldots, \lambda_r$ 為 $T$ 的相異特徵根，且 $c h a r_T(x)$ 在 $F$ 中可分解，則存在 $\beta_i$ 為 $K\left(\lambda_i\right)$ 的基底，$\forall i=1,2, \ldots, r$ ，使得
（a）$\beta=\beta_1 \cup \beta_2 \cup \cdots \cup \beta_r$ 為 $V$ 的基底，且 $[T]_\beta=\left[\begin{array}{llll}A_1 & & & O \\ & A_2 & & \\ & & \ddots & \\ O & & & A_r\end{array}\right]$ ，
稱 $T$ 的 Jordan form 或 Jordan 標準型（canonical form）．（也有下移與上移兩型）
其中，$A_i=\left[T_{K\left(\lambda_i\right)}\right]_{\beta_i}=\left[\begin{array}{cccc}J_{n_{i_1}}\left(\lambda_i\right) & & & O \\ & J_{n_{i_2}}\left(\lambda_i\right) & & \\ O & & \ddots & \\ & & & J_{n_{i_{i_i}}}\left(\lambda_i\right)\end{array}\right]_{m_i \times m_i}$ ，
$\left(T-\lambda_i I\right)_{K\left(\lambda_i\right)}$ 為 index $n_{\lambda_i}$ 的冪零算子，$m_i=m\left(\lambda_i\right)$ ，for $i=1,2, \ldots, r$ ．
（b）$k_i=\operatorname{dim}\left(\operatorname{ker}\left(T-\lambda_i I\right)\right)=g m\left(\lambda_i\right)$ ，for $i=1,2, \ldots, r$ ．
（4）$n$ 階方陣亦有類似上述定義與性質．