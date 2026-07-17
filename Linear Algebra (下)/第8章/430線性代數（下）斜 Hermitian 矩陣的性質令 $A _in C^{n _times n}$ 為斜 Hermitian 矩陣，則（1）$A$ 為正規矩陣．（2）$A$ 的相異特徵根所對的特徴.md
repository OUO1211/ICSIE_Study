430
線性代數（下）

斜 Hermitian 矩陣的性質
令 $A \in C^{n \times n}$ 為斜 Hermitian 矩陣，則
（1）$A$ 為正規矩陣．
（2）$A$ 的相異特徵根所對的特徵向量必正交．

【108成大数學】

（3）$A$ 的特徵根都是 0 或純虚數．【90台大數學、92中正應數、108成大数學】
（4） $\operatorname{det}(A)= \begin{cases}\text { 實數，} & \text { 當 } n \text { 為偶數 } \\ 0 \text { 或純虛數，當 } n \text { 為奇數 }\end{cases}$
【證明】
（1）$A^H A=-A A=A(-A)=A A^H$ ，故 $A$ 為正規．
（2）由正規的特性可得．
（3）設 $\boldsymbol{x} \neq \mathbf{0}, \lambda \in C, A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則 $\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H \lambda \boldsymbol{x}=\lambda \boldsymbol{x}^H \boldsymbol{x}=\lambda\|\boldsymbol{x}\|^2$ ，
又 $\boldsymbol{x}^H A \boldsymbol{x}=-\boldsymbol{x}^H A^H \boldsymbol{x}=-(A \boldsymbol{x})^H \boldsymbol{x}=-(\lambda \boldsymbol{x})^H \boldsymbol{x}=-\bar{\lambda} \boldsymbol{x}^H \boldsymbol{x}=-\bar{\lambda}\|\boldsymbol{x}\|^2$ ，
$\therefore \lambda\|\boldsymbol{x}\|^2=-\bar{\lambda}\|\boldsymbol{x}\|^2, \therefore \lambda=-\bar{\lambda}, \therefore \lambda$ 為 0 或純虛數。
（4） $\operatorname{det}(A)=\operatorname{det}\left(-A^H\right)=(-1)^n \operatorname{det}\left(\overline{A^T}\right)=(-1)^n \overline{\operatorname{det}\left(A^T\right)}=(-1)^n \overline{\operatorname{det}(A)}$ ，
$n$ 為偶數時： $\operatorname{det}(A)=\overline{\operatorname{det}(A)}$ ，所以 $\operatorname{det}(A) \in R$ ．
$n$ 為奇數時： $\operatorname{det}(A)=-\overline{\operatorname{det}(A)}$ ，所以 $\operatorname{det}(A)$ 為 0 或純虛數。