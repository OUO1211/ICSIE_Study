第 5 章 對角化理論

3



5－1 方陣的相似



方陣的相似（similar）

考虑方陣 $A, B$ ，

若存在可逆矩陣 $P$ 滿足 $B=P^{-1} A P$ ，則稱 $A$ 與 $B$ 相似，記作 $A \sim B$ 。

Note

（1）方陣的相似為等價關係。（即滿足反身性，對稱性，遞移性）

【證明】

【 92 交大應數、 94 嘉義應數、 94 中央數學】

（a）反身性（reflexive）：

取 $P=I$ ：單位矩陣，則 $\forall A, A=P^{-1} A P$ ，即 $A$ 與 $A$ 相似．

（b）對稱性（symmetric）：

設 $A$ 與 $B$ 相似，令可逆矩陣 $P$ 使 $B=P^{-1} A P$ ，即 $A=P B P^{-1}$ ，則取 $Q=P^{-1}$ ，可使 $A=Q^{-1} B Q$ ，即得 $B$ 與 $A$ 相似。

（c）遞移性（transitive）：

設 $A$ 與 $B$ 相似，$B$ 與 $C$ 相似，令可逆矩陣 $P, Q$ 使 $B=P^{-1} A P, C=Q^{-1} B Q$ ，

則得 $C=Q^{-1}\left(P^{-1} A P\right) Q=(P Q)^{-1} A(P Q)$ ，

則因 $P Q$ 亦為可逆矩陣，故得 $A$ 與 $C$ 相似。

故相似為方陣上的一種等價關係。

（2）對任意純量 $c, A \sim c I \Leftrightarrow A=c I$ ．因此可得，只有 $I$ 與 $I$ 相似，只有 $O$ 與 $O$ 相似．

（3）對 $V$ 上的線性映射 $T$ ，令 $\alpha, \beta$ 為 $V$ 上的兩組基底，則 $[T]_\alpha \sim[T]_\beta$ ．

【證明】



【107政大應數、98．107台科資工】

$$

\because\left[I_V\right]_\beta^\alpha[T]_\beta\left[I_V\right]_\alpha^\beta=[T]_\alpha \text {, 且 }\left[I_V\right]_\alpha^\beta=\left(\left[I_V\right]_\beta^\alpha\right)^{-1} \text {. }

$$