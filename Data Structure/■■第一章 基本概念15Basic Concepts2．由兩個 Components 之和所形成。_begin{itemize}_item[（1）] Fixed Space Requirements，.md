■■
第一章 基本概念
15
Basic Concepts

2．由兩個 Components 之和所形成。
\begin{itemize}
\item[（1）] Fixed Space Requirements，包含下列：
\begin{itemize}
\item[（1）] Instruction space．
\item[（2）] Space for simple variables．
\item[（3）] Fixed－size structured variables．
\item[（4）] Constants
\end{itemize}
\item[（2）] Variable Space Requirements
\begin{itemize}
\item[①] 此包含了 Space needed by structured variables whose size depends on the particular instance I of the problem being solved．
\item[（2）] 它也包含 The additional space required when a function used recursion．
\item[（3）] The variable space requirement of a program P working on an instance I is denoted SP（I）．
\item[（4）] SP（I）is usually given as a function of some characteristics of the instance I．例如：如果 Input 包含了一個 n 個數字的 Array，then n is an instance characteristics．
若 n is the only instance characteristics 則 Sp（n）表 Sp（I）。
\item[（5）] Space Requirement S（P）
$$
S(P)=c+S P(I)
$$
其中：c 是常數，表 fixed size requirement
\end{itemize}
\end{itemize}

\section*{例題 1－12}
float abc（float a，float b，float c）
｛
\}
```
    return a+b+b*c(a+b-c)/(a+b)+4;
```


解 $\mathrm{S}_{\mathrm{abc}}(\mathrm{I})=0$

\section*{例題 1－13}
```
float sum(float list[ ], int n)
{
    float tempsum = 0;
    int i;
    for(i=0; i < n; i++) tempsum += list[i];
    return tempsum;
}
```