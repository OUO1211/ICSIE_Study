第 3 圆兩

203



地板函數（Floor function、最大整數函數、下高斯函數）

$f(x)=\lfloor x\rfloor: R \rightarrow Z$ 定義成 $f(x)=n$ ，其中 $n \leq x<n+1$ 。

即 $f(x)=\lfloor x\rfloor=$ 即小於等於 $x$ 的數中最大的整數。

例如：$\lfloor 2.3\rfloor=2 ;\lfloor 4\rfloor=4,\lfloor-1.5\rfloor=-2$ 。

如右圖



【102成大巷道】



天花板函數（Ceiling function，最小整數函數、上高斯函數）

$g(x)=\lceil x\rceil: R \rightarrow Z$ 定義成 $g(x)=n$ ，其中 $n-1<x \leq n$ 。

即 $g(x)=\lceil x\rceil=$ 即大於等於 $x$ 的數中最小的整數。

例如：$\lceil 2.3\rceil=3 ;\lceil 4\rceil=4 ;\lceil-1.5\rceil=-1$ 。



性質

設 $x, y \in R$ ，則

（1）$x-1<\lfloor x\rfloor \leq x$ ．

（2）$\lfloor x+n\rfloor=\lfloor x\rfloor+n, \quad \forall n \in Z$ ．

（3）$\lfloor x\rfloor+\lfloor y\rfloor \leq\lfloor x+y\rfloor \leq\lfloor x\rfloor+\lfloor y\rfloor+1$ ．

（4）$\lfloor x\rfloor=x \Leftrightarrow x \in Z \Leftrightarrow\lceil x\rceil=x$ ．

（5）$\lfloor-x\rfloor=-\lceil x\rceil ;-\lfloor x\rfloor=\lceil-x\rceil$ ．

（6）$\lfloor x\rfloor+\lfloor-x\rfloor=\left\{\begin{array}{cc}0 & \text { if } x \in Z \text { ．} \\ -1 & \text { else．}\end{array}\right.$

（7）$\lfloor\sqrt{\lfloor x\rfloor}\rfloor=\lfloor\sqrt{x}\rfloor, \quad \forall x \in R, \quad x \geq 0$ ．