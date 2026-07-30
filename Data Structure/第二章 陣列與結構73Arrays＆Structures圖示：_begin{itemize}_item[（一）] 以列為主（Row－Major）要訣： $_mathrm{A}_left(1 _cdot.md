第二章 陣列與結構
73
Arrays＆Structures

圖示：
\begin{itemize}
\item[（一）] 以列為主（Row－Major）
要訣： $\mathrm{A}\left(1 \cdot \mu_1, 1 \cdot \mu_2, 1 \cdot \mu_3\right)$
以列為主
有 $\mu_1$ 個二維陣列（ $1 \cdots \mu_2, \cdots \mu_3$ ）
公式：$A(\mathrm{i}, \mathrm{j}, \mathrm{k})=\mathrm{L}_0+(\mathrm{i}-1) \mu_2, \mu_3 \mathrm{~d}+(\mathrm{j}-1) \mu_3 \mathrm{~d}+(\mathrm{k}-1) \mathrm{d}$
若陣列是 $\mathrm{A}\left(\mathrm{L}_1: \mu_1, \mathrm{~L}_2: \mu_2, \mathrm{~L}_3: \mu_3\right)$
則 $\mathrm{x}=\mu_1-\mathrm{L}_1+1$
$$
\begin{aligned}
& y=\mu_2-L_2+1 \\
& z=\mu_3-L_3+1
\end{aligned}
$$
$\rightarrow \quad \mathrm{A}(\mathrm{i}, \mathrm{j}, \mathrm{k})=\mathrm{L}_0+\left(\mathrm{i}-\mathrm{L}_1\right) \mathrm{yzd}+\left(\mathrm{j}-\mathrm{L}_2\right) \mathrm{zd}+\left(\mathrm{k}-\mathrm{L}_2\right) \mathrm{d}$
\item[（二）] 以行為主（Column－Major）（要訣： $\_\_\_\_$）
陣列 $\quad \mathrm{A}\left(1: \mu_1, 1: \mu_2, 1: \mu_3\right)$
$$
\rightarrow A(i, j, k)=L_0+(k-1) \mu_1 \mu_2 d+(j-1) \mu_1 d+(i-1) d
$$
陣列 $\mathrm{A}\left(\mathrm{L}_1: \mu_1, \mathrm{~L}_2: \mu_2, \mathrm{~L}_3: \mu_3\right)$
$$
\rightarrow \mathrm{A}(\mathrm{i}, \mathrm{j}, \mathrm{k})=\mathrm{L}_0+\left(\mathrm{k}-\mathrm{L}_3\right) \mathrm{xyd}+\left(\mathrm{j}-\mathrm{L}_2\right) x \mathrm{~d}+\left(\mathrm{i}-\mathrm{L}_1\right) \mathrm{d}
$$
\end{itemize}

例題 2－11
若 $\mathrm{A}(-3: 2,-2: 3,0: 4)$ 為三維陣列，且 $\mathrm{A}(-3,-2,0)=318$ 試求陣列 $\mathrm{A}(1,3,3)=$ ？ （Row－Major 且 $\mathrm{d}=1$ ）
\begin{itemize}
\item[解]
$$
\begin{aligned}
& x=6, \quad y=6, \quad z=5 \\
& A(1,3,3)=318+(4 \times 6 \times 5)+(5 \times 5)+3=466
\end{aligned}
$$
\item[（三）] N 維陣列
若以 $\mathrm{A}\left(1: \mu_1, 1: \mu_2, \cdots, 1: \mu_n\right)$ ，則表示有 $\mu_1$ 個 $\mathrm{N}-1$ 維陣列，有 $\mu_2$ 個 $\mathrm{N}-2$ 維陣列，．．．以此類推。
\end{itemize}