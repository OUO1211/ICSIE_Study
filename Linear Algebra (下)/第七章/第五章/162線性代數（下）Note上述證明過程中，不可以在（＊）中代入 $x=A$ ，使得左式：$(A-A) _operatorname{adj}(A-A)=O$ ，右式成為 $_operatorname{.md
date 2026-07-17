162
線性代數（下）

Note
上述證明過程中，不可以在（＊）中代入 $x=A$ ，
使得左式：$(A-A) \operatorname{adj}(A-A)=O$ ，右式成為 $\operatorname{char}_A(A)$ ，而得證畢。
原因如下：
＂設 $S(x)=T(x) U(x)$ ，其中 $S, T, U$ 均為方陣多項式，$A$ 為任意方陣，則 $S(A)=T(A) U(A)$＂不一定成立。

例如：
$T(x)=T_0+x T_1, U(x)=U_0+x U_1$ ，其中，$T_0, T_1, U_0, U_1$ 均為方陣，
則 $S(x)=\left(T_0+x T_1\right)\left(U_0+x U_1\right)=T_0 U_0+x\left(T_0 U_1+T_1 U_0\right)+x^2 T_1 U_1$ ，
而 $T(A) U(A)=\left(T_0+A T_1\right)\left(U_0+A U_1\right)=T_0 U_0+\underline{T_0 A U_1}+A T_1 U_0+A^2 T_1 U_1$ ，
但 $S(A)=T_0 U_0+A\left(T_0 U_1+T_1 U_0\right)+A^2 T_1 U_1=T_0 U_0+\underline{A T_0 U_1}+A T_1 U_0+A^2 T_1 U_1$ ，
不一定相等。

Note
（1）上述定理以矩陣來描述，若以線性算子來表達則為：
設 $T \in L(V, V)$ 且 $f(x)=\operatorname{char}_T(x)=\operatorname{det}(T-x I)$ ，則 $f(T)=O$ ．
（2）設 $A$ 為 $n$ 階方陣，且 $f(x)=\operatorname{char}_A(x), g(x) \in F[x]$ ，
若 $g(x)=f(x) q(x)+r(x)$ ，其中， $\operatorname{deg}(r(x))<\operatorname{deg}(f(x))$ ，或 $r(x)=0$ ，
則 $g(A)=r(A)$ ．
（3）若 $\boldsymbol{A}$ 可逆，且 $\operatorname{char}_A(x)=(-x)^n+a_{n-1} x^{n-1}+\ldots+a_1 x+a_0$ ，
則 $A^{-1}=\frac{-1}{a_0}\left((-1)^n A^{n-1}+a_{n-1} A^{n-2}+\ldots+a_1 I\right)$ ．
【91 成大應數、93 政大應數、93 中正應數、98 中興統計】
（4）設 $A \in R^{n \times n}$ ，則 $A, A^2, \ldots, A^{n+1}$ 為線性相依。
（故 $\operatorname{dim}\left(\operatorname{span}\left(\left\{I_n, A, A^2, \ldots\right\}\right)\right) \leq n$ ）

【97師大數學】

【證明】【 89.91 交大應數、 93 高雄統計、 94 中山應數．中興應數、 100 中央數學】
設 $\operatorname{char}_A(x)=(-1)^n x^n+a_{n-1} x^{n-1}+\ldots+a_1 x+a_0$ ，
則由 Cayley－Hamilton 定理得 $(-1)^n A^n+a_{n-1} A^{n-1}+\ldots+a_1 A+a_0 I=O$ ，
$$
\therefore(-1)^n A^{n+1}+a_{n-1} A^n+\ldots+a_1 A^2+a_0 A=O .
$$

即 $\left\{A, A^2, \ldots, A^{n+1}\right\}$ 為線性相依。