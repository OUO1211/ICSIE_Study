第12章 代數結構
487

整域（integral domain）
設 $(R,+, *)$ 為一具 unity 1 的交換環，且 $R$ 中不具任何零除元，則稱 $(R,+, *)$ 為一整域。
例如，
$(Z,+, *)$ 與 $\left(Z_5,+{ }_5,{ }^*{ }_5\right)$ 即為整域，但 $\left(Z_6,+{ }_6,{ }^*{ }_6\right)$ 則否。
$\left(R^{2 \times 2},+, \cdot\right)$ 中，$\because\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right] \cdot\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right]=\left[\begin{array}{ll}0 & 0 \\ 0 & 0\end{array}\right], \therefore\left[\begin{array}{ll}0 & 0 \\ 1 & 0\end{array}\right]$ 為一零除元，故 $\left(R^{2 \times 2},+, \cdot\right)$ 不為整域。

Note
\begin{itemize}
\item[（1）] 在 $Z_n$ 中，$\forall a \in Z_n, a \neq 0, a$ 為零除元 $\Leftrightarrow \operatorname{gcd}(a, n) \neq 1$ ．
【證明】
⇒ 設 $a$ 為零除元，則 $\exists b \neq 0, ~ a b \equiv 0(\bmod n) \therefore n \mid a b$ ．
若 $\operatorname{gcd}(a, n)=1$ ，則 $n \mid b$ 即 $b \equiv 0(\bmod n) \ldots \ldots$ 矛盾
⇐ 設 $\operatorname{gcd}(a, n)=d>1, \therefore a \frac{n}{d}=n \frac{a}{d} \equiv 0(\bmod n)$ ，
但 $a \neq 0, \frac{n}{d} \neq 0$ ，所以得 $a$ 為零除元……矛盾
所以得 $p$ 為質數 $\Leftrightarrow Z_p$ 為整域。
\item[（2）] 由前頁 Note－（2）知整域中非零元素具有乘法消去性。
\end{itemize}