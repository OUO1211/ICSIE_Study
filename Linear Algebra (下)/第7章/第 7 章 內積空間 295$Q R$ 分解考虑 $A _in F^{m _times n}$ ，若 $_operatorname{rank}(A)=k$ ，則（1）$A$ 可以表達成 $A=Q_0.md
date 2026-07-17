第 7 章 內積空間 295

$Q R$ 分解
考虑 $A \in F^{m \times n}$ ，若 $\operatorname{rank}(A)=k$ ，則
（1）$A$ 可以表達成 $A=Q_0 R_0$ ，
其中，$Q_0 \in F^{m \times n}, Q_0$ 行向量形成正交集，且具 $k$ 個非零行，$n-k$ 個零行． $R_0 \in F^{n \times n}$ ，為上三角矩陣，且對角項都是 1 ．
（2）$A$ 可以表達成 $A=Q R$ ，
其中，$Q \in F^{m \times k}, Q$ 的行向量形成單範正交集，$R \in F^{k \times n}$ ，且 $(R)_{i j}=0, \forall i>j$ ．
步驟：
（1）設矩陣 $A$ 的行向量為 $\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n$ 作正交化得 $\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_n$ ，即為 $Q_0$ 的各行向量．
（2）算出各 $\boldsymbol{v}_i$ 在 $\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_n$ 下的座標，即為 $R_0$ 的各行向量．
以上求得 $A=Q_0 R_0$ ．
（3）所求得的 $\boldsymbol{u}_1, \boldsymbol{u}_2, \ldots, \boldsymbol{u}_n$ 再做單範化得 $\boldsymbol{w}_1, \boldsymbol{w}_2, \ldots, \boldsymbol{w}_n$ ，刪去零向量，設得 $\boldsymbol{w}_1, \boldsymbol{w}_2, \ldots, \boldsymbol{w}_k$ 為單範正交集合，即為 $Q$ 的各行向量．
（4）算出各 $\boldsymbol{v}_i$ 在 $\boldsymbol{w}_1, \boldsymbol{w}_2, \ldots, \boldsymbol{w}_k$ 下的座標，即為 $R$ 的各行向量．
以上求得 $A=Q R$ 。（ $R$ 即 $\boldsymbol{v}_1, \boldsymbol{v}_2, \ldots, \boldsymbol{v}_n$ 到 $\boldsymbol{w}_1, \boldsymbol{w}_2, \ldots, \boldsymbol{w}_n$ 的轉移矩陣）