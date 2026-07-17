第 5 章 組合計數 519

5－3 二項式係數

重要的二項式係數等式
（1）對稱公式：$\binom{n}{r}=\binom{n}{n-r}$ 。
（2）加法公式：$\binom{n}{r}=\binom{n-1}{r}+\binom{n-1}{r-1}$ 。

【很重要】

（3）下標總和公式：$\binom{n}{0}+\binom{n+1}{1}+\binom{n+2}{2}+\ldots+\binom{n+k}{k}=\sum_{i=0}^k\binom{n+i}{i}=\binom{n+k+1}{k}$ 。
【很重要】
（4）上標總和公式 ：$\binom{0}{k}+\binom{1}{k}+\binom{2}{k}+\ldots+\binom{n}{k}=\sum_{i=0}^n\binom{i}{k}=\binom{n+1}{k+1}$ 。
【很重要】
（5）比例公式：$\binom{n}{k}=\frac{n}{k}\binom{n-1}{k-1} ;\binom{n}{k}=\frac{n}{n-k}\binom{n-1}{k}$ 。
【證明】
（1）$\binom{n}{r}=\frac{n!}{r!(n-r)!}, ~\binom{n}{n-r}=\frac{n!}{(n-r)!(n-n+r)!}$ ，兩式相等。
亦可以組合意義說明 ：
左式即為 $n$ 相異物中不重複選出 $r$ 件方法數；
而此亦等同於 $n$ 相異物中不重複選出 $(n-r)$ 件丟掉的方法數，即右式。
（2）$\binom{n-1}{r}+\binom{n-1}{r-1}=\frac{(n-1)!}{r!(n-1-r)!}+\frac{(n-1)!}{(r-1)!(n-r)!}=\frac{(n-1)!}{r!(n-r)!}(n-r+r)=\frac{n!}{r!(n-r)!}=\binom{n}{r}$ 。
亦可以組合意義說明 ：
左式即為 $n$ 相異物中不重複選出 $r$ 件方法數；而亦可考慮如下：
（1）必取某物 $A$ ，則只需再從剩下 $n-1$ 物中取出 $r-1$ 物，方法數有 $\binom{n-1}{r-1}$ 種，
（2）必不取某物 $A$ ，則需從剩下 $n-1$ 物中取出 $r$ 物，方法數有 $\binom{n-1}{r}$ 種，故等式成立。