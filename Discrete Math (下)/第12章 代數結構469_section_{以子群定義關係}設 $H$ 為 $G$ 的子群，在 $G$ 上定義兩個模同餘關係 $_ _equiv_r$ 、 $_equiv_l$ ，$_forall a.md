第12章 代數結構
469

\section*{以子群定義關係}

設 $H$ 為 $G$ 的子群，在 $G$ 上定義兩個模同餘關係 $: \equiv_r$ 、 $\equiv_l$ ，
$\forall a, b \in G, a \equiv_r b(\bmod H) \Leftrightarrow a b^{-1} \in H$（右模同餘）。
$\forall a, b \in G, a \equiv l(\bmod H) \Leftrightarrow a^{-1} b \in H($ 左模同餘 $)$ 。
例如 ：考慮 $\left(Z_6,+{ }_6\right)$ ，取 $H=\{0,2,4\}$ ，則可知 $\left(H,+{ }_6\right)$ 為 $\left(Z_6,+{ }_6\right)$ 之子群。
則因為 $0+2^{-1}=0+4=4 \in H$ ，所以 $0 \equiv_r 2(\bmod H)$ ，
$2+4^{-1}=2+2=4 \in H$ ，所以 $2 \equiv_r 4(\bmod H)$ ，
$4+0^{-1}=4+0=4 \in H$ ，所以 $4 \equiv_r 0(\bmod H)$,
而得 $\{0,2,4\}$ 為同一等價類；同理可得 $\{1,3,5\}$ 為同一等價類。
Note
\begin{itemize}
\item[（1）] 此模同餘關係為一等價關係。
\item[（2）] 由 $\equiv_r(\bmod H)$ 所造出的等價類 $[a]=H a, \forall a \in G$ 。
\item[（3）] 由 $\equiv_l(\bmod H)$ 所造出的等價類 $[a]=a H, ~ \forall a \in G$ 。
\item[（4）] $H$ 的相異右（左）陪集形成 $G$ 的一個分割。
\item[（5）] $H$ 的每個右（左）陪集中之元素個數相同。
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 對 $G$ 中任意元素 $x, y, z$ ，
$\because x x^{-1}=e \in H \quad \therefore x R x \ldots .$. 反身性。
設 $x \equiv_r y, \therefore x y^{-1} \in H, \therefore\left(x y^{-1}\right)^{-1}=y x^{-1} \in H, \therefore y \equiv_r x \ldots \ldots$ 對稱性。
設 $x \equiv_r y, ~ y \equiv_r z$ ，即 $x y^{-1} \in H, ~ y z^{-1} \in H, \therefore\left(x y^{-1}\right)\left(y z^{-1}\right)=x z^{-1} \in H, \therefore x \equiv_r z \ldots$ 逸移性，故 $\equiv_r$ 為一等價關係。同理，$\equiv_l$ 亦為一等價關係。
\item[（2）]
$$
\begin{aligned}
{[a] } & =\left\{x \in G \mid x \equiv_r a(\bmod H)\right\}=\left\{x \in G \mid x a^{-1} \in H\right\} \\
& =\left\{x \in G \mid x a^{-1}=h \text { for some } h \in H\right\}=\{x \in G \mid x=h a, \text { for some } h \in H\}=H a
\end{aligned}
$$
\item[（3）] 同理可得。
\item[（4）] 因為相異等價類形成一分割，而每一等價類對應一 $H$ 之右（左）陪集，故得證。
\item[（5）] 定義一函數 $f: H \rightarrow H a$ by $f(h)=h a, \forall h \in H$ ，
則顯然 $f$ 為 onto ，又 if $h_1 a=h_2 a$ ，then $h_1=h_2$ ，所以 $f$ 為1－1。
所以 $|H|=|H a|, \forall a \in G$ ，即每個 $H$ 的右陪集與 $H$ 有同樣多個元素。
同理，亦可得每個 $H$ 的左陪集與 $H$ 有同樣多個元素。
\end{itemize}