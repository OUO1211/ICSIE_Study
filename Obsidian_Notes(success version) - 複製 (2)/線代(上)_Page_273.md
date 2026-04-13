## 子空間的運算：和空間 (sum space)

> 考慮 $V$ 的子空間 $W_1,\ldots,W_k$，則
> $$
 W_1+\cdots+W_k=\{v_1+\cdots+v_k\mid v_i\in W_i,\ 1\leq i\leq k\}
 $$
> 稱為 $W_1,\ldots,W_k$ 的和空間。

> **Note**
>
> (1) 若 $W_1、W_2$ 均為 $V$ 的子空間，則 $W_1+W_2$ 也是 $V$ 的子空間。 【重要】
>
> **【證明】**
>
> $\because W_1,W_2\subseteq V$；$0\in W_1$，$0\in W_2$，$0=0+0\in W_1+W_2$，$\therefore W_1+W_2\neq\varnothing$。
>
> $\forall u,v\in W_1+W_2$、$\forall \alpha\in F$，令 $u=u_1+u_2$、$v=v_1+v_2$
>
> 其中，$u_1,v_1\in W_1$，$u_2,v_2\in W_2$，
>
> 則：$\because W_1$ 為 $V$ 的子空間；$\therefore \alpha u_1+v_1\in W_1$；
>
> 又：$\because W_2$ 為 $V$ 的子空間；$\therefore \alpha u_2+v_2\in W_2$，
>
> $\therefore (\alpha u_1+v_1)+(\alpha u_2+v_2)\in W_1+W_2$，即 $\alpha(u_1+u_2)+(v_1+v_2)\in W_1+W_2$
>
> 即 $\alpha u+v\in W_1+W_2$，$\therefore W_1+W_2$ 為 $V$ 的子空間。
>
> (2) $W_1\cup W_2\subseteq W_1+W_2$。
>
> **【證明】**
>
> $\forall w\in W_1\cup W_2$，
>
> 若 $w\in W_1$，因為 $w=w+0$，又 $0\in W_2$，$\therefore w\in W_1+W_2$，
>
> 若 $w\in W_2$，因為 $w=0+w$，又 $0\in W_1$，$\therefore w\in W_1+W_2$，
>
> $\therefore W_1\cup W_2\subseteq W_1+W_2$。
>
> (3) $W_1+W_2$ 是包含 $W_1\cup W_2$ 的最小子空間。 【99 東華應數】
>
> (4) $W_1+W_2$ 與 $W_1\cup W_2$ 最大的差別就是前者必為 $V$ 的子空間，但後者不一定。