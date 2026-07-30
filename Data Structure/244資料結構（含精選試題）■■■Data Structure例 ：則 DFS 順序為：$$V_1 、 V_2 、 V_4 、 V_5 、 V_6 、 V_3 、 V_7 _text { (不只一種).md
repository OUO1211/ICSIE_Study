244
資料結構（含精選試題）
■■■

Data Structure
例 ：

則 DFS 順序為：
$$
V_1 、 V_2 、 V_4 、 V_5 、 V_6 、 V_3 、 V_7 \text { (不只一種) }
$$

【註】若限定頂點編號由小到大，則只有一種 order。

\section*{二．橫向優先搜尋（Breadth First Search，BFS）}

橫向優先搜尋從頂點 V 開始，走過之後做個 mark。所有相鄰至 V 而尚未走訪的頂點，都將在下個步驟裡一一拜訪；而且相鄰至這些拜訪過的頂點且尚未走過的頂點，又將一一拜訪；重複上述，直到無頂點可以拜訪為止。
（一）演算法 ：
```
Procedure BFS(v : integer);
var w : integer, q : queue;
Begin
    visited[v] : = true;
    InitializeQueue(q);
    AddQueue(q, v);
```