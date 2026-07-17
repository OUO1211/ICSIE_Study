# 4-1 線性映射

## 線性映射(linear transformation, linear mapping)的定義

> **定義**
>
> 考慮向量空間 $V$、$V'$，若函數 $T: V \to V'$ 滿足
>
> 對任何 $V$ 中的向量 $u, v$ 與純量係數 $a$，
>
> (1) $T(u+v) = T(u) + T(v)$
>
> (2) $T(av) = aT(v)$
>
> 則稱 $T$ 為 $V$ 到 $V'$ 的**線性映射**，也記做 $T \in L(V, V')$。
>
> 【81,83 成大資工、92 中央資工、93 北科資工、95 暨南資工、107 中山應數】

> **Note**
>
> (1) $L(V,V') = \{T \mid T: V \to V' \text{ 為線性映射}\}$ 也是一個向量空間。
>
> (2) $T_0: V \to V'$ 為線性零映射 (zero mapping)，其中 $T_0(v) = 0$，$\forall v \in V$。
>
> (3) 當 $V' = V$ 時，線性變換 $T: V \to V$ 又稱為 $V$ 上的**線性算子** (linear operator)。
>
> (4) $I_v: V \to V$ 為線性單位映射 (identity mapping)，其中 $I_v(v) = v$，$\forall v \in V$。
>
> (5) 積分運算 $T: C[a,b] \to R$，$T(f) = \int_a^b f(x)dx$ 為線性映射，其中 $C[a,b]$ 為收集所有定義在 $[a,b]$ 上的連續函數所成的集合。【90 成大統計、105 中正應數】
>
> (6) 微分運算為線性映射【101 政大應數、105 中央統計】
>
> 【證明】
>
> 任取 $f(x), g(x) \in V$，$a \in R$，
>
> 則 $T(af(x) + g(x)) = (af(x) + g(x))' = af'(x) + g'(x) = aT(f(x)) + T(g(x))$，
>
> 故 $T$ 為 $V$ 到 $V$ 的線性映射。
>
> (7) 歐氏空間上的線性映射之一般形式 — 左乘映射與右乘映射：
>
> 給定 $m \times n$ 矩陣 $A$，定義 $L_A: F^{n\times 1} \to F^{m\times 1}$ 為 $L_A(x) = Ax$，$\forall x \in F^{n\times 1}$。
>
> 則 $L_A$ 為線性，稱為 $A$ 的**左乘映射**。
>
> 且若 $\alpha, \gamma$ 分別為 $F^{n\times 1}$、$F^{m\times 1}$ 的標準基底，則 $[L_A]_\alpha^\gamma = A$。
>
> 同理，可定義 $A$ 的**右乘映射** $R_A: F^{1\times m} \to F^{1\times n}$ 為 $R_A(x) = xA$，$\forall x \in F^{1\times m}$。
