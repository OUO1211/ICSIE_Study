第 8 章 內積筫子及其應用
495

正定矩陣的分解
設 $A \in C^{n \times n}$ ，則
（1）$A$ 為正定矩陣⇔存在可逆矩陣 $B \in C^{n \times n}$ ，使 $A=B^H B$ ．

【93政大應数】

（2）$A$ 為正定矩陣⇔存在矩陣 $B \in C^{m \times n}, \operatorname{rank}(B)=n$ ，使 $A=B^H B$ ．
（3）$A$ 為正定矩陣⇔存在正定矩陣 $B$ ，使 $A=B^2$ ．
【95中興應数、98 交大统胡】
【證明】
（1）$\Rightarrow \because A$ 為正定矩陣，故 $A$ 為正規矩陣，故 $A$ 可么正對角化，
故存在么正矩陣 $P \in C^{n \times n}$ ，使 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \lambda_2, \ldots, \lambda_n\right)$ ，
其中，$\lambda_i$ 為 $A$ 的特徵根，均為正。
故得 $A=P D P^H=P \sqrt{D} \sqrt{D} P^H=\left(P(\sqrt{D})^H\right)\left(\sqrt{D} P^H\right)=\left((\sqrt{D}) P^H\right)^H\left(\sqrt{D} P^H\right)=B^H B$ ，
其中，$B$ 定義為 $\sqrt{D} P^H, \sqrt{D}$ 定義為 $\operatorname{diag}\left(\sqrt{\lambda_1}, \sqrt{\lambda_2}, \ldots, \sqrt{\lambda_n}\right)$ ，
而因 $\sqrt{D}, P^H$ 均可逆，故 $B$ 亦可逆．
$\Leftarrow \forall \boldsymbol{x} \neq \mathbf{0}$ ，因 $B$ 可逆，$\therefore B \boldsymbol{x} \neq \mathbf{0}$ ，
$\therefore \boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H B^H B \boldsymbol{x}=(B \boldsymbol{x})^H B \boldsymbol{x}=\|B \boldsymbol{x}\|^2>0$ ，故 $A$ 為正定矩陣．
（2）⇒若 $A$ 為正定，則由（1）得知，存在一可逆矩陣 $B$ 使 $A=B^H B$ ，
而且 $B$ 為可逆，故 $\operatorname{rank}(B)=n$ ．
⇐若 $A=B^H B$ ，其中，$B \in C^{m \times n}, \operatorname{rank}(B)=n$ ，
則 $\forall \boldsymbol{x} \in C^{n \times 1}-\{\mathbf{0}\}, \boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H B^H B \boldsymbol{x}=(B \boldsymbol{x})^H B \boldsymbol{x}=\|B \boldsymbol{x}\|^2>0$ ，故 $A$ 為正定矩陣。
$(\because \operatorname{rank}(B)=n$ ，故 $B$ 為行獨立，$\therefore \operatorname{ker}(B)=\{\mathbf{0}\}, \therefore B \boldsymbol{x} \neq \mathbf{0}$ ．）
（3）$\Rightarrow \because A$ 為正定矩陣，故 $A$ 為正規矩陣，故 $A$ 可么正對角化，
故存在么正矩陣 $P \in C^{n \times n}$ ，使 $P^H A P=D=\operatorname{diag}\left(\lambda_1, \ldots, \lambda_n\right), \lambda_i$ 為 $A$ 的特徵根，均為正．
故得 $A=P D P^H=P \sqrt{D} \sqrt{D} P^H=\left(P(\sqrt{D}) P^H\right)\left(P \sqrt{D} P^H\right)=B^2$ ，
其中，$B$ 定義為 $P \sqrt{D} P^H, \sqrt{D}$ 定義為 $\operatorname{diag}\left(\sqrt{\lambda_1}, \ldots, \sqrt{\lambda_n}\right)$ ，
而因 $\sqrt{D}$ ，為正定矩陣，且 $B$ 與 $\sqrt{D}$ 么正相似，故 $B$ 亦為正定矩陣。
⇐ 因 $B$ 為正定矩陣，故 $B$ 可逆，故由（1）得 $A=B^2=B^H B$ 亦為正定．

Note
上述性質對 $n$ 階實對稱矩陣 $A$ 亦成立：
（1）$A$ 為正定矩陣 ⇔ 存在可逆矩陣 $B$ ，使 $A=B^T B$ ．

【90．107成大統計、 94 中興應數、108 成大數學】