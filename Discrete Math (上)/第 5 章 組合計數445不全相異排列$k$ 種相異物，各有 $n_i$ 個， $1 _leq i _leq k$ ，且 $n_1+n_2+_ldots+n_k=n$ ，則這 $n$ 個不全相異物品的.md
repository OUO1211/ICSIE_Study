第 5 章 組合計數
445

不全相異排列
$k$ 種相異物，各有 $n_i$ 個， $1 \leq i \leq k$ ，且 $n_1+n_2+\ldots+n_k=n$ ，
則這 $n$ 個不全相異物品的排列方式有 $\frac{n!}{n_{1}!\cdot n_{2}!\cdot \ldots \cdot n_{k}!}$ 種。
例如：
排列 ABCCC，
可先看成 $\mathrm{ABC}_1 \mathrm{C}_2 \mathrm{C}_3$ ，而共有 3 ！種排列，但其中，每 3 ！種為同一種 ABCCC 中的排列：如 $\mathrm{BAC}_1 \mathrm{C}_2 \mathrm{C}_3 、 \mathrm{BAC}_1 \mathrm{C}_3 \mathrm{C}_2 、 \mathrm{BAC}_2 \mathrm{C}_1 \mathrm{C}_3 、 \mathrm{BAC}_2 \mathrm{C}_3 \mathrm{C}_1 、 \mathrm{BAC}_3 \mathrm{C}_1 \mathrm{C}_2 、 \mathrm{BAC}_3 \mathrm{C}_2 \mathrm{C}_1$ 、都算成 BACCC ，故得排列 ABCCC 的方法數為 $\frac{5!}{3!}$ 。
同理可得，排列 AACCCDDD 的方法數為 $\frac{8!}{2!3!3!}$ 。
例題

10

How many arrangements of the letters in
（1）MISSISSIPPI．
（2）MISSISSIPPI have no consecutive Pˋs？
（3）MISSISSIPPI no consecutive Sˋs？
（4）CALIFORNIA has no consecutive letters the same？
（5）In SOCIOLOGICAL，A and G are adjacent？
（6）In SOCIOLOGICAL，all vowels are adjacent？
（1）四個 $I$ ，四個 $S$ ，兩個 $P$ ，一個 $M$ 的排列數為：$\frac{11!}{4!4!2!1!}{ }^{\circ}$
（2）扣掉 $P 、 P$ 相鄰的排法即可 ：$\frac{11!}{4!4!2!1!}-\frac{10!}{4!4!1!1!}$ 。
（3）先將 MIIIPPI 排好再選 4 個隙縫放 $S:\binom{8}{4} \times \frac{7!}{4!2!}$ 。
（4）扣掉 $A, A$ 相鄰，扣掉 $I 、 I$ 相鄰，再補 $A A$ 相鄰與 $I$ 相鄰：$\frac{10!}{2!2!}-\frac{9!}{2!}-\frac{9!}{2!}+8!$ 。
（5）AG 綁一起，成為 11 字符的排列，也考慮 AG 或 GA： $2 \times \frac{11!}{3!2!2!2!}$ 。
（6）指所有母音均需相鄰，故母音綁成一字符（X）成為 7 字符（XSCLGCL）的排列，而這 6 個母音（OIOOIA）也需考慮排列：$\frac{7!}{2!2!} \times \frac{6!}{2!3!}$ 。