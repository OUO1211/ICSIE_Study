286
線性代數（下）

而因 $\boldsymbol{u}_k=\boldsymbol{v}_k-\sum_{i=1}^{k-1} \frac{\left\langle\boldsymbol{v}_k, \boldsymbol{u}_i\right\rangle}{\left\langle\boldsymbol{u}_i, \boldsymbol{u}_i\right\rangle} \boldsymbol{u}_i, \therefore \boldsymbol{u}_k \in \operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{v}_k\right\}\right)$
又由歸納假設知 $\operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}\right\}\right)=\operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}\right\}\right)$ ，
所以 $\boldsymbol{u}_k \in \operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}, \boldsymbol{v}_k\right\}\right), \therefore \operatorname{span}\left(\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}\right) \subseteq \operatorname{span}\left(\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}, \boldsymbol{v}_k\right\}\right)$ ，
$\because\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}$ 為不含 $\mathbf{0}$ 的正交集，$\therefore\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}$ 線性獨立，
$$
\begin{aligned}
& \therefore \operatorname{dim}\left(\operatorname{span}\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}\right)=k=\operatorname{dim}\left(\operatorname{span}\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}, \boldsymbol{v}_k\right\}\right) \\
& \therefore \operatorname{span}\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{k-1}, \boldsymbol{u}_k\right\}=\operatorname{span}\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{k-1}, \boldsymbol{v}_k\right\} .
\end{aligned}
$$

Note
（1）若原 $S=\left\{v_1, v_2, \ldots, v_k\right\}$ 已為正交集，則在 Gram－Schmidt 正交化過程中，所得之 $\left\{\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_k\right\}=S .\left(\boldsymbol{v}_i=\boldsymbol{u}_i, \forall i\right)$
（2）當 $S=\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_k\right\}$ 不為線性獨立時，
設 $\boldsymbol{v}_j \in \operatorname{span}\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{j-1}\right\}$ ，且 $\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_{j-1}\right\}$ 為線性獨立，則可得 $\boldsymbol{u}_j=\mathbf{0}$ ，則將 $\boldsymbol{v}_j, \boldsymbol{u}_j$ 去掉再進行正交化步驟即可。