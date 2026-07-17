第 8 章 內積算子及其應用
533

【證明】
（a）$\|\boldsymbol{A}\|_2^2=\lambda_{\text {max }}\left(A^T A\right)=\lambda_{\text {max }}\left(A A^T\right)=\lambda_{\text {max }}\left(\left(A^T\right)^T A^T\right)=\left\|A^T\right\|_2^2$ ．
（b）$\left\|A^T A\right\|_2=\sqrt{\lambda_{\text {max }}\left(A^T A\right)^T\left(A^T A\right)}=\sqrt{\lambda_{\text {max }}\left(A^T A\right)^2}=\sqrt{\left[\lambda_{\text {max }}\left(A^T A\right)\right]^2}$
$$
=\left(\sqrt{\left[\lambda_{\max }\left(A^T A\right)\right]}\right)^2=\|A\|_2^2 .
$$
（3）考慮 $n$ 階實對稱矩陣 $A$ ，若 $\lambda_1, \ldots, \lambda_n$ 為 $A$ 的特徵根，則 $\|A\|_2=\max \left\{\left|\lambda_1\right|, \ldots,\left|\lambda_n\right|\right\}$
【證明】
【90政大應數、101清大應數】
$\because A$ 為對稱矩陣，故 $A^T A=A^2$ ，故 $\lambda_1^2, \lambda_2^2, \ldots, \lambda_n^2$ 為 $A^T A$ 的特徵根，
$$
\therefore\|A\|_2=\sqrt{\lambda_{\max }\left(A^T A\right)}=\max \left\{\sqrt{\lambda_1^2}, \sqrt{\lambda_2^2}, \ldots, \sqrt{\lambda_n^2}\right\}=\max \left\{\left|\lambda_1\right|,\left|\lambda_2\right|, \ldots,\left|\lambda_n\right|\right\} .
$$
（4）若 $Q$ 為正交矩陣，則 $\|Q\|_2^2=1$ ．
【證明】
$\because Q$ 為正交，故 $Q^T Q=I$ ，故 $\|Q\|_2^2=\lambda_{\text {max }}\left(Q^T Q\right)=\lambda_{\text {max }}(I)=1$ ．
（5）若 $A$ 為實對稱正定矩陣，則 $\|A\|_2=\lambda_{\max }(A)$ ．
【證明】

【94中央數學】

設 $\lambda_1, \lambda_2, \ldots, \lambda_n$ 為 $A$ 的所有特徵根，
則由（3）得 $\|A\|_2=\max \left\{\left|\lambda_1\right|,\left|\lambda_2\right|, \ldots,\left|\lambda_n\right|\right\}$ ，
又因 $A$ 為正定矩陣，故 $\lambda_i>0, \forall i$ ，
故 $\therefore\|A\|_2=\max \left\{\lambda_1, \lambda_2, \ldots, \lambda_n\right\}$ ．