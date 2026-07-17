第3章函数
173

映成（onto、surjection、蓋射、滿射）
考虑函数 $f: A \rightarrow B$ ，
若對所有 $b \in B$ ，均存在 $a \in A$ 使得 $f(a)=b$ ，則皤 $f$ 為映成函数。
（亦即 $f(A)=B$ ）
【105高雄資工】

例如，

因為 $c$ 沒有被對應到，故 $f$ 不為 onto，但 $g$ 為 onto。
又例如，
$f(x)=x+1: R \rightarrow R$ 為 onto 函數，
$(\because \forall y \in R$ ，取 $x=y-1$ ，得 $f(x)=(y-1)+1=y)$
$g(x)=x^2+1: R \rightarrow R$ 不為 onto 函數，
$(\because 0 \in R$ ，但不存在 $x \in R$ ，使 $g(x)=0)$
$h(x)=x^2+1: R^{+} \rightarrow(1, \infty)$ 為 onto 函數，
$$
\left(\because h\left(R^{+}\right)=\left\{x^2+1 \mid 0<x<\infty\right\}=(1, \infty)\right)
$$

對射函數（bijection、雙射、1－1 correspondence）
若 $f$ 是 1－1 and onto，則稱 $f$ 是對射函數。
例如：
$$
\begin{aligned}
& f(x)=x+1: R \xrightarrow{1-1, \text { onto }} R ; \\
& h(x)=x^2+1: R^{+} \xrightarrow{1-1, \text { onto }}(1, \infty) .
\end{aligned}
$$