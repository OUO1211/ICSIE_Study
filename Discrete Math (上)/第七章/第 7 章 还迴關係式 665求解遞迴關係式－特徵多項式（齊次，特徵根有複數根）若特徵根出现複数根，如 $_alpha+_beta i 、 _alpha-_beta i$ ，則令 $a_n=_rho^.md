第 7 章 还迴關係式 665

求解遞迴關係式－特徵多項式（齊次，特徵根有複數根）
若特徵根出现複数根，如 $\alpha+\beta i 、 \alpha-\beta i$ ，
則令 $a_n=\rho^n\left(B_1 \cos n \theta+B_2 \sin n \theta\right), ~ B_1, ~ B_2$ 為待解常数，
其中 $\rho=\sqrt{\alpha^2+\beta^2}, \cos \theta=\frac{\alpha}{\rho}, \sin \theta=\frac{\beta}{\rho}$ 。
推導方式可參考下方例題的解題過程。
例如，
若特徴根：$\alpha_1=1+\sqrt{3} i, \alpha_2=1-\sqrt{3} i$ ，
則 $\rho=\sqrt{1^2+(\sqrt{3})^2}=2, \cos \theta=\frac{1}{2}, \sin \theta=\frac{\sqrt{3}}{2}, ~ \theta=\frac{\pi}{3}$ ，
故可假設 $a_n=2^n\left(B_1 \cos \frac{n \pi}{3}+B_2 \sin \frac{n \pi}{3}\right)$ 。
例題
求解遞迴式：$\left\{\begin{array}{l}a_n=2\left(a_{n-1}-a_{n-2}\right), n \geq 2 \\ a_0=1, a_1=2\end{array}\right.$ ．
【101 政大資科】
解 特徵式：$\alpha^2-2 \alpha+2=0$ ，特徵根：$\alpha_1=1+i, \alpha_2=1-i$ ，
設 $a_n=c_1(1+i)^n+c_2(1-i)^n=(\sqrt{2})^n\left(c_1\left(\frac{1}{\sqrt{2}}+\frac{i}{\sqrt{2}}\right)^n+c_2\left(\frac{1}{\sqrt{2}}-\frac{i}{\sqrt{2}}\right)^n\right)$
$$
\begin{aligned}
& =(\sqrt{2})^n\left(c_1\left(\cos \frac{\pi}{4}+i \sin \frac{\pi}{4}\right)^n+c_2\left(\cos \frac{\pi}{4}-i \sin \frac{\pi}{4}\right)^n\right) \\
& =(\sqrt{2})^n\left(c_1\left(\cos \frac{n \pi}{4}+i \sin \frac{n \pi}{4}\right)+c_2\left(\cos \frac{n \pi}{4}-i \sin \frac{n \pi}{4}\right)\right) \\
& =(\sqrt{2})^n\left(\left(c_1+c_2\right) \cos \frac{n \pi}{4}+\left(c_1 i-c_2 i\right) \sin \frac{n \pi}{4}\right)=(\sqrt{2})^n\left(B_1 \cos \frac{n \pi}{4}+B_2 \sin \frac{n \pi}{4}\right)
\end{aligned}
$$

又由 $\left\{\begin{array}{l}a_0=1=(\sqrt{2})^0\left(B_1 \cos \frac{0 \pi}{4}+B_2 \sin \frac{0 \pi}{4}\right) \\ a_1=2=(\sqrt{2})\left(B_1 \cos \frac{\pi}{4}+B_2 \sin \frac{\pi}{4}\right)\end{array}\right.$ ，解得 $\left\{\begin{array}{l}1=B_1 \\ 2=B_1+B_2\end{array}\right.$ ，
故 $a_n=(\sqrt{2})^n\left(\cos \frac{n \pi}{4}+\sin \frac{n \pi}{4}\right), n \geq 0$ 。