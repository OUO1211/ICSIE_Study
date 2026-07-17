第 7 章 內積空間 285

7－2 Gram－Schmidt 正交化過程

Gram－Schmidt 正交化過程
考虑內積向量空間 $V$ 上的線性獨立集 $S=\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n\right\}$ ，令 $\boldsymbol{u}_1=\boldsymbol{v}_1$ ，
$$
\begin{aligned}
& \boldsymbol{u}_2=\boldsymbol{v}_2-\frac{\left\langle\boldsymbol{v}_2, \boldsymbol{u}_1\right\rangle}{\left\langle\boldsymbol{u}_1, \boldsymbol{u}_1\right\rangle} \boldsymbol{u}_1, \\
& \boldsymbol{u}_3=\boldsymbol{v}_3-\frac{\left\langle\boldsymbol{v}_3, \boldsymbol{u}_1\right\rangle}{\left\langle\boldsymbol{u}_1, \boldsymbol{u}_1\right\rangle} \boldsymbol{u}_1-\frac{\left\langle\boldsymbol{v}_3, \boldsymbol{u}_2\right\rangle}{\left\langle\boldsymbol{u}_2, \boldsymbol{u}_2\right\rangle} \boldsymbol{u}_2, \cdots, \quad\left(\text { 即 } \boldsymbol{u}_k=\boldsymbol{v}_k-\sum_{i=1}^{k-1} \frac{\left\langle\boldsymbol{v}_k, \boldsymbol{u}_i\right\rangle}{\left\langle\boldsymbol{u}_i, \boldsymbol{u}_i\right\rangle} \boldsymbol{u}_i, \text { for } 2 \leq k \leq n .\right)
\end{aligned}
$$

則 $\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_n\right\}$ 為不含零向量的正交集，且 $\operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_n\right\}\right)=\operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n\right\}\right)$ ．
【證明】

【重要】

induction on $n$ ，
$n=1$ 時，$\because\left\{\boldsymbol{v}_1\right\}$ 為線性獨立集合，故 $\left\{\boldsymbol{u}_1\right\}$ 為不含 $\mathbf{0}$ 的正交集，
而 $\operatorname{span}\left(\left\{\boldsymbol{v}_1\right\}\right)=\operatorname{span}\left(\left\{\boldsymbol{u}_1\right\}\right)$ 明顯成立。
設 $n=k-1$ ，命題成立，則 $n=k$ 時，
$\because\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_k\right\}$ 線性獨立，$\therefore\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}\right\}$ 線性獨立，
故由歸納假設知 $\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}\right\}$ 為不含 $\mathbf{0}$ 的正交集，
且 $\operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}\right\}\right)=\operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}\right\}\right)$ ，
而 for $j=1,2, \ldots, k-1$ ，
$$
\begin{aligned}
<\boldsymbol{u}_k, \boldsymbol{u}_j> & =<\boldsymbol{v}_k-\sum_{i=1}^{k-1} \frac{<\boldsymbol{v}_k, \boldsymbol{u}_i>}{<\boldsymbol{u}_i, \boldsymbol{u}_i>} \boldsymbol{u}_i, \boldsymbol{u}_j> \\
& =<\boldsymbol{v}_k, \boldsymbol{u}_j>-\sum_{i=1}^{k-1} \frac{<\boldsymbol{v}_k, \boldsymbol{u}_i>}{<\boldsymbol{u}_i, \boldsymbol{u}_i>}<\boldsymbol{u}_i, \boldsymbol{u}_j> \\
& =<\boldsymbol{v}_k, \boldsymbol{u}_j>-\frac{<\boldsymbol{v}_k, \boldsymbol{u}_j>}{<\boldsymbol{u}_j, \boldsymbol{u}_j>}<\boldsymbol{u}_j, \boldsymbol{u}_j>\left(\because\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}\right\} \text { 為正交集 }\right) \\
& =<\boldsymbol{v}_k, \boldsymbol{u}_j>-<\boldsymbol{v}_k, \boldsymbol{u}_j>=0 .
\end{aligned}
$$

即 $\boldsymbol{u}_k \perp \boldsymbol{u}_j$ ，for all $j=1,2, \ldots, k-1, \therefore\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}$ 為正交集，
若 $\boldsymbol{u}_k=\mathbf{0}$ ，則得 $\boldsymbol{v}_k=\sum_{i=1}^{k-1} \frac{\left\langle\boldsymbol{v}_k, \boldsymbol{u}_i\right\rangle}{\left\langle\boldsymbol{u}_i, \boldsymbol{u}_i\right\rangle} \boldsymbol{u}_i \in \operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}\right\}\right)=\operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}\right\}\right)$
與 $S=\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}, \boldsymbol{v}_k\right\}$ 為獨立集矛盾，故 $\boldsymbol{u}_k \neq \mathbf{0}, \therefore\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}$ 為不含 $\mathbf{0}$ 的正交集，