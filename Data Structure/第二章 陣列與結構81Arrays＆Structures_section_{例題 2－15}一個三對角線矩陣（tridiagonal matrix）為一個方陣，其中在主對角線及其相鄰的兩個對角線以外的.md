第二章 陣列與結構
81

Arrays＆Structures

\section*{例題 2－15}

一個三對角線矩陣（tridiagonal matrix）為一個方陣，其中在主對角線及其相鄰的兩個對角線以外的元素均為 O（如下圖所示）。在由此三個對角線所形成的带狀區域上的元素以列序储存在一個陣列 b 中，a［0］［0］存放在 b［0］。找出 b［k］，k 的公式，用以存放 a［i］［j］之值， $0 \leq \mathrm{i}, \mathrm{j}<\mathrm{n}$ 。
$$
\left[\begin{array}{cccccccccc}
x & x & & & & & & & & \\
x & x & x & & & & & & & \\
& x & x & x & & & & & \\
& & \cdot & x & \cdot & & & & & \\
& & & \cdot & \cdot & \cdot & & \text { 零 } & & \\
& & & & \cdot & \cdot & \cdot & & & \\
& & \text { 零 } & & & \cdot & x & x & & \\
& & & & & & x & x & x & \\
& & & & & & x & x & x \\
& & & & & & x & x & x
\end{array}\right]
$$

解 $\mathrm{k}=2 \mathrm{i}+\mathrm{j}-2$

例題 2－16
一個 generalized band matrix A，是一個 N×N 的矩陣，其中對角線下的 a－1 列為非零元素，對角線上的 b－1 列為非零元素，其餘為零元素，例如下圖為一個 $4 \times 4$ 且 a 為 3 ，b為 2 的 band matrix。
$$
\mathrm{a}\left[\begin{array}{cccc}
0 & \mathrm{~b} & \\
8 & 0 & 4 & 0 \\
9 & 3 & 2 & 9 \\
0 & 7 & 6 & 1
\end{array}\right]
$$