第 5 章 對角化理論

125



指數矩陣 $e^A$

定義 $e^A=\sum_{i=0}^{\infty} \frac{A^i}{i!}=I+\frac{A}{1}+\frac{A^2}{2!}+\frac{A^3}{3!}+\ldots$.

【93 交大應数、101 台大数學】

（1）若 $A$ 與 $B$ 相似，則 $e^A$ 與 $e^B$ 相似。

【93成大统計】

（2）若 $\lambda$ 為 $n$ 階方陣 $A$ 對應於 $\boldsymbol{x}$ 的特徵根，則 $e^\lambda$ 為 $e^A$ 對應於 $\boldsymbol{x}$ 的特徵根。

【93成大統計、101台大数學】

【證明】

（1）設可逆方陣 $P$ 使 $B=P^{-1} A P$ ，

則 $e^B=f(B)=\sum_{i=0}^{\infty} \frac{B^i}{i!}=\sum_{i=0}^{\infty} \frac{\left(P^{-1} A P\right)^i}{i!}=\sum_{i=0}^{\infty} \frac{P^{-1} A^i P}{i!}=P^{-1}\left(\sum_{i=0}^{\infty} \frac{A^i}{i!}\right) P=P^{-1} f(A) P=P^{-1} e^A P$ ，

即 $e^A$ 與 $e^B$ 相似．

（2）設 $\lambda$ 為 $A$ 的特徵根，滿足 $A \boldsymbol{x}=\lambda \boldsymbol{x}, ~ \boldsymbol{x} \neq \mathbf{0}$ ，

則 $A^i \boldsymbol{x}=\lambda^i \boldsymbol{x}$ ，且 $e^A \boldsymbol{x}=\sum_{i=0}^{\infty} \frac{A^i}{i!} \boldsymbol{x}=\sum_{i=0}^{\infty} \frac{A^i \boldsymbol{x}}{i!}=\sum_{i=0}^{\infty} \frac{\lambda^i \boldsymbol{x}}{i!}=e^\lambda \boldsymbol{x}$ ，即 $e^\lambda$ 為相對於 $\boldsymbol{x}$ 的特徵根．

Note

（1） $\operatorname{det}\left(e^A\right)=e^{\operatorname{tr}(A)}$ ．



【93成大統計】



【證明】

設 $n$ 方陣 $A$ 的所有特徵根為：$\lambda_1, \lambda_2, \ldots, \lambda_n$ ，則 $\operatorname{tr}(A)=A$ 的所有特徵根的和，

則可得 $e^A$ 的所有特徵根為 $e^{\lambda_i}, ~ i=1,2, \ldots, n$ ，

故 $\operatorname{det}\left(e^A\right)=e^A$ 的所有特徵根的積 $=e^{\lambda_1} \cdot e^{\lambda_2} \cdots \cdots e^{\lambda_n}=e^{\lambda_1+\lambda_2+\ldots+\lambda_n}=e^{\operatorname{tr}(A)}$ ．

（2）若 $A$ 可對角化成 $D$ ，則 $e^A=P e^D P^{-1}$ 為可逆矩陣．

【95彰師統計】

【證明】

設可逆矩陣 $P$ 使 $A=P D P^{-1}$ ，其中 $D=\operatorname{diag}\left(\lambda_1, \ldots, \lambda_n\right), \lambda_i$ 為 $A$ 的特徵根，

則 $\operatorname{det}\left(e^A\right)=\operatorname{det}\left(P e^D P^{-1}\right)=\operatorname{det}\left(e^D\right)=\operatorname{det}\left(\operatorname{diag}\left(e^{\lambda_1}, \ldots, e^{\lambda_n}\right)\right)=e^{\lambda_1+\ldots+\lambda_n} \neq 0$ ，故 $e^A$ 可逆。

（3）若 $A$ 為實對稱矩陣，則 $e^A$ 為對稱且正定矩陣．

【證明】

$\left(e^A\right)^T=\left(\sum_{i=0}^{\infty} \frac{A^i}{i!}\right)^T=\sum_{i=0}^{\infty} \frac{\left(A^i\right)^T}{i!}=\sum_{i=0}^{\infty} \frac{\left(A^T\right)^i}{i!}=\sum_{i=0}^{\infty} \frac{A^i}{i!}=e^A$ ，即 $e^A$ 為對稱矩陣．

又因 $A$ 為實對稱矩陣，故 $A$ 的所有特徵根 $\lambda_1, \ldots, \lambda_n \in R$ ，

$\therefore e^A$ 的特徵根 $e^{\lambda_i}, \ldots, e^{\lambda_n}$ 都為正，故 $e^A$ 為正定矩陣。