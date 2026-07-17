# 第二章 線性方程組與求解 122

## 線性系統的解空間

> **若 $Ax=b$ 有一組解 $x_0$，則 $Ax=b$ 的解空間為 $\{x_0+u \mid Au=0\}$。**
>
> 【100 中正統計、108 中山應數】

令其解集合為 $X=\{x \mid Ax=b\}$，並設 $S=\{x_0+u \mid u \in U\}$，$U=\{u \mid Au=0\}$，

欲證 $X=S$。

$(\subseteq)$ 任取 $x \in X$，則 $Ax=b$，則因為 $Ax_0=b$，

$\therefore A x-Ax_0=0$

即 $A(x-x_0)=0$

即 $x-x_0 \in U$

設 $u \in U$ 使得 $x-x_0=u$

即 $x=x_0+u$，即 $x \in S$

$\therefore X \subseteq S$。

$(\supseteq)$ 任取 $x_0+u \in S$，for some $u \in U$，

則 $A(x_0+u)=Ax_0+Au=b+0=b$

$\therefore x_0+u \in X$。

$\therefore S \subseteq X$

> **Note**
>
> (1) 通常把 $x_0$ 稱為特殊解，$u$ 稱為齊次解。
>
> (2) 相當於對 $Ax=0$ 的解平移而得 $Ax=b$ 的解。
>
> (3) 在無限體上，若 $Ax=b$ 有超過一組解，則 $Ax=b$ 有無限多解。