第 6 章 生成函數
631

指數生成函數的應用
例題

2

（15\％）A ship carries 48 flags， 12 each of the color red，white，blue，and black．Twelve of these flags are placed on a vertical pole in order to communicate a signal to other ship．Let $N$ be the number of the signals that contain at least three white flags or no white flags at all．Please use generating functions or exponential generating functions to compute $N$ ．In fact，$N=4^{12}+K \times 3^{11}$ ， where $K$ is an integer．Find the value of $K$ ．

【96中山資工】【100暨南資工】

解 考慮生成函數
$$
\begin{aligned}
G(x) & =\overbrace{\left(1+\frac{x^3}{3!}+\frac{x^4}{4!}+\cdots\right)}^{\text {white }} \overbrace{\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)}^{\text {red }} \overbrace{\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)}^{\text {blue }} \overbrace{\left(1+\frac{x}{1!}+\frac{x^2}{2!}+\cdots\right)}^{\text {black }} \\
& =\left(e^x-x-\frac{1}{2} x^2\right)\left(e^x\right)^3=e^{4 x}-x e^{3 x}-\frac{1}{2} x^2 e^{3 x} \\
& =\sum_{i=0}^{\infty} \frac{(4 x)^i}{i!}-\sum_{j=0}^{\infty} \frac{(3 x)^j x}{j!}-\frac{1}{2} \sum_{k=0}^{\infty} \frac{(3 x)^k x^2}{k!}
\end{aligned}
$$

取 $i=12, j=11, k=10$ ，得 $x^{12}$ 係數為 $\frac{4^{12}}{12!}-\frac{3^{11}}{11!}-\frac{1}{2} \cdot \frac{3^{10}}{10!}$ ，
故 $\frac{x^{12}}{12!}$ 係數為 $4^{12}-12 \times 3^{11}-\frac{1}{2} \times 12 \times 11 \times 3^{10}=4^{12}+3^{11} \times(-12-22)$ ，
得 $K=-34$ 。