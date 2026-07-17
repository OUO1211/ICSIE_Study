376
線性代數（下）

正交補空間與四大子空間
$A$ 為 $-m \times n$ 的實矩陣，則
（1）$C S\left(A^T\right)^{\perp}=N(A)$ ．
【92中興應数、97北科資工、97台大電機、102中正應数】
（2）$C S(A)^{\perp}=N\left(A^T\right)$ ．
【94師大數學、99交大資工、104中央資工】
（3） $\operatorname{CS}(A)=N\left(A^T\right)^{\perp}$ ．【94 交大電資、101 中正數學、102 中央資工】
（4）$C S\left(A^T\right)=N(A)^{\perp}$ ．
【證明】
（1）任取 $\boldsymbol{x} \in N(A)$ ，設 $\boldsymbol{y} \in C S\left(A^T\right)$ ，即 $\boldsymbol{y}=A^T z$ for some $z \in R^{m \times 1}$ ，
則 $\langle\boldsymbol{x}, \boldsymbol{y}\rangle=\left\langle\boldsymbol{x}, A^T z\right\rangle=\langle A \boldsymbol{x}, z\rangle=\langle\boldsymbol{0}, z\rangle=0$ ，
即 $\boldsymbol{x} \in C S\left(A^T\right)^{\perp}$ ，故 $N(A) \subseteq C S\left(A^T\right)^{\perp}$ ，
另外，$\because n=\operatorname{dim}(N(A))+\operatorname{rank}(A)=\operatorname{dim}(N(A))+\operatorname{rank}\left(A^T\right)=\operatorname{dim}(N(A))+\operatorname{dim}\left(C S\left(A^T\right)\right)$
且 $\because n=\operatorname{dim}\left(C S\left(A^T\right)\right)+\operatorname{dim}\left(C S\left(A^T\right)^{\perp}\right)$ ，
$\therefore \operatorname{dim}(N(A))=\operatorname{dim}\left(C S\left(A^T\right)^{\perp}\right)$ ，故得 $C S\left(A^T\right)^{\perp}=N(A)$ ．
另證：
令 $A=\left[\begin{array}{c}\boldsymbol{v}_1^T \\ \vdots \\ \boldsymbol{v}_m^T\end{array}\right], \boldsymbol{v}_i \in R^{n \times 1}, \therefore A^T=\left[\boldsymbol{v}_1, \ldots, \boldsymbol{v}_m\right]$ ，則
$$
\boldsymbol{x} \in N(A) \Leftrightarrow A \boldsymbol{x}=\mathbf{0} \Leftrightarrow\left[\begin{array}{c}
\boldsymbol{v}_1^T \\
\vdots \\
\boldsymbol{v}_m^T
\end{array}\right] \boldsymbol{x}=\mathbf{0} \Leftrightarrow\left\{\begin{array}{c}
\boldsymbol{v}_1^T \boldsymbol{x}=0 \\
\vdots \\
\boldsymbol{v}_m^T \boldsymbol{x}=0
\end{array} \Leftrightarrow\left\langle\boldsymbol{x}, \boldsymbol{v}_i\right\rangle=0, \forall i\right.
$$
$\Leftrightarrow \boldsymbol{x}$ 與 $A^T$ 的行向量都正交 $\Leftrightarrow \boldsymbol{x} \in C S\left(A^T\right)^{\perp}$ ，
$$
\therefore N(A)=C S\left(A^T\right)^{\perp} .
$$
（2）代 $A^T$ 入（1）中的 $A$ 可得 $C S(A)^{\perp}=N\left(A^T\right)$ ．
（3）（2）式左右取正交補空間得 $C S(A)=N\left(A^T\right)^{\perp}$ ．
（4）（1）式左右取正交補空間得 $C S\left(A^T\right)=N(A)^{\perp}$ ．

Note
設 $W$ 為 $V$ 的子空間，則前面有討論得 $V=W \oplus W^{\perp}$ ，故得對矩陣 $A \in R^{m \times n}$ ：
（1）$R^m=C S(A) \oplus N\left(A^T\right)$ ．
（2）$R^n=C S\left(A^T\right) \oplus N(A)$ ．