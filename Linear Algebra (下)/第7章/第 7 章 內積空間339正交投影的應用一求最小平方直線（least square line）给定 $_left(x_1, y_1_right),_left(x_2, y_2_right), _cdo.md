第 7 章 內積空間
339

正交投影的應用一求最小平方直線（least square line）
给定 $\left(x_1, y_1\right),\left(x_2, y_2\right), \cdots,\left(x_n, y_n\right)$ 為 $R^2$ 平面上的 $n$ 個點，$\left(x_1, x_2, \ldots, x_n\right.$ 不全相同）
則可由最小平方法得一直線 $y=a+b x$ ，使此直線適合（fit）這 $n$ 個點，
即 $E=\sqrt{\sum_{i=1}^n\left(a+b x_i-y_i\right)^2}$ 為最小，
而且稱此直線為最小平方直線．
Note
（1）求最小平方直線的方法：
$$
\text { 令 } A=\left[\begin{array}{cc}
1 & x_1 \\
1 & x_2 \\
\vdots & \vdots \\
1 & x_n
\end{array}\right], \boldsymbol{x}=\left[\begin{array}{l}
a \\
b
\end{array}\right], \boldsymbol{y}=\left[\begin{array}{c}
y_1 \\
y_2 \\
\vdots \\
y_n
\end{array}\right] \text {, 得 } A \boldsymbol{x}-\boldsymbol{y}=\left[\begin{array}{c}
a+b x_1-y_1 \\
a+b x_2-y_2 \\
\vdots \\
a+b x_n-y_n
\end{array}\right] \text {, 即 } E=\|A \boldsymbol{x}-\boldsymbol{y}\| \text {, }
$$

則欲求 $a, b$ 使得 $E$ 為最小，
相當於求 $\boldsymbol{x}$ 使 $\|A \boldsymbol{x}-\boldsymbol{y}\|$ 為最小，
相當於解 $A^T A \boldsymbol{x}=A^T \boldsymbol{y}$ ，而因 $A$ 為行獨立，故 $\boldsymbol{x}=\left(A^T A\right)^{-1} A^T \boldsymbol{y}$ ，
其中，
$$
A^T A=\left[\begin{array}{cccc}
1 & 1 & \cdots & 1 \\
x_1 & x_2 & \cdots & x_n
\end{array}\right]\left[\begin{array}{cc}
1 & x_1 \\
1 & x_2 \\
\vdots & \vdots \\
1 & x_n
\end{array}\right]=\left[\begin{array}{cc}
n & \sum_{i=1}^n x_i \\
\sum_{i=1}^n x_i & \sum_{i=1}^n x_i^2
\end{array}\right], A^T \boldsymbol{y}=\left[\begin{array}{cccc}
1 & 1 & \cdots & 1 \\
x_1 & x_2 & \cdots & x_n
\end{array}\right]\left[\begin{array}{c}
y_1 \\
y_2 \\
\vdots \\
y_n
\end{array}\right]=\left[\begin{array}{c}
\sum_{i=1}^n y_i \\
\sum_{i=1}^n x_i y_i
\end{array}\right],
$$

故得 $\boldsymbol{x}=\left[\begin{array}{cc}n & \sum_{i=1}^n x_i \\ \sum_{i=1}^n x_i & \sum_{i=1}^n x_i^2\end{array}\right]^{-1}\left[\begin{array}{c}\sum_{i=1}^n y_i \\ \sum_{i=1}^n x_i y_i\end{array}\right]$ ．
【101台大電機類題、99暨南資工】
（2）有時求抛物線 $y=a+b x+c x^2$ 使最適資料，則取 $A=\left[\begin{array}{ccc}1 & x_1 & x_1^2 \\ 1 & x_2 & x_2^2 \\ \vdots & \vdots & \vdots \\ 1 & x_n & x_n^2\end{array}\right], \boldsymbol{x}=\left[\begin{array}{c}a \\ b \\ c\end{array}\right], \boldsymbol{y}=\left[\begin{array}{c}y_1 \\ y_2 \\ \vdots \\ y_n\end{array}\right]$ ，再
解正規方程即可．