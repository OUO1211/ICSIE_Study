502
離散數學（上）

條件機率
考慮樣本空間 $S$ 中的非空事件 $E, F$ ，
（1）稱 $\operatorname{Pr}(F \mid E)=\frac{\operatorname{Pr}(E \bigcap F)}{\operatorname{Pr}(E)}$ 為已知事件 $E$ 發生之下，發生 $F$ 的機率。
（2）貝氏定理（Bayes＇Theorem）： $\operatorname{Pr}(F \mid E)=\frac{\operatorname{Pr}(E \mid F) \operatorname{Pr}(F)}{\operatorname{Pr}(E \mid F) \operatorname{Pr}(F)+\operatorname{Pr}(E \mid \bar{F}) \operatorname{Pr}(\bar{F})}$ ，
其中， $\bar{F}=S-F$ ，為 $F$ 的狳事件（complement，也稱補事件）。【108 台大工科】
解 $\operatorname{Pr}(F \mid E)=\frac{\operatorname{Pr}(E \bigcap F)}{\operatorname{Pr}(E)}=\frac{\operatorname{Pr}(E \bigcap F)}{\operatorname{Pr}(E \bigcap F)+\operatorname{Pr}(E \bigcap \bar{F})}$
$$
=\frac{\operatorname{Pr}(F) \times \frac{\operatorname{Pr}(E \bigcap F)}{\operatorname{Pr}(F)}}{\operatorname{Pr}(F) \times \frac{\operatorname{Pr}(E \bigcap F)}{\operatorname{Pr}(F)}+\operatorname{Pr}(\bar{F}) \times \frac{\operatorname{Pr}(E \bigcap \bar{F})}{\operatorname{Pr}(\bar{F})}}=\frac{\operatorname{Pr}(E \mid F) \operatorname{Pr}(F)}{\operatorname{Pr}(E \mid F) \operatorname{Pr}(F)+\operatorname{Pr}(E \mid \bar{F}) \operatorname{Pr}(\bar{F})} .
$$

例題 11
（5\％）Find $\operatorname{Pr}(Y \mid X)$ if $\operatorname{Pr}(X \mid Y)=1 / 3, \operatorname{Pr}(X \mid \bar{Y})=1 / 4$ ，and $\operatorname{Pr}(Y)=2 / 3$ by using Bayes＇ theorem where $X$ and $Y$ are events from a simple space $S$ 。【 107 成大電機】【 107 政大資科】

解 $\operatorname{Pr}(Y \mid X)=\frac{\operatorname{Pr}(Y \cap X)}{\operatorname{Pr}(X)}=\frac{\operatorname{Pr}(Y) \cdot \operatorname{Pr}(X \mid Y)}{\operatorname{Pr}(X \mid Y) \cdot \operatorname{Pr}(Y)+\operatorname{Pr}(X \mid \bar{Y}) \cdot \operatorname{Pr}(\bar{Y})}=\frac{\frac{2}{3} \times \frac{1}{3}}{\frac{1}{3} \times \frac{2}{3}+\frac{1}{4} \times \frac{1}{3}}=\frac{8}{11}$ 。

例題 12
We have two boxes．The first contains two green balls and seven red balls；the second contains four green balls and three red balls．Bob selects a ball by first choosing one of the two boxes at random．He then selects one of the balls in this box at random．Consider the following events $E$ and $F$ ．
$E$ ：the event that Bob has selected a red ball．
$F$ ：the event that Bob has selected a ball from the first box．
（1）$(2 \%)$ What is the probability $\operatorname{Pr}(E \mid F)$ ？
（2）（1\％）What is the probability $\operatorname{Pr}(E \mid \bar{F})$ ？
（3）（2\％）What is the probability $\operatorname{Pr}(F \mid E)$ ？

【99中正資工】