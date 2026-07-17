第 8 章 內積算子及其應用
499

Cholesky 分解
考虑對稱矩陣 $A \in R^{n \times n}$ ，
若 $A$ 為正定矩陣，則
（1）$A$ 可分解成 $L D L^T$（又稱對稱分解），
其中 $L$ 為對角項均為 1 的下三角矩陣，且 $D$ 為對角項都為正的對角矩陣。
（2）$A$ 可分解成 $L L^T$ ，（此又稱 $A$ 的 Cholesky 分解）
其中 $L$ 為下三角矩陣，且對角項都為正。
Note
（1）上述結論對複矩陣亦成立．
（2）上述結論的逆敘述其實也成立。
（3）也有的書對其中的 $L$ 並不要求對角項都正．
${ }^{(4)}$ 完成 Cholesky 分解的步驟：
（i）以列運算 $\left(r_{i j}^{(k)}\right)$ 使 $A$ 列等價至上三角，
所用的列運算對應的列基本矩陣乘積，即為 $L$ 。
（ii）將所得上三角的對角項保留形成對角矩陣，即為 $D$ 。
所得即為 $A=L D L^T$ ．
（iii）由 $A=L D L^T=(L \sqrt{D})\left(\sqrt{D} L^T\right)$ ，其中 $\sqrt{D}=\operatorname{diag}\left(\sqrt{d_{11}}, \ldots, \sqrt{d_{n n}}\right), d_{i i}$ 為 $D$ 的對角項．
取 $L \sqrt{D}=L^{\prime}$ 為下三角矩陣．
所得即為 $A=L^{\prime} L^{\prime T}$ ．