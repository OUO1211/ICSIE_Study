474
線性代數（下）

8－3 正定與正半定

正定（positive definite）、正半定（positive semi definite）
（1）考慮 $V$ 上的線性算子 $T$ ，
若 $T$ 為自伴算子且 $<T(\boldsymbol{v}), \boldsymbol{v} \gg 0, \forall \boldsymbol{v} \in V-\{\boldsymbol{0}\}$ ，則稱 $T$ 為正定算子．
若 $T$ 為自伴算子且 $\langle T(\boldsymbol{v}), \boldsymbol{v}\rangle \geq 0, \forall \boldsymbol{v} \in V$ ，則稱 $T$ 為正半定算子．
（2）考慮 $A \in C^{n \times n}$ ，
若 $A$ 為 Hermitian 且 $\boldsymbol{x}^H A \boldsymbol{x}>0, \forall \boldsymbol{x} \in C^{n \times 1}-\{\mathbf{0}\}$ ，則稱 $A$ 為正定矩陣．
若 $A$ 為 Hermitian 且 $\boldsymbol{x}^H A \boldsymbol{x} \geq 0, \forall \boldsymbol{x} \in C^{n \times 1}$ ，則稱稱 $A$ 為正半定矩陣．
（3）考慮 $A \in R^{n \times n}$ ，
若 $A$ 為對稱且 $\boldsymbol{x}^T A \boldsymbol{x}>0, \forall \boldsymbol{x} \in R^{n \times 1}-\{\mathbf{0}\}$ ，則稱 $A$ 為正定矩陣。
若 $A$ 為對稱且 $\boldsymbol{x}^T A \boldsymbol{x} \geq 0, \forall \boldsymbol{x} \in R^{n \times 1}$ ，則稱 $A$ 為正半定矩陣．
【98 中央統計、104 中央數學、104．105 中興統計】
Note
（1）正半定有時也稱非負定（non－negative definite）．
（2）一般將 $\boldsymbol{x}^T A \boldsymbol{x}$（或 $\boldsymbol{x}^H A \boldsymbol{x}$ ）稱作 $A$ 的二次式（quadratic form），以 $Q(\boldsymbol{x})$ 表之。
（3）因為 $A \in C^{n \times n}$ 時，$A$ 為 Hermitian $\Leftrightarrow \boldsymbol{x}^H A \boldsymbol{x} \in R$ ，（8－1 證過了）
故判斷 $A$ 是否為正定矩陣，其實只需正定性成立就夠了，即 $\boldsymbol{x}^H A \boldsymbol{x} \geq 0, \forall \boldsymbol{x} \in C^{n \times 1}$ 。
（4）對實矩陣 $A$ ，其實不一定要對稱矩陣才可滿足正定性，只是比較常對對稱矩陣來討論，有些就只以滿足正定性當成正定矩陣的定義，而本章大部分都是對對稱矩陣來定義。
（5）若 $A, B$ 均為正定矩陣，則 $A+B$ 也是，$A+I$ 也是．
【101 中山應數】
【證明】【 89 成大統計、 93 台科資工、 94 台大資工、 94 中正數學、 94 嘉義應數】 $\forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^H A \boldsymbol{x}>0, \boldsymbol{x}^H B \boldsymbol{x}>0$,
$\therefore \boldsymbol{x}^H(A+B) \boldsymbol{x}=\boldsymbol{x}^H A \boldsymbol{x}+\boldsymbol{x}^H B \boldsymbol{x}>0$ ，所以 $A+B$ 為正定矩陣．
$\therefore \boldsymbol{x}^H(A+I) \boldsymbol{x}=\boldsymbol{x}^H A \boldsymbol{x}+\boldsymbol{x}^H I \boldsymbol{x}=\boldsymbol{x}^H A \boldsymbol{x}+\|\boldsymbol{x}\|^2>0$ ，所以 $A+I$ 為正定矩陣．