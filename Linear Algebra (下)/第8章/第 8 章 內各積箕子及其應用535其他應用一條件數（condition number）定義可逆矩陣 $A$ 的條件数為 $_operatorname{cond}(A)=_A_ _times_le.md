第 8 章 內各積箕子及其應用
535

其他應用一條件數（condition number）
定義可逆矩陣 $A$ 的條件数為 $\operatorname{cond}(A)=\|A\| \times\left\|A^{-1}\right\|$ ．
Note
（1）因矩陣的長度有 1 －norm， 2 －norm，$\infty$－norm 各種定法，故對應的也有 $\operatorname{cond}_1(A)$ ， $\operatorname{cond}_2(A), \operatorname{cond}_{\infty}(A)$ 不同定法．
（2） $\operatorname{cond}_2(A)=\sqrt{\frac{\lambda_{\text {max }}\left(A^H A\right)}{\lambda_{\text {min }}\left(A^H A\right)}}$ ．
【證明】
由前頁性質可得：$\|A\|_2=\sqrt{\lambda_{\text {max }}\left(A^H A\right)}$ ，
又 $\because A^H A$ 為正定，故 $\lambda_{\min }\left(A^H A\right)>0$ ，且因 $A^T A$ 與 $A A^H$ 有相同特徴根，
$$
\begin{aligned}
& \therefore\left\|A^{-1}\right\|_2=\sqrt{\lambda_{\max }\left(\left(A^{-1}\right)^H A^{-1}\right)}=\sqrt{\lambda_{\max }\left(\left(A A^H\right)^{-1}\right)}=\frac{1}{\sqrt{\lambda_{\min }\left(A A^H\right)}}, \\
& \therefore \operatorname{cond}_2(A)=\|A\|_2\left\|A^{-1}\right\|_2=\sqrt{\lambda_{\max }\left(A^H A\right)} \cdot \frac{1}{\sqrt{\lambda_{\min }\left(A^H A\right)}} .
\end{aligned}
$$
（3）若 $A \in C^{n \times n}$ 為 Hermitian，可逆矩陣，且 $\lambda_1, \lambda_2, \cdots, \lambda_n$ 為 $A$ 的特徵根，
若 $\left|\lambda_1\right| \leq\left|\lambda_2\right| \leq \cdots \leq\left|\lambda_n\right|$ ，則 $\operatorname{cond}_2(A)=\frac{\left|\lambda_n\right|}{\left|\lambda_1\right|}$ ．
【證明】
∵ 此時 $A^H A$ 的特徵根為 $A$ 的特徵根的平方，再由（2）就可得證。
（4）事實上，任意可逆方陣 $A$ 的條件數均不少於 1 ．
而其討論主要是應用在解 $A \boldsymbol{x}=\boldsymbol{b}$ 時：
（a）當 $\operatorname{cond}(A)=1$ 時，則 $\boldsymbol{b}$ 中元素小小的改變所造成解的改變是很微小的，此時稱這樣的 $A$ 為 well－conditioned。
（b）當 $\operatorname{cond}(A)$ 越大時，則 $\boldsymbol{b}$ 中元素小小的改變所造成解的改變是很巨大的，此時稱這樣的 $A$ 為 ill－conditioned．
例如：考慮 $A=\left[\begin{array}{cc}3 & -1 \\ 2 & 1\end{array}\right]$ ，則
$A$ 的第一列和為 $|3|+|-1|=4$ ，第二列和為 $|2|+|1|=3, \therefore\|A\|_{\infty}=4$ ， $A^{-1}=\left[\begin{array}{cc}\frac{1}{5} & \frac{1}{5} \\ \frac{-2}{5} & \frac{3}{5}\end{array}\right]$ ，第一列和為 $\left|\frac{1}{5}\right|+\left|\frac{1}{5}\right|=\frac{2}{5}$ ，第二列和為 $\left|\frac{-2}{5}\right|+\left|\frac{3}{5}\right|=1, \therefore\left\|A^{-1}\right\|_{\infty}=4$ ， $\therefore \operatorname{cond}_{\infty}(A)=\|A\|_{\infty}\left\|A^{-1}\right\|_{\infty}=4 \cdot 1=4$ 。