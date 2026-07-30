306
資料結構（含精選試題）

Data Structure

（ $\mathrm{F}_{\mathrm{a}-1}$ ）減1。
\begin{itemize}
\item[（2）] 若 $\mathrm{k}=\mathrm{f}\left[\mathrm{F}_{\mathrm{a}-1}\right]$ ．key
則表示成功找到所要的記錄。
\end{itemize}
（3）若 $\mathrm{k}>\mathrm{f}\left[\mathrm{F}_{\mathrm{a}-1}\right]$ ．key
那搜尋的範圍縮減成從 $\mathrm{F}_{\mathrm{a}-1}+1$ 到 $\mathrm{F}_{\mathrm{a}}-1$ 記錄，而此剩餘之記錄個數為：
$$
F_a-1-\left(F_{a-1}+1\right)+1=F_a-F_{a-1}-1=F_{a-2}-1
$$
仍然是某一個費氏數（ $\mathrm{F}_{\mathrm{a}-2}$ ）減1。
描述費氏搜尋法的決策樹過程（如下圖），例：$n=33$ 之費氏搜尋二元樹。
algorithm：
Procedure fibsrch（g ：afile；var i ：integer；n，k ：integer）
｛Search a file，g，stored in nondecressing order by field key for a record i such that fi［i］．key＝k．Assume that $\mathrm{F}_{\mathrm{a}}+\mathrm{m}=\mathrm{n}+1, \mathrm{~m} \geq 0$ and $\mathrm{F}_{\mathrm{a}-1}>\mathrm{n}+1 . \mathrm{n}$ is the number of records in g． $\mathrm{F}_{\mathrm{a}}$ and $\mathrm{F}_{\mathrm{a}-1}$ are consecutive fibonacci numbers．If k is not present i is set to 0．\}
Var done ：boolean；
p, q, t, a : integer;
Begin
$$
\begin{aligned}
& \left.\mathrm{a}:=\text { fibindex }(\mathrm{n}+1) ; \text { \{Returns larges integer } \mathrm{a}: \mathrm{F}_{\mathrm{a}} \leq \mathrm{n}+1\right\} \\
& \mathrm{i}:=\text { fib }(\mathrm{a}-1) ; \quad\{\text { Returns the a-1st fibonacci number }\} \\
& \mathrm{p}:=\mathrm{fib}(\mathrm{a}-2) ; \\
& \mathrm{q}:=\mathrm{fib}(\mathrm{a}-3) ;
\end{aligned}
$$