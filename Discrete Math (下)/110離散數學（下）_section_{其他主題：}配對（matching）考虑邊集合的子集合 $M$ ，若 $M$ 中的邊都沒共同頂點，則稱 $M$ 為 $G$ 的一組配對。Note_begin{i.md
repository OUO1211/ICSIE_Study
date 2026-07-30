110
離散數學（下）

\section*{其他主題：}

配對（matching）
考虑邊集合的子集合 $M$ ，若 $M$ 中的邊都沒共同頂點，則稱 $M$ 為 $G$ 的一組配對。
Note
\begin{itemize}
\item[（1）] 配對又稱為邊獨立集。
\item[（2）] 如果 $M$ 中的邊均不與點 $v$ 相連，則稱點 $v$ 為 $M$－未飽和點（ $M$－unsaturated）。
\item[（3）] 稱由 $M$ 中的某些邊與 $E-M$ 中的某些邊交錯而成的 path 為 $M$－交錯路徑（ $M$－alternating path）。（單一個邊也算是 $M$－交錯路徑）
\item[（4）] 稱兩端點均為 $M$－未飽和點的交錯路徑為 $M$－可增長路徑（ $M$－augmenting path）。例如右圖中，
$$
\begin{aligned}
& M_1=\{(a, b),(c, f),(g, z)\}, \\
& M_2=\{(a, d),(c, f),(b, e),(g, z)\} \text { 均為 } G \text { 的 }
\end{aligned}
$$
matching。
而 $d-c-f-g-z-e$ 即為一 $M_1$ 可增長路徑。
\item[（5）] A matching is not maximum if there is an augmenting path．
【證明】
設 $M$ 為圖 $G$ 中之一組 matching，
令 $P: v_1-v_2-v_3-v_4-\ldots-v_{2 k-2}-v_{2 k-1}-v_{2 k}$ 為一 $M$－augmenting path，
即 $\left(v_{2 t-1}, v_{2 t}\right) \notin M, \forall t=1,2, \ldots, k$ ，且 $\left(v_{2 t}, v_{2 t+1}\right) \in M, \forall t=1,2, \ldots, k-1$ ，
且 $|P|=2 k-1,|P \cap M|=k-1,|P-M|=k$ ，
Now，考慮另一組邊集合：$M^*=(M-P) \cup(P-M)=M \oplus P$ ，
（即刪去 $M$ 中與 $P$ 交集的部分，保留 $M$ 的其他邊並加入 $P$ 中不屬於 $M$ 的部分）
則因為此 $M^*$ 中的邊亦彼此獨立，故為一 matching，且
$\left|M^*\right|=|M-P|+|P-M|=|M|+1$ ，即 $M$ 並不為 $G$ 之最大 matching。
\item[（6）] 完美配對（perfect matching）：若 $G$ 中的點均能被 $M$ 中的邊所連，則稱 $M$ 為一完美配對。例如上圖中，$M_2=\{(a, d),(c, f),(b, e),(g, z)\}$ 即為一完美配對。
\end{itemize}