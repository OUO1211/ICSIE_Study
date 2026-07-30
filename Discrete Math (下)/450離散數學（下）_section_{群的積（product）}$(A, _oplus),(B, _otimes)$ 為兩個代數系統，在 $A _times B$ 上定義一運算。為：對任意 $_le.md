450
離散數學（下）

\section*{群的積（product）}
$(A, \oplus),(B, \otimes)$ 為兩個代數系統，在 $A \times B$ 上定義一運算。為：
對任意 $\left(a_1, b_1\right),\left(a_2, b_2\right) \in A \times B,\left(a_1, b_1\right) \circ\left(a_2, b_2\right)=\left(a_1 \oplus a_2, b_1 \otimes b_2\right)$ ，
若 $(A, \oplus),(B, \otimes)$ 均為群，則 $(A \times B, \circ)$ 亦為群。

\section*{【證明】}

令 $\left(a_1, b_1\right),\left(a_2, b_2\right),\left(a_3, b_3\right) \in A \times B$ ，
封閉性：$\left(a_1, b_1\right) \circ\left(a_2, b_2\right)=\left(a_1 \oplus a_2, b_1 \otimes b_2\right) \in A \times B \circ \ldots \ldots . .\left(\because a_1 \oplus a_2 \in A, b_1 \otimes b_2 \in B\right)$
結合性：$\left(\left(a_1, b_1\right) \circ\left(a_2, b_2\right)\right) \circ\left(a_3, b_3\right)=\left(a_1 \oplus a_2, b_1 \otimes b_2\right) \circ\left(a_3, b_3\right)=\left(\left(a_1 \oplus a_2\right) \oplus a_3,\left(b_1 \otimes b_2\right) \otimes b_3\right)$
$$
\begin{aligned}
& =\left(a_1 \oplus\left(a_2 \oplus a_3\right), b_1 \otimes\left(b_2 \otimes b\right)\right) \\
& =\left(a_1, b_1\right) \circ\left(a_2 \oplus a_3, b_2 \otimes b_3\right)=\left(a_1, b_1\right) \circ\left(\left(a_2, b_2\right) \circ\left(a_3, b_3\right)\right)
\end{aligned}
$$
單位元素為 $e=\left(e_A, e_B\right)$ 。
$\because\left(a_1, b_1\right) \circ\left(e_A, e_B\right)=\left(a_1 \oplus e_A, b_1 \otimes e_B\right)=\left(a_1, b_1\right)$,
$\left(e_A, e_B\right) \circ\left(a_1, b_1\right)=\left(e_A \oplus a_1, e_B \otimes b_1\right)=\left(a_1, b_1\right) \circ$
反元素性質：$\left(a_1, b_1\right)^{-1}=\left(a_1^{-1}, b_1^{-1}\right)$ 。
$\because\left(a_1, b_1\right) \circ\left(a_1^{-1}, b_1^{-1}\right)=\left(a_1 \oplus a_1^{-1}, b_1 \otimes b_1^{-1}\right)=\left(e_A, e_B\right)$,
$\left(a_1^{-1}, b_1^{-1}\right) \circ\left(a_1, b_1\right)=\left(a_1^{-1} \oplus a_1, b_1^{-1} \otimes b_1\right)=\left(e_A, e_B\right) \circ$

\section*{Note}
$(A \times B, \circ)$ 中的單位元素為 $\left(e_A, e_B\right)$ ，其中 $e_A$ 為 $A$ 之單位元素，$e_B$ 為 $B$ 之單位元素，且 $(a, b)$ 之反元素 $(a, b)^{-1}=\left(a^{-1}, b^{-1}\right)$ 。