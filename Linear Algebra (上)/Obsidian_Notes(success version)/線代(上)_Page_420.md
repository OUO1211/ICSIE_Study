## 座標變換矩陣(change of coordinate matrix)

> 令 $\beta=\{b_1,\ldots,b_n\}$，$\beta'=\{b_1',\ldots,b_n'\}$ 為空間 $V$ 之兩組基底組且 $\beta=[b_1,\ldots,b_n]$，$\beta'=[b_1',\ldots,b_n']$，
>
> 定義 $P=\big[[b_1]_{\beta'},\ldots,[b_n]_{\beta'}\big]$ 之矩，稱作 $\beta$ 到 $\beta'$ 的座標變換矩陣，
>
> 且 $P$ 會滿足
>
> (1) $\forall v\in V$，$[v]_{\beta'}=P[v]_\beta$。
>
> (2) $B'P=B$，故得 $P=(B')^{-1}B$。　　　　【94,95 中央資工、99 政大應數】

> **【證明】**
>
> (1) 設 $[v]_\beta=\begin{bmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{bmatrix}$，則 $v=x_1b_1+x_2b_2+\cdots+x_nb_n$，故
>
> $$
> \begin{aligned}
> v
> &=x_1(c_{11}b_1'+\cdots+c_{n1}b_n')+x_2(c_{12}b_1'+\cdots+c_{n2}b_n')+\cdots+x_n(c_{1n}b_1'+\cdots+c_{nn}b_n') \\
> &=(x_1c_{11}+\cdots+x_nc_{1n})b_1'+(x_1c_{21}+\cdots+x_nc_{2n})b_2'+\cdots+(x_1c_{n1}+\cdots+x_nc_{nn})b_n',
> \end{aligned}
> $$
>
> 即
>
> $$
> [v]_{\beta'}=
> \begin{bmatrix}
> x_1c_{11}+\cdots+x_nc_{1n} \\
> x_1c_{21}+\cdots+x_nc_{2n} \\
> \vdots \\
> x_1c_{n1}+\cdots+x_nc_{nn}
> \end{bmatrix}
> =
> \begin{bmatrix}
> c_{11} & c_{12} & \cdots & c_{1n} \\
> c_{21} & c_{22} & \cdots & c_{2n} \\
> \vdots & \vdots & & \vdots \\
> c_{n1} & c_{n2} & \cdots & c_{nn}
> \end{bmatrix}
> \begin{bmatrix}
> x_1 \\
> x_2 \\
> \vdots \\
> x_n
> \end{bmatrix}
> =P[v]_\beta.
> $$
>
> (2) 設 $[b_1]_{\beta'}=\begin{bmatrix} c_{11} \\ \vdots \\ c_{n1} \end{bmatrix}$，$[b_2]_{\beta'}=\begin{bmatrix} c_{12} \\ \vdots \\ c_{n2} \end{bmatrix}$，$\ldots$，$[b_n]_{\beta'}=\begin{bmatrix} c_{1n} \\ \vdots \\ c_{nn} \end{bmatrix}$，
>
> 即
>
> $$
> \begin{aligned}
> c_{11}b_1'+\cdots+c_{n1}b_n'&=b_1,\\
> c_{12}b_1'+\cdots+c_{n2}b_n'&=b_2,\\
> &\vdots\\
> c_{1n}b_1'+\cdots+c_{nn}b_n'&=b_n,
> \end{aligned}
> $$
>
> 即
>
> $$
> [b_1'\ b_2'\ \cdots\ b_n']
> \begin{bmatrix}
> c_{11} & c_{12} & \cdots & c_{1n} \\
> c_{21} & c_{22} & \cdots & c_{2n} \\
> \vdots & \vdots & & \vdots \\
> c_{n1} & c_{n2} & \cdots & c_{nn}
> \end{bmatrix}
> =
> [b_1\ b_2\ \cdots\ b_n],
> $$
>
> 即 $B'P=B$。

> **Note**
>
> (1) $P$ 又稱作 $\beta$ 到 $\beta'$ 的轉移矩陣(transition matrix)，也記做 $[I]_\beta^{\beta'}$。
>
> (2) $P$ 為可逆矩陣且 $P^{-1}=\big[[b_1']_\beta,\ldots,[b_n']_\beta\big]$，即 $\left([I]_\beta^{\beta'}\right)^{-1}=[I]_{\beta'}^\beta$。