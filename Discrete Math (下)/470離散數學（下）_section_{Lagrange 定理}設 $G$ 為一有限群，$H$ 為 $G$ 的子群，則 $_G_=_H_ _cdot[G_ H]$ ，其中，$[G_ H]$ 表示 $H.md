470
離散數學（下）

\section*{Lagrange 定理}

設 $G$ 為一有限群，$H$ 為 $G$ 的子群，則 $|G|=|H| \cdot[G: H]$ ，
其中，$[G: H]$ 表示 $H$ 在 $G$ 中所形成相異右（左）陪集的個數。
【證明】
（1）在 $G$ 上定義一關係：$\forall a . b \in G, a \equiv_r b(\bmod H) \Leftrightarrow a b^{-1} \in H \ldots \ldots$ 則此關係為一等價關係。
（2）所得等價類 $[a]=\left\{x \in G \mid a \equiv_r x(\bmod H)\right\}=H a$ 為一 $H$ 之右陪集。
（3）由定義一函數 $f: H \rightarrow H a$ ，by $f(h)=h a$ ，可驗證得 $f$ 為 1－1 且 onto，得知 $|H|=|H a|$ 。
（4）因為相異等價類形成一分割，$\therefore|G|=|U[a]|=\sum|[a]|=\sum|H|=[G: H] \cdot|H|$ 。
Note
$[G: H]$ 又稱為 $H$ 在 $G$ 中的指標（index of $H$ in $G$ ）。
例如：考慮 $\left(Z_6,+_6\right)$ ，
取 $H=\{0,2,4\}$ ，則可知 $\left(H,+{ }_6\right)$ 為 $\left(Z_6,+{ }_6\right)$ 之子群，
且 $H$ 有兩個相異的左陪集：｛0，2，4\}, \{1, 3, 5\}, $H$ 有兩個相異的右陪集：｛0，2，4\}, \{1, 3, 5\},即 $[G: H]=2$ 。

Lagrange 定理的應用
I．設 $G$ 為一有限群，$H$ 為 $G$ 的子群，則（1）$|H \||G|$ ；（2）$[G: H]||G|$ 。
【90 台科資工】【 90 中興資科】【92、 94 中山資工】【 94 暨南資工】【 98 、 110 台大資工】

II．設 $\boldsymbol{G}$ 為一群，$|G|=p$ 為質數，則 $\boldsymbol{G}$ 為循環群。【94 中山資工】

【證明】
令（ $G, *$ ）為一群，元素個數為 $p$ ，且 $p$ 為一質數，則
$\because|G|=p \geq 2, \therefore G$ 存在非單位元素，令為 $a$ ，
考慮 $H=\langle a\rangle=\left\{a^k \mid k \in Z\right\}$ ，則 $H$ 為 $G$ 之一子群，且 $H$ 為一循環群，且 $H \neq\{e\}$ ，
故由 Lagrange 定理知 $|H|||G|$ ，
但 $|G|$ 為質數，$\therefore|H|=|G|$ ，故得 $H=G$ ，故知 $G$ 為一循環群。
Note
但反之末必，例如 $\left(Z_6,+_6\right)$ 為一循環群但有6元素。