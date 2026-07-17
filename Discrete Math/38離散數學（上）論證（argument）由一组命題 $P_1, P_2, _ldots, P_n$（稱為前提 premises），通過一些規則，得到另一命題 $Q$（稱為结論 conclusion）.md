38
離散數學（上）

論證（argument）
由一组命題 $P_1, P_2, \ldots, P_n$（稱為前提 premises），通過一些規則，得到另一命題 $Q$（稱為结論 conclusion），這個過程稱為論證。

Note
（1）若當所有前提 $P_1, P_2, \ldots, P_n$ 為真時，$Q$ 為真，則稱論證＂$P_1, P_2, \ldots, P_n \mapsto Q$＂為真實的（有效的、正確的、valid）。
（2）一個非真實的論證稱為謬論（fallacy）或不真實的（invalid）。
（3）論證 $P_1, P_2, \ldots, P_n \mapsto Q$ 為正確的
$\Leftrightarrow P_1, P_2, \ldots, P_n$ 邏輯蘊含 $Q$
$\Leftrightarrow P_1 \wedge P_2 \wedge \ldots \wedge P_n \rightarrow Q$ 為真理。
（4）常用之正確的論證型式：
$p \rightarrow q$
（1）
$$
\frac{p}{\therefore q}
$$

肯定律（modus ponens）
$\frac{p}{\therefore q}$
（2）
$$
\frac{\sim q}{\therefore \sim p}
$$

反證法（modus tollens）
$p \rightarrow q$ p
（5）
$\frac{q}{\therefore p \wedge q}$
conjunction
（6）
$$
\frac{p}{\therefore p \vee q}
$$
disjunction
$$
p \rightarrow q
$$
（3）
$$
\sim p \rightarrow F
$$

矛盾法
0
（4）
$$
\frac{q \rightarrow r}{\therefore p \rightarrow r}
$$

三段論證
◯
vgo v（g－ v（g－
（7）
$$
\frac{p \wedge q}{\therefore p}
$$
simplication
（5）判斷是否為真實論證的方法：
（1）以真值表判斷 $P_1 \wedge P_2 \wedge \ldots \wedge P_n \rightarrow Q$ 是否永真。
（2）若找不到反例，則 $P_1 \wedge P_2 \wedge \ldots \wedge P_n \rightarrow Q$ 為永真。
（3）用常見論證方式推導。