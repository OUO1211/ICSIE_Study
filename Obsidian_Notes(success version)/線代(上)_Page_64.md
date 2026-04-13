> **例題 16**
>
> Let matrix $A$ satisfy $A^k = O$, for some integer $k$（即為冪零，nilpotent 矩陣）. Prove that
>
> (1) $I - A$ is invertible, and find its inverse.
>
> 【96 政大統計、103 台大數學/清大數學、105 中山總數、106 中興統計】
>
> (2) $I + A$ is invertible, and find its inverse.
>
> 【105 台大資工、108 交大資工】

**解**

(1) 考慮多項式 $f(x) = 1 - x^k = (1-x)(1 + x + x^2 + \cdots + x^{k-1})$

$f(A) = I - A^k = (I-A)(I + A + A^2 + \cdots + A^{k-1})$

而 $A^k = O$，故 $(I-A)(I + A + A^2 + \cdots + A^{k-1}) = I$

故得 $(I-A)^{-1} = I + A + A^2 + \cdots + A^{k-1}$

(2) $\because A^k = O$，故 $(-A)^k = O$，即 $-A$ 亦為 nilpotent，代入(1)的結果即可得：

$I + A$ 可逆，且 $(I+A)^{-1} = I - A + A^2 - \cdots + (-A)^{k-1}$
