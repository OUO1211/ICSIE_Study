462
離散數學（下）

\section*{循環群（cyclic group）}

設 $G$ 為一群，若存在 $G$ 中元素 $a$ ，使滿足 $G=\left\{a^k \mid k \in Z\right\}$ ，則稱 $G$ 為一循環群。
且稱 $a$ 為 $G$ 的生成元（generator），記作 $G=\langle a\rangle$ ．
【92台科資工】
例如 ：
$\left(Z_6,+{ }_6\right)$ 可由 5 生成 ：
$$
\begin{array}{lll}
5^1=5, & 5^2=5+5=10 \equiv 4, & 5^3=5+5+5=15 \equiv 3, \\
5^4=5+5+5+5=20 \equiv 2, & 5^5=25 \equiv 1, & 5^6=30 \equiv 0 .
\end{array}
$$
也可以由 1 生成：
$1^1=1,1^2=1+1=2,1^3=1+1+1=3,1^4=4,1^5=5,1^6=6=0$ 。
故 $Z_6=\langle 5\rangle=\langle 1\rangle$ 。
Note
\begin{itemize}
\item[（1）] 循環群 $G=\left\{a^k \mid k \in Z\right\}$ 中，$a^0=e$ 表單位元素，$a^{-t}=\left(a^t\right)^{-1}$ 表 $a^t$ 的反元素。
\item[（2）] $a \in G,<a>=\left\{a^i \mid i \in Z\right\}$ 為 $G$ 的一子群。
\end{itemize}

【99台大資工】
\begin{itemize}
\item[（3）] 對元素 $a$ ，則稱使 $a^k=e$ 之最小整數 $k$ 為 $a$ 之基數（order），記作 $\circ(a)=k$ 。
例如 ：$\left(Z_6,+{ }_6\right)$ 中，$\circ(5)=6 ; \circ(1)=6$ ；
$$
\begin{aligned}
& <2>=\{2,4,0\}, \circ(2)=3 ; \\
& <3>=\{3,0\}, \circ(3)=2 ; \\
& <4>=\{4,2,0\}, \circ(4)=3 \circ
\end{aligned}
$$
\item[（4）] 設 $G$ 為一群，元素 $a$ 的 order 為 $n$ ，則 $a^m=e \Leftrightarrow n \mid m 。$
【證明】
⇐ 若 $n \mid m$ ，令 $m=n \cdot t, t \in Z$ ，則 $a^m=\left(a^n\right)^t=e^t=e$ 。
⇒ 若 $m$ 不為 $n$ 之倍數，令 $m=n \cdot t+b, 0<b<n, t, b \in Z$ ，
則 $a^b=a^{m-t n}=a^m\left(a^n\right)^{-t}=e e^{-t}=e$ 與。 $(a)=n$（ $n$ 為使 $a^k=e$ 之最小數）矛盾。
\end{itemize}
（5）設 $G$ 為一群，$|G| \geq 2$ ，則 $G$ 必有非簡單（nontrivial）的循環子群。
【證明】
$\because|G| \geq 2, \therefore$ 存在非單位元素 $a \in G$ ，考慮 $H=\langle a\rangle=\left\{a^k \mid k \in Z\right\}$ ，則
\begin{itemize}
\begin{itemize}
\item[（1）] $H$ 為循環群（由定義可知）。
\item[（2）] $H$ 為 $G$ 之子群：∵ 對任意 $H$ 中的元素 $x, y$ ，令 $x=a^m, y=a^n$ ，則 $x y^{-1}=a^{m-n} \in H$ 。
\end{itemize}
\end{itemize}