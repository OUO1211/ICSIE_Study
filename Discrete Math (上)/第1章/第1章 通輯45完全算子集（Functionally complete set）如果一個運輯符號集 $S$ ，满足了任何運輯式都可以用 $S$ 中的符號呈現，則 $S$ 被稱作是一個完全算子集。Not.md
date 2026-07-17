第1章 通輯

45



完全算子集（Functionally complete set）

如果一個運輯符號集 $S$ ，满足了任何運輯式都可以用 $S$ 中的符號呈現，則 $S$ 被稱作是一個完全算子集。



Note

（1）$\{\sim, \vee, \wedge, \rightarrow, \leftrightarrow\}$ 為完全算子集。

（2）$\{\sim, \vee, \wedge, \rightarrow\}$ 為完全算子集，因為 $p \leftrightarrow q \equiv(p \rightarrow q) \wedge(q \rightarrow p)$ 。

（3）$\{\sim, \vee, \wedge\}$ 為完全算子集，因為 $p \rightarrow q \equiv(\sim p) \vee q$ 。

（4）$\{\sim, \wedge\}$ 為完全算子集，因為 $p \vee q \equiv \sim[(\sim p) \wedge(\sim q)]$ 。

（5）$\{\sim, \vee\}$ 為完全算子集，因為 $p \wedge q \equiv \sim[(\sim p) \vee(\sim q)]$ 。



【103台大電機】



（6）$\{\uparrow\}$ 為完全算子集，其中，$\uparrow$ 為 Nand 運算子，定義成 $p \uparrow q \equiv \sim(p \wedge q)$ 。

解 由真值表可得 $(\sim p) \equiv p \uparrow p$ ；

$$

\begin{aligned}

\therefore p \vee q & \equiv \sim((\sim p) \wedge(\sim q)) \equiv(\sim p) \uparrow(\sim q) \\

& \equiv(p \uparrow p) \uparrow(q \uparrow q) ; \\

\therefore p \wedge q & \equiv \sim(\sim(p \wedge q)) \equiv \sim(p \uparrow q) \\

& \equiv(p \uparrow q) \uparrow(p \uparrow q) ;

\end{aligned}

$$



故知由 $\sim, \vee, \wedge$ 組成的敘述均可以↑表達，故 $\{\uparrow\}$ 為完全算子集。

（7）$\{\downarrow\}$ 為完全算子集，其中，$\downarrow$ 為 Nor 運算子，定義成 $p \downarrow q \equiv \sim(p \vee q)$ 。

解 由真值表可得 $(\sim p) \equiv p \downarrow p$ ；

$$

\begin{aligned}

\therefore p \vee q & \equiv \sim(\sim(p \vee q)) \equiv \sim(p \downarrow q) \\

& \equiv(p \downarrow q) \downarrow(p \downarrow q) ; \\

\therefore p \wedge q & \equiv \sim((\sim p) \vee(\sim q)) \equiv(\sim p) \downarrow(\sim q) \\

& \equiv(p \downarrow p) \downarrow(q \downarrow q) ;

\end{aligned}

$$



故知由 $\sim, \vee, \wedge$ 組成的敘述均可以 ↓ 表達，故 $\{\downarrow\}$ 為完全算子集。