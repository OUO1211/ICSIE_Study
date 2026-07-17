264
線性代數（下）

科西不等式（Cauchy－Schwarz inequality）
衬任意向量 $\boldsymbol{u}, \boldsymbol{v},|<\boldsymbol{u}, \boldsymbol{v}>| \leq\|\boldsymbol{u}\| \times\|\boldsymbol{v}\|$ ．
【證明】
【102中央數學、103 雲科資工、104 中正應數】
若 $\boldsymbol{v}=\mathbf{0}$ ，明顯成立．
設 $\boldsymbol{v} \neq \boldsymbol{0}$ ，令 $c=\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\langle\boldsymbol{v}, \boldsymbol{v}\rangle}=\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|^2} \in F$ ，
則 $0 \leq\|\boldsymbol{u}-c \boldsymbol{v}\|^2=\langle\boldsymbol{u}-c \boldsymbol{v}, \boldsymbol{u}-c \boldsymbol{v}\rangle$
$$
\begin{aligned}
& =\langle\boldsymbol{u}, \boldsymbol{u}-c \boldsymbol{v}\rangle-c<\boldsymbol{v}, \boldsymbol{u}-c \boldsymbol{v}\rangle \\
& =\langle\boldsymbol{u}, \boldsymbol{u}\rangle-\bar{c}<\boldsymbol{u}, \boldsymbol{v}\rangle-c<\boldsymbol{v}, \boldsymbol{u}\rangle+c \bar{c}<\boldsymbol{v}, \mathbf{v}> \\
& =\|\boldsymbol{u}\|^2-\left(\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|^2}\right)\langle\boldsymbol{u}, \boldsymbol{v}\rangle-\left(\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|^2}\right) \overline{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}+\overline{c c}\|\boldsymbol{v}\|^2 \\
& =\|\boldsymbol{u}\|^2-\frac{|\langle\boldsymbol{u}, \boldsymbol{v}\rangle|^2}{\|\boldsymbol{v}\|^2}-\frac{|\langle\boldsymbol{u}, \boldsymbol{v}\rangle|^2}{\|\boldsymbol{v}\|^2}+\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|^2} \overline{\left(\frac{\langle\boldsymbol{u}, \boldsymbol{v}\rangle}{\|\boldsymbol{v}\|^2}\right)\|\boldsymbol{v}\|^2} \\
& =\|\boldsymbol{u}\|^2-\frac{|\langle\boldsymbol{u}, \boldsymbol{v}\rangle|^2}{\|\boldsymbol{v}\|^2}
\end{aligned}
$$

故得 $\frac{|\langle\boldsymbol{u}, \boldsymbol{v}\rangle|^2}{\|\boldsymbol{v}\|^2} \leq\|\boldsymbol{u}\|^2$ ，
$$
\begin{aligned}
& \therefore|<\boldsymbol{u}, \boldsymbol{v}>|^2 \leq\|\boldsymbol{u}\|^2\|\boldsymbol{v}\|^2, \\
& \therefore|<\boldsymbol{u}, \boldsymbol{v}>| \leq\|\boldsymbol{u}\|\|\boldsymbol{v}\| .
\end{aligned}
$$

Note
（1）在 $C^n$ 上的標準內積， $\boldsymbol{u}=\left(u_1, u_2, \ldots, u_n\right), \boldsymbol{v}=\left(v_1, v_2, \ldots, v_n\right) \in C^n$ ，則

【94 中山應數】

Cauchy－Schwarz 不等式為：$\left|\sum_{i=1}^n u_i \bar{v}_i\right| \leq\left[\sum_{i=1}^n\left|u_i\right|^2\right]^{\frac{1}{2}}\left[\sum_{i=1}^n\left|v_i\right|^2\right]^{\frac{1}{2}}$ ．
三角不等式為：$\left[\sum_{i=1}^n\left|u_i+v_i\right|^2\right]^{\frac{1}{2}} \leq\left[\sum_{i=1}^n\left|u_i\right|^2\right]^{\frac{1}{2}}+\left[\sum_{i=1}^n\left|v_i\right|^2\right]^{\frac{1}{2}}$ ．
（2）在 $V=C[a, b], F=R$ ，若定義為 $\langle f, g\rangle=\int_a^b f(x) g(x) d x$ ，則

【94中央統計】

Cauchy－Schwarz 不等式為：$\left|\int_a^b f(x) g(x) d x\right| \leq\left[\int_a^b f(x)^2 d x\right]^{\frac{1}{2}}\left[\int_a^b g(x)^2 d x\right]^{\frac{1}{2}}$ ．
三角不等式為：$\left[\int_a^b(f(x)+g(x))^2 d x\right]^{\frac{1}{2}} \leq\left[\int_a^b f(x)^2 d x\right]^{\frac{1}{2}}+\left[\int_a^b g(x)^2 d x\right]^{\frac{1}{2}}$ ．