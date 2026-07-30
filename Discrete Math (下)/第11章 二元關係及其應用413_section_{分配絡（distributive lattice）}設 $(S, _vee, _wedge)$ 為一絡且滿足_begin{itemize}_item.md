第11章 二元關係及其應用
413

\section*{分配絡（distributive lattice）}

設 $(S, \vee, \wedge)$ 為一絡且滿足
\begin{itemize}
\item[（1）] $\forall a, b, c \in S, a \vee(b \wedge c)=(a \vee b) \wedge(a \vee c)$ 。（ $\vee$ 對 $\wedge$ 具有分配性），
\item[（2）] $\forall a, b, c \in S, a \wedge(b \vee c)=(a \wedge b) \vee(a \wedge c)$ 。（ $\wedge$ 對 $\vee$ 具有分配性），則稱 $(S, \vee, \wedge)$ 為一分配絡。
\end{itemize}

例如 $(N, \max , \min ) 、(P(A), \cup, \cap, A, \varnothing) 、\left(D_m, 1 \mathrm{~cm}, \operatorname{gcd}, m, 1\right)$ 均為分配絡。
Note
\begin{itemize}
\item[（1）] 判別分配絡的充要條件：
設 $(S, \vee, \wedge)$ 為一絡，
則（ $S, \vee, \wedge$ ）為分配絡 ⇔（ $S, \vee, \wedge$ ）不具與右圖同構的子絡 ${ }^{\circ}{ }_b$
【證明】
以下僅說明此二圖不具分配性。
左：$e \vee(b \wedge d)=e \vee c=e$ ，但 $(e \vee b) \wedge(e \vee d)=a \wedge d=d 。$
右 ：$b \vee(c \wedge d)=b \vee e=b$ ，但 $(b \vee c) \wedge(b \vee d)=a \wedge a=a \circ$
\item[（2）] 元素個數 $<5$ 的絡必為分配絡（因為那兩個圖都需 5 個點）。
\end{itemize}