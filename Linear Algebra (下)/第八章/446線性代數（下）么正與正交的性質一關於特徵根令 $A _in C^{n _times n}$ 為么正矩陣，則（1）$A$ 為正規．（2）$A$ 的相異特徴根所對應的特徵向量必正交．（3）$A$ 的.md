446
線性代數（下）

么正與正交的性質一關於特徵根
令 $A \in C^{n \times n}$ 為么正矩陣，則
（1）$A$ 為正規．
（2）$A$ 的相異特徴根所對應的特徵向量必正交．
（3）$A$ 的特徵根 $\lambda,|\lambda|=1$ ．
【90政大應数、93交大應数、95中央数學】
（4）$|\operatorname{det}(A)|=1$ ．
【證明】
（1）$\because A^H A=A A^H$ ，故 $A$ 為正規．
（2）由正規可得．
（3）設 $\boldsymbol{x} \neq \mathbf{0}, \lambda \in C, A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則 $\boldsymbol{x}^H A^H A \boldsymbol{x}=(A \boldsymbol{x})^H(A \boldsymbol{x})=|\lambda|^2\|\boldsymbol{x}\|^2$ ，
又 $\boldsymbol{x}^H A^H A \boldsymbol{x}=\boldsymbol{x}^H I \boldsymbol{x}=\boldsymbol{x}^H \boldsymbol{x}=\|\boldsymbol{x}\|^2$ ，
$\therefore|\lambda|^2\|\boldsymbol{x}\|^2=\|\boldsymbol{x}\|^2, \therefore|\lambda|=1$ ．
（4） $1=\operatorname{det}(I)=\operatorname{det}\left(A^H A\right)=\operatorname{det}\left(A^H\right) \operatorname{det}(A)=\operatorname{det}\left(\overline{A^T}\right) \operatorname{det}(A)=\overline{\operatorname{det}(A)} \operatorname{det}(A)=|\operatorname{det}(A)|^2$ ，
$\therefore|\operatorname{det}(A)|=1$ ．

Note
（1）若 $A \in R^{n \times n}$ 為正交矩陣，則
（a）$A$ 為正規．
（b）$A$ 的相異特徵根對應的特徵向量必正交．

【很重要】

（c）$A$ 的實特徵根必為 $\pm 1$ ．
（d） $\operatorname{det}(A)= \pm 1$ ．
（2）對么正（正交）算子也有以上各性質．