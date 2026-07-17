第 7 章 內積空間 395

正交補空間與 $\mathrm{A} x=\mathrm{b}$ 的相關性質
設 $A \in R^{m \times n}, ~ \boldsymbol{b} \in R^{m \times 1}$ ，則
（1）$A \boldsymbol{x}=\boldsymbol{b}$ 有解⇔對任意 $\boldsymbol{y}$ ，若 $\boldsymbol{y}$ 滿足 $A^T \boldsymbol{y}=\mathbf{0}$ ，則 $\boldsymbol{b}^T \boldsymbol{y}=0$ ．
【89．93 中興應数、105 中正應数】
（2）若對任何 $\boldsymbol{b} \in R^m, A \boldsymbol{x}=\boldsymbol{b}$ 均至少有一解 $\boldsymbol{x} \in R^n$ ，則 $A^T \boldsymbol{y}=\mathbf{0}$ 在 $R^m$ 中恰只一解．
【 91 清大應数、106 中山應数】
（1）⇒ 設 $A \boldsymbol{x}=\boldsymbol{b}$ 有解，則 $\boldsymbol{b} \in R(A)$ ，
若 $\boldsymbol{y}$ 滿足 $A^T \boldsymbol{y}=\mathbf{0}$ ，則 $\boldsymbol{y} \in N\left(A^T\right)=R(A)^{\perp}$ ，故 $<\boldsymbol{y}, \boldsymbol{b}>=0$ ，即 $\boldsymbol{b}^T \boldsymbol{y}=0$ ．
⇐設對任意 $\boldsymbol{y}$ 使 $A^T \boldsymbol{y}=\mathbf{0}$ ，則 $\boldsymbol{b}^T \boldsymbol{y}=0$ ，即 $\langle\boldsymbol{y}, \boldsymbol{b}\rangle=0, \forall \boldsymbol{y} \in N\left(A^T\right)$ ，
即 $\langle\boldsymbol{b}, \boldsymbol{y}\rangle=0, \forall \boldsymbol{y} \in N\left(A^T\right), \therefore \boldsymbol{b} \in N\left(A^T\right)^{\perp}=R(A) \therefore A \boldsymbol{x}=\boldsymbol{b}$ 有解。
（2）由題意知 $\forall \boldsymbol{b} \in R^m, \boldsymbol{b} \in R(A)$ ，故得 $R(A)=R^m$ ，
又因 $R^m=R(A) \oplus N\left(A^T\right)$ ，故得 $N\left(A^T\right)=\{\mathbf{0}\}$ ，即 $A^T \boldsymbol{y}=\mathbf{0}$ 只 $\boldsymbol{y}=\mathbf{0}$ 一解．
極小解（minimal solution）
設 $A \in F^{m \times n}, \boldsymbol{b} \in F^{m \times 1}$ ，且 $A \boldsymbol{x}=\boldsymbol{b}$ 有解，
若 $\boldsymbol{s}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的某一解且滿足 $A \boldsymbol{x}=\boldsymbol{b}$ 的其他解 $\boldsymbol{u}$ ，必使 $\|\boldsymbol{s}\| \leq\|\boldsymbol{u}\|$ ，
則稱 $\boldsymbol{s}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的極小解。
【91 政大應数】
Note
設 $A \in F^{m \times n}, \boldsymbol{b} \in F^{m \times 1}$ ，若 $A \boldsymbol{x}=\boldsymbol{b}$ 有解，則
（1）唯一存在 $\boldsymbol{s} \in R\left(A^H\right)$ 使得 $\boldsymbol{s}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的極小解。
（2）若 $\boldsymbol{u}$ 滿足 $\left(A A^H\right) \boldsymbol{u}=\boldsymbol{b}$ ，則 $\underline{\underline{s=} A^H \boldsymbol{u}}$ ．

解 令 $W=R\left(A^H\right)$ ，則 $W^{\perp}=N(A)$ ，且 $F^{n \times 1}=W \oplus W^{\perp}$ ，
（1）設 $\boldsymbol{x}_0$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 之一解，則存在 $\boldsymbol{s} \in W, \boldsymbol{y} \in W^{\perp}$ ，使 $\boldsymbol{x}_0=\boldsymbol{s}+\boldsymbol{y}$ ，
$\therefore \boldsymbol{b}=A \boldsymbol{x}_0=A(\boldsymbol{s}+\boldsymbol{y})=A \boldsymbol{s}+A \boldsymbol{y}=A \boldsymbol{s}$ ，故 $\boldsymbol{s}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的一解．
若 $\boldsymbol{v}$ 亦為 $A \boldsymbol{x}=\boldsymbol{b}$ 的一解，則得 $\boldsymbol{v}=\boldsymbol{s}+\boldsymbol{u}$ for some $\boldsymbol{u} \in N(A)=W^{\perp}$ ，
$\therefore\|\boldsymbol{v}\|^2=\|\boldsymbol{s}+\boldsymbol{u}\|^2=\|\boldsymbol{s}\|^2+\|\boldsymbol{u}\|^2 \geq\|\boldsymbol{s}\|^2$ ，且等號成立於 $\boldsymbol{u}=\mathbf{0}$ ，即 $\boldsymbol{s}$ 為唯一最小解．
（2）令 $\boldsymbol{u}$ 滿足 $A A^H \boldsymbol{u}=\boldsymbol{b}$ ，取 $\boldsymbol{v}=A^H \boldsymbol{u} \in W$ ，則 $\boldsymbol{v}$ 為 $A \boldsymbol{x}=\boldsymbol{b}$ 的一組解，$\therefore \boldsymbol{v}-\boldsymbol{s} \in W$ ，
又因 $A(\boldsymbol{v}-\boldsymbol{s})=A \boldsymbol{v}-A \boldsymbol{s}=\boldsymbol{b}-\boldsymbol{b}=\mathbf{0}, \therefore \boldsymbol{v}-\boldsymbol{s} \in W^{\perp}$ ，
$$
\therefore \boldsymbol{v}-\boldsymbol{s} \in W \cap W^{\perp}=\{\mathbf{0}\}, \therefore \boldsymbol{v}-\boldsymbol{s}=\mathbf{0}, \therefore \boldsymbol{s}=\boldsymbol{v}=A^H \boldsymbol{u} .
$$