# 第二章 線性方程組與求解 159

## 齊次方程解的個數

> 考慮方程組 $Ax=0$，其中 $A:m\times n$，則
>
> (1) $\operatorname{rank}(A)=n \Leftrightarrow Ax=0$ 只零解。
>
> (2) $\operatorname{rank}(A)<n \Leftrightarrow Ax=0$ 有無限多解。
>
> (3) 若 $m<n$，則 $Ax=0$ 必有非零解。
>
> (4) $Ax=0$ 有非零解 $\Leftrightarrow Ax=0$ 有無限多解。
>
> (5) $Ax=0$ 只有零解 $\Leftrightarrow A$ 列等價於 $I_n$（$A$ 為方陣時）

(1)(2) 與 $Ax=b$ 的討論方式相同。

(3) 因此時必有自由變數故無窮多解

也可說是因為 $\operatorname{rank}(A)\leq m<n$。

(4) $\Rightarrow$ 今 $x\neq 0$ 使 $Ax=0$，考慮 $kx$，$k$ 為任意常數，則 $A(kx)=k(Ax)=k0=0$，即 $kx$ 亦為解，

故 $Ax=0$ 有無限多解

$\Leftarrow$ 明顯成立。

(5) 由(1)得 $Ax=0$ 恰一解 $\Leftrightarrow \operatorname{rank}(A)=n$，又，

若 $\operatorname{rank}(A)=n$，表 $A$ 的簡化列梯陣有 $n$ 個非零列，故 $A$ 可列運算到 $I_n$。

若 $A$ 與 $I_n$ 列等價，則 $Ax=0$ 與 $I_nx=0$ 相同，而 $I_nx=0$ 只有一解，故 $Ax=0$ 只有零解。

故得證。