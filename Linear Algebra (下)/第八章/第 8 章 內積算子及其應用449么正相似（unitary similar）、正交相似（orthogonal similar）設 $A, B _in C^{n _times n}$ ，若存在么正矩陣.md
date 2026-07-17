第 8 章 內積算子及其應用
449

么正相似（unitary similar）、正交相似（orthogonal similar）
設 $A, B \in C^{n \times n}$ ，若存在么正矩陣 $P \in C^{n \times n}$ ，使得 $B=P^H A P$ ，則稱 $A$ 與 $B$ 么正相似。
設 $A, B \in R^{n \times n}$ ，若存在正交矩陣 $P \in R^{n \times n}$ ，使得 $B=P^T A P$ ，則稱 $A$ 與 $B$ 正交相似。
Note
（1）若 $A$ 與 $B$ 么正相似，則 $A$ 與 $B$ 相似．
（2）若 $A$ 與 $B$ 正交相似，則 $A$ 與 $B$ 相似。
（3）么正相似所保持的特性：
設 $A, B \in C^{n \times n}$ ，若 $A$ 與 $B$ 么正相似，則
（a）$A$ 為正規矩陣 $\Leftrightarrow B$ 為正規矩陣．
（b）$A$ 為 Hermitian ⇔ $B$ 為 Hermitian 矩陣．
（c）$A$ 為 Skew－Hermitian 矩陣 $\Leftrightarrow B$ 為 Skew－Hermitian 矩陣．
（d）$A$ 為么正矩陣 $\Leftrightarrow B$ 為么正矩陣．
（e） $\operatorname{tr}\left(A^H A\right)=\operatorname{tr}\left(B^H B\right)$ ．

【100台聯電機、100竹教應數】

（f）$\sum_{i, j=1}^n\left|A_{i j}\right|^2=\sum_{i, j=1}^n\left|B_{i j}\right|^2$ ．

【100竹教應數】

【證明】
因 $A, B$ 么正相似，故存在么正矩陣 $P$ 使得 $P^H A P=B$ ，
（a）設 $A$ 為正規，則 $A^H A=A A^H$ ，
故 $B^H B=\left(P^H A P\right)^H\left(P^H A P\right)=\left(P^H A^H P\right)\left(P^H A P\right)=P^H A^H A P =P^H A A^H P=P^H A P P^H A^H P=B B^H$ ，即 $B$ 為正規。
設 $B$ 為正規，則 $B^H B=B B^H$ ，
故 $A^H A=\left(P B P^H\right)^H\left(P B P^H\right)=\left(P B^H P^H\right)\left(P B P^H\right)=P B^H B P^H =P B B^H P^H=P B P^H P B^H P^H=A A^H$ ，即 $A$ 為正規，
（其實即將前半證明中的 $P$ 以 $P^H$ 代入即可。）
（b）～（f）請讀者自行練習。
（4）正交相似所保持的特性
設 $A, B \in R^{n \times n}$ ，若 $A$ 與 $B$ 正交相似，則
（a）$A$ 為對稱矩陣 $\Leftrightarrow B$ 為對稱矩陣．
（b）$A$ 為斜對稱 $\Leftrightarrow B$ 為斜對稱矩陣．
（c）$A$ 為正交矩陣 $\Leftrightarrow B$ 為正交矩陣。