32
資料結構（含精選試題）
Data Structure

解 We guess that the solution $\mathrm{T}(\mathrm{n})=\mathrm{O}(\mathrm{n} \log \mathrm{n})$
We start by assuming that this bound holds for $\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor$ that is，
$$
\begin{aligned}
\mathrm{T}\left(\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor\right) & \leq \mathrm{c}\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor \log \left\lfloor\frac{\mathrm{n}}{2}\right\rfloor \\
\Rightarrow \mathrm{T}(\mathrm{n}) & \leq 2\left(\mathrm{c}\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor \log \left\lfloor\frac{\mathrm{n}}{2}\right\rfloor\right)+\mathrm{n} \\
& \leq \mathrm{cn} \log \left(\frac{\mathrm{n}}{2}\right)+\mathrm{n} \\
& =\mathrm{cn} \log \mathrm{n}-\mathrm{cn} \log 2+\mathrm{n} \\
& =\mathrm{cn} \log \mathrm{n}-\mathrm{cn}+\mathrm{n} \\
& \leq \mathrm{cn} \log \mathrm{n}
\end{aligned}
$$

例題 1－42
$\mathrm{T}(\mathrm{n})=2 \mathrm{~T}\left(\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor+17\right)+\mathrm{n}$
解 When n is large，the difference between $\mathrm{T}\left(\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor\right)$ and
$\mathrm{T}\left(\left\lfloor\frac{\mathrm{n}}{2}\right\rfloor+17\right) \quad$ is not that large
∴ guess that $\mathrm{T}(\mathrm{n})=\mathrm{O}(\mathrm{n} \log \mathrm{n})$

Comparison of functions
Transitivity：
\begin{itemize}
\item[] － $\mathrm{f}(\mathrm{n})=\theta(\mathrm{g}(\mathrm{n}))$ and $\mathrm{g}(\mathrm{n})=\theta(\mathrm{h}(\mathrm{n}))$ imply $\mathrm{f}(\mathrm{n})=\theta(\mathrm{h}(\mathrm{n}))$
\item[] －O 與 $\Omega$ 亦同
\end{itemize}

Relfexivity：
\begin{itemize}
\item[] － $\mathrm{f}(\mathrm{n})=\theta(\mathrm{f}(\mathrm{n})), \mathrm{O} 、 \Omega$ 亦同
\end{itemize}

Symmetry：
\begin{itemize}
\item[] － $\mathrm{f}(\mathrm{n})=\theta(\mathrm{g}(\mathrm{n}))$ iff $\mathrm{g}(\mathrm{n})=\theta(\mathrm{f}(\mathrm{n}))$
\end{itemize}

Transpose symmetry
\begin{itemize}
\item[] － $\mathrm{f}(\mathrm{n})=\mathrm{O}(\mathrm{g}(\mathrm{n}))$ iff $\mathrm{g}(\mathrm{n})=\Omega(\mathrm{f}(\mathrm{n}))$
\end{itemize}