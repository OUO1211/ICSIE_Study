476
線性代數（下）

正定的性質
考慮正定矩陣 $A \in C^{n \times n}$ ，則
（1）$A$ 為正規矩陣。
（2）$A$ 的相異特徵根所對應的特徴向量必正交．
（3）$A$ 為正半定矩陣．
（4）$A$ 的所有特徵根皆為正．

【很重要】

（5）$A$ 為可逆．
（6）$A$ 的主對角項皆為正。

【91 政大應数】

（7）若 $A$ 與 $B$ 么正相似，則 $A$ 為正定矩陣 $\Leftrightarrow B$ 為正定矩陣．
【證明】
（1）$\because A$ 為 Hermitian，故 $A$ 為正規．
（2）$\because A$ 為正規，故 $A$ 的相異特徵根所對的特徵向量正交．
（3）$\because \forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^H A \boldsymbol{x}>0$ ，且 $\boldsymbol{x}=\mathbf{0}$ 時 $\boldsymbol{x}^H A \boldsymbol{x}=0$ ，故得 $\forall \boldsymbol{x} \in C^{n \times 1}, \boldsymbol{x}^H A \boldsymbol{x} \geq 0$ ．
（4）令 $\lambda$ 為 $A$ 的特徵根， $\boldsymbol{x} \neq \mathbf{0}$ ，使 $A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則
$$
\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H \lambda \boldsymbol{x}=\lambda \boldsymbol{x}^H \boldsymbol{x}=\lambda\|\boldsymbol{x}\|^2 \text {, 又因 } \forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^H A \boldsymbol{x}>0 \text {, 且 }\|\boldsymbol{x}\|^2>0 \therefore \lambda>0 \text {. }
$$
（5）若 $A$ 不可逆，則 $\operatorname{ker}(A) \neq\{\mathbf{0}\}$ ，即 $\exists \boldsymbol{x} \neq \mathbf{0}$ ，使 $A \boldsymbol{x}=\mathbf{0}, \therefore \boldsymbol{x}^H A \boldsymbol{x}=0$ ，與 $A$ 為正定矩陣矛盾．故 $A$ 為可逆矩陣．
（也可說：因 $A$ 的特徵根都為正數，故行列式 $=$ 所有特徵根乘積 $>0$ ）
（6）取 $\boldsymbol{x}=\boldsymbol{e}_i$ ，則 $\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{e}_i^H A \boldsymbol{e}_i=\boldsymbol{e}_i^H A^{(i)}=(A)_{i i}$ ，for $i=1,2, \ldots, n$ ．
因 $\boldsymbol{x} \neq \mathbf{0}, \therefore \boldsymbol{x}^H A \boldsymbol{x}>0, \therefore A$ 的主對角項都為正．
（7）因 $A, B$ 么正相似，故存在么正矩陣 $P$ 使得 $P^H A P=B$ ，
設 $A$ 為正定，則 $\forall \boldsymbol{x} \neq \mathbf{0}, \because P$ 可逆，故 $P \boldsymbol{x} \neq \mathbf{0}$ ，又因 $A$ 為正定，故得 $(P \boldsymbol{x})^H A(P \boldsymbol{x})>0$ ，
$\therefore \boldsymbol{x}^H B \boldsymbol{x}=\boldsymbol{x}^H P^H A P \boldsymbol{x}=(P \boldsymbol{x})^H A(P \boldsymbol{x})>0$ ，即 $B$ 為正定。
同理可得若 $B$ 為正定，則 $A$ 亦為正定．

Note
（1）對正定算子或實正定矩陣，上述性質亦成立。

【84．92 中興應數】

（2）對實對稱矩陣 $A$ ，下列彼此為等價條件：
（a）$A$ 為正定．
（b）$A$ 的所有特徵根都為正數．

【94竹師數教、96 清大統計、104 中正資工】