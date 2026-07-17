第 5 章 對角化理論

155



對角化應用一解線性微分方程組

考慮缐性方程組：

$$

\left\{\begin{array}{c}

y_1^{\prime}(t)=a_{11} y_1(t)+a_{12} y_2(t)+\cdots+a_{1 n} y_n(t) \\

y_2^{\prime}(t)=a_{21} y_1(t)+a_{22} y_2(t)+\cdots+a_{2 n} y_n(t) \\

\vdots \\

y_n^{\prime}(t)=a_{n 1} y_1(t)+a_{n 2} y_2(t)+\cdots+a_{n n} y_n(t)

\end{array} \text {, 且初值條件為 } \begin{array}{r}

y_1(0)=c_1 \\

y_2(0)=c_2 \\

\vdots \\

y_n(0)=c_n

\end{array}\right. \text {, }

$$



則其解為 $\boldsymbol{y}(t)=\left[\begin{array}{c}y_1(t) \\ y_2(t) \\ \vdots \\ y_n(t)\end{array}\right]=e^{A t}\left[\begin{array}{c}c_1 \\ c_2 \\ \vdots \\ c_n\end{array}\right]$ ，其中 $A=\left[a_{i j}\right]_{n \times n}$ 為係数矩陣。

【96清大统計】



例題 10

（20\％）Solve $\frac{d \boldsymbol{u}}{d t}=\left[\begin{array}{ll}3 & 1 \\ 1 & 3\end{array}\right] \boldsymbol{u}$ ，if $\boldsymbol{u}(0)=\left[\begin{array}{l}1 \\ 0\end{array}\right]$ ，and find $e^{A t}$ ．

【96海洋資工、90清大資工類題、103．106．108．109台大工科】

解 令 $A=\left[\begin{array}{ll}3 & 1 \\ 1 & 3\end{array}\right], \boldsymbol{u}=\left[\begin{array}{l}u_1(t) \\ u_2(t)\end{array}\right], \frac{d}{d t} \boldsymbol{u}=A \boldsymbol{u}, \boldsymbol{u}(0)=\left[\begin{array}{l}1 \\ 0\end{array}\right]$ ，所以所求 $\boldsymbol{u}=e^{A t} \boldsymbol{u}(0)$ ．

因 $\operatorname{char}_A(x)=(x-4)(x-2)$ ，得特徵根 4，2，

完成對角化，取 $P=\left[\begin{array}{cc}1 & -1 \\ 1 & 1\end{array}\right]$ ，得 $P^{-1} A P=D=\left[\begin{array}{ll}4 & 0 \\ 0 & 2\end{array}\right]$ ，

則 $e^{A t}=P e^{D t} P^{-1}=\left[\begin{array}{cc}1 & -1 \\ 1 & 1\end{array}\right]\left[\begin{array}{cc}e^{4 t} & 0 \\ 0 & e^{2 t}\end{array}\right]\left[\begin{array}{cc}1 & -1 \\ 1 & 1\end{array}\right]^{-1}=\ldots=\frac{1}{2}\left[\begin{array}{ll}e^{4 t}+e^{2 t} & e^{4 t}-e^{2 t} \\ e^{4 t}-e^{2 t} & e^{4 t}+e^{2 t}\end{array}\right]$ ，

$\therefore \boldsymbol{u}=e^{A t} \boldsymbol{u}(0)=\frac{1}{2}\left[\begin{array}{ll}e^{4 t}+e^{2 t} & e^{4 t}-e^{2 t} \\ e^{4 t}-e^{2 t} & e^{4 t}+e^{2 t}\end{array}\right]\left[\begin{array}{l}1 \\ 0\end{array}\right]$ ，即 $\boldsymbol{u}=\frac{1}{2}\left[\begin{array}{c}e^{4 t}+e^{2 t} \\ e^{4 t}-e^{2 t}\end{array}\right]$ ．