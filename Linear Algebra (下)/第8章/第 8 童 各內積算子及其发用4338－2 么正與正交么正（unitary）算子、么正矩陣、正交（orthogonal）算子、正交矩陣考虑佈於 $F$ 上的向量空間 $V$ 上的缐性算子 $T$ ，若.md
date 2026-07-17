第 8 童 各內積算子及其发用
433

8－2 么正與正交

么正（unitary）算子、么正矩陣、正交（orthogonal）算子、正交矩陣
考虑佈於 $F$ 上的向量空間 $V$ 上的缐性算子 $T$ ，若 $T T^*=T * T=I$ ，則
當 $F=C$ 時，稱 $T$ 為么正算子；當 $F=R$ 時，則稱 $T$ 为正交算子。
考虑佈於 $F$ 上 $n$ 階方陣 $A$ ，
當 $F=C$ 時，$A$ 滿足 $A^H A=A A^H=I$ ，則稱 $A$ 為么正矩陣。
當 $F=R$ 時，$A$ 滿足 $A^T A=A A^T=I$ ，則稱 $A$ 為正交矩陣。
例如，
$$
\begin{aligned}
& A=\left[\begin{array}{cc}
i / 2 & -\sqrt{3} / 2 \\
\sqrt{3} / 2 & -i / 2
\end{array}\right], \\
& A A^H=\left[\begin{array}{cc}
i / 2 & -\sqrt{3} / 2 \\
\sqrt{3} / 2 & -i / 2
\end{array}\right]\left[\begin{array}{cc}
-i / 2 & \sqrt{3} / 2 \\
-\sqrt{3} / 2 & i / 2
\end{array}\right]=\left[\begin{array}{cc}
1 & 0 \\
0 & 1
\end{array}\right]=\left[\begin{array}{cc}
-i / 2 & \sqrt{3} / 2 \\
-\sqrt{3} / 2 & i / 2
\end{array}\right]\left[\begin{array}{cc}
i / 2 & -\sqrt{3} / 2 \\
\sqrt{3} / 2 & -i / 2
\end{array}\right]=A^H . \\
& B=\frac{1}{2}\left[\begin{array}{cc}
1+i & 1-i \\
1-i & 1+i
\end{array}\right], \\
& B B^H=\frac{1}{2}\left[\begin{array}{cc}
1+i & 1-i \\
1-i & 1+i
\end{array}\right] \frac{1}{2}\left[\begin{array}{cc}
1-i & 1+i \\
1+i & 1-i
\end{array}\right]=\left[\begin{array}{ll}
1 & 0 \\
0 & 1
\end{array}\right]=\frac{1}{2}\left[\begin{array}{ll}
1-i & 1+i \\
1+i & 1-i
\end{array}\right] \frac{1}{2}\left[\begin{array}{cc}
1+i & 1-i \\
1-i & 1+i
\end{array}\right]=B^H B, \\
& C=\frac{1}{2}\left[\begin{array}{ccc}
1 & -i & -1+i \\
i & 1 & 1+i \\
1+i & -1+i & 0
\end{array}\right], \\
& C C^H=\frac{1}{2}\left[\begin{array}{ccc}
1 & -i & -1+i \\
i & 1 & 1+i \\
1+i & -1+i & 0
\end{array}\right] \frac{1}{2}\left[\begin{array}{ccc}
1 & -i & 1-i \\
i & 1 & -1-i \\
-1-i & 1-i & 0
\end{array}\right]=\left[\begin{array}{ccc}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{array}\right]=C^H C .
\end{aligned}
$$

故 $A, B, C$ 均為么正矩陣．
【98中山通訊類題、97政大資科】

Note
（1）等覧定義： $\begin{aligned} & A \text { 為么正 } \Leftrightarrow A^{-1}=A^H \\ & A \text { 為正交 } \Leftrightarrow A^{-1}=A^T\end{aligned}$
（2）等價定義：考慮方陣 $A$ ，則 $A$ 為么正（或正交）⇔ $A$ 的行（列）向量形成單範正交集。
【證明】
【99政大應數、103．104中央資工】
$A$ 的行向量形成單範正交