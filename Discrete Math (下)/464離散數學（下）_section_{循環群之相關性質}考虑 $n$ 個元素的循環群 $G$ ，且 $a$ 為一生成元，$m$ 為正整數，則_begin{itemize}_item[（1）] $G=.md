464
離散數學（下）

\section*{循環群之相關性質}

考虑 $n$ 個元素的循環群 $G$ ，且 $a$ 為一生成元，$m$ 為正整數，則
\begin{itemize}
\item[（1）] $G=\left\{e, a, a^2, \ldots, a^{n-1}\right\}$ 。
\item[（2）] $\circ\left(a^m\right)=\frac{n}{\operatorname{gcd}(m, n)} 。$
\item[（3）] $a^m$ 為 $G$ 之一生成元 $\Leftrightarrow \operatorname{gcd}(m, n)=1$ 。
\item[（4）] $G$ 中共有 $\phi(n)$ 個生成元。
\item[（5）] 若 $G$ 為一循環群，則 $G$ 必為交換群。
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] 此可視為循環群之定義。
\item[（1）] 由循環群之定義可明顯得證。
\item[（2）] 令 $b=a^m, e$ 為 $G$ 單位元素。考慮 $H=\langle b\rangle$ ，欲證明：$|H|=\frac{n}{\operatorname{gcd}(n, m)}$ ，令 $s=\min \left\{i \mid b^i=e\right\} \quad, \therefore\left(a^m\right)^s=e \Leftrightarrow n \mid m s$ ，
令 $d=\operatorname{gcd}(m, n)$ ，則 $\operatorname{gcd}\left(\frac{m}{d}, \frac{n}{d}\right)=1$ ，
一方面，$\because s \times \frac{m / d}{n / d}=\frac{m s}{n} \in Z, \left.\therefore \frac{n}{d} \right\rvert\, s$ ；
另一方面，$b^{\frac{n}{d}}=a^{m \cdot \frac{n}{d}}=\left(a^n\right)^{\frac{m}{d}}=e$ ，而 $s$ 是最小使 $b^s=e$ 成立的數，$\therefore s \left\lvert\, \frac{n}{d}\right.$ ，故得 $s=\frac{n}{d}$ 。
\item[（3）] 直接由（2）得到。
\item[（4）] 因為小於 $n$ 且與 $n$ 互質之數的個數為 $\phi(n)$ 。
\item[（5）] let $x, y \in G$ ，then $x=a^h, y=a^k$ for some $h, k$ ， $\therefore x^* y=a^h * a^k=a^{h+k}=a^{k+h}=a^k * a^h=y^* x$ ．
\end{itemize}

Note
$\phi(n)=\{m \mid 1 \leq m<n, \operatorname{gcd}(m, n)=1\} \mid$ ：Euler＇s phi function．