306 線性代數(上)

## 判斷相依或獨立一列運算或行列式

> **例 5**  
> 判斷 $\mathbb{R}^3$ 中，下列向量集合線性獨立或線性相依。  
> (1) $(1,0,0)^T,(0,1,1)^T,(1,0,1)^T$。  
> (2) $(1,0,0)^T,(0,1,0)^T,(0,0,1)^T,(1,2,3)^T$。  
> (3) $(2,1,-2)^T,(3,2,-2)^T,(2,2,0)^T$。  
> (4) $(2,1,-2)^T,(-2,-1,2)^T,(4,2,-4)^T$。  
> (5) $(1,1,3)^T,(0,2,1)^T$。  
> $[97.102 \text{ 中央資工、}100 \text{ 成大資工、}100.104.107 \text{ 台大電機、}100 \text{ 台大電信類題}]$

解

(1)
$$
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 1\\
1 & 0 & 1
\end{bmatrix}
\xrightarrow{R_3-R_1}
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 1\\
0 & 0 & 1
\end{bmatrix}
\xrightarrow{R_2-R_3}
\begin{bmatrix}
1 & 0 & 0\\
0 & 1 & 0\\
0 & 0 & 1
\end{bmatrix}
$$
故為線性獨立。

(2)
$$
\begin{bmatrix}
1\\
0\\
0
\end{bmatrix}
+2
\begin{bmatrix}
0\\
1\\
0
\end{bmatrix}
+3
\begin{bmatrix}
0\\
0\\
1
\end{bmatrix}
=
\begin{bmatrix}
1\\
2\\
3
\end{bmatrix}
$$
故為線性相依。

(3)
$$
\begin{bmatrix}
2 & 1 & -2\\
3 & 2 & -2\\
2 & 2 & 0
\end{bmatrix}
\xrightarrow{R_2-\frac{3}{2}R_1,\;R_3-R_1}
\begin{bmatrix}
2 & 1 & -2\\
0 & 0.5 & 1\\
0 & 1 & 2
\end{bmatrix}
\xrightarrow{R_3-2R_2}
\begin{bmatrix}
2 & 1 & -2\\
0 & 0.5 & 1\\
0 & 0 & 0
\end{bmatrix}
$$
故為線性相依。

(4) 因 $(-2,-1,2)^T=-1.(2,1,-2)^T$，故此集合為線性相依。

(5) 因這兩向量無倍數關係存在，故必為線性獨立。

> **例 6**  
> $(10\%)$ Find all possible $a\in R$ such that the vectors $(1,3,a),(a,4,3),(0,a,1)\in R^3$ are linearly dependent.  
> $[96.102 \text{ 成大統計、}106 \text{ 高雄應數類題、}105 \text{ 台大數學}]$

解 $\;2,-1\pm\sqrt{3}$。

計算
$$
\det\begin{bmatrix}
1 & a & 0\\
3 & 4 & 3\\
a & 3 & 1
\end{bmatrix}
=a^3-6a+4=(a-2)(a^2+2a-2),
$$
由前單 A 行相依 $\Leftrightarrow \det(A)=0$，

故得 $a\in\{2,-1\pm\sqrt{3}\}$。