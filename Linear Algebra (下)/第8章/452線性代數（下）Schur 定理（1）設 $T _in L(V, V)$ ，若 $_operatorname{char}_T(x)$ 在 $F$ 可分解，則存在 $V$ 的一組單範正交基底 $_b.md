452
線性代數（下）

Schur 定理
（1）設 $T \in L(V, V)$ ，若 $\operatorname{char}_T(x)$ 在 $F$ 可分解，
則存在 $V$ 的一組單範正交基底 $\beta$ ，使 $[T]_\beta$ 為上三角矩陣。

【95台大数學】

（2）設 $A \in C^{n \times n}$ ，則存在一個么正矩陣 $P \in C^{n \times n}$ ，使 $P^H A P$ 為上三角矩陣。

【97 中山應数】

（3）設 $A \in R^{n \times n}$ ，且 $\operatorname{char}_A(x)$ 在 $R$ 中可分解，則存在正交矩陣 $P \in R^{n \times n}$ ，使 $P^T A P$ 為上三角矩陣。

【證明】
（1）induction on $\operatorname{dim}(V)$ ，
$\operatorname{dim}(V)=1$ 時，$T$ 的矩陣表示當然是一個上三角矩陣。
設 $\operatorname{dim}(V)=n-1$ 時，此命題成立，則 $\operatorname{dim}(V)=n$ 時，
$\because \operatorname{char}_T(x)$ 在 $F$ 中可分解，故 $T$ 有特徵根，故 $T *$ 有特徵根，取一個設為 $\lambda$ ，
則存在一單位向量 $\boldsymbol{v}$ ，使得 $T^*(\boldsymbol{v})=\lambda \boldsymbol{v}$ ，令 $W=\operatorname{span}(\{\boldsymbol{v}\})$ ，
則 $\operatorname{dim} W^{\perp}=n-1$ ，且 $W^{\perp}$ 必為 $T-$ 不變，（證明如下：）
則 $\operatorname{dim} W^{\perp}=n-1$ ，且 $W^{\perp}$ 必為 $T-$ 不變，（證明如下：）
$\left(\begin{array}{l}\forall \boldsymbol{x} \in W^{\perp}, \text { 任取 } \boldsymbol{y}=c \boldsymbol{v} \in W, \text { for some } c \in F, \\ \text { 則 }\langle T(\boldsymbol{x}), \boldsymbol{y}\rangle=\left\langle\boldsymbol{x}, T^*(\boldsymbol{y})\right\rangle=\left\langle\boldsymbol{x}, T^*(\boldsymbol{v})\right\rangle=\langle\boldsymbol{x}, c \lambda \boldsymbol{v}\rangle=\overline{c \lambda}\langle\boldsymbol{x}, \boldsymbol{v}\rangle=0, \\ \therefore T(\boldsymbol{x}) \in W^{\perp}, \text { 即 } T\left(W^{\perp}\right) \subseteq W^{\perp} .\end{array}\right)$
令 $U=T_{W^{\perp}}: T$ 限制在 $W^{\perp}$ 所得線性映射，
則 $\operatorname{char}_U(x) \mid \operatorname{char}_T(x)$ ，故 $\operatorname{char}_U(x)$ 在 $F$ 亦解，但 $\operatorname{dim}\left(W^{\perp}\right)=n-1$ ，
故由歸納假設得知：存在一 $W^{\perp}$ 的單範正交基底 $\gamma$ 使得 $[U]_\gamma$ 為一上三角矩陣，設為 $R$ ，則 $\because V=W \oplus W^{\perp}$ ，故取 $\beta=\gamma \cup\{\boldsymbol{v}\}$ 可成為 $V$ 的一單範正交基底，
且 $[T]_\beta=\left[\begin{array}{l|l}R & 0 \\ \hline 0 & \lambda\end{array}\right]$ 為一上三角矩陣．
（2），（3）的證明技巧類似（1）．讀者可自行練習．