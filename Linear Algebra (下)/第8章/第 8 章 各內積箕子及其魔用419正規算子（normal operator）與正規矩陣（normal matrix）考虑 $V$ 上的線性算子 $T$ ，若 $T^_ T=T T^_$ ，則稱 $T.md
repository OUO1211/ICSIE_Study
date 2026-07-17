第 8 章 各內積箕子及其魔用
419

正規算子（normal operator）與正規矩陣（normal matrix）
考虑 $V$ 上的線性算子 $T$ ，若 $T^* T=T T^*$ ，則稱 $T$ 為正規算子。
考虑方陣 $A$ ，若 $A^H A=A A^H$ ，則稱 $A$ 為正規矩陣。
Note
（1）$T$ 為 $V$ 上的正規算子 $\Leftrightarrow\|T(\boldsymbol{v})\|=\left\|T^*(\boldsymbol{v})\right\|, \forall \boldsymbol{v} \in V$ ．
【證明】
【91成大應數】
考慮 $V$ 中任意向量 $\boldsymbol{v}$ ，
$$
\begin{aligned}
& \|T(\boldsymbol{v})\|=\left\|T^*(\boldsymbol{v})\right\| \Leftrightarrow\|T(\boldsymbol{v})\|^2=\left\|T^*(\boldsymbol{v})\right\|^2 \\
& \Leftrightarrow<T(\boldsymbol{v}), T(\boldsymbol{v})>=<T^*(\boldsymbol{v}), T^*(\boldsymbol{v})>\Leftrightarrow<T^*(T(\boldsymbol{v})), \boldsymbol{v}>=<T\left(T^*(\boldsymbol{v})\right), \boldsymbol{v}> \\
& \Leftrightarrow<T^*(T(\boldsymbol{v})), \boldsymbol{v}>-<T\left(T^*(\boldsymbol{v})\right), \boldsymbol{v}>=0 \Leftrightarrow<T^*(T(\boldsymbol{v}))-T\left(T^*(\boldsymbol{v})\right), \boldsymbol{v}>=0 \\
& \Leftrightarrow<\left(T^* T-T T^*\right)(\boldsymbol{v}), \boldsymbol{v}>=0 \\
& \Leftrightarrow T^* T-T T^*=O \Leftrightarrow T^* T=T T^* \Leftrightarrow T \text { 為正規算子. }
\end{aligned}
$$
（2）若 $T$ 為正規算子，則 $\forall c \in F, T-c I$ 亦為正規算子．
【證明】
$$
\begin{aligned}
(T-c I)^*(T-c I) & =\left(T^*-\bar{c} I\right)(T-c I)=T^* T-c T^*-\bar{c} T+|c|^2 I \\
& =T T^*-c T^*-\bar{c} T+|c|^2 I=(T-c I)\left(T^*-\bar{c} I\right)=(T-c I)(T-c I)^*
\end{aligned}
$$
（3）若 $\lambda$ 為正規算子 $T$ 的特徵根且 $\boldsymbol{v}$ 為其對應特徵向量，
則 $\bar{\lambda}$ 為 $T^*$ 的特徵根，且 $\boldsymbol{v}$ 為其對應的特徵向量。
【證明】
令 $\boldsymbol{v}$ 為 $T$ 相對於 $\lambda$ 的特徵向量，即 $(T-\lambda I) \boldsymbol{v}=\mathbf{0}$ ，則由（2）得 $T-\lambda I$ 為正規算子，
$$
\therefore 0=\|(T-\lambda I)(\boldsymbol{v})\|=\left\|(T-\lambda I)^*(\boldsymbol{v})\right\|=\left\|\left(T^*-\bar{\lambda} I\right)(\boldsymbol{v})\right\|=\left\|T^*(\boldsymbol{v})-\bar{\lambda} \boldsymbol{v}\right\|,
$$
$\therefore T^*(\boldsymbol{v})=\bar{\lambda} \boldsymbol{v}$ ，即 $\boldsymbol{v}$ 為 $T$ 相對於 $\bar{\lambda}$ 的特徵向量。
（4）若 $\lambda_1, \lambda_2$ 為正規算子 $T$ 的相異特徵根且 $\boldsymbol{v}_1, \boldsymbol{v}_2$ 為其對應特徵向量，則 $\boldsymbol{v}_1 \perp \boldsymbol{v}_2$ 。
【證明】

【重要】
$$
\begin{aligned}
& \lambda_1<\boldsymbol{v}_1, \boldsymbol{v}_2>=<\lambda_1 \boldsymbol{v}_1, \boldsymbol{v}_2>=<T\left(\boldsymbol{v}_1\right), \boldsymbol{v}_2>=<\boldsymbol{v}_1, T *\left(\boldsymbol{v}_2\right)>=<\boldsymbol{v}_1, \overline{\lambda_2} \boldsymbol{v}_2>=\lambda_2<\boldsymbol{v}_1, \boldsymbol{v}_2>, \\
& \therefore \lambda_1<\boldsymbol{v}_1, \boldsymbol{v}_2>-\lambda_2<\boldsymbol{v}_1, \boldsymbol{v}_2>=0, \therefore\left(\lambda_1-\lambda_2\right)<\boldsymbol{v}_1, \boldsymbol{v}_2>=0,
\end{aligned}
$$

但 $\lambda_1 \neq \lambda_2, \therefore<v_1, v_2>=0$ ，即 $v_1 \perp v_2$ ．
（5）對正規矩陣 $A$ 亦有上述各性質：
（a）$\forall \boldsymbol{x},\|A \boldsymbol{x}\|=\left\|A^H \boldsymbol{x}\right\|$ ．
（b）若 $A \boldsymbol{x}=\lambda \boldsymbol{x}, \boldsymbol{x} \neq \mathbf{0}$ ，則 $A^H \boldsymbol{x}=\bar{\lambda} \boldsymbol{x}$ 。

【95高師數學】
（c）厢異特徵根所對向量正交．
【很重要】