# $T^2$ 的核空間與值域

## 性質

設 $\dim(V) < \infty$，$T \in L(V,V)$（即 $T$ 為 $V$ 上的線性算子），則

1. $\ker(T) \subseteq \ker(T^2)$
2. $\mathrm{Im}(T^2) \subseteq \mathrm{Im}(T)$
3. 下列四敘述等價：
   $$\mathrm{Im}(T^2)=\mathrm{Im}(T) \Leftrightarrow \mathrm{rank}(T^2)=\mathrm{rank}(T) \Leftrightarrow \mathrm{nullity}(T^2)=\mathrm{nullity}(T) \Leftrightarrow \ker(T^2)=\ker(T)$$
4. $\ker(T^2)=\ker(T) \Leftrightarrow \ker(T)\cap\mathrm{Im}(T)=\{0\}$

【100 成大應數、102 中山應數、103 交大應數、107 台聯電機】

> [!note]
> 若 $T$ 為 [[冪等算子與冪等矩陣|投影算子]]（即 $T^2=T$），則自動有 $\mathrm{Im}(T^2)=\mathrm{Im}(T)$，由性質 3、4 可得 $\ker(T)\cap\mathrm{Im}(T)=\{0\}$，再配合 [[核空間與值域定義|Sylvester 維度定理]]，即得
> $$V = \ker(T) \oplus \mathrm{Im}(T)$$
> 即定義域可分解為核空間與值域的 [[直和]]。【90,92,93 中興應數、94 中山應數、94 清大數學、107 中央數學】

## 證明

**(1) $\ker(T) \subseteq \ker(T^2)$**：任取 $v \in \ker(T)$，得 $T(v)=0$，則 $T^2(v)=T(T(v))=T(0)=0$，故 $v \in \ker(T^2)$。

**(2) $\mathrm{Im}(T^2) \subseteq \mathrm{Im}(T)$**：任取 $v \in \mathrm{Im}(T^2)$，即存在 $u\in V$ 使 $v=T^2(u)=T(T(u))$。令 $w=T(u)\in V$，則 $v=T(w) \in \mathrm{Im}(T)$。

**(3) 四敘述等價**：

- $\mathrm{Im}(T^2)=\mathrm{Im}(T) \Rightarrow \dim(\mathrm{Im}(T^2))=\dim(\mathrm{Im}(T)) \Rightarrow \mathrm{rank}(T^2)=\mathrm{rank}(T)$。
- 反之若 $\mathrm{rank}(T^2)=\mathrm{rank}(T)$，由 (2) 知 $\mathrm{Im}(T^2)$ 為 $\mathrm{Im}(T)$ 的子空間，維度又相等，故 $\mathrm{Im}(T^2)=\mathrm{Im}(T)$。
- 同理，$\ker(T^2)=\ker(T) \Leftrightarrow \mathrm{nullity}(T^2)=\mathrm{nullity}(T)$（利用 (1) 的包含關係）。
- 再由 Sylvester 維度定理 $\dim(V)=\mathrm{rank}(T)+\mathrm{nullity}(T)=\mathrm{rank}(T^2)+\mathrm{nullity}(T^2)$，可得 $\mathrm{rank}(T^2)=\mathrm{rank}(T) \Leftrightarrow \mathrm{nullity}(T^2)=\mathrm{nullity}(T)$，四者串成一個等價鏈。

**(4) $\ker(T^2)=\ker(T) \Leftrightarrow \ker(T)\cap\mathrm{Im}(T)=\{0\}$**：

$(\Rightarrow)$ 設 $\ker(T^2)=\ker(T)$。任取 $v \in \ker(T)\cap\mathrm{Im}(T)$，即 $T(v)=0$ 且存在 $u\in V$ 使 $v=T(u)$。則

$$T^2(u) = T(T(u)) = T(v) = 0 \;\Rightarrow\; u \in \ker(T^2) = \ker(T) \;\Rightarrow\; T(u)=0$$

但 $v=T(u)$，故 $v=0$，即 $\ker(T)\cap\mathrm{Im}(T)=\{0\}$。

$(\Leftarrow)$ 設 $\ker(T)\cap\mathrm{Im}(T)=\{0\}$。由 (1)，$\ker(T)\subseteq\ker(T^2)$。任取 $v\in\ker(T^2)$，即 $T(T(v))=0$，故 $T(v)\in\ker(T)$；又 $T(v)\in\mathrm{Im}(T)$，兩者交集僅 $\{0\}$，故 $T(v)=0$，即 $v\in\ker(T)$，得 $\ker(T^2)\subseteq\ker(T)$。合併兩包含關係，$\ker(T^2)=\ker(T)$。

**相關**：[[核空間與值域定義]]、[[求核空間與值域方法]]、[[冪等算子與冪等矩陣]]、[[直和]]、[[線性映射的合成]]
