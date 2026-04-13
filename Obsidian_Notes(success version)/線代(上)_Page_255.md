## 常見向量空間

> **1. $n$ 維歐氏空間 ($n$-tuple Euclidean space)：**
>
> 記為 $V=F^n=\{(x_1,x_2,\ldots,x_n)\mid x_i\in F\}$，
>
> 且 $\mathbf{x}=(x_1,x_2,\ldots,x_n)$，$\mathbf{y}=(y_1,y_2,\ldots,y_n)\in V$，$\alpha\in F$，
>
> 定義向量加法：$\mathbf{x}+\mathbf{y}=(x_1+y_1,x_2+y_2,\ldots,x_n+y_n)$，
>
> 定義純量積：$\alpha\cdot\mathbf{x}=(\alpha x_1,\alpha x_2,\ldots,\alpha x_n)$，
>
> $F=R$ 時，稱為實歐氏空間；$F=C$ 時，稱為複歐氏空間。
>
> 若以行向量表示，記成 $F^{1\times n}$；若以列向量表示，記成 $F^{n\times 1}$。
>
> 【100 成大數學】

Note

(1) $(R^n,+,\cdot,R)$、$(C^n,+,\cdot,C)$、$(C^n,+,\cdot,R)$ 都是向量空間，但 $(R^n,+,\cdot,C)$ 不是向量空間，因為純量積的運算違反封閉性：$\mathbf{x}=(x_1,\ldots,x_n)\in R^n$，$\alpha\in C$，但 $\alpha\mathbf{x}\notin R^n$。

(2) 其零向量為 $(0,\ldots,0)$。

> **2. 矩陣空間 (matrix space)：**
>
> $M_{m\times n}(R)$，$M_{m\times n}(C)$
>
> 又記成 $R^{m\times n}$（實矩陣空間），或 $C^{m\times n}$（複矩陣空間）。
>
> 而其向量加法「$+$」定義為矩陣的加法；純量積「$\cdot$」定義為矩陣的純量積。

Note

其零向量為零矩陣。

> **3. 函數空間 (function space)：**
>
> $V=\{f\mid f$ 為定義域 $D[a,b]$ 到體 $F$ 的函數$\}$
>
> 其加法和純量積也定義為函數的加法與係數積。
>
> 【100 中正應數】

Note

(1) 其零向量為零函數 $f(x)=0$。

(2) **多項式空間 (polynomial space)：**
$V=F[x]=\{f(x)\mid f(x)$ 為體 $F$ 的多項式$\}$，有時也記成 $P(F)$。

(3) **$n$ 次多項式空間 ($n$-th polynomial space)：**
$V=F_n[x]=\{f(x)\in F[x]\mid \deg f(x)\leq n$ 或 $f(x)=0\}$，有時也記成 $P_n(F)$。

（有些題目出釋曰：$F_n[x]=\{f(x)\in F[x]\mid \deg f(x)<n$ 或 $f(x)=0\}$。）

(4) **連續函數空間 (space of continuous function)：**
$V=C[a,b]=\{f\mid f$ 為 $[a,b]$ 映到體 $F$ 的連續函數$\}$。 【106 中央數學】