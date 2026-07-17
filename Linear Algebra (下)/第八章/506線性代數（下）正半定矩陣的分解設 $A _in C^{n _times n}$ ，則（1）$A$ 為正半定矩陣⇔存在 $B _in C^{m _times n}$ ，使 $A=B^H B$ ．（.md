506
線性代數（下）

正半定矩陣的分解
設 $A \in C^{n \times n}$ ，則
（1）$A$ 為正半定矩陣⇔存在 $B \in C^{m \times n}$ ，使 $A=B^H B$ ．
（2）$A$ 為正半定矩陣⇔存在正半定矩陣 $B$ ，使 $A=B^2$ ．
【證明】
（1）$\Rightarrow \because A$ 為正半定矩陣，故 $A$ 為正規矩陣，故 $A$ 可么正對角化，
故存在么正矩陣 $P \in C^{n \times n}$ ，使 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \lambda_2, \ldots, \lambda_n\right)$ ，
其中，$\lambda_i$ 為 $A$ 的特徵根，均為非負。
故得 $A=P D P^H=P \sqrt{D} \sqrt{D} P^H=\left(P(\sqrt{D})^H\right)\left(\sqrt{D} P^H\right)=\left((\sqrt{D}) P^H\right)^H\left(\sqrt{D} P^H\right)=B^H B$ ，
其中，$B$ 定義為 $\sqrt{D} P^H, \sqrt{D}$ 定義為 $\operatorname{diag}\left(\sqrt{\lambda_1}, \sqrt{\lambda_2}, \ldots, \sqrt{\lambda_n}\right)$ ， $\Leftarrow \forall \boldsymbol{x} \in C^{n \times n}, \boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H B^H B \boldsymbol{x}=(B \boldsymbol{x})^H B \boldsymbol{x}=\|B \boldsymbol{x}\|^2 \geq 0$ ，故 $A$ 為正半定矩陣．
（2）$\Rightarrow \because A$ 為正半定矩陣，故 $A$ 為正規矩陣，故 $A$ 可么正對角化，
故存在么正矩陣 $P \in C^{n \times n}$ ，使 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \lambda_2, \ldots, \lambda_n\right)$ ，
其中，$\lambda_i$ 為 $A$ 的特徵根，均為非負。
故得 $A=P D P^H=P \sqrt{D} \sqrt{D} P^H=\left(P(\sqrt{D}) P^H\right)\left(P \sqrt{D} P^H\right)=B^2$ ，
其中，$B$ 定義為 $P \sqrt{D} P^H, \sqrt{D}$ 定義為 $\operatorname{diag}\left(\sqrt{\lambda_1}, \sqrt{\lambda_2}, \ldots, \sqrt{\lambda_n}\right)$ ，
而因 $\sqrt{D}$ 為正半定矩陣，且 $B$ 與 $\sqrt{D}$ 么正相似，故 $B$ 亦為正半定矩陣．
$\Leftarrow B$ 為正半定，所以特徵根均非負，所以 $B^2$ 特徵根都非負，故 $A$ 為正半定矩陣．

Note
（1）對稱矩陣 $A \in R^{n \times n}$ ，也有類似性質．
（2）上述性質中的 $B$ 不一定為方陣。