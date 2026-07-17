## 第 2 章　線性方程組與求解

$$= abcd \begin{vmatrix} a & -a^2 & \dfrac{(bc+cd+db)a}{abcd} \\ b & -b^2 & \dfrac{(cd+da+ac)b}{abcd} \\ c & -c^2 & \dfrac{(da+ab+bd)c}{abcd} \\ d & -d^2 & \dfrac{(ab+bc+ca)d}{abcd} \end{vmatrix} = abcd \begin{vmatrix} a & -a^2 & \dfrac{1}{b} & \dfrac{1}{c} & \dfrac{1}{d} \\ b & -b^2 & \dfrac{1}{a} & \dfrac{1}{c} & \dfrac{1}{d} \\ c & -c^2 & \dfrac{1}{a} & \dfrac{1}{b} & \dfrac{1}{d} \\ d & -d^2 & \dfrac{1}{a} & \dfrac{1}{b} & \dfrac{1}{c} \end{vmatrix}$$

$$= abcd \begin{vmatrix} a & -a^2 & \dfrac{1}{a} \\ b & -b^2 & \dfrac{1}{b} \\ c & -c^2 & \dfrac{1}{c} \\ d & -d^2 & \dfrac{1}{d} \end{vmatrix} \begin{vmatrix} 1 & a & a^2 & a^3 \\ 1 & b & b^2 & b^3 \\ 1 & c & c^2 & c^3 \\ 1 & d & d^2 & d^3 \end{vmatrix}$$

---

> **試題 20**
>
> Prove that $\begin{vmatrix} 1 & 1 & 1 & \cdots & 1 \\ x_1 & x_2 & x_3 & \cdots & x_n \\ x_1^2 & x_2^2 & x_3^2 & \cdots & x_n^2 \\ \vdots & \vdots & \vdots & & \vdots \\ x_1^{n-1} & x_2^{n-1} & x_3^{n-1} & \cdots & x_n^{n-1} \end{vmatrix} = \left(\sum_{j=1}^{n} x_j\right) \begin{vmatrix} 1 & x_2 & x_3 & \cdots & x_n \\ \vdots & & & & \vdots \\ x_2^{n-2} & x_3^{n-2} & \cdots & x_n^{n-2} \end{vmatrix}$ for
>
> $n \geq 2$. 【95 交大應數、101 中正數學】

**解** induction on $n$.

$n = 2$ 時，左式 $= \begin{vmatrix} 1 & 1 \\ x_1 & x_2 \end{vmatrix} = x_2 - x_1$，右式 $= (x_1 + x_2)\begin{vmatrix} 1 \end{vmatrix} = x_2 - x_1^2$，成立。

設 $n = k$ 時原命題成立，則 $n = k+1$ 時，

$$\begin{vmatrix} 1 & 1 & 1 & \cdots & 1 \\ x_1 & x_2 & x_3 & \cdots & x_{k+1} \\ \vdots & \vdots & \vdots & & \vdots \\ x_1^k & x_2^k & x_3^k & \cdots & x_{k+1}^k \end{vmatrix} \xrightarrow{c_i - c_1} \begin{vmatrix} 1 & 0 & \cdots & 0 \\ x_1 & x_2 - x_1 & \cdots & x_{k+1} - x_1 \\ \vdots & \vdots & & \vdots \\ x_1^k & x_2^k - x_1^k & \cdots & x_{k+1}^k - x_1^k \end{vmatrix}$$

$$= \begin{vmatrix} x_2 - x_1 & x_3 - x_1 & \cdots & x_{k+1} - x_1 \\ x_2^2 - x_1^2 & x_3^2 - x_1^2 & \cdots & x_{k+1}^2 - x_1^2 \\ \vdots & \vdots & & \vdots \\ x_2^k - x_1^k & x_3^k - x_1^k & \cdots & x_{k+1}^k - x_1^k \end{vmatrix}$$
