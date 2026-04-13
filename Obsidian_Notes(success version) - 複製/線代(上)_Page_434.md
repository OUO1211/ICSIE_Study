> **試題 2**
>
> Show that the set $\{a + b\sqrt{2} \mid a, b \text{ are rational numbers}\}$ together with the operations of addition and multiplication is a vector space.
>
> 【99 成大數學】

解：設 $S = \{a + b\sqrt{2} \mid a, b \in Q\}$，

依照加法定義 $(a + b\sqrt{2}) + (c + d\sqrt{2}) = (a+c) + (b+d)\sqrt{2}$，其中 $a, b \in Q$。

(1) 向量加法具結合性：

$\forall a + b\sqrt{2} \in S$，$m = a + b\sqrt{2}$，$u = (a+c) + (b+d)\sqrt{2} \in S$。

$(u + v) + w = (a + c + e) + (b + d + f)\sqrt{2} = u + (v + w)$。

(2) 具零元素 $0 = 0 + 0\sqrt{2} \in S$。

(3) 具向量加法反元素：

$\forall -v = -a - b\sqrt{2} \in S$，取 $-v = (-a) + (-b)\sqrt{2}$，則 $v + (-v) = 0 = (-v) + v$。

(4) 向量加法具交換性：

$\forall m, v \in S$，$m + v = v + m$，$a + b\sqrt{2}$，$v + c + d\sqrt{2} = u + v$。

(5) 純量乘積對向量加法有分配性：

$\forall k \in Q$，$u = a + b\sqrt{2}$，$v = c + d\sqrt{2} \in S$，$k(u + v) = k(a+c) + k(b+d)\sqrt{2} = (ka + kb\sqrt{2}) = k \cdot u + k \cdot v$。

(6) 純量乘積對純量加法有分配性：

$\forall k, h \in Q$，$v \in S$，$(k + h)v = (k+h)a + (k+h)b\sqrt{2} = ka + kb\sqrt{2} + ha + hb\sqrt{2} = kv + hv$。

(7) 純量乘積純量乘法具結合性：

$\forall k, h \in Q$，$v \in S$，$(kh)v = kha + khb\sqrt{2} = k(ha + hb\sqrt{2}) = k(hv)$。

(8) 單位純量乘積的不變性：

$\forall v \in S$，$1 \cdot v = a + b\sqrt{2} = v$。

故 $(S, +, \cdot)$ 為佈於 $Q$ 的向量空間。
