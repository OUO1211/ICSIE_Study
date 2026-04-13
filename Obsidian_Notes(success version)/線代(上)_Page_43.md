## 可逆 (invertible) 矩陣

> **定義：可逆矩陣**
>
> 考慮 $m \times n$ 矩陣 $A$，
>
> (1) 若存在 $n \times m$ 矩陣 $L$ 滿足 $LA = I_n$，則稱 $L$ 為 $A$ 的左反矩陣。
>
> (2) 若存在 $n \times m$ 矩陣 $R$ 滿足 $AR = I_m$，則稱 $R$ 為 $A$ 的右反矩陣。
>
> (3) $m = n$ 時，若存在 $n \times n$ 矩陣 $B$ 滿足 $AB = BA = I_n$，則稱 $B$ 為 $A$ 的反矩陣 (inverse)，記做 $B = A^{-1}$ 且稱 $A$ 為可逆矩陣。
>
> 〔109 中正統計〕

例如：

$B = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \end{bmatrix}$ 為 $A = \begin{bmatrix} 1 & 0 \\ 0 & 1 \\ 0 & 0 \end{bmatrix}$ 的左反矩陣，（$\because BA = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}$），也說：$A$ 為 $B$ 的右反矩陣；

但 $B$ 不為 $A$ 的右反矩陣，（$\because AB = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 0 \end{bmatrix}$），也說：$A$ 不為 $B$ 的左反矩陣。

**Note**

(1) $B = A^{-1}$ 若且唯若 $B$ 為 $A$ 的右反矩陣且 $B$ 為 $A$ 的左反矩陣。

(2) 若已知 $A$ 為 $n$ 階方陣 $A$，則

(a) 若 $AB = I$ 且 $AC = I$，則 $B = C$。（即右反矩陣唯一；同理可得左反矩陣唯一。）

(b) $AB = I$ 若且唯若 $BA = I$。（即唯一左（右）反矩陣就是其反矩陣）

〔89 台大資工、100 政大統計、101 台大電信、105 成大統計、106 中興應數〕

**【證明】**（以下證明使用了第三章的內容）

若 $AB = I$，則

$$
\because n = \operatorname{rank}(I_n) = \operatorname{rank}(AB) \leq \operatorname{rank}(A) \leq n，
$$

故 $\operatorname{rank}(A) = n$，

又因為 $A$ 為 $n \times n$，故 $A$ 可逆，所以存在 $X$，使得 $AX = XA = I$。

由 $AB = I = AX$，可得 $XAB = XAX$，$\therefore IB = IX$，$\therefore B = X$，

再由 $XA = I$，可得 $BA = I$。

同理也可以由 $BA = I$ 推得 $AB = I$。

(3) 若 $A$ 為可逆矩陣，則又稱 $A$ 為非奇異 (nonsingular) 矩陣（精確定義在第 2 章）。

(4) 若 $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$ 且 $ad - bc \neq 0$，則 $B = \dfrac{1}{ad - bc}\begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$ 為 $A$ 的反矩陣。