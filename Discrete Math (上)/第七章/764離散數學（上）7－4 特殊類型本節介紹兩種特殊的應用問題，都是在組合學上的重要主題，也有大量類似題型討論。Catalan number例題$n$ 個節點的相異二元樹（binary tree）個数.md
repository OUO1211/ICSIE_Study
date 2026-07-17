764
離散數學（上）

7－4 特殊類型
本節介紹兩種特殊的應用問題，都是在組合學上的重要主題，也有大量類似題型討論。
Catalan number
例題
$n$ 個節點的相異二元樹（binary tree）個数。
此處討論的是有區分左右，每個父節點頂多 2 個子節點的樹狀結構。例如，右圖為 3 個節點的相異二元樹。

解 Step 1 ．
令 $b_n$ 為所求，則扣掉 1 個點為 root，對剩下的 $n-1$ 個點：
若左邊 $k$ 點（左邊形成 $b_k$ 個樹），右邊 $n-1-k$ 點（右邊形成 $b_{n-1}$ 個樹）， $0 \leq k \leq n-1$ ，
故得 $b_n=b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0=\sum_{k=0}^{n-1} b_k b_{n-1-k}$ ，
其中，$b_0$ 定義為 1 ，且 $b_1=1$ ，代表 1 個點的退化樹。
Step 2.
以生成函數解遞迴關係式：
$$
\begin{equation*}
\sum_{n=1}^{\infty} b_n x^n=\sum_{n=1}^{\infty}\left(b_0 b_{n-1}+b_1 b_{n-2}+\ldots+b_{n-1} b_0\right) x^n \tag{*}
\end{equation*}
$$

令 $T(x)=\sum_{k=0}^{\infty} b_k x^k$ 表數列 $\left\{b_k\right\}_{k=0}^{\infty}$ 所對應的生成函數，則由 $(*)$ 可得：
$$
\begin{aligned}
& T(x)-b_0=x \sum_{n-1=0}^{\infty}\left(b_0 \cdot b_{n-1}+b_1 \cdot b_{n-2}+\ldots+b_{n-1} \cdot b_0\right) x^{n-1} \\
& =x \sum_{k=0}^{\infty}\left(b_0 \cdot b_k+b_1 \cdot b_{k-1}+\ldots+b_k \cdot b_0\right) x^k=x \cdot T^2(x) \\
& \therefore x T^2(x)-T(x)+1=0, \text { 得 } T(x)=\frac{1 \pm \sqrt{1-4 x}}{2 x}, \\
& \therefore 2 x T(x)=1 \pm(1-4 x)^{1 / 2}=1 \pm \sum_{k=0}^{\infty}\binom{1 / 2}{k}(-4 x)^k \ldots \ldots(* *)
\end{aligned}
$$