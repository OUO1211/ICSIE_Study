78

線性代數（下）



可對角化的充要條件

設 $T \in L(V, V), \operatorname{dim}(V)=n, \lambda_1, \lambda_2, \ldots, \lambda_r$ 為 $T$ 的相異特徵根，則下列敘述互為等價：

（1）$T$ 可對角化

（2） $\operatorname{char}_T(x)$ 在 $F$ 中可分解，且 $m\left(\lambda_i\right)=g m\left(\lambda_i\right), \forall i=1,2, \ldots, r$ ．

（3）$V=V\left(\lambda_1\right) \oplus V\left(\lambda_2\right) \oplus \cdots \oplus V\left(\lambda_r\right)$ ．

【證明】

（1）⇒（2）



設 $T$ 可對角化，即存在 $V$ 的基底 $\beta$ 使得 $[T]_\beta=D=$

$$

D=\left[\begin{array}{cccc}

\lambda_1 I_{m_1} & & & O \\

& \lambda_2 I_{m_2} & & \\

O & & \ddots & \\

O & & & \lambda_r I_{m_r}

\end{array}\right] \text { 為對角矩陣, }

$$



其中 $m_1+m_2+\ldots+m_r=n$ ，

$\because \beta$ 中的向量都是由 $T$ 的特徵向量所組成，

令 $\beta=\beta_1 \cup \beta_2 \cup \ldots \cup \beta_r$ ，其中 $\beta_i=\left\{\boldsymbol{v}_{i, 1}, \boldsymbol{v}_{i, 2}, \ldots, \boldsymbol{v}_{i, m_i}\right\}$ 為 $\beta$ 中相對於 $\lambda_i$ 的特徵向量 $i=1,2, \ldots, r$ ．

${\text { 則 } \operatorname{char}_T(x)=\operatorname{char}_D(x)=\operatorname{det}\left[\begin{array}{cccc}\left(\lambda_1-x\right) I_{m_1} & & & O \\ & \left(\lambda_2-x\right) I_{m_2} & & \\ O & & \ddots & \\ & & & \left(\lambda_r-x\right) I_{m_r}\end{array}\right] \text { ］}}$

$$

=\left(\lambda_1-x\right)^{m_1}\left(\lambda_2-x\right)^{m_2} \cdots\left(\lambda_r-x\right)^{m_r},

$$



即 $\operatorname{char}_T(x)$ 可在 $F$ 中分解，且 $\lambda_i$ 的代數重數 $m\left(\lambda_i\right)=m_i, \forall i=1,2, \ldots, r$ ，

又 $\because \beta$ 為線性獨立，故 $\beta_i$ 亦為線性獨立，

$$

\therefore m\left(\lambda_i\right)=m_i=\left|\beta_i\right| \leq \operatorname{dim}\left(V\left(\lambda_i\right)\right)=g m\left(\lambda_i\right), \forall i=1,2, \ldots, r,

$$



另一方面，已知 $g m\left(\lambda_i\right) \leq m\left(\lambda_i\right)$ ，故得 $m\left(\lambda_i\right)=g m\left(\lambda_i\right), \forall i=1,2, \ldots, r$ ，

（2）⇒（3）

因為 $V\left(\lambda_1\right)+V\left(\lambda_2\right)+\ldots+V\left(\lambda_r\right) \subseteq V$

且 $\operatorname{dim}\left(V\left(\lambda_1\right)+V\left(\lambda_2\right)+\ldots+V\left(\lambda_r\right)\right)=\operatorname{dim}\left(V\left(\lambda_1\right)\right)+\operatorname{dim}\left(V\left(\lambda_2\right)\right)+\ldots+\operatorname{dim}\left(V\left(\lambda_r\right)\right)$

$$

\begin{aligned}

& =g m\left(\lambda_1\right)+g m\left(\lambda_2\right)+\ldots+g m\left(\lambda_r\right)=m\left(\lambda_1\right)+m\left(\lambda_2\right)+\ldots+m\left(\lambda_r\right)=n \quad\left(\because \operatorname{char}_T(x)\right. \text { 可分解) } \\

& =\operatorname{dim}(V), \\

& \therefore V\left(\lambda_1\right)+V\left(\lambda_2\right)+\ldots+V\left(\lambda_r\right)=V,

\end{aligned}

$$



因 $\lambda_1, \lambda_2, \ldots, \lambda_r$ 為 $T$ 的相異特徵根，故 $V\left(\lambda_1\right), V\left(\lambda_2\right), \ldots, V\left(\lambda_r\right)$ 為獨立子空間，

$$

\therefore V\left(\lambda_1\right) \oplus V\left(\lambda_2\right) \oplus \ldots \oplus V\left(\lambda_r\right)=V .

$$