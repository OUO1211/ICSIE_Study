第一章 基本概念
11
Basic Concepts

\section*{例題 1－8}

Write a recursive C program to calculate the greatest common divisor（GCD）of A and B
解 GCD（A，B）is defined as follows．
$$
\operatorname{GCD}(\mathrm{A}, \mathrm{~B})=\left\{\begin{array}{cl}
\mathrm{B} & , \text { if }(\mathrm{A} \bmod \mathrm{~B})=\phi \\
\operatorname{GCD}(\mathrm{B}, \mathrm{~A} \bmod \mathrm{~B}) & , \text { otherwise }
\end{array}\right.
$$
Hence，
$$
\begin{aligned}
& \text { Int GCD (int } A, \text { int } B \text { ) } \\
& \quad \begin{array}{l}
\quad \text { if }(A \% B==0) \text { return } B ; \\
\text { else return } G C D(B, A \% B) ; \\
\}
\end{array}
\end{aligned}
$$
（四）資結類之遞迴考題：
\begin{itemize}
\item[1．] Binary Tree 之 Traversal algorithm 及其應用
\item[2．] Graph 之 DFS
\item[3．] Binary Search
\item[4．] Quick SORT
\end{itemize}

等等。

\section*{例題 1－9}

Binary Search 之 Recursive algorithm

\section*{解 程 式（Recursive Program）}
int binsearch（int list［ ］，int searchnum，int left，int right）
$$
\begin{aligned}
& \text { /* Search list[0] <=... <= list[n-1] for searchnum. } \\
& \text { Return its position if found. Otherwise return -1 */ } \\
& \text { int middle; } \\
& \text { if(left <= right) \{ } \\
& \text { middle = (left + right)/2; } \\
& \text { switch(COMPARE(list[middle], searchnum)) \{ } \\
& \text { case "<": return binsearch(list, }
\end{aligned}
$$