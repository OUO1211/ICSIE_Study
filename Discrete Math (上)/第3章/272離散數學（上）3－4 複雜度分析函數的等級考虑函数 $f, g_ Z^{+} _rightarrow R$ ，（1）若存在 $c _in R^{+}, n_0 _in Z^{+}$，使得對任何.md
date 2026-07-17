272

離散數學（上）



3－4 複雜度分析



函數的等級

考虑函数 $f, g: Z^{+} \rightarrow R$ ，

（1）若存在 $c \in R^{+}, n_0 \in Z^{+}$，使得對任何 $n \geq n_0$ ，均有 $|f(n)| \leq c|g(n)|$ ，則稱 $f(n)=O(g(n))$ 。

（2）若存在 $c \in R^{+}, n_0 \in Z^{+}$，使得對任何 $n \geq n_0$ ，均有 $|f(n)| \geq c|g(n)|$ ，則稱 $f(n)=\Omega(g(n)) 。$

（3）若存在 $c_1, c_2 \in R^{+}, n_0 \in Z^{+}$，使得對任何 $n \geq n_0$ ，均有 $c_1|g(n)| \leq|f(n)| \leq c_2|g(n)|$ ，則稱 $f(n)=\Theta(g(n))$ 。



【99清大資應】



Note

（1）有些書上是以＂$\in$＂代替＂$=$＂。

（2）由定義可知

$$

f(n)=O(g(n)) \Leftrightarrow g(n)=\Omega(f(n))

$$

（3）由定義可知

$$

f(n)=\Omega(g(n)) \Leftrightarrow g(n)=O(f(n)) 。

$$

（4）由定義可知

$$

f(n)=\Theta(g(n)) \Leftrightarrow\left\{\begin{array}{l}

f(n)=O(g(n)) \\

f(n)=\Omega(g(n))

\end{array}\right.

$$

（5）以極限來看複雜度：

（1）若 $\lim _{n \rightarrow \infty} \frac{f(n)}{g(n)}=0$ ，則 $f(n)=O(g(n))$ 。

（2）若 $\lim _{n \rightarrow \infty} \frac{f(n)}{g(n)}=\infty$ ，則 $f(n)=\Omega(g(n))$ 。

（3）若 $\lim _{n \rightarrow \infty} \frac{f(n)}{g(n)}=$ 正實數，則 $f(n)=\Theta(g(n))$ 。

（6）常見級別：$O(1)<O(\log n)<O(n)<O(n \log n)<O\left(n^2\right)<O\left(2^n\right)<O(n!)$ ．

（7）對數函數的各種常見底數： $\log _2 n=\lg n ; \log _e n=\ln n ; \log _{10} n=\log n$ 。

（8）若 $f(n)$ 為 $k$ 次多項式，則 $f(n)=\Theta\left(n^k\right)$ 。

（9）若 $f_1=O\left(g_1\right), f_2=O\left(g_2\right)$ ，則 $f_1+f_2=O\left(\max \left(g_1, g_2\right)\right)$ 。

（10）求函數之複雑度常用技巧：由直觀看法、已知、求極限、依定義證明。