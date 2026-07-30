8 資料結構（含精選試題）
■

Data Structure
\begin{itemize}
\item[2．] 資結類
\item[3．] 其它類（e．g．Permutation，Tower of Hanoi）
\end{itemize}
（三）數學類之遞迴考題（如下例題）：

\section*{例題 1－3}

Write a recursive algorithm for factorial function n！as follows．
$$
n!= \begin{cases}1 & \text {, if } n=\phi \\ n *(n-1)! & \text {, if } n \geq 1\end{cases}
$$

\section*{解 Procedure Fac（int n）}
begin
$$
\begin{aligned}
& \text { if }(\mathrm{n}==0) \text { return } 1 \text {; } \\
& \text { else return } \mathrm{n}^* \operatorname{Fac}(\mathrm{n}-1) \text {; }
\end{aligned}
$$
end．

\section*{例題 1－4}

承上， $\mathrm{Fac}(3)$ 之值為？在求算 $\mathrm{Fac}(3)$ 時，共呼叫 Fac 函數幾次？（含 Fac（3）此次）

\section*{解 $\cdot \mathrm{Fac}(3)=6$}
∵Fac（3）
→3*Fac(2)
→2*Fac(1)
$$
\begin{array}{r}
\hookrightarrow 1^* \operatorname{Fac}(0) \\
\hookrightarrow 1
\end{array}
$$
－共呼叫4次

\section*{例題 1－5}

Fibonacci Number（費氏數列）
定義為：
$$
F_n=\left\{\begin{array}{cl}
\phi & , \text { if } n=0 \\
1 & , \text { if } n=1 \\
F_{n-1}+F_{n-2} & , \text { if } n \geq 2
\end{array}\right.
$$
（1）Write a recursive function in C