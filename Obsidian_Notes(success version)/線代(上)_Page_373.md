## 和空間的維度公式

考慮有限維向量空間 $V$ 的子空間 $W_1, W_2$，則

> **定理（數學所）**
> $$\dim(W_1 + W_2) = \dim(W_1) + \dim(W_2) - \dim(W_1 \cap W_2)$$

**【證明】**

令 $S = \{v_1, v_2, \ldots, v_k\}$ 為 $W_1 \cap W_2$ 的一組基底，

因為 $W_1 \cap W_2 \subseteq W_1$，$W_1 \cap W_2 \subseteq W_2$，故由獨立集擴增定理，可找到

$S_1 = \{v_1, v_2, \ldots, v_k, x_1, x_2, \ldots, x_m\}$ 為 $W_1$ 之一組基底，

$S_2 = \{v_1, v_2, \ldots, v_k, y_1, y_2, \ldots, y_n\}$ 為 $W_2$ 之一組基底，

欲說明 $\beta = \{v_1, v_2, \ldots, v_k, x_1, x_2, \ldots, x_m, y_1, y_2, \ldots, y_n\}$ 為 $W_1 + W_2$ 之一組基底。

（生成）：$\forall w = w_1 + w_2 \in W_1 + W_2$，其中 $w_1 \in W_1$，$w_2 \in W_2$，

取 $w_1 = \sum_{i=1}^k \alpha_i v_i + \sum_{i=1}^m \beta_i x_i$，$w_2 = \sum_{i=1}^k \delta_i v_i + \sum_{i=1}^n \gamma_i y_i$，$\alpha_i, \beta_i, \delta_i, \gamma_i \in F$，

則 $w = w_1 + w_2 = \sum_{i=1}^k (\alpha_i + \delta_i) v_i + \sum_{i=1}^m \beta_i x_i + \sum_{i=1}^n \gamma_i y_i$，即 $span(\beta) = W_1 + W_2$。

（獨立）：若 $\sum_{i=1}^k \alpha_i v_i + \sum_{i=1}^m \beta_i x_i + \sum_{i=1}^n \gamma_i y_i = 0$，……$(\ast)$，for some $\alpha_i, \beta_i, \gamma_i \in F$，

則 $\sum_{i=1}^n \gamma_i y_i = -\sum_{i=1}^k (-\alpha_i) v_i + \sum_{i=1}^m (-\beta_i) x_i \in span(S_1) \cap span(S_2)$，則 $\sum_{i=1}^n \gamma_i y_i \in W_1 \cap W_2$，

而 $\therefore S = \{v_1, v_2, \ldots, v_k\}$ 為 $W_1 \cap W_2$ 的一組基底，故令 $\sum_{i=1}^n \gamma_i y_i = \sum_{i=1}^k \delta_i v_i$，

$\Rightarrow \sum_{i=1}^n \gamma_i y_i + \sum_{i=1}^k (-\delta_i) v_i = 0$，

而因 $S_2$ 為基底，故 $\delta_i = 0$，$\forall 1 \le i \le k$，$\gamma_i = 0$，$\forall 1 \le i \le n$，

代回$(\ast)$，又因 $S_1$ 為基底，得 $\alpha_i = 0$，$\forall 1 \le i \le k$，$\beta_i = 0$，$\forall 1 \le i \le m$，故 $\beta$ 為獨立集。

而因 $\dim(W_1 + W_2) = k + m + n$，$\dim(W_1) = k + m$，$\dim(W_2) = k + n$，$\dim(W_1 \cap W_2) = k$，

故定理成立。

> **Note**
>
> (1) 推廣：$\dim(W_1 + W_2) = \dim(W_1) + \dim(W_2) \Leftrightarrow W_1 \cap W_2 = \{0\}$。
>
> (2) $\dim(S + T + U) = \dim(S) + \dim(T) + \dim(U) - \dim(S \cap T) - \dim(S \cap U) - \dim(T \cap U) + \dim(S \cap T \cap U)$ 不恆成立。 【95 交大應數，99 台大電機】
>
> 例如，考慮 $V = \mathbb{R}^3$，$S = span\{(1,0,0)\}$，$T = span\{(0,1,0)\}$，$U = span\{(1,1,0)\}$。
