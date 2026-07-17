第 3 章 函數
197

合成與可逆的重要性質
考虑 $f: A \rightarrow B, \quad g: B \rightarrow C$ 兩函数，
（1）若 $f \circ g$ 為一對一，則 $g \circ f$ 亦為一對一。

【99 台大電機】【105 台婦電機】

（2）若 $f \circ g$ 為 onto，則 $g \circ f$ 亦 onto。

【99台大電機】

（3）若 $f \circ g$ 為可逆，則 $g \circ f$ 亦為可逆，且 $(g \circ f)^{-1}=f^{-1} \circ g^{-1}$ 。
【證明】
（1）設 $(g \circ f)\left(a_1\right)=(g \circ f)\left(a_2\right)$ ，其中，$a_1 、 a_2 \in A$ ，
則因為 $g: 1-1$ ，故可由 $g\left(f\left(a_1\right)\right)=g\left(f\left(a_2\right)\right)$ ，得 $f\left(a_1\right)=f\left(a_2\right)$ ，
又因為 $f: 1-1$ ，故可由 $f\left(a_1\right)=f\left(a_2\right)$ ，得 $a_1=a_2$ ，所以 $g \circ f$ 为 1－1．
（2）對 $C$ 中任意元素 $c$ ，
因為 $g$ 為 onto，故存在 $B$ 中元素 $b$ ，使 $g(b)=c$ ，
又因為 $f$ 為 onto，故存在 $A$ 中元素 $a$ ，使得 $f(a)=b$ ，
即存在 $a \in A$ ，使得 $(g \circ f)(a)=g(f(a))=g(b)=c$ ，故 $g \circ f$ 为 onto $*$
（3）由（1）、（2）知 $g \circ f$ 可逆；
且因為 $(g \circ f) \circ\left(f^{-1} \circ g^{-1}\right)=g \circ f \circ f^{-1} \circ g^{-1}=g \circ g^{-1}=I_C$ ，
$\left(f^{-1} \circ g^{-1}\right) \circ(g \circ f)=f^{-1} \circ g^{-1} \circ g \circ f=f^{-1} \circ f=I_A \circ$
$\therefore(g \circ f)^{-1}=\left(f^{-1} \circ g^{-1}\right)$ 。