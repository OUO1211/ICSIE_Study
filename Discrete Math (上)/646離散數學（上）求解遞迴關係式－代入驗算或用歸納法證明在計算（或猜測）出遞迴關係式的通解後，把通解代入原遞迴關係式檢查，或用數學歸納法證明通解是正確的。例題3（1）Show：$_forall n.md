646
離散數學（上）

求解遞迴關係式－代入驗算或用歸納法證明
在計算（或猜測）出遞迴關係式的通解後，把通解代入原遞迴關係式檢查，或用數學歸納法證明通解是正確的。

例題

3

（1）Show：$\forall n \in N, \operatorname{Ack}(1, n)=n+2$ ．
【93成大工科】【106成大電機】
（2）Show：$\forall n \in N, \operatorname{Ack}(2, n)=2 n+3$ ．
（3）Show：$\forall n \in N, \operatorname{Ack}(3, n)=2^{n+3}-3$ ．
（4） $\operatorname{Ack}(3,2)=$ ？

【92清大資應】【96師大資工】

（5） $\operatorname{Ack}(1,3)=? \quad \operatorname{Ack}(2,3)=? \quad \operatorname{Ack}(4,1)=?$【96師大資工】【106成大電機】

解（1）對 $n$ 做歸納法：$n=0$ 時， $\operatorname{Ack}(1,0)=2=0+2$ ，原式成立，
設 $n=k \geq 0$ 時，原式成立，則 $n=k+1$ 時，
$$
\operatorname{Ack}(1, k+1)=\operatorname{Ack}(0, \operatorname{Ack}(1, k))=\operatorname{Ack}(0, k+2)=k+3=(k+1)+2,
$$

原式亦成立。
（2）請讀者自行練習。
（3）請讀者自行練習。
（4） $\operatorname{Ack}(3,1)=\operatorname{Ack}(2, \operatorname{Ack}(3,0))=\operatorname{Ack}(2, \operatorname{Ack}(2,1))=\operatorname{Ack}(2,5)=13$ ，
$$
\therefore \operatorname{Ack}(3,2)=\operatorname{Ack}(2, \operatorname{Ack}(3,1))=\operatorname{Ack}(2,13)=29 \circ
$$
（5）
$$
\begin{aligned}
& \operatorname{Ack}(1,3)=3+2=5 \\
& \operatorname{Ack}(2,3)=9 \\
& \operatorname{Ack}(4,1)=8 \cdot 2^{13}-3
\end{aligned}
$$