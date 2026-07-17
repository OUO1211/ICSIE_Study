22　線性代數(上)

# 矩陣的乘法不恆成立的性質

> **定理** （1）乘法交換律不恆成立。  
> 推廣：矩陣的二項式定理 $(A+B)^2=A^2+2AB+B^2$ 不恆成立。  
> 【99 成大資工、99.100 政大統計、101 台聯電機、108.109 中央資工、109 中山資工】

> **例** 例如取  
> $A=\begin{bmatrix}1&0\\0&0\end{bmatrix},\ B=\begin{bmatrix}0&0\\1&0\end{bmatrix}$，則 $AB=\begin{bmatrix}0&0\\0&0\end{bmatrix}$，$BA=\begin{bmatrix}0&0\\1&0\end{bmatrix}$。

> **定理** （2）若 $A\ne O$ 且 $B\ne O$，則 $AB\ne O$ 不恆成立。  
> （即「若 $AB=O$，則 $A=O$ 或 $B=O$」不恆成立）  
> （3）「對任意正整數，若 $A^n=O$，則 $A=O$」不恆成立。  
> （4）「若 $A^2=A$，則 $A=O$ 或 $I$」不恆成立。  
> （5）「若 $A^2=I$，則 $A=I$ 或 $-I$」不恆成立。  
> 【97 政大應數 99 交大應數 108 台聯電機】

> **例** 例如：  
> 取 $A=\begin{bmatrix}1&0\\0&0\end{bmatrix},\ B=\begin{bmatrix}0&0\\1&0\end{bmatrix}$，則 $AB=\begin{bmatrix}0&0\\0&0\end{bmatrix}$。  
> 取 $A=\begin{bmatrix}0&0\\1&0\end{bmatrix}$，則 $A^2=\begin{bmatrix}0&0\\0&0\end{bmatrix}$，但 $A\ne O$。  
> 取 $A=\begin{bmatrix}1&0\\0&0\end{bmatrix}$，則 $A^2=\begin{bmatrix}1&0\\0&0\end{bmatrix}$，但 $A\ne O$，且 $A\ne I$。  
> 取 $\begin{bmatrix}1&0\\0&1\end{bmatrix}$、$\begin{bmatrix}1&0\\0&-1\end{bmatrix}$、$\begin{bmatrix}-1&0\\0&1\end{bmatrix}$、$\begin{bmatrix}-1&0\\0&-1\end{bmatrix}$ 均滿足 $A^2=I$。

> **定理** （6）乘法消去律（若 $AB=AC$ 且 $A\ne O$，則 $B=C$）不恆成立。  
> 【93.94.101 中興資科、99 成大資工、102 中正統計、103 台北統計、109 中央資工】

> **例** 例如  
> 取 $A=\begin{bmatrix}1&0\\2&0\end{bmatrix},\ B=\begin{bmatrix}1&2\\0&0\end{bmatrix},\ C=\begin{bmatrix}1&2\\1&1\end{bmatrix}$，則 $AB=\begin{bmatrix}1&2\\2&4\end{bmatrix}=AC$，但 $B\ne C$。  
> 取 $A=\begin{bmatrix}1&0&0\\0&1&0\\0&0&0\end{bmatrix},\ B=\begin{bmatrix}0&0&0\\0&0&0\\0&0&1\end{bmatrix},\ C=\begin{bmatrix}0&0&0\\0&0&0\\0&0&2\end{bmatrix}$，則 $AB=\begin{bmatrix}0&0&0\\0&0&0\\0&0&0\end{bmatrix}=AC$，但 $B\ne C$。