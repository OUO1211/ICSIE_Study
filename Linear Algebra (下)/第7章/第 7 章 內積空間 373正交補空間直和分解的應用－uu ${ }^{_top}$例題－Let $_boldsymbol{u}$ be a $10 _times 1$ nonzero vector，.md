第 7 章 內積空間 373

正交補空間直和分解的應用－uu ${ }^{\top}$
例題－
Let $\boldsymbol{u}$ be a $10 \times 1$ nonzero vector，find the eigenvalues of $\boldsymbol{u} \boldsymbol{u}^T$ and $\operatorname{det}\left(\boldsymbol{u} \boldsymbol{u}^T\right)$ ．
【95交大统計】
解 $\boldsymbol{u} \boldsymbol{u}^T$ 為一 $10 \times 10$ 的矩陣，且 $\boldsymbol{u}^T \boldsymbol{u}$ 為一純量．
$$
\because\left(\boldsymbol{u} \boldsymbol{u}^T\right) \boldsymbol{u}=\boldsymbol{u}\left(\boldsymbol{u}^T \boldsymbol{u}\right)=\left(\boldsymbol{u}^T \boldsymbol{u}\right) \boldsymbol{u},
$$
$\therefore \boldsymbol{u}^T \boldsymbol{u}$ 為 $\boldsymbol{u} \boldsymbol{u}^T$ 的一特徵根，相對於特徵向量 $\boldsymbol{u}$ ，
令 $W=\operatorname{span}\{\boldsymbol{u}\}$ ，又取 $\left\{\boldsymbol{u}_2, \ldots, \boldsymbol{u}_{10}\right\}$ 為 $W^{\perp}$ 的一組基底，
則 for $2 \leq i \leq 10,\left(\boldsymbol{u} \boldsymbol{u}^T\right) \boldsymbol{u}_i=\boldsymbol{u}\left(\boldsymbol{u}^T \boldsymbol{u}_i\right)=\left(\boldsymbol{u}^T \boldsymbol{u}_i\right) \boldsymbol{u}=0 \boldsymbol{u}=\mathbf{0}=0 \boldsymbol{u}_i$ ，
即 0 為 $\boldsymbol{u} \boldsymbol{u}^T$ 的一特徵根，相對於特徵向量 $\boldsymbol{u}_i$ ，
$\because \boldsymbol{u}_2, \ldots, \boldsymbol{u}_{10}$ 為獨立的向量， 0 的幾何重數 $=9$ ，故 0 的重根數 $\geq 9$ ，
又 $\boldsymbol{u} \boldsymbol{u}^T$ 為 $10 \times 10,10$ 個特徵根，而已經有 $\boldsymbol{u}^T \boldsymbol{u}$ 為一特徵根了，所以 0 的重根數 $=9$ ，
因為 0 的特徵空間有 $\boldsymbol{u}_2 \sim \boldsymbol{u}_{10}$ 這九個獨立的特徵向量，故
0 的代數重數 $\geq 0$ 的幾何重數 $=\operatorname{dim}(V(0)) \geq 9$ ，
即特徴根就是 $\left\{\boldsymbol{u}^T \boldsymbol{u}, 0,0,0,0,0,0,0,0,0\right\}$ ，
又 $\operatorname{det}\left(\boldsymbol{u} \boldsymbol{u}^T\right)=\boldsymbol{u} \boldsymbol{u}^T$ 的所有特徵根的乘積 $=0$ 。