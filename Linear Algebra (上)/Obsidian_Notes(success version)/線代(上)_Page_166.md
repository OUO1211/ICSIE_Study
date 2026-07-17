# 第 2 章 線性方程組與求解 165

## 可逆與線性系統

> 考慮 $n$ 階方陣 $A$，則下列敘述彼此等價：  
> (1) $A$ 可逆。  
> (2) $Ax=0$ 只有零解。  
> (3) $\operatorname{rank}(A)=n$。  
> (4) $A$ 可列（或行）運算成為 $I_n$。  
> (5) $A$ 可表為若干列（或行）基本矩陣之積。  
> (6) $A$ 存左（或右）反矩陣。  

以下證明均討論列，讀者可自行練習行的證法。

$(1)\Rightarrow(2)$

設 $A$ 可逆，即 $A^{-1}$ 存在。設 $Ax=0$，則
$$
A^{-1}(Ax)=A^{-1}0=0
$$
即 $Ix=0$，即 $x=0$，即 $Ax=0$ 只有零解。

$(2)\Rightarrow(3)$

因為恰一組解，故 $\operatorname{rank}(A)=\text{行數 }n$。

$(3)\Rightarrow(4)$

因為 $\operatorname{rank}(A)=\text{行數 }n$ 且 $A$ 為方陣，故 $A$ 列運算最高可成為 $I_n$。  
$\therefore$ $Ax=0$ 只有零解，$\therefore \operatorname{rank}(A)=n$，即 $A$ 列等價 $I_n$。

$(4)\Rightarrow(5)$

$A$ 可列運算至 $I_n$，設對應的列基本矩陣為 $E_1,\ldots,E_k$，使
$$
(E_k\cdots E_1)A=I
$$
即
$$
A=(E_k\cdots E_1)^{-1}=E_1^{-1}\cdots E_k^{-1}
$$
為列基本矩陣的乘積。

$(5)\Rightarrow(1)$

$\because$ 列基本矩陣均可逆，故列基本矩陣的乘積亦為可逆，故 $A$ 可逆。

$(1)\Rightarrow(6)$

由定義顯而易得。

$(6)\Rightarrow(1)$

設 $BA=I$。設 $Ax=0$，則
$$
B(Ax)=B0
$$
即
$$
Ix=0 \therefore x=0
$$
即 $Ax=0$ 只有零解，故得 $A$ 可逆。