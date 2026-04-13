> **例題 7**
>
> For any square matrix $A$, show that:
>
> (1) $AA^T$ is symmetric.
>
> (2) $B = \dfrac{A + A^T}{2}$ is symmetric. 〔104 政大資科〕
>
> (3) $C = \dfrac{A - A^T}{2}$ is skew-symmetric. 〔104 政大資料〕
>
> **解：**
>
> (1) $(AA^T)^T = (A^T)^T A^T = AA^T$，所以 $AA^T$ 為 symmetric。
>
> (2) $B^T = \left(\dfrac{A + A^T}{2}\right)^T = \dfrac{A^T + (A^T)^T}{2} = \dfrac{A^T + A}{2} = B$，所以 $B$ 為 symmetric。
>
> (3) $C^T = \left(\dfrac{A - A^T}{2}\right)^T = \dfrac{A^T - (A^T)^T}{2} = \dfrac{A^T - A}{2} = -C$，所以 $C$ 為 skew-symmetric。

> **例題 8**
>
> (4%) Let $A$ be a non-symmetric matrix. Determine and explain whether the following matrix ($B$, $C$): (1) must be symmetric, (2) must be skew-symmetric, or (3) otherwise. Where $B = A - A^T$ and $C = (I + A)(I - A^T)$.
>
> 〔106 交大資工〕
>
> **解：**
>
> $B^T = (A - A^T)^T = A^T - (A^T)^T = A^T - A = -B$，所以 $B$ 為 skew-symmetric；
>
> 但 $A^T \ne A$，$\therefore B \ne 0$，
>
> $\therefore B$ 不會同時是 symmetric，選 (2)。
>
> 另外，
>
> $C = (I + A)(I - A^T)$
>
> 故 $C = I + A - A^T - AA^T$
>
> 若 $C^T = C$，則 $-A + A^T = A - A^T$，
>
> 而得 $A^T = A$，與已知不合；
>
> 若 $C^T = -C$，則 $-AA^T = -I + A^T - A + AA^T$
>
> 而得 $I = AA^T$，但不是每個非對稱的 $A$ 都能滿足這點，
>
> 故選 (3)。