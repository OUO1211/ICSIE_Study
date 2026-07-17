第 7 章 內積空間
247

7－1 內積空間

內積空間（inner product space）的定義
考虑佈於 $F$ 的向量空間 $V$ ，
若函数 $f: V \times V \rightarrow F$ 滿足
（1）$\forall \boldsymbol{u}, \boldsymbol{v}, \boldsymbol{w} \in V, \alpha, \beta \in F, f(\alpha \boldsymbol{u}+\beta \boldsymbol{v}, \boldsymbol{w})=\alpha f(\boldsymbol{u}, \boldsymbol{w})+\beta f(\boldsymbol{v}, \boldsymbol{w})$ ，

（左線性）

（2）$\forall \boldsymbol{u}, \boldsymbol{v} \in V, f(\boldsymbol{u}, \boldsymbol{v})=\overline{f(\boldsymbol{v}, \boldsymbol{u})}$ ，

（共軛交換性）

（3）$\forall \boldsymbol{v} \in V-\{\boldsymbol{0}\}, f(\boldsymbol{v}, \boldsymbol{v})>0$ ，

（正定性）

則稱 $f$ 為 $V$ 上的一種內積，並將 $f(\boldsymbol{u}, \boldsymbol{v})$ 記做 $\langle\boldsymbol{u}, \boldsymbol{v}\rangle$ ，稱 $V$ 為一種內積空間。
【97師大数學】
Note
（1）此處當 $F$ 為複數 $C$ 時，稱為複內積空間．當 $F=$ 實數 $R$ 時，稱為實內積空間．
（2）歐氏空間上常用的：標準內積（standard inner product）：
實歐氏空間：
行向量觀點：$\forall \boldsymbol{x}, \boldsymbol{y} \in R^{n \times 1}, \boldsymbol{x}=\left[\begin{array}{c}x_1 \\ x_2 \\ \vdots \\ x_n\end{array}\right], \boldsymbol{y}=\left[\begin{array}{c}y_1 \\ y_2 \\ \vdots \\ y_n\end{array}\right]$ ，
$$
<\boldsymbol{x}, \boldsymbol{y}>=\boldsymbol{y}^T \boldsymbol{x}=x_1 y_1+x_2 y_2+\cdots+x_n y_n
$$

列向量觀點：
$$
\begin{aligned}
& \forall \boldsymbol{x}, \boldsymbol{y} \in R^{1 \times n}, \boldsymbol{x}=\left[\begin{array}{llll}
x_1 & x_2 & \cdots & x_n
\end{array}\right], \boldsymbol{y}=\left[\begin{array}{llll}
y_1 & y_2 & \cdots & y_n
\end{array}\right] \\
& \langle\boldsymbol{x}, \boldsymbol{y}\rangle=\boldsymbol{x} \boldsymbol{y}^T=x_1 y_1+x_2 y_2+\cdots+x_n y_n
\end{aligned}
$$

複歐氏空間：

行向量觀點：
$$
\begin{aligned}
& \forall \boldsymbol{x}, \boldsymbol{y} \in C^{n \times 1}, \boldsymbol{x}=\left[\begin{array}{c}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{array}\right], \boldsymbol{y}=\left[\begin{array}{c}
y_1 \\
y_2 \\
\vdots \\
y_n
\end{array}\right], \\
& \langle\boldsymbol{x}, \boldsymbol{y}\rangle=\boldsymbol{y}^H \boldsymbol{x}=x_1 \overline{y_1}+x_2 \overline{y_2}+\cdots+x_n \overline{y_n} .
\end{aligned}
$$

列向量觀點：
$$
\begin{aligned}
& \forall \boldsymbol{x}, \boldsymbol{y} \in C^{1 \times n}, \boldsymbol{x}=\left[\begin{array}{llll}
x_1 & x_2 & \cdots & x_n
\end{array}\right] \mathbf{y}=\left[\begin{array}{llll}
y_1 & y_2 & \cdots & y_n
\end{array}\right], \\
& \langle\boldsymbol{x}, \boldsymbol{y}\rangle=\boldsymbol{x} \boldsymbol{y}^H=x_1 \overline{y_1}+x_2 \overline{y_2}+\cdots+x_n \overline{y_n} .
\end{aligned}
$$

例如：