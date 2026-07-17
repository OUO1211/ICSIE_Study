424
線性代數（下）

Hermitian 矩陣的性質
令 $A \in C^{n \times n}$ 為 Hermitian 矩陣，則
（1）$A$ 為正規矩陣．

【96成大電通】

（2）$A$ 的相異特徴根所對的特徴向量必正交．

【很重要】

（3）$A$ 的特徵根都是實数（即特徵式在 $R$ 中可分解）。

【很重要】

（4）$A \in C^{n \times n}$ 為 Hermitian 矩陣 $\Leftrightarrow \boldsymbol{x}^H A \boldsymbol{x} \in R, \forall \boldsymbol{x} \in C^{n \times 1}$ ．
【93彰師数學、102成大應数】
【證明】
（1）$A^H A=A A=A A^H$ ，故 $A$ 為正規。
（2）由正規可得，或另證如下：
∵ 設 $A \boldsymbol{x}=\lambda_1 \boldsymbol{x}, A \boldsymbol{y}=\lambda_2 \boldsymbol{y}, \boldsymbol{x}, \boldsymbol{y} \neq \mathbf{0}$ ，故
$$
\lambda_1\langle\boldsymbol{x}, \boldsymbol{y}\rangle=\left\langle\lambda_1 \boldsymbol{x}, \boldsymbol{y}\right\rangle=\langle A \boldsymbol{x}, \boldsymbol{y}\rangle=\left\langle\boldsymbol{x}, A^H \boldsymbol{y}\right\rangle=\left\langle\boldsymbol{x}, \overline{\lambda_2} \boldsymbol{y}\right\rangle=\lambda_2\langle\boldsymbol{x}, \boldsymbol{y}\rangle,
$$
（ ∵ 由（3）可得 Hermitian 矩陣的特徵根必為實數）
$$
\therefore \lambda_1<\boldsymbol{x}, \boldsymbol{y}>-\lambda_2<\boldsymbol{x}, \boldsymbol{y}>=0, \therefore\left(\lambda_1-\lambda_2\right)<\boldsymbol{x}, \boldsymbol{y}>=0 \text {, }
$$

但 $\lambda_1 \neq \lambda_2, \therefore\langle\boldsymbol{x}, \boldsymbol{y}\rangle=0$ ，即 $\boldsymbol{x} \perp \boldsymbol{y}$ 。
（3）設 $\boldsymbol{x} \neq \mathbf{0}, \lambda \in C, A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則 $\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H \lambda \boldsymbol{x}=\lambda \boldsymbol{x}^H \boldsymbol{x}=\lambda\|\boldsymbol{x}\|^2$ ，
又 $\boldsymbol{x}^H A \boldsymbol{x}=\boldsymbol{x}^H A^H \boldsymbol{x}=(A \boldsymbol{x})^H \boldsymbol{x}=(\lambda \boldsymbol{x})^H \boldsymbol{x}=\bar{\lambda} \boldsymbol{x}^H \boldsymbol{x}=\bar{\lambda}\|\boldsymbol{x}\|^2$ ，
$$
\therefore \lambda\|\boldsymbol{x}\|^2=\bar{\lambda}\|\boldsymbol{x}\|^2 \therefore \lambda=\bar{\lambda}, \therefore \lambda \in R \text {. }
$$

另證：
設 $\boldsymbol{x} \neq \mathbf{0}, \lambda \in C, A \boldsymbol{x}=\lambda \boldsymbol{x}$ ，則 $\because A$ 為正規，$\therefore A^H \boldsymbol{x}=\bar{\lambda} \boldsymbol{x}$ ，
又 $A^H \boldsymbol{x}=A \boldsymbol{x}, \therefore \lambda \boldsymbol{x}=\bar{\lambda} \boldsymbol{x}$ ，又 $\because \boldsymbol{x} \neq \mathbf{0}, \therefore \lambda=\bar{\lambda}, \therefore \lambda \in R$ ．
（4）$\left.(\Rightarrow) \forall \boldsymbol{x} \in C^{n \times 1}, \because \overline{\boldsymbol{x}^H A \boldsymbol{x}}=\overline{\left(\boldsymbol{x}^H A \boldsymbol{x}\right.}\right)^T=\left(\boldsymbol{x}^H A \boldsymbol{x}\right)^H=\boldsymbol{x}^H A^H \boldsymbol{x}=\boldsymbol{x}^H A \boldsymbol{x}, \therefore \boldsymbol{x}^H A \boldsymbol{x} \in R$ ．
（ ）$\forall \boldsymbol{x}, \boldsymbol{y} \in C^{n \times 1},(\boldsymbol{x}+\boldsymbol{y})^H A(\boldsymbol{x}+\boldsymbol{y})=\boldsymbol{x}^H A \boldsymbol{x}+\boldsymbol{x}^H A \boldsymbol{y}+\boldsymbol{y}^H A \boldsymbol{x}+\boldsymbol{y}^H A \boldsymbol{y}$,
其中，$(\boldsymbol{x}+\boldsymbol{y})^H A(\boldsymbol{x}+\boldsymbol{y}) \in R, \boldsymbol{x}^H A \boldsymbol{x} \in R, \boldsymbol{y}^H A \boldsymbol{y} \in R$ ，故 $\boldsymbol{y}^H A \boldsymbol{x}+\boldsymbol{x}^H A \boldsymbol{y} \in R$ ，
$$
\begin{equation*}
\therefore\left(\boldsymbol{y}^H A \boldsymbol{x}+\boldsymbol{x}^H A \boldsymbol{y}\right)^H=\boldsymbol{y}^H A \boldsymbol{x}+\boldsymbol{x}^H A \boldsymbol{y} \therefore \boldsymbol{x}^H A^H \boldsymbol{y}+\boldsymbol{y}^H A^H \boldsymbol{x}=\boldsymbol{y}^H A \boldsymbol{x}+\boldsymbol{x}^H A \boldsymbol{y} \tag{1}
\end{equation*}
$$

代入 $i \boldsymbol{x}$ 入 $\boldsymbol{x}$ 於（1）中，得：$(i \boldsymbol{x})^H A^H \boldsymbol{y}+\boldsymbol{y}^H A^H(i \boldsymbol{x})=\boldsymbol{y}^H A(i \boldsymbol{x})+(i \boldsymbol{x})^H A \boldsymbol{y}$
$$
\begin{align*}
& \Rightarrow-i(\boldsymbol{x})^H A^H \boldsymbol{y}+i \boldsymbol{y}^H A^H \boldsymbol{x}=i \boldsymbol{y}^H A \boldsymbol{x}-i(\boldsymbol{x})^H A \boldsymbol{y} \\
& \Rightarrow-\boldsymbol{x}^H A^H \boldsymbol{y}+\boldsymbol{y}^H A^H \boldsymbol{x}=\boldsymbol{y}^H A \boldsymbol{x}-\boldsymbol{x}^H A \boldsymbol{y} \cdots \cdots( \tag{2}
\end{align*}
$$
（1）+ （2）得 $\boldsymbol{y}^H A^H \boldsymbol{x}=\boldsymbol{y}^H A \boldsymbol{x}$ ，故 $A^H=A$ ．