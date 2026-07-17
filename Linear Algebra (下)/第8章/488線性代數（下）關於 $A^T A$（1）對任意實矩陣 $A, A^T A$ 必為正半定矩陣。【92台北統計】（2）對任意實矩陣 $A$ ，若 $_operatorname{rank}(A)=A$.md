488
線性代數（下）

關於 $A^T A$
（1）對任意實矩陣 $A, A^T A$ 必為正半定矩陣。

【92台北統計】

（2）對任意實矩陣 $A$ ，若 $\operatorname{rank}(A)=A$ 的行數，則 $A^T A$ 為正定矩陣．
【 89 中央統計、 92 台北統計、 101 政大統計】
【證明】
（1）$\forall \boldsymbol{x}, \boldsymbol{x}^T\left(A^T A\right) \boldsymbol{x}=\langle A \boldsymbol{x}, A \boldsymbol{x}\rangle=\|A \boldsymbol{x}\|^2 \geq 0$ ，即正半定．
（2）$\because \operatorname{rank}(A)=A$ 的行數，故 $A$ 行獨立，故 $\operatorname{ker}(A)=\{\mathbf{0}\}$ ，
即 $A \boldsymbol{x}=\mathbf{0}$ 只 $\boldsymbol{x}=\mathbf{0}$ 為解，
$\forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^T\left(A^T A\right) \boldsymbol{x}=<A \boldsymbol{x}, A \boldsymbol{x}>=\|A \boldsymbol{x}\|^2 \geq 0$ ，但 $A \boldsymbol{x} \neq \mathbf{0}$ ，when $\boldsymbol{x} \neq \mathbf{0}$ ，
故得 $\forall \boldsymbol{x} \neq \mathbf{0}, \boldsymbol{x}^T\left(A^T A\right) \boldsymbol{x}>0$ ，
即 $A^T A$ 為正定矩陣。

Note
對任意實矩陣 $A, A^T A$ 之特徵根必為非負實數。

【96．102．104 中央資工、105 交大資工】