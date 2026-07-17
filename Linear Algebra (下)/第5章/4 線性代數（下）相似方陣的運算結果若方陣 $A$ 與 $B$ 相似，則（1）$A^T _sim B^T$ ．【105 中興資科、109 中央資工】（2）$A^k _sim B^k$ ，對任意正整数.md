4 線性代數（下）



相似方陣的運算結果

若方陣 $A$ 與 $B$ 相似，則

（1）$A^T \sim B^T$ ．

【105 中興資科、109 中央資工】

（2）$A^k \sim B^k$ ，對任意正整数 $k$ ．

【104．109 中央資工、105 中興資科】

（3）$c A \sim c B$ ，對任意純量係數 $c$ 。

（4）$A+c I \sim B+c I$ ，對任意純量係數 $c$ 。

（5）$f(A) \sim f(B)$ ，對任意多項式 $f$ ．

【94 彰師資工、105 中興資科】

（6）$A^{-1} \sim B^{-1}$ ，（若 $A, B$ 均可逆）．

【104．109 中央資工】

【證明】

$\because A \sim B$ ，所以存在可逆方陣 $P$ 使得 $B=P^{-1} A P$ ，

（1）$B^T=\left(P^{-1} A P\right)^T=P^T A^T\left(P^{-1}\right)^T=P^T A^T\left(P^T\right)^{-1}$ ，取 $Q^{-1}=P^T$ ，故得 $B^T=Q^{-1} A^T Q$ ，即 $A^T \sim B^T$ ，

即得 $B^k=\left(P^{-1} A P\right)^k=\overbrace{\left(P^{-1} A P\right)\left(P^{-1} A P\right)\left(P^{-1} A P\right) \cdots\left(P^{-1} A P\right)}^k$

$$

=\overbrace{P^{-1} A P P^{-1} A P P^{-1} A P \cdots P^{-1} A P}^k=P^{-1} A^k P,

$$



故得 $A^k \sim B^k$ ．

（3）$c B=c\left(P^{-1} A P\right)=P^{-1}(c A) P$ ，故得 $c A \sim c B$ 。

（4）$B+c I=P^{-1} A P+c I=P^{-1} A P+P^{-1}(c I) P=P^{-1}(A+c I) P$ ，故得 $(A+c I) \sim(B+c I)$ ．

（5）設 $f(x)=a_0+a_1 x+a_2 x^2+\cdots+a_n x^n=\sum_{i=0}^n a_i x^i, \quad \forall i, \quad a_i \in F$ ，

則 $f(B)=\sum_{i=0}^n a_i B^i=\sum_{i=0}^n a_i\left(P^{-1} A P\right)^i=\sum_{i=0}^n a_i\left(P^{-1} A^i P\right)=P^{-1}\left(\sum_{i=0}^n a_i A^i\right) P=P^{-1} f(A) P$

故得 $f(A) \sim f(B)$ ．

（6）$B^{-1}=\left(P^{-1} A P\right)^{-1}=P^{-1} A^{-1}\left(P^{-1}\right)^{-1}=P^{-1} A^{-1} P$ ，故得 $A^{-1} \sim B^{-1}$ ．