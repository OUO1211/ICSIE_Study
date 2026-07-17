第 3 章 函數

193



可逆函數（invertible function）

考虑函数 $f: A \rightarrow B$ 之反關係 $f^{-1}: B \rightarrow A$ ，其中 $f^{-1}(y)=x \Leftrightarrow f(x)=y$ 。

若 $f^{-1}$ 為一函数，則稱 $f^{-1}$ 為 $f$ 之反函数，且稱函数 $f$ 為可逆的。

【107台大工科】

例如：



函數 $f_1$

的反關係



不是函數，故稱 $f_1$ 不可逆。



函數 $f_2$

的反關係

$b$ 是函數，故稱 $f_2$ 可逆。



Note

（1）另有一種定義反函數的方式如下：

$$

f: A \rightarrow B,

$$



若存在 $g_l: B \rightarrow A$ ，使得 $g_l \circ f=I_A$ ，則稱 $g_l$ 為 $f$ 之左反函數；

若存在 $g_r: B \rightarrow A$ ，使得 $f \circ g_r=I_B$ ，則稱 $g_r$ 為 $f$ 之右反函數；

若存在 $g: B \rightarrow A$ ，使得 $g=g_l=g_r$ ，則稱 $g$ 為 $f$ 之反函數，記為 $g=f^{-1}$ ；

其中，$I_A: A \rightarrow A ; I_B: B \rightarrow B$ 為 identity function，即 $\forall a \in A, I_A(a)=a ; \forall b \in B$ ， $I_B(b)=b$ 。

（2）函數 $f: A \rightarrow B$ 可逆 $\Leftrightarrow f:$ 為一對一且映成。

【證明】

$(\Rightarrow)$ 1－1：設 $f(a)=f(b)$ ，則因為 $f^{-1}$ 為函數，∴ $f^{-1}(f(a))=f\left(f^{-1}(b)\right), \therefore a=b$ 。 onto：$\forall b \in B$ ，take $a=f^{-1}(b) \in A$ ，則 $f(a)=f\left(f^{-1}(b)\right)=b$ 。

（ ⟸ ）考慮函數 $g: B \rightarrow A$ 定義為 $\forall b \in B, ~ g(b)=a$, if $\exists a \in A$ 使得 $f(a)=b$ 。

則因為 $f$ 為 onto，故 $B$ 中的值均有定義；因為 $f$ 為 1－1，故 $g$ 為 well－defined，且由 $g$ 的定義可知 $g(b)=a \Leftrightarrow f(a)=b$ ，故知 $g$ 為 $f$ 的反函數，$f$ 可逆。

（3）求 $f^{-1}$ ：令 $y=f$ ，互換 $x, y$ 符號，重新整理成 $y=g(x)$ ，則 $g=f^{-1}$ 。

例如：

$y=f(x)=5 x+6: R \rightarrow R$ 為 1－1 且 onto 函數，

由 $\frac{y-6}{5}=x$ ，互換 $x, y$ 得到 $\frac{x-6}{5}=y$ ，故 $f^{-1}(x)=\frac{x-6}{5}$ 。