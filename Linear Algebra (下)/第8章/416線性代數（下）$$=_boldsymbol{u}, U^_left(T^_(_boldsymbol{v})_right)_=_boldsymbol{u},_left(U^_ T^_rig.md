416
線性代數（下）
$$
=<\boldsymbol{u}, U^*\left(T^*(\boldsymbol{v})\right)>=<\boldsymbol{u},\left(U^* T^*\right)(\boldsymbol{v})>,
$$

故 $(T U)^*(\boldsymbol{v})=\left(U^* T^*\right)(\boldsymbol{v}), \forall \boldsymbol{v} \in V$ ，即 $(T U)^*=U^* T^*$ ．
（6）$\left\langle\boldsymbol{u}, I^*(\boldsymbol{v})\right\rangle=\langle I(\boldsymbol{u}), \boldsymbol{v}\rangle=\langle\boldsymbol{u}, \boldsymbol{v}\rangle=\langle\boldsymbol{u}, I(\boldsymbol{v})\rangle$ ，故 $(I)^*(\boldsymbol{v})=I(\boldsymbol{v}), \forall \boldsymbol{v} \in V$ ，即 $(I)^*=I$ 。
（7）$\because T$ 可逆，故 $T^{-1}$ ，故 $\left(T^{-1}\right)^*$ 亦必存在，
又 $\left(T^{-1}\right)^* T^*=\left(T T^{-1}\right)^*=I^*=I, T^*\left(T^{-1}\right)^*=\left(T^{-1} T\right)^*=I^*=I$ ，故 $\left(T^*\right)^{-1}=\left(T^{-1}\right)^*$ ．
（8）令 $A=[T]_\beta, B=\left[T^*\right]_\beta, \because \beta=\left\{\boldsymbol{v}_1, \ldots, \boldsymbol{v}_n\right\}$ 為 $V$ 的單範正交基底，
$$
\therefore T\left(\boldsymbol{v}_j\right)=\sum_{i=1}^n<T\left(\boldsymbol{v}_j\right), \boldsymbol{v}_i>\boldsymbol{v}_i, \therefore\left[T\left(\boldsymbol{v}_j\right)\right]_\beta=\left[\begin{array}{c}
<T\left(\boldsymbol{v}_j\right), \boldsymbol{v}_1> \\
<T\left(\boldsymbol{v}_j\right), \boldsymbol{v}_2> \\
\vdots \\
<T\left(\boldsymbol{v}_j\right), \boldsymbol{v}_n>
\end{array}\right] \text {, }
$$

所以 $A=\left[\begin{array}{cccc}<T\left(\boldsymbol{v}_1\right), \boldsymbol{v}_1> & <T\left(\boldsymbol{v}_2\right), \boldsymbol{v}_1> & \cdots & <T\left(\boldsymbol{v}_n\right), \boldsymbol{v}_1> \\ <T\left(\boldsymbol{v}_1\right), \boldsymbol{v}_2> & <T\left(\boldsymbol{v}_2\right), \boldsymbol{v}_2> & \cdots & <T\left(\boldsymbol{v}_n\right), \boldsymbol{v}_2> \\ \vdots & \vdots & \ddots & \vdots \\ <T\left(\boldsymbol{v}_1\right), \boldsymbol{v}_n> & <T\left(\boldsymbol{v}_2\right), \boldsymbol{v}_n> & \cdots & <T\left(\boldsymbol{v}_n\right), \boldsymbol{v}_n>\end{array}\right]$ ，
同理可得 $B=\left[\begin{array}{cccc}<T^*\left(\boldsymbol{v}_1\right), \boldsymbol{v}_1> & <T^*\left(\boldsymbol{v}_2\right), \boldsymbol{v}_1> & \cdots & <T^*\left(\boldsymbol{v}_n\right), \boldsymbol{v}_1> \\ <T^*\left(\boldsymbol{v}_1\right), \boldsymbol{v}_2> & <T^*\left(\boldsymbol{v}_2\right), \boldsymbol{v}_2> & \cdots & <T^*\left(\boldsymbol{v}_n\right), \boldsymbol{v}_2> \\ \vdots & \vdots & \ddots & \vdots \\ <T^*\left(\boldsymbol{v}_1\right), \boldsymbol{v}_n> & <T^*\left(\boldsymbol{v}_2\right), \boldsymbol{v}_n> & \cdots & <T^*\left(\boldsymbol{v}_n\right), \boldsymbol{v}_n>\end{array}\right]$ ，
而 $(B)_{i j}=\left\langle T^*\left(\boldsymbol{v}_j\right), \boldsymbol{v}_i\right\rangle=\overline{\left\langle\boldsymbol{v}_i, T^*\left(\boldsymbol{v}_j\right)\right\rangle}=\overline{\left\langle T\left(\boldsymbol{v}_i\right), \boldsymbol{v}_j\right\rangle}=\overline{(A)_{j i}}=\left(A^H\right)_{i j}, \therefore B=A^H$ ．
（9）設 $\beta=\left\{\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n\right\}$ 為 $V$ 的一組單範正交基底，
令 $[T]_\beta=A$ ，則 $\left[T^*\right]_\beta=A^H$ ，若 $\lambda$ 為 $T$ 的特徵根，
則 $\operatorname{det}(A-\lambda I)=0$ ，
$$
\begin{aligned}
& \therefore \operatorname{det}\left((A-\lambda I)^H\right)=0, \\
& \therefore \operatorname{det}\left(A^H-\bar{\lambda} I\right)=0,
\end{aligned}
$$
$\therefore \bar{\lambda}$ 為 $T^*$ 的特徵根．