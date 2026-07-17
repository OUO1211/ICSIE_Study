> **試題 10**
>
> (10%) Let $\{e_1, e_2, e_3\}$ be the standard basis of $R^3$ and $f: R^3 \to R^3$ be the linear map given on the standard basis by $f(e_1) = 2e_1 + e_3$ and $f(e_2) = e_1 + 3e_2$. Determine the $3 \times 2$ matrix of this map on the basis $3e_1 - e_2$, $2e_1 + e_3$ of $R^3$.
>
> 【95 交大統計】

> **解**
>
> 令 $\alpha_1 = e_1$，$\alpha_2 = e_2$，為 $R^3$ 的標準基底。
>
> 令 $\alpha_1 = \{e_1, e_2\}$ 為 $R^2$ 的標準基底。
>
> 則 $\alpha_1$ 到 $\alpha_2$ 的座標變換矩陣 $[I_{\alpha_1}]_{\alpha_2}^{\alpha_1}$
>
> 其中 $\alpha_1 = 3e_1 - e_2$，$\alpha_2 = 2e_1 + e_3$
>
> 由 $[I_{\alpha_1}]_{\alpha_2}^{\alpha_1}$，再 $[I_{\alpha_1}]_e^{\alpha_1} = \begin{bmatrix} 0 & 1 \\ 1 & 5 \end{bmatrix}$
>
> 且由 $f$ 知標準矩陣 $[f]_e^e = \begin{bmatrix} 2 & 1 & 0 \\ 0 & 3 & 0 \\ 1 & 0 & 0 \end{bmatrix}$
>
> 此外由題意下列矩陣，最終所求矩陣為：
>
> $$[f]_{\alpha_1}^{\alpha_2} = ([I_{\alpha_2}]_e^{\alpha_2})^{-1} \cdot [f]_e^e \cdot [I_{\alpha_1}]_e^{\alpha_1} = \begin{bmatrix} 0 & 1 \\ 1 & 5 \end{bmatrix}$$
>
> $$= ([I_{\alpha_2}]_e^{\alpha_2})^{-1} \cdot [f]_e^e \cdot [I_{\alpha_1}]_e^{\alpha_1} = \begin{bmatrix} -8 & 24 \\ -5 & -4 \\ 2 & -17 \end{bmatrix}$$
