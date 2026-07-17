第 6 章 生成函數
625

6－2指數生成函數（exponential generating function）

给定数列 $a_0, a_1, a_2, \ldots$ ，
則稱函数 $a_0+a_1 x+a_2 \frac{x^2}{2!}+a_3 \frac{x^3}{3!}+\cdots=\sum_{i=0}^{\infty} a_i \frac{x^i}{i!} \quad$ 為此数列所對應的指数生成函数。
Note
常用指數生成函數：
（1）$e^x=1+\frac{x}{1!}+\frac{x^2}{2!}+\frac{x^3}{3!}+\cdots=\sum_{i=0}^{\infty} \frac{x^i}{i!}$ ．
（2）$e^{-x}=1-\frac{x}{1!}+\frac{x^2}{2!}-\frac{x^3}{3!}+\cdots=\sum_{i=0}^{\infty} \frac{(-x)^i}{i!}$ ．
（3）$\frac{e^x+e^{-x}}{2}=1+\frac{x^2}{2!}+\frac{x^4}{4!}+\cdots=\sum_{i \text { ：even }}^{\infty} \frac{x^i}{i!}$ ．
（4）$\frac{e^x-e^{-x}}{2}=\frac{x}{1!}+\frac{x^3}{3!}+\frac{x^5}{5!} \cdots=\sum_{i: \text { odd }}^{\infty} \frac{x^i}{i!}$ ．
（5）$(1+x)^n=P_0^n+P_1^n \frac{x}{1!}+P_2^n \frac{x^2}{2!}+\cdots+P_n^n \frac{x^n}{n!}$ ．