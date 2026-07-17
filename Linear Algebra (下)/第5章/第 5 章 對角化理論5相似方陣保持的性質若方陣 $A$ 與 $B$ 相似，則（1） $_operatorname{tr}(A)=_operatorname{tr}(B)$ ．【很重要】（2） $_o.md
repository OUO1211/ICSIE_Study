第 5 章 對角化理論

5



相似方陣保持的性質

若方陣 $A$ 與 $B$ 相似，則

（1） $\operatorname{tr}(A)=\operatorname{tr}(B)$ ．



【很重要】



（2） $\operatorname{det}(A)=\operatorname{det}(B)$ ．



【很重要】



（3） $\operatorname{rank}(A)=\operatorname{rank}(B)$ ．

（4）nullity $(A)=\operatorname{nullity}(B)$ ．

【證明】

設可逆矩陣 $P$ 使 $B=P^{-1} A P$ ，則

（1） $\operatorname{tr}(B)=\operatorname{tr}\left(P^{-1} A P\right)=\operatorname{tr}\left((A P) P^{-1}\right)=\operatorname{tr}\left(A P P^{-1}\right)=\operatorname{tr}(A)$ ．

（2） $\operatorname{det}(B)=\operatorname{det}\left(P^{-1} A P\right)=\operatorname{det}\left((A P) P^{-1}\right)=\operatorname{det}\left(A P P^{-1}\right)=\operatorname{det}(A)$ ．

（3） $\operatorname{rank}(B)=\operatorname{rank}\left(P^{-1} A P\right)=\operatorname{rank}(A P)=\operatorname{rank}(A)$ ．

（4）nullity $(B)=n-\operatorname{rank}(B)=n-\operatorname{rank}(A)=\operatorname{nullity}(A)$ ，其中 A，B 為 $n \times n$ 矩陣．



Note

（1）因此，由上述性質，若發現某給定兩矩陣的上述各量不相同，則必不相似。例如 $\left[\begin{array}{ll}1 & 3 \\ 2 & 4\end{array}\right]$ 與 $\left[\begin{array}{ll}1 & 3 \\ 2 & 6\end{array}\right]$ 不相似。

（2）但若 $\operatorname{det}(A)=\operatorname{det}(B), ~ \operatorname{tr}(A)=\operatorname{tr}(B), ~ \operatorname{rank}(A)=\operatorname{rank}(B)$ ，則 $A$ 與 $B$ 仍有可能不相似．

【證明】



【94 中興應數】



考慮 $A=\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right], B=\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right]$ ，

若存在可逆矩陣 $P=\left[\begin{array}{ll}a & b \\ c & d\end{array}\right]$ 使 $A=P^{-1} B P$ ，（即 $P A=B P$ ），則

$\left[\begin{array}{ll}a & b \\ c & d\end{array}\right]\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right]=\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right]\left[\begin{array}{ll}a & b \\ c & d\end{array}\right]$ ，即 $\left[\begin{array}{ll}a & b \\ c & d\end{array}\right]=\left[\begin{array}{cc}a & b \\ a+c & b+d\end{array}\right]$ 得 $a=b=0$ ，

即 $P=\left[\begin{array}{ll}0 & 0 \\ c & d\end{array}\right]$ ，但這樣的 $P$ 無論如何是不會可逆的，

故 $A$ 與 $B$ 不相似．