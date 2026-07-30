74
資料結構（含精選試題）
■■

Data Structure
若 $\mathrm{A}(1,1, \cdots, 1)$ 的位址是 $\mathrm{L}_0$ ，則以 Row－Major 來看：
$\mathrm{A}\left(\mathrm{i}_1, 1, \cdots, 1\right)$ 的位址是 $\mathrm{L}_0+\left(\mathrm{i}_1-1\right) \mu_2 \mu_3 \cdots \mu_{\mathrm{n}},(\mathrm{d}=1)$
$\mathrm{A}\left(\mathrm{i}_1, \mathrm{i}_2, \cdots, 1\right)$ 的位址是 $\mathrm{L}_0+\left(\mathrm{i}_1-1\right) \mu_2 \mu_3 \cdots \mu_{\mathrm{n}}+$
$$
\left(i_2-1\right) \mu_3 \mu_4 \cdots \mu_n
$$
$$
\begin{gathered}
\vdots \\
\vdots
\end{gathered}
$$
$\therefore \mathrm{A}\left(\mathrm{i}_1, \mathrm{i}_2, \cdots, \mathrm{i}_{\mathrm{n}}\right)$ 的位址是：
$$
L_0+\left(i_1-1\right) \mu_2 \mu_3 \cdots \mu_n+\left(i_2-1\right) \mu_3 \mu_4 \cdots \mu_n+\cdots+\left(i_{n-1}-1\right) \mu_n+\left(i_n-1\right)
$$
$\rightarrow=\mathrm{L}_0+\sum_{\mathrm{j}=1}^{\mathrm{n}}\left(\mathrm{i}_1-1\right) \mathrm{a}_{\mathrm{j}}$ ，其中
$$
\left[\begin{array}{l}
a_j=\prod_{k=j+1}^n U_k, \quad 1 \leq j \leq n \\
a_n=1
\end{array}\right.
$$
若以Column－major來看，視為有 $\mu_{\mathrm{n}}$ 個 $\mathrm{N}-1$ 維陣列，有 $\mu_{\mathrm{n}-1}$ 個 $\mathrm{N}-2$ 維陣列 ⋯，（ $\mathrm{d}=1$ ）若 $\mathrm{A}(1,1,1, \cdots, 1)=\mathrm{L}_0$
則 $\mathrm{A}\left(1,1, \cdots, \mathrm{i}_{\mathrm{n}}\right)=\mathrm{L}_0+\left(\mathrm{i}_{\mathrm{n}}-1\right) \mu_1 \mu_2 \cdots \mu_{\mathrm{n}-1}$
$$
\begin{aligned}
A\left(1,1, \cdots, i_{n-1}, i_n\right)=L_0+ & \left(i_n-1\right) \mu_1 \mu_2 \cdots \mu_{n-1} \\
& \left(i_{n-1}-1\right) \mu_1 \mu_2 \cdots \mu_{n-2}
\end{aligned}
$$
$$
\begin{aligned}
& \vdots \\
& \vdots
\end{aligned}
$$
$$
\begin{aligned}
& \therefore \quad A\left(i_1, i_2, \cdots, i_n\right)=L_0+\left(i_n-1\right) \mu_1 \mu_2 \cdots \mu_{n-1} \\
&+\left(i_{n-1}-1\right) \mu_1 \mu_2 \cdots \mu_{n-2} \\
& \vdots \\
&+\left(i_2-1\right) \mu_1+\left(i_1-1\right)
\end{aligned}
$$
$$
\begin{aligned}
\rightarrow & =L_0+\sum_{j=1}^n\left(i_j-1\right) a_j \\
& {\left[\begin{array}{l}
a_j=\prod_{k=1}^{j-1} U_k, \quad 2 \leq j \leq n \\
a_j=1, \text { if } j=1
\end{array}\right.}
\end{aligned}
$$