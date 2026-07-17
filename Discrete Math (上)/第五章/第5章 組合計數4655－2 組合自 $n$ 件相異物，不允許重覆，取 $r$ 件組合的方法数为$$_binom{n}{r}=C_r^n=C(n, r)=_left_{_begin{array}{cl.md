第5章 組合計數
465

5－2 組合

自 $n$ 件相異物，不允許重覆，取 $r$ 件組合的方法数为
$$
\binom{n}{r}=C_r^n=C(n, r)=\left\{\begin{array}{cl}
\frac{n!}{r!(n-r)!} & n \geq r \\
0 & n<r
\end{array} .\right.
$$

Note
當 $n$ 推廣成實數，稱之為一般化的二項式係數，定義為 $\frac{n \times(n-1) \times \ldots \times(n-r+1)}{r!}, r \in N$ 。例如 $\binom{-1 / 2}{3}=\frac{\left(\frac{-1}{2}\right) \times\left(\frac{-1}{2}-1\right) \times\left(\frac{-1}{2}-2\right)}{3 \times 2 \times 1}=\frac{-5}{16}$ 。

【102 逢甲資エ】

例題 1
A committee of 14 is to be selected from 10 men and 10 women．In how many ways can the selection be carried out if
（1）$(7 \%)$ there must be seven men and seven women？
（2）$(7 \%)$ there must be at least eight men？

【108中山資工】

解（1）從十個男生中任取七個的方法數是 $\binom{10}{7}$ ；從十個女生中任取七個的方法數是 $\binom{10}{7}$ ；故所求為 $\binom{10}{7} \times\binom{ 10}{7}$ 。
（2）從十個男生中任取八個搭配十個女生任取六個的方法數是 $\binom{10}{8} \times\binom{ 10}{6}$ ；
從十個男生中任取九個搭配十個女生任取五個的方法數是 $\binom{10}{9} \times\binom{ 10}{5}$ ；
從十個男生中任取十個搭配十個女生任取四個的方法數是 $\binom{10}{10} \times\binom{ 10}{4}$ ；
故所求為 $\binom{10}{8} \times\binom{ 10}{6}+\binom{10}{9} \times\binom{ 10}{5}+\binom{10}{10} \times\binom{ 10}{4}$ 。