第 6 章 Jordan form 及其應用

199



形成喬丹型的步驟

（1）將矩陣 $A \in F^{n \times n}$ 的特徵多項式分解求根，為方便說明，設 $\operatorname{char}_A(x)=(x-\alpha)^a(x-\beta)^b$ ， （即特徵根為 $\alpha, \beta$ ，且 $m(\alpha)=a, m(\beta)=b, a+b=n$ ．）

（2）計算 $\operatorname{dim}(\operatorname{ker}(A-\alpha I))$ ，設得 $a_1$ ，則在最右一行劃 $a_1$ 個點，

（這即是 $\alpha$ 的幾何重數 $g m(\alpha)$ ）

再計算 $\operatorname{dim}\left(\operatorname{ker}(A-\alpha I)^2\right)$ ，設得 $a_2$ ，則在右邊數來第二行劃 $\left(a_2-a_1\right)$ 個點，

再計算 $\operatorname{dim}\left(\operatorname{ker}(A-\alpha I)^3\right)$ ，設得 $a_3$ ，則在右邊數來第三行劃 $\left(a_3-a_2\right)$ 個數，



直到 $\operatorname{dim}\left(\operatorname{ker}(A-\alpha I)^k\right)=\operatorname{dim}\left(\operatorname{ker}(A-\alpha I)^{k+1}\right)$ ，for some $k \in Z^{+}$．

（3）數所得的點圖，第一列設有 $n_1$ 個點，則形成 Jordan block $J_{n_1}(\alpha)$ 。

第二列設有 $n_2$ 個點，則形成 Jordan block $J_{n_2}(\alpha)$ ．

一直做到最後．

（4）再考慮 $\operatorname{dim}(\operatorname{ker}(A-\beta I))$ ，重複步驟（2）（3），可得 Jordan block：$J_{n_1^{\prime}}(\beta), J_{n_2^{\prime}}(\beta), \ldots$ ．

（5）若有其他特徵根，也求出其對應的 Jordan block．

（6）將所有得到的 Jordan block 放在對角線的位置即形成 $J_A$ ：Jordan form of $A$ ．