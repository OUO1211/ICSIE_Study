第 8 章 內積算子及其應用
455
$$
\therefore \sum_{k=1}^n\left|(A)_{k i}\right|^2=\sum_{k=1}^n\left|(A)_{i k}\right|^2, \therefore\left\{\begin{array}{c}
\left|(A)_{11}\right|^2=\left|(A)_{11}\right|^2+\left|(A)_{12}\right|^2+\ldots+\left|(A)_{1 n}\right|^2 \\
\left|(A)_{12}\right|^2+\left|(A)_{22}\right|^2=\left|(A)_{22}\right|^2+\ldots+\left|(A)_{2 n}\right|^2 \\
\vdots \\
\left|(A)_{1 n}\right|^2+\left|(A)_{2 n}\right|^2+\ldots+\left|(A)_{n n}\right|^2=\left|(A)_{n n}\right|^2
\end{array}\right.
$$

故得 $\left|(A)_{p q}\right|^2=0, \forall p<q, \therefore(A)_{p q}=0, \forall p<q$ ，
又 $\because A$ 為上三角，故 $(A)_{p q}=0, \forall p>q$ ，故 $A$ 為對角矩陣。
（ ⇐）因 $A$ 為對角矩陣，故明顯為上三角．
$$
\text { 令 } A=\left[\begin{array}{llll}
a_{11} & & & O \\
& a_{22} & & \\
& & \ddots & \\
O & & & a_{n n}
\end{array}\right] \text {, 則 } A^H A=\left[\begin{array}{cccc}
\left|a_{11}\right|^2 & & & O \\
& \left|a_{22}\right|^2 & & \\
& & \ddots & \\
O & & & \left|a_{n n}\right|^2
\end{array}\right]=A A^H \text {, }
$$

故 $A$ 為正規．
（3）（ ⇒）若 $A$ 為上三角，且 $A^T=A$ ，則因 $A^T$ 為下三角，故 $A$ 為對角矩陣．
（ ⇐）明顯成立。
（4）（ ⟸）因 $A$ 可么正對角化，設 $A$ 與對角矩陣 $D$ 么正相似，
則因 $D$ 為對角矩陣，所以 $D$ 為正規矩陣，所以 $A$ 亦為正規矩陣。
$(\Rightarrow) \because A \in C^{n \times n}$ ，由 Schur 定理知 $A$ 必可與某上三角矩陣 $R$ 么正相似，
而 $A$ 正規，故 $R$ 正規，故 $R$ 為對角矩陣（由（2）），
即 $A$ 與一對角矩陣么正相似，故 $A$ 可么正對角化．
（5）（ ⟸ ）因 $A$ 可正交對角化，設 $A$ 與對角矩陣 $D$ 正交相似，
則因 $D$ 為對角矩陣，所以 $D$ 為對稱矩陣，所以 $A$ 亦為對稱矩陣。
$(\Rightarrow) \because A \in R^{n \times n}$ 為對稱矩陣，故特徵根均為實數，故 $\operatorname{char}_A(x)$ 在 $R$ 中可分解，
由 Schur 定理知 $A$ 必可與某上三角矩陣 $R$ 正交相似，
而 $A$ 對稱，故 $R$ 對稱，故 $R$ 為對角矩陣（由（3）），
即 $A$ 與一對角矩陣正交相似，故 $A$ 可正交對角化．