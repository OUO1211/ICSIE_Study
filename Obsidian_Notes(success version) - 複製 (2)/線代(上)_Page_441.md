（接上頁試題 13 的解）

可解得 $\gamma = \left\{ \begin{bmatrix} \frac{1}{2} & \frac{1}{2} \\ \frac{1}{2} & \frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & -\frac{1}{2} \\ \frac{1}{2} & -\frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & \frac{1}{2} \\ -\frac{1}{2} & -\frac{1}{2} \end{bmatrix}, \begin{bmatrix} \frac{1}{2} & -\frac{1}{2} \\ -\frac{1}{2} & \frac{1}{2} \end{bmatrix} \right\}$。

> **試題 14**
>
> (10%) Let $A = \begin{bmatrix} W & X \\ Y & Z \end{bmatrix}$, where $\text{rank}(A) = r = \text{rank}(W_{r \times r})$, show that there are matrices $B$ and $C$ such that $A = \begin{bmatrix} W & WC \\ BW & BWC \end{bmatrix} = \begin{bmatrix} I \\ B \end{bmatrix} W [I \; C]$.
>
> 【97 中興統計】

解：因為 $\text{rank}(W) = r$，故 $W$ 可逆，

又因 $CS(W) \subseteq CS(A)$，又 $CS(A) = \{Ax : x \in F^{n \times 1}\} = CS\begin{pmatrix} \begin{bmatrix} W & X \\ Y & Z \end{bmatrix} \end{pmatrix}$，

$$\text{rank}\begin{pmatrix} \begin{bmatrix} I & O \\ -YW^{-1} & I \end{bmatrix} \begin{bmatrix} W & X \\ Y & Z \end{bmatrix} \end{pmatrix} = \text{rank}\begin{pmatrix} \begin{bmatrix} W & X \\ O & Z - YW^{-1}X \end{bmatrix} \end{pmatrix}$$

$$= \text{rank}(W) + \text{rank}(Z - YW^{-1}X) = \text{rank}(A)$$

$\therefore r + \text{rank}(Z - YW^{-1}X) = r$，$\therefore Z - YW^{-1}X = O$，$\therefore Z = YW^{-1}X$。

$\therefore r + \text{rank}(Z - YW^{-1}X) = r$，令 $B = YW^{-1}$，$C = W^{-1}X$，

$$\therefore A = \begin{bmatrix} W & X \\ Y & Z \end{bmatrix} = \begin{bmatrix} W & WC \\ BW & BWC \end{bmatrix} = \begin{bmatrix} I \\ B \end{bmatrix} W \begin{bmatrix} I & C \end{bmatrix}$$。

> **試題 15**
>
> Let $A$, $B \in R^{m \times n}$. Show that $\text{rank}(AB) \leq R(B) \cap N(A) = \{0\}$.

解：先證明 $\text{rank}(AB) \leq \text{rank}(B) \Leftrightarrow \text{nullity}(AB) = k - \text{nullity}(B) = \text{nullity}(AB) = \text{nullity}(B)$，

由定義（用限制域）$N(B) \subseteq N(AB)$，

$$\Rightarrow \exists x \in N(AB) \setminus N(B)$$，即 $x \notin N(B)$，故 $Bx \neq 0$，

則 $Bx \in N(A)$，又 $Bx \in N(B)$，故 $x \in N(B)$，矛盾，

$\therefore N(B) = N(AB)$，故 $\text{nullity}(AB) = \text{nullity}(B)$，即 $\text{rank}(AB) = \text{rank}(B)$。

以下說明：$N(B) = N(AB) \Leftrightarrow R(B) \cap N(A) = \{0\}$：

（$\Rightarrow$）$N(B) \subseteq N(AB)$，故若 $R(B) \cap N(A) \neq \{0\}$，則存在非零 $y \in R(B) \cap N(A)$，

即 $\exists x \notin N(B)$，使 $Bx = y \in N(A)$，故 $ABx = 0$，故 $x \in N(AB) \setminus N(B)$，矛盾。

（$\Leftarrow$）取 $x \in N(AB)$，故 $ABx = 0$，即 $Bx \in N(A)$，且 $Bx \in R(B)$，

故 $Bx \in R(B) \cap N(A) = \{0\}$，故 $Bx = 0$，即 $x \in N(B)$，故 $N(AB) \subseteq N(B)$，

故 $N(B) = N(AB)$。
