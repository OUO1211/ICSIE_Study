Rayleigh 商式（Rayleigh quotient）
考虑 Hermitian 矩陣 $A \in C^{n \times n}, \boldsymbol{x} \neq \mathbf{0}$ ，則
定義 $\rho(\boldsymbol{x})=\frac{Q(\boldsymbol{x})}{\|\boldsymbol{x}\|^2}=\frac{\boldsymbol{x}^H A \boldsymbol{x}}{\|\boldsymbol{x}\|^2}$ 穑为 $\boldsymbol{x}$ 的 Rayleigh 商去
考慮對稱矩陣 $A \in R^{n \times n}$ ，则䖞 $\boldsymbol{x} \neq \mathbf{0}$ ，
定義 $\rho(\boldsymbol{x})=\frac{Q(\boldsymbol{x})}{\|\boldsymbol{x}\|^2}=\frac{\boldsymbol{x}^T A \boldsymbol{x}}{\|\boldsymbol{x}\|^2}$ 稱为 $\boldsymbol{x}$ 的 Rayleigh 商式
Note
（1）也有將之稱為 $A$ 的 Rayleigh 商式，記成 $\rho_A(x)$
（2）$\rho(x)=\frac{Q(x)}{\|x\|^2}=\frac{x^H A x}{x^H x}=\frac{\langle A x, x\rangle}{\langle x, x\rangle}$ ．
（3）若 $\lambda$ 為 $A$ 相對於非零向量 $x$ 的特徽根，則 $P(x)=\lambda$
【證明】
$$
\rho(\boldsymbol{x})=\frac{\langle A \boldsymbol{x}, \boldsymbol{x}\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}=\frac{\langle\lambda \boldsymbol{x}, \boldsymbol{x}\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}=\frac{\lambda\langle\boldsymbol{x}, \boldsymbol{x}\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}=\lambda
$$