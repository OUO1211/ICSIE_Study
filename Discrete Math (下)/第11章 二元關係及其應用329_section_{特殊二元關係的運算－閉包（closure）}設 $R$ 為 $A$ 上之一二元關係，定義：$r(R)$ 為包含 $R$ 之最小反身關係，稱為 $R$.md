第11章 二元關係及其應用
329

\section*{特殊二元關係的運算－閉包（closure）}

設 $R$ 為 $A$ 上之一二元關係，定義：
$r(R)$ 為包含 $R$ 之最小反身關係，稱為 $R$ 之反身包（reflexive closure）。
$s(R)$ 為包含 $R$ 之最小對稱關係，稱為 $R$ 之對稱包（symmetric closure）。
$t(R)$ 為包含 $R$ 之最小遞移關係，稱為 $R$ 之遞移包（transitive closure），也記成 $R^{+}$。
【93 交大資工】【 95 中興資科】【 96 中興資網】
Note
\begin{itemize}
\item[（1）] 求各閉包的方式，就是先寫出原來的 $R$ ，然後再加入一些有序對，使滿足反身（或對稱、遞移），加到剛好滿足即可；而如果本身就具有那個特色，就不需要再加新的有序對。
\item[（2）] 做遞移閉包時，新加入的邊也要跟舊的邊一起滿足遞移性，後面還要會使用 Warshall 演算法幫助求算遞移閉包。
\item[（1）] Rosen 的書是把 $t(R)$ 記成 $R^*$ 。
\item[（2）] $r(R)=R \bigcup R^0$ ，其中 $R^0=\{(x, x) \mid \forall x \in A\}$ 。
\item[（3）] $s(R)=R \bigcup R^{-1}$ ．
\item[（4）] $\bigcup_{l=1}^{\infty} R^l=R^{+}$為包含 $R$ 最小的遞移關係。
\end{itemize}

【102中央資工】【101 北科資工】

【證明】
\begin{itemize}
\begin{itemize}
\item[（1）] 由 $R^{+}$的定義可得 $R \subseteq R^{+}$．
\item[（2）] $R^{+}$有遞移性：
若 $(a, b) \in R^{+}$且 $(b, c) \in R^{+}$，
即代表在 $R$ 的關係圖形中 $a$ 有 path 可走到 $b$ ，且 $b$ 有 path 可走到 $c$ ，
故 $a$ 有 path 可走到 $c$ ，故 $(a, c) \in R^{+}$。
\item[（3）] 若 $S$ 為包含 $R$ 的一種遞移關係，則 $R^{+} \subseteq S$ ：
因為 $S$ 有遞移性，故 $S^{+}$也有遞移性，且 $S^{+} \subseteq S$ ，
而因為 $R \subseteq S$ ，故 $R^{+} \subseteq S^{+}$，故 $R^{+} \subseteq S^{+} \subseteq S$ ，得證。
\end{itemize}
\item[（5）] $r(t(R))$ 為包含 $R$ 之最小反身遞移關係，稱為 $R$ 之反身遞移包（reflexive transitive closure）
，記成 $R^*=R^0 \bigcup R^{+}=R^0 \bigcup R^1 \bigcup R^2 \bigcup \ldots$ 。
\item[（6）] $t(s(r(R)))$ 表示包含 $R$ 之等價關係稱為 $R$ 之等價包。
\item[（7）] 若 $R$ 有對稱性，則 $t(R)$ 也有對稱性。【91 交大資科】【94 中山電機】【96 交大資訊】［證明］
若 $R$ 有對稱性，則 $R^2, R^3, \ldots$ 有對稱性，（可從關係矩陣為對稱矩陣看出）
\end{itemize}