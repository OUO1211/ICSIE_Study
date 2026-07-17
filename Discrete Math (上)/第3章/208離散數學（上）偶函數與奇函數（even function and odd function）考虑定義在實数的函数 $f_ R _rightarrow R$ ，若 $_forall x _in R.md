208

離散數學（上）



偶函數與奇函數（even function and odd function）

考虑定義在實数的函数 $f: R \rightarrow R$ ，

若 $\forall x \in R, f(-x)=f(x)$ ，則稱 $f$ 為偶函数；

若 $\forall x \in R, f(-x)=-f(x)$ ，則稱 $f$ 為奇函數。

【91成大資工】



例如

$f(x)=x^2$ 即為一偶函數；$f(x)=x^3$ 即為一奇函數。

Note

Any function can be the sum of an even function and an odd function．



【91、93成大資工】



【證明】

對任意給的函數 $f(x)$ ，令 $A(x)=\frac{f(x)+f(-x)}{2}, \quad B(x)=\frac{f(x)-f(-x)}{2}$ ，

則 $A(-x)=A(x), ~ \therefore A(x)$ 為偶函數；

$B(-x)=-B(x), \therefore B(x)$ 為奇函數，

又 $f(x)=A(x)+B(x)$ ，故得任意函數均可表為一奇函數與一偶函數的和。