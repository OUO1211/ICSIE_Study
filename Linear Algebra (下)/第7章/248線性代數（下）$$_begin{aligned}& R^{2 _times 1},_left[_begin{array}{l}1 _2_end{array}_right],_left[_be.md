248

線性代數（下）

$$

\begin{aligned}

& R^{2 \times 1},<\left[\begin{array}{l}

1 \\

2

\end{array}\right],\left[\begin{array}{l}

3 \\

4

\end{array}\right]>=\left[\begin{array}{ll}

3 & 4

\end{array}\right]\left[\begin{array}{l}

1 \\

2

\end{array}\right]=3 \times 1+4 \times 2=11 \\

& R^{1 \times 2},<(1,2),(3,4)>=\left[\begin{array}{ll}

1 & 2

\end{array}\right]\left[\begin{array}{l}

3 \\

4

\end{array}\right]=1 \times 3+2 \times 4=11 \\

& C^{2 \times 1},<\left[\begin{array}{c}

1+i \\

2 i

\end{array}\right],\left[\begin{array}{c}

3 i \\

4-i

\end{array}\right]>=\left[\begin{array}{ll}

-3 i & 4+i

\end{array}\right]\left[\begin{array}{c}

1+i \\

2 i

\end{array}\right]=-3 i \times(1+i)+(4+i) \times 2 i=-3 i+3+8 i-2=1+5 i \\

& C^{1 \times 2},<(1+i, i),(3,2-i)>=[1+i i]\left[\begin{array}{c}

3 \\

2+i

\end{array}\right]=3 \times(1+i)+i \times(2+i)=3+3 i+2 i-1=2+5 i

\end{aligned}

$$

（3）矩陣 $A$ 使 $\langle\boldsymbol{x}, \boldsymbol{y}\rangle=\boldsymbol{y}^H A \boldsymbol{x}$ 為內積 $\Leftrightarrow A$ 為正定矩陣．（亦即特徵根均正）

（第八章會給正定矩陣的定義）

【101．107政大應數、109政大統計】

（4）設 $A \in F^{n \times n}$ ，則 $\langle A \boldsymbol{x}, \boldsymbol{y}\rangle=\left\langle\boldsymbol{x}, A^H \boldsymbol{y}\right\rangle,\langle\boldsymbol{x}, A \boldsymbol{y}\rangle=\left\langle A^H \boldsymbol{x}, \boldsymbol{y}\right\rangle, \forall \boldsymbol{x}, \boldsymbol{y} \in F^{n \times 1}$ 。

【證明】

【97台北統計、103政大統計】

$$

\begin{aligned}

& \langle A \boldsymbol{x}, \boldsymbol{y}\rangle=\boldsymbol{y}^H A \boldsymbol{x}=\left(A^H \boldsymbol{y}\right)^H \boldsymbol{x}=\left\langle\boldsymbol{x}, A^H \boldsymbol{y}\right\rangle \\

& \langle\boldsymbol{x}, A \boldsymbol{y}\rangle=(A \boldsymbol{y})^H \boldsymbol{x}=\boldsymbol{y}^H A^H \boldsymbol{x}=\left\langle A^H \boldsymbol{x}, \boldsymbol{y}\right\rangle

\end{aligned}

$$

（5）蓮續函數空間上常用內積：設 $V=C([a, b])=\{f \mid f:[a, b] \rightarrow R$ 為連續函數 $\}$ ，

定義函數 $\langle f, g\rangle: V \times V \rightarrow R$ 為 $\langle f, g\rangle=\int_a^b f(t) g(t) d t$,

則 $<,>$ 為 $V$ 上的一內積。

【證明】

【 91 彰師數學、 92 中正資工、 103 交大應數、 105 中正應數】

$\forall \alpha, \beta \in F, f, g, h \in V$,

（a）$\langle\propto f+\beta g, h\rangle$

$$

\begin{aligned}

& =\int_a^b(\alpha f+\beta g)(t) h(t) d t=\int_a^b(\alpha f(t)+\beta g(t)) h(t) d t=\int_a^b \alpha f(t) h(t)+\beta g(t) h(t) d t \\

& =\int_a^b \alpha f(t) h(t) d t+\int_a^b \beta g(t) h(t) d t=\alpha \int_a^b f(t) h(t) d t+\beta \int_a^b g(t) h(t) d t \\

& =\alpha<f, h>+\beta<g, h>

\end{aligned}

$$

（b）$\langle f, g\rangle=\int_a^b f(t) g(t) d t=\int_a^b g(t) f(t) d t=\langle g, f\rangle=\overline{\langle g, f\rangle}$ ．

（c）for $\left.f \neq O,\langle f, f\rangle=\int_a^b[f(t)]^2 d t\right\rangle 0$（因為函數 $[f(t)]^2$ 在 $x$－軸上方）．

故 $<,>$ 為 $V$ 上的一內積．

（6）若是 $V \times V \rightarrow C$ 則需定義為 $\langle f, g\rangle=\int_a^b f(t) \overline{g(t)} d t$ ，才是 $V$ 上的一內積．



【97高師數學】