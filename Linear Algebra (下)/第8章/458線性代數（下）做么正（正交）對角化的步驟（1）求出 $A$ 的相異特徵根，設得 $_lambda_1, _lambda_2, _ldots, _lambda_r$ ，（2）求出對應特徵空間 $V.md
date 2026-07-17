458
線性代數（下）

做么正（正交）對角化的步驟
（1）求出 $A$ 的相異特徵根，設得 $\lambda_1, \lambda_2, \ldots, \lambda_r$ ，
（2）求出對應特徵空間 $V\left(\lambda_i\right)$ 的一組單範正交基底：$\beta_i, 1 \leq i \leq r$ ，
（3）則 $\beta=\beta_1 \cup \beta_2 \cup \cdots \cup \beta_r$ 亦為單範正交集，
（4）排列 $\beta$ 中的向量形成么正矩陣 $U$ 的行向量，
（5）則 $A=U^H D U$ ，其中 $D$ 為對角項為 $A$ 的所有特徵根所形成的對角矩陣。
（依照 $\beta_i$ 的順序而排列 $\lambda_i$ ）
Note
（1）作正交對角化的步驟與上述雷同．
（2）考慮 $n$ 階實對稱矩陣 $A$ ，則存在 $A$ 的特徵根 $\lambda_1, \ldots, \lambda_n$ 與對應的特徵向量所成的單範正交集 $\left\{\boldsymbol{u}_1, \ldots, \boldsymbol{u}_n\right\}$ ，使 $A$ 表達成 $A=\lambda_1 \boldsymbol{u}_1 \boldsymbol{u}_1^T+\ldots+\lambda_n \boldsymbol{u}_n \boldsymbol{u}_n^T$ ．（spectral decomposition）

例題
（6\％）Let $A=\left[\begin{array}{cc}1 & 1-i \\ 1+i & 2\end{array}\right]$ ．Find a unitary matrix $U$ to diagonalize $A$ ，i．e．，$D=U^{-1} A U$ ．Please must arrange the eigenvalues in descending order in the matrix $D$ ．

【109交大資エ】

解 $\operatorname{char}_A(x)=\left|\begin{array}{cc}1-x & 1-i \\ 1+i & 2-x\end{array}\right|=(1-x)(2-x)-2=x^2-3 x=x(x-3)$ ，得特徵根 3,0 ，
$$
\begin{aligned}
& V(3)=\operatorname{ker}(A-3 I)=\operatorname{ker}\left(\left[\begin{array}{cc}
-2 & 1-i \\
1+i & -1
\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{c}
1-i \\
2
\end{array}\right]\right\}, \\
& \left\|\left[\begin{array}{c}
1-i \\
2
\end{array}\right]\right\| \sqrt{2+4}=\sqrt{6} \\
& V(0)=\operatorname{ker}(A-0 I)=\operatorname{ker}\left(\left[\begin{array}{cc}
1 & 1-i \\
1+i & 2
\end{array}\right]\right)=\operatorname{span}\left\{\left[\begin{array}{c}
1-i \\
-1
\end{array}\right]\right\}, \\
& \left\|\left[\begin{array}{c}
1-i \\
-1
\end{array}\right]\right\| \sqrt{2+1}=\sqrt{3}
\end{aligned}
$$

故單範化後取 $U=\left[\begin{array}{cc}\frac{1-i}{\sqrt{6}} & \frac{1-i}{\sqrt{3}} \\ \frac{2}{\sqrt{6}} & \frac{-1}{\sqrt{3}}\end{array}\right]$ 為 unitary matrix，使 $U^{-1} A U=D=\left[\begin{array}{ll}3 & 0 \\ 0 & 0\end{array}\right]$ ．