318
線性代數（下）

正交投影矩陣（orthogonal projection matrix）
對内積空間 $V$ 上的子空間 $W$ ，
若矩陣 $P$ 滿足 $P \boldsymbol{x}=\operatorname{proj}_W \boldsymbol{x}, \forall \boldsymbol{x}$ ，
則稱 $P$ 為一 $W$ 上的正交投影矩陣，有時簡稱投影矩陣。

【94 交大電資】

Note
（1）當 $W=C S(A)$ 為行獨立，取 $P=A\left(A^T A\right)^{-1} A^T$ 即為一正交投影矩陣。

【96 清大統計】

（2）設 $A_{m \times n}$ 行獨立，$P=A\left(A^T A\right)^{-1} A^T$ 為正交投影矩陣，則
（a）$P^2=P$ ．
【證明】
$$
P^2=\left(A\left(A^T A\right)^{-1} A^T\right)\left(A\left(A^T A\right)^{-1} A^T\right)=A\left(A^T A\right)^{-1} A^T A\left(A^T A\right)^{-1} A^T=A\left(A^T A\right)^{-1} A^T=P .
$$
（b）$P^T=P$ ．
【統計所】
【證明】
$$
P^T=\left(A\left(A^T A\right)^{-1} A^T\right)^T=\left(A^T\right)^T\left(\left(A^T A\right)^{-1}\right)^T A^T=A\left(\left(A^T A\right)^T\right)^{-1} A^T=A\left(A^T A\right)^{-1} A^T=P .
$$
（c） $\operatorname{CS}(P)=\operatorname{CS}(A)$ ．
【92中興應數、101台聯電機】
【證明】
任取 $\boldsymbol{y} \in \operatorname{CS}(P)$ ，則存在 $\boldsymbol{x}$ ，使 $\boldsymbol{y}=P \boldsymbol{x}$ ，
即 $\boldsymbol{y}=A\left(A^T A\right)^{-1} A^T \boldsymbol{x}=A\left[\left(A^T A\right)^{-1} A^T \boldsymbol{x}\right] \in C S(A), \therefore C S(P) \subseteq C S(A)$ ．
又任取 $\boldsymbol{y} \in C S(A)$ ，則存在 $\boldsymbol{x}$ ，使 $\boldsymbol{y}=A \boldsymbol{x}$ ，
故 $P \boldsymbol{y}=\left(A\left(A^T A\right)^{-1} A^T\right) A \boldsymbol{x}=A\left(A^T A\right)^{-1}\left(A^T A\right) \boldsymbol{x}=A \boldsymbol{x}=\boldsymbol{y}$ ，
$$
\therefore \boldsymbol{y} \in C S(P), \quad \therefore C S(A) \subseteq C S(P) .
$$

故得 $\operatorname{CS}(A)=\operatorname{CS}(P)$ ．
（3）若方陣 $P$ 滿足 $P^2=P, P^H=P$ ，則 $P$ 為投影在 $C S(P)=W$ 上的正交投影矩陣．