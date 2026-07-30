第一章 基本概念
25
Basic Concepts

例題 1－30
$$
\mathrm{T}(\mathrm{n})=\mathrm{T}(\sqrt{\mathrm{n}})+1, \mathrm{~T}(2)=1
$$
求 $\mathrm{T}(\mathrm{n})=\mathrm{O}(?)$
解 $\mathrm{T}(\mathrm{n})=\mathrm{T}\left(\mathrm{n}^{\frac{1}{2}}\right)+1$
$$
\begin{aligned}
& =\mathrm{T}\left(\mathrm{n}^{\frac{1}{4}}\right)+1+1 \\
& =\mathrm{T}\left(\mathrm{n}^{\frac{1}{8}}\right)+1+1+1
\end{aligned}
$$
$$
\begin{aligned}
& \vdots \\
& =\mathrm{T}(2)+1+1 \cdots+1 \\
\because & \mathrm{n}^{\frac{1}{2^i}}=2 \\
\Rightarrow & \frac{1}{2^i} \cdot \log \mathrm{n}=1 \Rightarrow 2^{\mathrm{i}}=\log \mathrm{n} \Rightarrow \mathrm{i}=\log \log \mathrm{n} \\
\therefore & \mathrm{~T}(\mathrm{n})=\mathrm{O}(\log \log \mathrm{n})
\end{aligned}
$$

1－7 Master Method
$\mathrm{T}(\mathrm{n})=\mathrm{aT}\left(\frac{\mathrm{n}}{\mathrm{b}}\right)+\mathrm{f}(\mathrm{n})$ ，where $\mathrm{a} \geq 1$ and $\mathrm{b}>1$ are constants， $\mathrm{f}(\mathrm{n})$ is an asymptoticaly positive function

Theorem：Master Theorem
$$
\mathrm{T}(\mathrm{n})=\mathrm{aT}\left(\frac{\mathrm{n}}{\mathrm{~b}}\right)+\mathrm{f}(\mathrm{n})
$$

Case 1：If $\mathrm{f}(\mathrm{n})=\mathrm{O}\left(\mathrm{n}^{\log _{\mathrm{b}}{ }^{\mathrm{a}}-\varepsilon}\right)$ for some constant $\varepsilon>0$ then $T(n)=\theta\left(n^{\log _b{ }^a}\right)$

Case 2：If $\mathrm{f}(\mathrm{n})=\theta\left(\mathrm{n}^{\log _{\mathrm{b}}{ }^{\mathrm{a}}}\right)$ ，then $\mathrm{T}(\mathrm{n})=\theta\left(\mathrm{n}^{\log _{\mathrm{b}}{ }^{\mathrm{a}}} \log \mathrm{n}\right)$
Case 3：If $\mathrm{f}(\mathrm{n})=\Omega\left(\mathrm{n}^{\log _{\mathrm{b}}{ }^{\mathrm{a}}+\varepsilon}\right)$ for some constant $\varepsilon>0$ and if $\mathrm{af}\left(\frac{\mathrm{n}}{\mathrm{b}}\right) \leq \mathrm{cf}(\mathrm{n})$ ，for $\mathrm{c}<1$ and 夠大 n， then $\mathrm{T}(\mathrm{n})=\theta(\mathrm{f}(\mathrm{n}))$