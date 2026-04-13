## 552 線性代數(上)

## $T^2$ 的核空間與值域

> 設 $\dim(V)<\infty$，$T\in L(V,V)$，則
>
> (1) $\ker(T)\subseteq\ker(T^2)$。
>
> (2) $\operatorname{Im}(T^2)\subseteq\operatorname{Im}(T)$。
>
> (3) $\operatorname{Im}(T^2)=\operatorname{Im}(T)\Leftrightarrow \operatorname{rank}(T^2)=\operatorname{rank}(T)\Leftrightarrow \operatorname{nullity}(T^2)=\operatorname{nullity}(T)\Leftrightarrow \ker(T^2)=\ker(T)$。
>
> (4) $\ker(T^2)=\ker(T)\Leftrightarrow \ker(T)\cap\operatorname{Im}(T)=\{0\}$。
>
> 【100 成大應數、102 中山應數、103 交大應數、107 台聯電機】

> **【證明】**
>
> (1) 任取 $v\in\ker(T)$，得 $T(v)=0$，則 $T^2(v)=T(T(v))=T(0)=0$，$\therefore v\in\ker(T^2)$，
>
> $\therefore \ker(T)\subseteq\ker(T^2)$。
>
> (2) 任取 $v\in\operatorname{Im}(T^2)$，
>
> 則存在 $u\in V$ 使得 $v=T^2(u)=T(T(u))=T(w)$，($令\,w=T(u)\in V$，)
>
> 即 $v\in T(V)$，$\therefore \operatorname{Im}(T^2)\subseteq\operatorname{Im}(T)$。
>
> (3) 設 $\operatorname{Im}(T^2)=\operatorname{Im}(T)$，則 $\dim(\operatorname{Im}(T^2))=\dim(\operatorname{Im}(T))$，故 $\operatorname{rank}(T^2)=\operatorname{rank}(T)$。
>
> 設 $\operatorname{rank}(T^2)=\operatorname{rank}(T)$，則由 (2) 可得 $\operatorname{Im}(T^2)$ 為 $\operatorname{Im}(T)$ 的子空間，所以 $\operatorname{Im}(T^2)=\operatorname{Im}(T)$。
>
> 設 $\ker(T^2)=\ker(T)$，則 $\dim(\ker(T^2))=\dim(\ker(T))$，故 $\operatorname{nullity}(T^2)=\operatorname{nullity}(T)$。
>
> 設 $\operatorname{nullity}(T^2)=\operatorname{nullity}(T)$，則由 (1) 可得 $\ker(T)$ 為 $\ker(T^2)$ 的子空間，所以 $\ker(T)=\ker(T^2)$。
>
> 再由 Sylvester 第一定理：$\dim(V)=\operatorname{rank}(T)+\operatorname{nullity}(T)$，且 $\dim(V)=\operatorname{rank}(T^2)+\operatorname{nullity}(T^2)$，
>
> $\therefore \operatorname{rank}(T^2)=\operatorname{rank}(T)\Leftrightarrow \operatorname{nullity}(T^2)=\operatorname{nullity}(T)$。
>
> (4) $(\Rightarrow)$ 設 $\ker(T^2)=\ker(T)$，則對 $\forall v\in\ker(T)\cap\operatorname{Im}(T)$，
>
> $\because T(v)=0$，且存在 $u\in V$，使 $v=T(u)$，
>
> $\therefore T^2(u)=T(T(u))=T(v)=0$，$\therefore u\in\ker(T^2)$，
>
> 又因 $\ker(T^2)=\ker(T)$，$\therefore u\in\ker(T)$，$\therefore T(u)=0$，即 $v=0$，$\therefore \ker(T)\cap\operatorname{Im}(T)=\{0\}$。
>
> $(\Leftarrow)$ 設 $\ker(T)\cap\operatorname{Im}(T)=\{0\}$，由 (1) 得 $\ker(T)\subseteq\ker(T^2)$，
>
> 任取 $v\in\ker(T^2)$，即 $T^2(v)=0$，即 $T(T(v))=0$，即 $T(v)\in\ker(T)$，又因 $T(v)\in\operatorname{Im}(T)$，
>
> 且 $\ker(T)\cap\operatorname{Im}(T)=\{0\}$，故 $T(v)=0$，即 $v\in\ker(T)$，得 $\ker(T^2)\subseteq\ker(T)$，
>
> 故 $\ker(T^2)=\ker(T)$。

> **Note**
>
> 故若 $T$ 為投影算子即可得 $\operatorname{Im}(T^2)=\operatorname{Im}(T)$，而得 $\ker(T)\cap\operatorname{Im}(T)=\{0\}$，再由 Sylvester 定理知
>
> $$V=\ker(T)\oplus\operatorname{Im}(T).$$
>
> 【90.92.93 中興應數、94 中山應數、94 清大數學、107 中央數學】