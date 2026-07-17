第1章 通輯
27

下列為完成等價證明時，常被使用的性質：
1．分配律（distributive）
（1）$p \vee(q \wedge r) \equiv(p \vee q) \wedge(p \vee r)$
（2）$p \wedge(q \vee r) \equiv(p \wedge q) \vee(p \wedge r)$
2．結合律（associative）
（1）$(p \vee q) \vee r \equiv p \vee(q \vee r)$
（2）$(p \wedge q) \wedge r \equiv p \wedge(q \wedge r)$
3．交換律（commutative）
（1）$p \vee q \equiv q \vee p$
（2）$p \wedge q \equiv q \wedge p$ ．
4．吸收律（absorption）
（1）$p \vee(p \wedge q) \equiv p$
（2）$p \wedge(p \vee q) \equiv p$
5．藇等律（idempotent）
（1）$p \vee p \equiv p$
（2）$p \wedge p \equiv p$
6．單位元性質（identity），也稱同一律
（1）$p \vee F \equiv p$
（2）$p \wedge T \equiv p$
7．控制律（domination）
（1）$p \vee T \equiv T$
（2）$p \wedge F \equiv F$
8．否定律（negation）
（1）$p \vee \sim p \equiv T$
（2）$p \wedge \sim p \equiv F$
9．雙否定律（double negative）
$$
\sim(\sim p) \equiv p
$$

10．笛摩根定律（De Morgan＇s law）
$(1) \sim(p \vee q) \equiv \sim p \wedge \sim q$
（2）$\sim(p \wedge q) \equiv \sim p \vee \sim q$
【99中興資科】

Note
（1）以上各式均可由檢查真值表證明，也都滿足對偶性質。
（2）$p \leftrightarrow q \equiv(p \rightarrow q) \wedge(q \rightarrow p)$ 。
（3）一般化的笛摩根定律：對任何正整數 $k>1$ ，
$$
\sim\left(p_1 \wedge \cdots \wedge p_k\right) \equiv \sim p_1 \vee \cdots \vee \sim p_k ; \sim\left(p_1 \vee \cdots \vee p_k\right) \equiv \sim p_1 \wedge \cdots \wedge \sim p_k .
$$