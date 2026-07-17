第8章 各內積算子及其應用
505

正半定矩陣的性質
考虑正半定矩陣 $A \in C^{n \times n}$ ，則
（1）$A$ 為正規矩陣。
（2）$A$ 的相異特徵根所對應的特徵向量必正交．
（3）$A$ 的所有特徵根皆為非負．

【88 清大统計】

（4）$A$ 的主對角項皆為非負．
（5）若 $A$ 與 $B$ 么正相似，則 $A$ 為正半定矩陣 $\Leftrightarrow B$ 為正半定矩陣．
【證明】
（1）$\because A$ 為 Hermitian，故 $A$ 為正規．
（2）$\because A$ 為正規，故 $A$ 的相異特徵徵根所對的特徵向量正交．
（3）令 $\lambda$ 為 $A$ 的特徵根， $\boldsymbol{x} \neq \mathbf{0}$ ，使 $A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則
$$
\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H \lambda \boldsymbol{x}=\lambda \boldsymbol{x}^H \boldsymbol{x}=\lambda\|\boldsymbol{x}\|^2,
$$

又因 $\forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^H A \boldsymbol{x} \geq 0$ ，且 $\|\boldsymbol{x}\|^2>0 \therefore \lambda \geq 0$ ．
（4）取 $\boldsymbol{x}=\boldsymbol{e}_i$ ，則 $\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{e}_i^H A \boldsymbol{e}_i=\boldsymbol{e}_i^H A^{(i)}=(A)_{i i}$ ，for $i=1,2, \ldots, n$ ，因 $\boldsymbol{x} \neq \mathbf{0}, \therefore \boldsymbol{x}^H A \boldsymbol{x} \geq 0, \therefore A$ 的主對角項都為非負．
（5）因 $A, B$ 么正相似，故存在么正矩陣 $P$ 使得 $P^H A P=B$ ，設 $A$ 為正半定，則 $\forall x \in C^{n \times 1}, P x \in C^{n \times 1},(P x)^H A(P x) \geq 0$ ， $\therefore \boldsymbol{x}^H B \boldsymbol{x}=\boldsymbol{x}^H P^H A P \boldsymbol{x}=(P \boldsymbol{x})^H A(P \boldsymbol{x}) \geq 0$ ，即 $B$ 為正半定．
同理可得若 $B$ 為正半定，則 $A$ 亦為正半定．

Note
（1）正半定對稱矩陣 $A \in R^{n \times n}$ ，也有類似上述性質．
（2）對實對稱矩陣 $A$ ，下列彼此為等價條件：
（a）$A$ 為正半定．
（b）$A$ 的所有特徵根都非負．
（c）$A$ 的所有主子矩陣（principal submatrix）的行列式都是非負．