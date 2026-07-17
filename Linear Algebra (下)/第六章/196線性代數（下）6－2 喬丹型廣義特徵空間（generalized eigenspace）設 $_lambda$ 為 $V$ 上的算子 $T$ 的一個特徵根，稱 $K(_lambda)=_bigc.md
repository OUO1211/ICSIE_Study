196
線性代數（下）

6－2 喬丹型

廣義特徵空間（generalized eigenspace）
設 $\lambda$ 為 $V$ 上的算子 $T$ 的一個特徵根，
稱 $K(\lambda)=\bigcup_{i=1}^{\infty}\left(\operatorname{ker}(T-\lambda I)^i\right)$ 為 $T$ 相對於 $\lambda$ 的廣義特微空間。
Note
（1）$K(\lambda)$ 中的非零向量稱為 $T$ 相對於 $\lambda$ 的廣義特徵向量．
（2）設 $T \in L(V, V), \lambda$ 為 $T$ 的特徵根，則（i）$K(\lambda)$ 為 $V$ 的子空間，（ii）$K(\lambda)$ 為 $T$ 不變．
【 85 台大資工、 94 交大電資、 94 交大應數】
（3）設 $T \in L(V, V), \operatorname{dim}(V)=n, \lambda_1, \lambda_2, \ldots, \lambda_r$ 為 $T$ 的相異特徵根，且 $\operatorname{char}_T(x)$ 在 $F$ 中可分解，則 $V=K\left(\lambda_1\right) \oplus K\left(\lambda_2\right) \oplus \cdots \oplus K\left(\lambda_r\right)$ ．
（4）也可定義方陣 $A$ 的廣義特徵空間與廣義特徵向量，上述性質也都成立。

例題
（12\％）Let $A=\left[\begin{array}{cc}1 & 1 \\ -1 & 3\end{array}\right]$ ．
（1）Find the eigenvalues and eigenvectors of $A$ ．
（2）Solve $(A-2 I) \boldsymbol{v}=\boldsymbol{e}$ for $\boldsymbol{v}$ ，where $\boldsymbol{e}$ is an eigenvector of $A$ ．
（3）Given the matrix $A$ with respect to the basis $\{\boldsymbol{e}, \boldsymbol{v}\}$ ．
【92．101．104師大資工】
解（1） $\operatorname{char}_A(x)=\left|\begin{array}{cc}1-x & 1 \\ -1 & 3-x\end{array}\right|=x^2-4 x+4=(x-2)^2$ ，得特徴根2．
且 $V(2)=\operatorname{ker}(A-2 I)=\operatorname{ker}\left(\left[\begin{array}{ll}-1 & 1 \\ -1 & 1\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{l}1 \\ 1\end{array}\right]\right\}$ ，故 2 所對的特徵向量為 $\left[\begin{array}{l}t \\ t\end{array}\right], t \neq 0$ 。
（2）$(A-2 I)=\left[\begin{array}{ll}-1 & 1 \\ -1 & 1\end{array}\right]$ ，解 $\left[\begin{array}{ll}-1 & 1 \\ -1 & 1\end{array}\right]\left[\begin{array}{l}x_1 \\ x_2\end{array}\right]=\left[\begin{array}{l}1 \\ 1\end{array}\right]=\boldsymbol{e}$ ，得 $\boldsymbol{v}=\left[\begin{array}{l}x_1 \\ x_2\end{array}\right]=\left[\begin{array}{c}s \\ 1+s\end{array}\right], s \in F$ ．
（3）因 $A \boldsymbol{e}=2 \boldsymbol{e}, A \boldsymbol{v}=\left[\begin{array}{cc}1 & 1 \\ -1 & 3\end{array}\right]\left[\begin{array}{c}s \\ 1+s\end{array}\right]=\left[\begin{array}{l}1+2 s \\ 3+2 s\end{array}\right]=l \boldsymbol{e}+2 \boldsymbol{v}$ ，
故 $A$ 相對於 $\{\boldsymbol{e}, \boldsymbol{v}\}$ 的矩陣表示為 $\left[\begin{array}{ll}2 & 1 \\ 0 & 2\end{array}\right]$ ．