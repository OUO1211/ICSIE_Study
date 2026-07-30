318
資料結構（含精選試題）
Data Structure

是最小就是最大的數字，因為每次的 Partition 分成 $\mathrm{n}-1$ 與 0 ，故：
$$
n+(n-1)+(n-2)+\cdots+1=(n(n-1)) / 2 \rightarrow 0\left(n^2\right)
$$
亦即 $\mathrm{T}(\mathrm{n}) \leq \mathrm{cn}+\mathrm{T}(\mathrm{n}-1)$
$$
\begin{aligned}
& \leq \mathrm{cn}+\mathrm{T}(\mathrm{cn}+\mathrm{T}(\mathrm{n}-2) \\
& \leq 2 \mathrm{cn}+\mathrm{T}(\mathrm{n}-2) \\
& \leq 3 \mathrm{cn}+\mathrm{T}(\mathrm{n}-3)
\end{aligned}
$$
$$
\begin{aligned}
& : \\
& : \\
\leq & (\mathrm{n}-1) \mathrm{cn}+\mathrm{T}(1) \\
= & 0\left(\mathrm{n}^2\right)
\end{aligned}
$$

3．Average Case 下，Time Complexity 為 o（n log n）
$$
\begin{aligned}
\mathrm{T}(\mathrm{n}) & =\underset{1 \leq \mathrm{s} \leq \mathrm{n}}{\operatorname{AVE}}(\mathrm{~T}(\mathrm{~s})+\mathrm{T}(\mathrm{n}-\mathrm{s}))+\mathrm{cn} \\
& =1 / \mathrm{n} \sum_{\mathrm{s}=1}^{\mathrm{n}}(\mathrm{~T}(\mathrm{~s})+\mathrm{T}(\mathrm{n}-\mathrm{s}))+\mathrm{cn}
\end{aligned}
$$
故 $\mathrm{T}(\mathrm{n})=1 / \mathrm{n}(\mathrm{T}(1)+\mathrm{T}(\mathrm{n}-1)+\mathrm{T}(2)+\mathrm{T}(\mathrm{n}-2)+\cdots+\mathrm{T}(\mathrm{n})+\mathrm{T}(0))+\mathrm{cn}$
$$
\begin{equation*}
=1 / \mathrm{n}(2 \mathrm{~T}(1)+2 \mathrm{~T}(2)+\cdots+2 \mathrm{~T}(\mathrm{n}-1)+\mathrm{T}(\mathrm{n}))+\mathrm{cn} \tag{1}
\end{equation*}
$$
$\rightarrow(\mathrm{n}-1) \mathrm{T}(\mathrm{n})=2 \mathrm{~T}(1)+2 \mathrm{~T}(2)+\cdots+2 \mathrm{~T}(\mathrm{n}-1)+\mathrm{cn}^2$
（P．S． $\mathrm{T}(\mathrm{n}-1)=0$ ）
將 $\mathrm{n}=\mathrm{n}-1$ 代入②
$$
\begin{equation*}
\rightarrow(\mathrm{n}-2) \mathrm{T}(\mathrm{n})=2 \mathrm{~T}(1)+2 \mathrm{~T}(2)+\cdots+2 \mathrm{~T}(\mathrm{n}-2)+\mathrm{c}(\mathrm{n}-1)^2 \tag{2}
\end{equation*}
$$
（1）－（2）
$$
\begin{aligned}
& (n-1) T(n)-(n-2) T(n-1)=2 T(n-1)+c(2 n-1) \\
& (n-1) T(n)-n T(n-1)=c(2 n-1)
\end{aligned}
$$
$\frac{\mathrm{T}(\mathrm{n})}{\mathrm{n}}=\frac{\mathrm{T}(\mathrm{n}-1)}{\mathrm{n}-1}+\mathrm{c}\left(1 / \mathrm{n}+\frac{1}{\mathrm{n}-1}\right)$ ，如此可遞迴得到 ：
$$
\begin{array}{ccc}
\frac{T(n-1)}{n-1}= & \frac{T(n-2)}{n-2}+c\left(\frac{1}{n-1}+\frac{1}{n-1}\right) \\
\vdots & \vdots & \vdots
\end{array}
$$
$\frac{\mathrm{T}(2)}{2}=\frac{\mathrm{T}(1)}{1}+\mathrm{c}(1 / 2+1 / 1)$
假設 $\mathrm{H}_{\mathrm{n}}=\frac{1}{\mathrm{n}}+\frac{1}{\mathrm{n}-1}+\frac{1}{\mathrm{n}-2}+\cdots+1 / 2+1$ ，故