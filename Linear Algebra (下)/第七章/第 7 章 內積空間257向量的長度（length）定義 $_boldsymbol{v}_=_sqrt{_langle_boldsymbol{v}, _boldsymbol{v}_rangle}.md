第 7 章 內積空間
257

向量的長度（length）
定義 $\|\boldsymbol{v}\|=\sqrt{\langle\boldsymbol{v}, \boldsymbol{v}\rangle}$ 為向量 $\boldsymbol{v}$ 的長度．
Note
（1）向量的長度也稱為向量的範數（norm）．
（2）若 $\|\boldsymbol{v}\|=1$ ，則稱 $\boldsymbol{v}$ 為單位向量（unit vector）．
（3）定義向量 $\boldsymbol{u}$ 與 $\boldsymbol{v}$ 的距離（distance）為 $\|\boldsymbol{u}-\boldsymbol{v}\|$ ．
（4）在歐氏空間下的標準內積定出的長度為 $\|\boldsymbol{x}\|=\left[\sum_{i=1}^n\left|x_i\right|^2\right]^{\frac{1}{2}}$ ，其中 $\boldsymbol{x}=\left(x_1, \ldots, x_n\right)$ ，
又記為 $\|\boldsymbol{x}\|_2 、 2$－norm．
例如： $\boldsymbol{x}=\left[\begin{array}{l}1 \\ 2\end{array}\right],\|\boldsymbol{x}\|=\sqrt{1^2+2^2}=\sqrt{5}, \boldsymbol{y}=[0,2],\|\boldsymbol{y}\|=\sqrt{0^2+2^2}=2$ ．
（5）考慮向量空間 $V_F, \forall \boldsymbol{u}, \boldsymbol{v} \in V, \alpha \in F$ ，
（a）$\|\boldsymbol{v}\| \geq 0$ ，且等號成立於 $\boldsymbol{v}$ 為零向量時．
（b）$\|\alpha \boldsymbol{v}\|=|\alpha|\|\boldsymbol{v}\|$ ．
（c）$\|\boldsymbol{u}\|-\|\boldsymbol{v}\| \leq\|\boldsymbol{u}+\boldsymbol{v}\| \leq\|\boldsymbol{u}\|+\|\boldsymbol{v}\|$ ．（三角不等式）
（以上是定義長度時須具備的）
【證明】
【 84 交大統計、 96 海洋資工、 96 政大數教、 104 中正應數】
（i）$\|\boldsymbol{u}+\boldsymbol{v}\|^2=\langle\boldsymbol{u}+\boldsymbol{v}, \boldsymbol{u}+\boldsymbol{v}\rangle$
$$
\begin{aligned}
& =<\boldsymbol{u}, \boldsymbol{u}>+<\boldsymbol{u}, \boldsymbol{v}>+<\boldsymbol{v}, \boldsymbol{u}>+<\boldsymbol{v}, \boldsymbol{v}>=<\boldsymbol{u}, \boldsymbol{u}>+<\boldsymbol{u}, \boldsymbol{v}>+\overline{<\boldsymbol{u}, \boldsymbol{v}>}+<\boldsymbol{v}, \boldsymbol{v}> \\
& =\|\boldsymbol{u}\|^2+\|\boldsymbol{v}\|^2+2 \operatorname{Re}(<\boldsymbol{u}, \boldsymbol{v}>) \ldots \ldots(<\boldsymbol{u}, \boldsymbol{v}>\text { 的實部 }) \\
& \leq\|\boldsymbol{u}\|^2+\|\boldsymbol{v}\|^2+2 k \boldsymbol{u}, \boldsymbol{v}>1 \\
& \leq\|\boldsymbol{u}\|^2+\|\boldsymbol{v}\|^2+2\|\boldsymbol{u}\|\|\boldsymbol{v}\|,(\text { 此處先用下一頁會證的結果: 柯西不等式 }) \\
& =(\|\boldsymbol{u}\|+\|\boldsymbol{v}\|)^2
\end{aligned}
$$

故得 $\|\boldsymbol{u}\|+\|\boldsymbol{v}\| \geq\|\boldsymbol{u}+\boldsymbol{v}\|$ ．
（ii）$\because u=(u+v)+(-v), \therefore\|u\| \leq\|u+v\|+\|-v\|=\|u+v\|+\|v\|$ ，
$$
\begin{aligned}
& \therefore\|u\|-\|v\| \leq\|u+v\|, \ldots \ldots .^* \\
& \because v=(u+v)+(-u), \therefore\|v\| \leq\|u+v\|+\|-u\|=\|u+v\|+\|u\|, \\
& \therefore\|v\|-\|u\| \leq\|u+v\|, \ldots \ldots .^{* *}
\end{aligned}
$$

由＊，＊＊得 $|\|\boldsymbol{u}\|-\|\boldsymbol{v}\|| \leq\|\boldsymbol{u}+\boldsymbol{v}\|$ ．