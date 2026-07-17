572
離散數學（上）

題型四 遞增（increasing）
例題
（10\％）Suppose $1 \leq a<b<c<d \leq 12$ ．How many sets $\{a, b, c, d\}$ are there，where no consecutive integers（e．g．， 1 and 2,2 and 3,3 and $4, \cdots$ ）appear in $\{a, b, c, d\}$ ？

【83 成大電機】【90、104 成大資工】【99 中山電機類題】【101 台大資工】
解 定義 $y_1=a-1, y_2=b-a, y_3=c-b, y_4=d-c, y_5=12-d$ ，
則 $y_1+y_2+y_3+y_4+y_5=11$ ，且 $y_1, y_5 \geq 0, y_2, y_3, y_4 \geq 2$ ，
則此方程式之整數解個數即為所求 ：$\binom{11-2 \times 3+4}{4}$ 。

例題 10
How many times will the＂print＂statement be executed in the program segment of nested loops？ for $\mathrm{i}=1$ to 100 do
for $\mathrm{j}=1$ to i do
for $\mathrm{k}=1$ to j do
print（＂Hello！＂）
【很重要】
解 解法一：
此 program 執行 print 時，由意題知必為 $1 \leq k \leq j \leq i \leq 100$ ，
定義 $y_1=k-1, y_2=j-k, y_3=i-j, y_4=100-i$ ，
則 $y_1+y_2+y_3+y_4=99$ ，且 $y_1, y_2, y_3, y_4 \geq 0$ ，
而此方程式之整數解個數為 $\binom{99+3}{3}$ ，亦即為執行次數。
解法二：
由此 program 之 $i, j, k$ ，可得執行次數為
$$
\begin{aligned}
\sum_{i=1}^{100}\left(\sum_{j=1}^i\left(\sum_{k=1}^i 1\right)\right) & =\sum_{i=1}^{100}\left(\sum_{j=1}^i j\right)=\sum_{i=1}^{100} \frac{i(i+1)}{2}=\frac{1}{2}\left(\sum_{i=1}^{100} i^2+\sum_{i=1}^{100} i\right) \\
& =\frac{1}{2}\left(\frac{100 \cdot 101 \cdot 201}{6}+\frac{100 \cdot 101}{2}\right)=\frac{100 \cdot 101 \cdot 102}{6}=\binom{102}{3}
\end{aligned}
$$