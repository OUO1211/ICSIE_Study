## 第 3 章　向量空間

## 生成集的性質

> 考慮向量空間 $V$，及其上的向量集 $S, S_1, S_2$，則
>
> (1) $S \subseteq \text{span}(S)$。 【101 中央資工、109 台北統計】
>
> (2) 若 $S_1 \subseteq S_2 \subseteq V$，則 $\text{span}(S_1) \subseteq \text{span}(S_2)$。
>
> (3) $\text{span}(S_1) \cup \text{span}(S_2) \subseteq \text{span}(S_1 \cup S_2)$。
>
> (4) $\text{span}(S_1) \cap \text{span}(S_2) \supseteq \text{span}(S_1 \cap S_2)$。
>
> (5) 對任意子空間 $W$，若 $S \subseteq$ 包含於 $W$，則 $\text{span}(S) \subseteq W$。
>
> 故可推得：$\text{span}(S)$ 為包含 $S$ 的最小子空間。 【103,108 台大資工、109 台北統計】

**【證明】**

(1)$\sim$(4) 直觀可得，讀者可自行練習證明。

(5) 任取 $u \in \text{span}(S)$，則 $u = \alpha_1 v_1 + \cdots + \alpha_k v_k$，for some $v_1, \ldots, v_k \in S$，$\alpha_1, \ldots, \alpha_k$ 為純量係數。

則：$\because S \subseteq W$，$\therefore v_1, \ldots, v_k \in W$，

又因為 $W$ 為 $V$ 的子空間，向量加法具封閉性，$\therefore \alpha_1 v_1 + \cdots + \alpha_k v_k \in W$，即 $u \in W$，

故 $\text{span}(S) \subseteq W$。