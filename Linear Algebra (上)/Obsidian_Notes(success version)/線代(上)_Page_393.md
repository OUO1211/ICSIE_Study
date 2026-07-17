## 秩的重要性質

令 $A$ 為 $m \times n$ 的矩陣，則

> **定理**
>
> (1) $\operatorname{rank}(A)=\operatorname{rank}(A^T)$。 【102 交大資工、108 成大統計、108 台大資工、110 政大統計】
>
> (2) $\operatorname{rank}(A)\leq \min\{m,n\}$。 【100 台大電信】
>
> (3) 列運算與行運算都不改變 rank.
>
> （甲若 $A \overset{r}{\sim} B$ 或 $A \overset{c}{\sim} B$，則 $\operatorname{rank}(A)=\operatorname{rank}(B)$。）
>
> (4) $\operatorname{rank}(AB)\leq \min\{\operatorname{rank}(A),\operatorname{rank}(B)\}$。 【97 勤益數學】 【很重要】
>
> (5) 若方陣 $P,Q$ 均可逆，則
>
> (i) $\operatorname{rank}(PA)=\operatorname{rank}(A)$。  (ii) $\operatorname{rank}(AQ)=\operatorname{rank}(A)$。 【101 台大數學】 【重要】
>
> (6) $\operatorname{rank}(A+B)\leq \operatorname{rank}(A)+\operatorname{rank}(B)$。 【重要】
>
> (7) $|\operatorname{rank}(A)-\operatorname{rank}(B)|\leq \operatorname{rank}(A+B)$。

> **【證明】**
>
> (1) $\because\ RS(A)=CS(A^T)$，$\therefore\ \dim(RS(A))=\dim(CS(A^T))$，$\therefore\ \operatorname{rank}(A)=\operatorname{rank}(A^T)$。
>
> (2) $\because\ CS(A)=\{Ax\mid x\in F^{n\times 1}\}\subseteq F^{m\times 1}$，$\therefore\ \dim(CS(A))\leq m$，
>
> $\because\ RS(A)=\{xA\mid x\in F^{1\times m}\}\subseteq F^{1\times n}$，$\therefore\ \dim(RS(A))\leq n$，
>
> 故得 $\operatorname{rank}(A)\leq \min\{m,n\}$。
>
> (3) 若 $A \overset{r}{\sim} B$，則 $RS(A)=RS(B)$，故 $\operatorname{rank}(A)=\operatorname{rank}(B)$。
>
> 若 $A \overset{c}{\sim} B$，則 $CS(A)=CS(B)$，故 $\operatorname{rank}(A)=\operatorname{rank}(B)$。
>
> (4) $\because\ CS(AB)\subseteq CS(A)$，$\therefore\ \dim(CS(AB))\leq \dim(CS(A))$，即 $\operatorname{rank}(AB)\leq \operatorname{rank}(A)$，
>
> $\because\ RS(AB)\subseteq RS(B)$，$\therefore\ \dim(RS(AB))\leq \dim(RS(B))$，即 $\operatorname{rank}(AB)\leq \operatorname{rank}(B)$，
>
> 故得 $\operatorname{rank}(AB)\leq \min\{\operatorname{rank}(A),\operatorname{rank}(B)\}$。
>
> (5i) $\operatorname{rank}(PA)\leq \operatorname{rank}(A)=\operatorname{rank}(P^{-1}PA)\leq \operatorname{rank}(PA)$，$\therefore\ \operatorname{rank}(PA)=\operatorname{rank}(A)$。
>
> 另證：
>
> 因為 $P$ 可逆，故 $P$ 可表為若干列基本矩陣相乘，
>
> 則 $PA$ 與 $A$ 均列等價，故由 (3) 得 $\operatorname{rank}(PA)=\operatorname{rank}(A)$。
>
> (5ii) 與 (5i) 類似。
>
> (6) 任取 $y\in CS(A+B)$，即存在 $x\in F^{n\times 1}$，使 $y=(A+B)x=Ax+Bx$，
>
> 即 $y\in CS(A)+CS(B)$，故 $CS(A+B)\subseteq CS(A)+CS(B)$。
>
> $\therefore\ \dim(CS(A+B))\leq \dim(CS(A)+CS(B))$
>
> $= \dim(CS(A))+\dim(CS(B))-\dim(CS(A)\cap CS(B))$
>
> $\leq \dim(CS(A))+\dim(CS(B))$