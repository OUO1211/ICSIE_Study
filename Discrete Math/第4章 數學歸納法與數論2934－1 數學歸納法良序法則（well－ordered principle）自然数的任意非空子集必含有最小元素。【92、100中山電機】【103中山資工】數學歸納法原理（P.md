第4章 數學歸納法與數論
293

4－1 數學歸納法

良序法則（well－ordered principle）
自然数的任意非空子集必含有最小元素。
【92、100中山電機】【103中山資工】

數學歸納法原理（Principle of Mathematical Induction）
令 $P(n)$ 為定義於集合 $T=\left\{n_0, n_1, \ldots\right\} \subseteq N$ 的命題，
假設 $P(n)$ 有下列兩個性質：
（1）$P\left(n_0\right)$ 為真。
即歸纳基底（basis step）
（2）對任何 $k \in T$ ，若 $P(k)$ 為真，則 $P(k+1)$ 為真。則 $P(n)$ 為真，對任何 $n \in T$ 。

即㑴纳步骤（inductive step）。
【91 交大資科】【103 中山資工】

【證明】
反之，設存在有命題 $P(n)$ 滿足（1）、（2），但卻非永真，
令 $S=\{t \mid P(t):$ False $\}$ ，則 $S \neq \varnothing$ 且 $S \subseteq N$ ，
由良序法則知 $S$ 必存在有最小元素，令為 $m$ ，
即 $P\left(n_0\right), \ldots, P(m-1)$ 均 True，但 $P(m)$ False，
則此與 $P(n)$ 滿足（1）、（2）矛盾，故不存在反例。
Note
（1）歸納法需在良序集之下實施。
（2）＂若 $P(k)$ 為真＂稱為歸納假設（inductive hypothesis）。
（3）若所用歸納步驟為：＂若 $P\left(n_0\right), \ldots, P(k)$ 為真，則 $P(k+1)$ 為真＂，
則稱為＂強數學歸納法（strong form）＂或＂完全歸納法＂。

【103 中山資工】【108 成大工科】