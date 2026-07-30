10
資料結構（含精選試題）
Data Structure

解（1）int Bin（int n，int m）
\begin{itemize}
\begin{itemize}
\item[] ｛
$$
\text { if }(\mathrm{n}==\mathrm{m} \| \mathrm{m}==0) \text { return } 1 \text {; }
$$
else
$$
\text { return }(\operatorname{Bin}(n-1, m)+\operatorname{Bin}(n-1, m-1)) \text {; }
$$
\}
\end{itemize}
\item[（2）] $\binom{5}{3}=10$
\item[（3）] 19 次
\end{itemize}

例題 1－7
Ackerman＇s function
$$
A(m, n)=\left\{\begin{array}{cl}
n+1 & , \text { if } m=0 \\
A(m-1,1) & , \text { if } n=0 \\
A(m-1, A(m, n-1)) & , \text { otherwise }
\end{array}\right.
$$
\begin{itemize}
\item[（1）] Write a recursive algorithm
\item[（2）] $\mathrm{A}(2,2)=$ ？
\end{itemize}

解（1）Procedure Ack（int n，int m）
\begin{itemize}
\begin{itemize}
\item[] ｛
if $(\mathrm{m}==0)$ then return（ $\mathrm{n}+1$ ）；
else if $(\mathrm{n}==0)$ then return Ack（m－1，1）；
else return Ack（m－1，Ack（m，n－1））；
\}
\item[（2）] $\mathrm{A}(2,2)=7$
\end{itemize}
\end{itemize}

Exercise
\begin{itemize}
\item[（1）] $\mathrm{A}(2,1)=$ ？（2） $\mathrm{A}(1,2)=$ ？（3） $\mathrm{A}(2,3)=$ ？
\end{itemize}

解（1） 5 （2） 4 （3） 9