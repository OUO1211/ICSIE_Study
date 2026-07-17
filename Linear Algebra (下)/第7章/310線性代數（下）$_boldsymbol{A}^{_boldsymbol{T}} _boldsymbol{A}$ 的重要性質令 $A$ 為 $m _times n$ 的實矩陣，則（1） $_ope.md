310
線性代數（下）

$\boldsymbol{A}^{\boldsymbol{T}} \boldsymbol{A}$ 的重要性質
令 $A$ 為 $m \times n$ 的實矩陣，則
（1） $\operatorname{ker}\left(A^T A\right)=\operatorname{ker}(A)$ ．
（2） $\operatorname{rank}\left(A^T A\right)=\operatorname{rank}(A)$ ．

【重要】

（3）$A$ 為行獨立 $\Leftrightarrow A^T A$ 為可逆矩陣．

【98．99 嘉義應数】

（4）$L \operatorname{ker}\left(A A^T\right)=L \operatorname{ker}(A)$ ．
（5） $\operatorname{rank}\left(A A^T\right)=\operatorname{rank}(A)$ ．
（6）$A$ 為列獨立 $\Leftrightarrow A A^T$ 為可逆矩陣．
【證明】
（1）任取 $\boldsymbol{x} \in \operatorname{ker}\left(A^T A\right)$ ，則 $A^T A \boldsymbol{x}=\mathbf{0}$ ，
$\therefore \boldsymbol{x}^T A^T A \boldsymbol{x}=\boldsymbol{x}^T \mathbf{0}=0$ ，即 $(A \boldsymbol{x})^T A \boldsymbol{x}=0, \therefore\langle A \boldsymbol{x}, A \boldsymbol{x}\rangle=0$ 。（此處為標準內積）
$\therefore A \boldsymbol{x}=\mathbf{0}$ ，故得 $\boldsymbol{x} \in \operatorname{ker}(A), \therefore \operatorname{ker}\left(A^T A\right) \subseteq \operatorname{ker}(A)$ ，
又，任取 $\boldsymbol{x} \in \operatorname{ker}(A), A \boldsymbol{x}=\mathbf{0} \therefore A^T A \boldsymbol{x}=A^T \mathbf{0}=\mathbf{0} \therefore \boldsymbol{x} \in \operatorname{ker}\left(A^T A\right), \therefore \operatorname{ker}(A) \subseteq \operatorname{ker}\left(A^T A\right)$ ．
故得 $\operatorname{ker}\left(A^T A\right)=\operatorname{ker}(A)$ ．
（2）
$$
\begin{aligned}
& \because A \in R^{m \times n}, \therefore n=\operatorname{nullity}(A)+\operatorname{rank}(A), \\
& \because A^T A \in R^{n \times n}, \therefore n=\operatorname{nullity}\left(A^T A\right)+\operatorname{rank}\left(A^T A\right),
\end{aligned}
$$

由（1）可得 $\operatorname{nullity}\left(A^T A\right)=\operatorname{nullity}(A)$ ，所以 $\operatorname{rank}\left(A^T A\right)=\operatorname{rank}(A)$ ．
（3）$A$ 為行獨立 $\Leftrightarrow A \boldsymbol{x}=\mathbf{0}$ 只 $\mathbf{0}$ 解 $\Leftrightarrow \operatorname{ker}(A)=\{\mathbf{0}\} \Leftrightarrow \operatorname{ker}\left(A^T A\right)=\{\mathbf{0}\} \Leftrightarrow A^T A$ 可逆．
（也可由：$A$ 為行獨立 $\Leftrightarrow \operatorname{rank}(A)=n \Leftrightarrow \operatorname{rank}\left(A^T A\right)=n \Leftrightarrow A^T A$ ．）
另外，把（1）～（3）的 $A$ 換入 $A^T$ 可得（4）～（6）．

Note
對複數矩陣，運算換成共軛轉置，上述結果亦成立：
（1） $\operatorname{ker}\left(A^H A\right)=\operatorname{ker}(A)$ ．
（2） $\operatorname{rank}\left(A^H A\right)=\operatorname{rank}(A)$ ．
（3）$A$ 為行獨立 $\Leftrightarrow A^H A$ 為可逆矩陣．
（4）$L \operatorname{ker}\left(A A^H\right)=L \operatorname{ker}(A)$ ．
（5） $\operatorname{rank}\left(A A^H\right)=\operatorname{rank}(A)$ ．
（6）$A$ 為列獨立 $\Leftrightarrow A A^H$ 為可逆矩陣．