302 線性代數（下）

∵ for $\boldsymbol{v} \in V, \operatorname{proj}_W(\boldsymbol{v}) \in W$ ，又 for $\boldsymbol{w} \in W, \operatorname{proj}_W(\boldsymbol{v})-\boldsymbol{w} \in W$ ，
$\therefore \boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})$ 與 $\operatorname{proj}_W(\boldsymbol{v})-\boldsymbol{w}$ 必正交，
$$
\begin{aligned}
\therefore\|\boldsymbol{v}-\boldsymbol{w}\|^2 & =\mid \boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})+\operatorname{proj}_W(\boldsymbol{v})-\boldsymbol{w}\left\|^2=\right\| \boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})\left\|^2+\right\| \operatorname{proj}_W(\boldsymbol{v})-\boldsymbol{w} \|^2 \\
& \geq\left\|\boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})\right\|^2, \\
\therefore\|\boldsymbol{v}-\boldsymbol{w}\| & \geq\left\|\boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})\right\| .
\end{aligned}
$$
（4）$\left\|\boldsymbol{v}-\operatorname{proj}_W(\boldsymbol{v})\right\|$ 稱為 $\boldsymbol{v}$ 到 $W$ 的距離．