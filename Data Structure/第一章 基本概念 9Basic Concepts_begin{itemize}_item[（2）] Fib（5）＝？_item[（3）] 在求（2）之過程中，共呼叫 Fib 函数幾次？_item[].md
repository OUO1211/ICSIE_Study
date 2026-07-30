第一章 基本概念 9
Basic Concepts
\begin{itemize}
\item[（2）] Fib（5）＝？
\item[（3）] 在求（2）之過程中，共呼叫 Fib 函数幾次？
\item[] 解（1）int Fib（int n）
```
    {
        if (n==0) return  \( . \mathrm { 
        else if (n==1) return 1;
            else return (Fib(n-1)+Fib(n-2));
    }
```

\begin{itemize}
\item[（2）] $\operatorname{Fib}(5)=5$
\item[（3）] 呼叫 15 次
\end{itemize}
Exercise
承例 1－5，寫出 Iterative algorithm or program
\item[解] int Fib（int n）
```
{ if (n==0) return 6 ;
    if (n==1) return 1;
    else{ int a=0,b=1, c;
        for (i=2; i<=n; i++)
            { c=a+b;
            a=b;
            b=c;
        }
    } return c;
}
```

\end{itemize}

例題 1－6
Binomial coefficient is defined as follows．
$$
\binom{n}{m}=\left\{\begin{array}{cl}
1 & , \text { if } n=m \text { 或 } m=\phi \\
\binom{n-1}{m}+\binom{n-1}{m-1} & , \text { otherwise }
\end{array}\right.
$$
\begin{itemize}
\item[（1）] Write a recursive C program
\item[（2）] $\binom{5}{3}=$ ？
\item[（3）] 共呼叫此函数幾次（連同 $\binom{5}{3}$ 此次）？
\end{itemize}