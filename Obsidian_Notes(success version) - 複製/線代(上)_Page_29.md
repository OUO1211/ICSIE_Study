## 矩陣的轉置(transpose)與共軛轉置(conjugate transpose)

> **考慮 $m \times n$ 矩陣 $A=[a_{ij}]$，則**
>
> (1) 稱 $A^T=[a_{ji}]_{n\times m}$ 為 $A$ 的轉置矩陣；
>
> (2) 稱 $A^H=[\overline{a_{ji}}]_{n\times m}$ 為 $A$ 的共軛轉置矩陣。

**Note**

(1) 考慮實數 $a,b$，則複數 $w=a+bi$ 的共軛複數為 $\bar{w}=a-bi$。  
例如，$3-4i$ 的共軛為 $3+4i$；$-7+5i$ 的共軛為 $-7-5i$

(2) $A^T$ 有時也被記作 $A'$；$A^H$ 有時也被記作 $A^*$，稱做伴隨矩陣(adjoint matrix)。

(3) $A^H=\overline{A^T}$ 表示對 $A$ 作轉置後再對所有元素取共軛複數，當然 $A^H=\overline{A}^T$ 也成立。

例如：  
$A=\begin{bmatrix}1&0&6\\2&4&7\\3&5&8\end{bmatrix}$，$A^T=\begin{bmatrix}1&2&3\\0&4&5\\6&7&8\end{bmatrix}$；

$B=\begin{bmatrix}1&4\\2&5\\3&6\end{bmatrix}$，$B^T=\begin{bmatrix}1&2&3\\4&5&6\end{bmatrix}$；

$C=\begin{bmatrix}1+i&0&6\\2&4&-7\\3&5i&8\end{bmatrix}$，$C^H=\begin{bmatrix}1-i&2&3\\0&4&-5i\\6&-7&8\end{bmatrix}$；

$D=\begin{bmatrix}1&-4\\2&5\\3&-6i\end{bmatrix}$，$D^H=\begin{bmatrix}1&2&3\\-4&5&6i\end{bmatrix}$。