第1章 通輯
75

述詞邏輯的推論規則（rules of inference）
全稱個例化（universal instantiation／specification）：$\underline{\forall x, P(x)}$
$$
\therefore P(c) .
$$

全稱通則化（universal generalization）：對任意 $c, P(c)$
$$
\therefore \forall x, P(x) .
$$

存在個例化（existential instantiation／specification）：$\underline{\exists x, P(x)}$
$\therefore P(c)$ for some $c$
存在通則化（existential generalization）：for some $c, P(c)$
$\therefore \exists x, P(x)$.
全稱性的否定後件（universal modus tollens）
$$
\begin{aligned}
& \forall x[P(x) \rightarrow Q(x)] \\
& \sim Q(a), \text { for some } a \\
& \therefore \sim P(a) .
\end{aligned}
$$

例題
（5\％）Give an argument using rules of inference to show if the conclusion follows from the hypotheses．
Hypotheses：
Everyone in the class has a graphing calculator．
Everyone who has a graphing calculator understands the trigonometric functions．
Conclusion：
Ralphie，who is in the class，understands the trigonometric functions．

【98成大工科】

解 論域為班上同學，則原敘述相當於
$\forall x, C(x) \rightarrow G(x)$ $\_\_\_\_$敘述（1）
$\forall x, G(x) \rightarrow T(x)$ $\_\_\_\_$敘述（2）
$C$（Ralphie） $\_\_\_\_$敘述（3）
$\therefore T$（Ralphie） $\_\_\_\_$敘述（4）
由敘述（1）與 Rule of Universal Specification可得 $C$（Ralphie）$\rightarrow G$（Ralphie） $\_\_\_\_$敘述（5）
由敘述（3），（5）與 Modus Ponens，可得 $G$（Ralphie） $\_\_\_\_$敘述（6）

由敘述（2）與 Rule of Universal Specification