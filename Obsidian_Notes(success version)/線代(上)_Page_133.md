# 第二章 線性方程組與求解 134

## 線性系統的應用問題

> **例題 6**
>
> (10%) If the polynomial function $f(x)=ax^4+bx^3+cx^2+dx+e$ satisfies $f(-2)=150$, $f(-1)=16$, $f(0)=2$, $f(1)=18$, $f(2)=166$, then $a,b,c,d,e$ are \_\_\_\_, \_\_\_\_, \_\_\_\_, \_\_\_\_, \_\_\_\_, respectively.
>
> 【100 雲科資工‧107 中央通試題‧109 台大資工】

**解**

由
$$
\begin{cases}
16a-8b+4c-2d+e=150 \quad \cdots (1) \\
a-b+c-d+e=16 \quad \cdots (2) \\
0a+0b+0c+0d+e=2 \quad \cdots (3) \\
a+b+c+d+e=18 \quad \cdots (4) \\
16a+8b+4c+2d+e=166 \quad \cdots (5)
\end{cases}
$$

整理得
$$
\begin{cases}
((1)+(5))/2: 16a+4c+e=158, \\
((2)+(4))/2: a+c+e=17, \\
(3): e=2
\end{cases}
$$

故可得
$$
\begin{cases}
16a+4c=156 \\
a+c=15
\end{cases}
$$

而得 $a=8$，$c=7$

再代 $(4),(5)$ 得
$$
\begin{cases}
b+d=1 \\
8b+2d=8
\end{cases}
$$

而得 $b=1$，$d=0$

故所求為，$f(x)=8x^4+x^3+7x^2+2$。