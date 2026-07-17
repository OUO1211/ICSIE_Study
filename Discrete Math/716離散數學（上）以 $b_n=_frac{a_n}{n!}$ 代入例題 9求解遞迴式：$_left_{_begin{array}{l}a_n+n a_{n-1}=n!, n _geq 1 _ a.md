716
離散數學（上）

以 $b_n=\frac{a_n}{n!}$ 代入

例題 9
求解遞迴式：$\left\{\begin{array}{l}a_n+n a_{n-1}=n!, n \geq 1 \\ a_0=1,\end{array}\right.$ 。【 81 、 86 成大資エ】【 101 資訊技師】

解 原式等於：$\frac{a_n}{n!}+\frac{a_{n-1}}{(n-1)!}=1$ ，
令 $b_n=\frac{a_n}{n!}$ 代入原式，得 $\left\{\begin{array}{l}b_n+b_{n-1}=1 \\ b_0=1\end{array}\right.$ ，可由特徴式解得 $b_n=\frac{(-1)^n+1}{2}$ ，
還原得 $a_n=\frac{n!\left((-1)^n+1\right)}{2}, n \geq 0$ ．