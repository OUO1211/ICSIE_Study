第二章 陣列與結構
71

Arrays＆Structures
【題型三】給予二個已知位址量，但判斷出 Row 或 Column major 皆有可能，故兩者皆須求算。
求算出的結果可能有：$\left\{\begin{array}{l}\text {（1）兩者皆合 } \\ \text {（2）一合，一不合 }\end{array}\right.$

例題 2－6
二维陣列 $\mathrm{A}(1 \cdots \mathrm{~m}, 1 \cdots \mathrm{n})$ ，若 $\mathrm{A}(3,3)$ 的 Location 為121且 $\mathrm{A}(6,4)$ 之位置為159，則 $\mathrm{A}(5$,4）之 Location 為？（元素大小為1）

解 判斷出 Row 或 Column－major 皆有可能
\begin{itemize}
\item[（1）] 先算 Row－major
$$
\begin{aligned}
& \mathrm{A}(6,4)=\mathrm{A}(3,3)+[(6-3) * \mathrm{n}+(4-3)] * 1 \\
& 159=121+3 \mathrm{n}+1 \\
& \Rightarrow 3 \mathrm{n}=37 \\
& \because \mathrm{n}=\frac{37}{3} \text { 非整數 } \quad \therefore \text { 不合 }
\end{aligned}
$$
\item[（2）] 用 Column－major 求算
則 $\mathrm{A}(6,4)=\mathrm{A}(3,3)+[(4-3) * \mathrm{~m}+(6-3)] * 1$
$$
159=121+m+3
$$
$\because \mathrm{m}=35$ 列
$$
\begin{aligned}
\therefore \mathrm{A}(5,4) & =\mathrm{A}(3,3)+[(4-3) * 35+(5-3)] * 1 \\
& =121+35+2=158
\end{aligned}
$$
\end{itemize}

例題 2－7
二维陣列 A，其中 A［7，8］之 Location 為2732，A［13，16］之 Location 為3364，元素大小為 4 ，則 $\mathrm{A}[9,6]$ 之 Location 為何？

解 此題兩者皆合，皆須求算出來。

【題型四】給予三個已知位址量，求 A［i，j］之 Location。
Hint：給三個已知位址量，表示 d 要自行假設
$$
\text { 判斷出 } \begin{cases}\text { (1)Row - major } & \Rightarrow \text { 可求 } \ell_0 \text {, 行數及d } \\ \text { (2)Column - major } & \Rightarrow \text { 可求 } \ell_0 \text {, 列數及d }\end{cases}
$$