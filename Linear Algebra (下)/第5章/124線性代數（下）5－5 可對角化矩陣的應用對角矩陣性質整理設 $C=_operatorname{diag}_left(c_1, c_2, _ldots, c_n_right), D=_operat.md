124

線性代數（下）



5－5 可對角化矩陣的應用



對角矩陣性質整理

設 $C=\operatorname{diag}\left(c_1, c_2, \ldots, c_n\right), D=\operatorname{diag}\left(d_1, d_2, \ldots, d_n\right)$ 為對角矩陣，則

（1）$C+D=\operatorname{diag}\left(c_1+d_1, c_2+d_2, \ldots, c_n+d_n\right)$ ．

（2）$k D=\operatorname{diag}\left(k d_1, k d_2, \ldots, k d_n\right)$ ．

（3）$C D=\operatorname{diag}\left(c_1 d_1, c_2 d_2, \ldots, c_n d_n\right)$ ．

（4）$D^{-1}=\operatorname{diag}\left(d_1^{-1}, d_2^{-1}, \ldots, d_n^{-1}\right)$ ，若 $D$ 可逆．

（5）$D^m=\operatorname{diag}\left(d_1^m, d_2^m, \ldots, d_n^m\right), m \in Z^{+}$．

（6）$f(D)=\operatorname{diag}\left(f\left(d_1\right), f\left(d_2\right), \ldots, f\left(d_n\right)\right), f(x)$ 為多項式。

（7）$D$ 的特徵根為 $d_1, d_2, \ldots, d_n$ ．

（8） $\operatorname{det}(D)=d_1 d_2 \ldots d_n$ ．

Note

設多項式 $f(x)$ ，可逆矩陣 $P$ ，對角矩陣 $D$ ，滿足 $A=P D P^{-1}$ ，則 $f(A)=P f(D) P^{-1}$ 。

（即若 $A$ 可對角化，且 $f(x)$ 為多項式，則 $f(A)$ 亦可以對角化．）

【證明】



【95高雄應數】



令 $f(x)=\sum_{i=0}^{\infty} a_i x^i$ ，設 $D=\operatorname{diag}\left(d_1, d_2, \ldots, d_n\right)=P^{-1} A P$ ，則 $A=P D P^{-1}$ ，且

$f(A)=\sum_{i=0}^{\infty} a_i A^i=\sum_{i=0}^{\infty} a_i\left(P D P^{-1}\right)^i=\sum_{i=0}^{\infty} a_i\left(P D^i P^{-1}\right)=P\left(\sum_{i=0}^{\infty} a_i D^i\right) P^{-1}=P f(D) P^{-1}$ ，故得證．