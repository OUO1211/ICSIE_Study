> **例題 7**
>
> Let $\{v_1, v_2, v_3, v_4\}$ be a basis of a vector space $V$ over a field $F$. Determine if the following set is a basis of $V$. Justify your answer.
>
> (1) (5%) $\{v_1, v_1 + v_2, v_1 + v_2 + v_3, v_1 + v_2 + v_3 + v_4\}$。 【98 中正資工】
>
> (2) (5%) $\{v_1 + v_2, v_2 + v_3, v_3 + v_4, v_4 + v_1\}$。 【83 台大資工 題組，96 成大 數學】

**解**

$\because \{v_1, v_2, v_3, v_4\}$ 為 $V$ 的基底，故 $\dim(V) = 4$。

(1) Yes。

先證明此為線性獨立集：

設 $\alpha_1 v_1 + \alpha_2(v_1 + v_2) + \alpha_3(v_1 + v_2 + v_3) + \alpha_4(v_1 + v_2 + v_3 + v_4) = 0$，

則 $(\alpha_1 + \alpha_2 + \alpha_3 + \alpha_4)v_1 + (\alpha_2 + \alpha_3 + \alpha_4)v_2 + (\alpha_3 + \alpha_4)v_3 + \alpha_4 v_4 = 0$，

而 $\{v_1, v_2, v_3, v_4\}$ 為線性獨立，故 $\begin{cases} \alpha_1 + \alpha_2 + \alpha_3 + \alpha_4 = 0 \\ \alpha_2 + \alpha_3 + \alpha_4 = 0 \\ \alpha_3 + \alpha_4 = 0 \\ \alpha_4 = 0 \end{cases}$，

$\therefore \alpha_1 = \alpha_2 = \alpha_3 = \alpha_4 = 0$，

$\therefore \{v_1, v_1+v_2, v_1+v_2+v_3, v_1+v_2+v_3+v_4\}$ 為線性獨立集，

又因為 $\dim V = 4$ 個向量，故可為 $V$ 的一組基底。

(2) No。

$\because (v_1 + v_2) - (v_2 + v_3) + (v_3 + v_4) - (v_4 + v_1) = 0$，

$\therefore \{v_1 + v_2, v_2 + v_3, v_3 + v_4, v_4 + v_1\}$ 為線性相依，故不為基底。
