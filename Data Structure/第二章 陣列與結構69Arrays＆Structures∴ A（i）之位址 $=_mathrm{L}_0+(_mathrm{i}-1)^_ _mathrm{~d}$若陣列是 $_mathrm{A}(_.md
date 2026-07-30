第二章 陣列與結構
69
Arrays＆Structures

∴ A（i）之位址 $=\mathrm{L}_0+(\mathrm{i}-1)^* \mathrm{~d}$
若陣列是 $\mathrm{A}(\mathrm{L}: \mu) \rightarrow \mathrm{A}(\mathrm{i})=\mathrm{L}_0+(\mathrm{i}-\mathrm{L})^* \mathrm{~d}$

\section*{例題 2－1}

假設一維陣列 A（1：1000），每元素大小為4units，若 A（1）之位址為100則A（900）之位址為何？

解
$$
\begin{aligned}
\mathrm{A}(900) & =\mathrm{A}(1)+(900-1) \times 4 \\
& =100+899 \times 4=100+3596=3696
\end{aligned}
$$

\section*{二．二維陣列}

二維陣列採用 Row－Major 或 Column－Major 方式，將資料循序存到一維的連續記憶體中。
（一）Row－Major 方式
假設陣列是A（1：$\mu_1$ ，1：$\mu_2$ ），有 $\mu_1$ 個 Row，$\mu_2$ 個 Column 每個元素佔 d 個空間，$\mathrm{L}_0$ 是起始位址。
則 $A(\mathrm{i}, \mathrm{j})=\mathrm{L}_0+(\mathrm{i}-1) \mu_2 \mathrm{~d}+(\mathrm{j}-1) \mathrm{d}$
若 陣列是 $\mathrm{A}\left(\mathrm{L}_1: \mu_1, \mathrm{~L}_2: \mu_2\right)$ ，則有 m 列n行
其中 $\left\{\begin{array}{l}\mathrm{m}=\mu_1-\mathrm{L}_1+1 \\ \mathrm{n}=\mu_2-\mathrm{L}_2+1\end{array}\right.$
則 $A(\mathrm{i}, \mathrm{j})=\mathrm{L}_0+\left(\mathrm{i}-\mathrm{L}_1\right) \cdot \mathrm{nd}+\left(\mathrm{j}-\mathrm{L}_2\right) \cdot \mathrm{d}$
（二）Column－Major 方式
若陣列是 $\mathrm{A}\left(1: \mu_1, 1: \mu_2\right)$
則 $\quad A(\mathrm{i}, \mathrm{j})=\mathrm{L}_0+(\mathrm{j}-1) \mu_1 \mathrm{~d}+(\mathrm{i}-1) \mathrm{d}$
若陣列是 $\mathrm{A}\left(\mathrm{L}_1: \mu_1, \mathrm{~L}_2: \mu_2\right)$
則 $\mathrm{A}(\mathrm{i}, \mathrm{j})=\mathrm{L}_0+\left(\mathrm{j}-\mathrm{L}_2\right) \cdot \mathrm{md}+\left(\mathrm{i}-\mathrm{L}_1\right) \cdot \mathrm{d}$
（三）二維陣列的4種考試題型
【題型一】給予所有已知量，求 A［i，j］之 Location

\section*{例題 2－2}

有一陣列 $\mathrm{A}(-4: 3,-3: 2)$ ，其 $\mathrm{A}(-4,-3)=100$（起始位址），则 $\mathrm{A}(1,1)$ 所佔位址為？（假设 $\mathrm{d}=1$ ）（Row－Major）