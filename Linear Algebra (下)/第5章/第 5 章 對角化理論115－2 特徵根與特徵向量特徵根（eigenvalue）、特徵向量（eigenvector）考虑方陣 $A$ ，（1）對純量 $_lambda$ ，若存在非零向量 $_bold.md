第 5 章 對角化理論

11



5－2 特徵根與特徵向量



特徵根（eigenvalue）、特徵向量（eigenvector）

考虑方陣 $A$ ，

（1）對純量 $\lambda$ ，若存在非零向量 $\boldsymbol{v}$ ，使得 $A \boldsymbol{v}=\lambda \boldsymbol{v}$ ，則稱 $\boldsymbol{v}$ 為 $A$ 相對於 $\lambda$ 的一個特徵向量。

（2）對非零向量 $\boldsymbol{v}$ ，若存在純量 $\lambda$ ，使得 $A \boldsymbol{v}=\lambda \boldsymbol{v}$ ，則稱 $\lambda$ 為 $A$ 相對於 $\boldsymbol{v}$ 的一個特徵根．

例如：

（1）$\because\left[\begin{array}{cccc}0 & 0 & 1 & 0 \\ 0 & 0 & 0 & 1 \\ 2 & 1 & 1 & 1 \\ -5 & 2 & 5 & -1\end{array}\right]\left[\begin{array}{l}1 \\ 1 \\ 3 \\ 3\end{array}\right]=\left[\begin{array}{l}3 \\ 3 \\ 9 \\ 9\end{array}\right]=3\left[\begin{array}{l}1 \\ 1 \\ 3 \\ 3\end{array}\right]$ ，故 $\left[\begin{array}{l}1 \\ 1 \\ 3 \\ 3\end{array}\right]$ 為特徵向量，對應的特徵根為 3 ．

（2）$A=\left[\begin{array}{lll}0 & 1 & 0 \\ 0 & 0 & 1 \\ 0 & 0 & 0\end{array}\right]$ ，則 $A\left[\begin{array}{l}1 \\ 0 \\ 0\end{array}\right]=\left[\begin{array}{l}0 \\ 0 \\ 0\end{array}\right]=0 \cdot\left[\begin{array}{l}1 \\ 0 \\ 0\end{array}\right]$ ，即 0 為對應於 $\left[\begin{array}{l}1 \\ 0 \\ 0\end{array}\right]$ 的特徵根．

【93 中興資科】



Note

（1）矩陣算子版本：考慮 $V$ 上的線性算子 $T$ ，

（a）對純量 $\lambda$ ，若存在 $V$ 中的非零向量 $\boldsymbol{v}$ ，使得 $T(\boldsymbol{v})=\lambda \boldsymbol{v}$ ，則稱 $\boldsymbol{v}$ 為 $T$ 相對於 $\lambda$ 的一個特徵向量．

（b）對非零向量 $\boldsymbol{v}$ ，若存在純量 $\lambda$ ，使得 $T(\boldsymbol{v})=\lambda \boldsymbol{v}$ ，則稱 $\lambda$ 為 $T$ 相對於 $\boldsymbol{v}$ 的一個特徵根 （又稱特徵值）．

（2）往後各節的討論與定義都可有矩陣版本與線性映射版本而不再贅述。

（3）特徵根可為 0 ，但特徵向量不可為 0 ．

（4） $\operatorname{ker}(T)$ 中的非零向量均為特徵根 0 所對應的特徵向量。

（5）考慮 $V$ 上的線性算子 $T$ ，令 $\lambda$ 為 $T$ 的一個特徵根，則

（a）若 $\boldsymbol{v}$ 為相對於 $\lambda$ 的一特徵向量，

則對任意非零純量 $k, k \boldsymbol{v}$ 亦為相對於 $\lambda$ 的特徵向量．

（b）若 $v_1, v_2$ 為相對於 $\lambda$ 的特徵向量，且 $v_1+v_2 \neq 0$ ，

則 $v_1+v_2$ 亦為相對於 $\lambda$ 的特徵向量。

【104政大資科】

（6）並不是每個線性算子（方陣）都有特徵根的．（後面有例題）