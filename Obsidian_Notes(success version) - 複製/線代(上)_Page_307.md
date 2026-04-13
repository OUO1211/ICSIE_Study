## 判斷相依或獨立－依定義證明

> **例題 9**
>
> 已知 $\{u, v, w\}$ 為線性獨立集，討論下列各集合是否為線性獨立集：
>
> (1) $\{u + v, u - v\}$
> (2) $\{u, u + v, u + v + w\}$
> (3) $\{u + v, v + w, w + u\}$ 【105 交大資工、106 中山應數】
> (4) $\{3u, 2u - v, u + w\}$ 【95 中山電機類、98 清大統計】

**解**

(1) 設 $\alpha(u + v) + \beta(u - v) = 0$，

則 $(\alpha + \beta)u + (\alpha - \beta)v = 0$，但 $u, v$ 線性獨立，$\therefore \begin{cases} \alpha + \beta = 0 \\ \alpha - \beta = 0 \end{cases}$

$\therefore \alpha = \beta = 0$，得證。

(2) 設 $\alpha u + \beta(u + v) + \gamma(u + v + w) = 0$，

則 $(\alpha + \beta + \gamma)u + (\beta + \gamma)v + \gamma w = 0$，但 $u, v, w$ 線性獨立，$\therefore \begin{cases} \alpha + \beta + \gamma = 0 \\ \beta + \gamma = 0 \\ \gamma = 0 \end{cases}$

$\therefore \alpha = \beta = \gamma = 0$，得證。

(3),(4) 可仿上述討論而得證。

又上述若為三維歐式空間，則亦可如下討論。

(4) 今令 $A = \begin{bmatrix} 3 & 2 & 1 \\ 0 & -1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$，$B = [3u \; 2u - v \; u + w]$，$C = [u \; v \; w]$，

則 $B = CA$，而因為 $A, C$ 可逆，故 $B$ 可逆，故 $B$ 行獨立。