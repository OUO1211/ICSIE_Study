第1章 邏輯 3

1－1 命題與真值表

命題（proposition 、 statement）
具有真假值的語句。
Note
（1）例如： $1+2=3$ ，地球是圓的。
（2）可以是真或是假，但不能同時成立，只能取其一。有時用 $\mathbf{T}$（真、 1 ）與 $\mathbf{F}$（假、 0 ）來代表，又稱兩值邏輯。
（3）疑問句、命令句、威嘆句、祈使句都不屬於命題。
（4）專門處理命題的邏輯系統稱為命題演算或命題邏輯（propositional logic）。
（5）可分成兩類：（i）原子（atom）命題；（ii）複合（compound）命題。

連接詞（或稱運算子）
（1）～not ：$\sim p$ 稱為＂非 $p$＂，為 $p$ 的否定敘述，又記為 $\neg p 、 \bar{p}$ 。
（2）$\wedge$ and $: p \wedge q$ 稱為＂$p$ 且 $q$＂。
（3）$\vee$ or $\quad: p \vee q$ 稱為＂$p$ 或 $q$＂。
（4）→imply ：$p \rightarrow q$ 稱為＂若 $p$ 則 $q$＂、＂$p$ 蕴含 $q$＂。
（5）↔ if and only if ：$p \leftrightarrow q$ 稱為＂$p$ 若且唯若 $q$＂。

\begin{tabular}{|c|c|}
\hline$p$ & $\sim p$ \\
\hline 0 & 1 \\
\hline 1 & 0 \\
\hline
\end{tabular}

\begin{tabular}{|c|c|c|c|c|c|c|c|c|}
\hline$p$ & $q$ & $p \wedge q$ & $p \vee q$ & $p \rightarrow q$ & $p \leftrightarrow q$ & $p \oplus q$ & $p \uparrow q$ & $p \downarrow q$ \\
\hline 0 & 0 & 0 & 0 & 1 & 1 & 0 & 1 & 1 \\
\hline 0 & 1 & 0 & 1 & 1 & 0 & 1 & 1 & 0 \\
\hline 1 & 0 & 0 & 1 & 0 & 0 & 1 & 1 & 0 \\
\hline 1 & 1 & 1 & 1 & 1 & 1 & 0 & 0 & 0 \\
\hline
\end{tabular}

Note
（1）へ又稱 conjunction，遇到＂but＂也適用此運算。
（2）$\vee$ 又稱 disjunction。此處的＂或＂是有涵蓋兩者皆成立的部分，如不涵蓋兩者皆成立的部分，則稱＂互斥或＂（exclusive disjunction 記成 $p \oplus q$ ，有時又記為 $\Delta$ 或 $\underline{v}$ ）。
（3）$p \rightarrow q$ 又稱條件命題（conditional），也記作＂$p \Rightarrow q$＂。其中，$p$ 稱為 $q$ 的充分條件（sufficient）， $q$ 稱為 $p$ 的必要條件（necessary）。也等同於＂$p$ only if $q$＂。