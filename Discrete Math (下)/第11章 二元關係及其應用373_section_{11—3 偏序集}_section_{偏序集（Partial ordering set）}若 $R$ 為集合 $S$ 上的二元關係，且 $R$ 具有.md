第11章 二元關係及其應用
373

\section*{11—3 偏序集}

\section*{偏序集（Partial ordering set）}

若 $R$ 為集合 $S$ 上的二元關係，且 $R$ 具有反身性，反對稱性及遞移性，則稱 $R$ 為集合 $S$ 上的一種偏序關係，且稱 $(S, R)$ 為一偏序集，一般記為 $(S, \leq)$ 。

【104中山資工】
Note
常見的偏序集：
\begin{itemize}
\item[（1）] $(Z, \geq)$ ，另外，$(N, \geq),(Z, \leq),(N, \leq)$ 也都是。
【98、99中興資科】【108 成大工科】【證明】
反身性：$\because \forall a \in Z, a \geq a$ 。
反對稱性：若 $a \geq b, b \geq a$ ，則有 $a=b$ 。
遞移性：若 $a \geq b, b \geq c$ ，則有 $a \geq c 。$
所以 $\geq$ 為定義在 $Z$ 上的偏序關係。
\item[（2）] $(P(A), \subseteq)$ ，其中，$P(A)$ 為給定某集合 $A$ 的幂集合。
【98中央資工】【99 台大電機】【102、108中興資科】【103 成大工科】【證明】
反身性：$\forall X \in P(A), X \subseteq X$ 。
反對稱性：若 $X \subseteq Y$ ，且 $Y \subseteq X$ ，則有 $X=Y$ 。
遞移性：若 $X \subseteq Y$ ，且 $Y \subseteq Z$ ，則有 $X \subseteq Z$ 。
所以 $\subseteq$ 為定義在 $P(A)$ 上的偏序關係。
\item[（3）] $\left(D_m, \mid\right)$ ，其中，$m \in Z^{+}, D_m=\{m$ 之所有正因數 $\}$ 。
【93中央資工】【97 中教資科】【107 高雄資工】
\end{itemize}

【證明】
反身性：$\because \forall a \in D_m, a \mid a$ 。
反對稱性：$\forall a, b \in D_m$ ，若 $a \mid b$ ，且 $b \mid a$ ，則有 $a=b$ 。
遞移性：$\forall a, b, c \in D_m$ ，若 $a \mid b$ ，且 $b \mid c$ ，則有 $a \mid c$ 。
所以 $\mid$ 為定義在 $D_m$ 上的偏序關係。

（4）$\left(Z^{+}, \mid\right)$。

【101 中興資科】【104 台南資工】