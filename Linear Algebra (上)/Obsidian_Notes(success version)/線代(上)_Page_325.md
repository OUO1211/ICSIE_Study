## 可逆與四大子空間的性質整理

下列為 $n$ 階方陣 $A$ 可逆的等價條件：

> **定理**
>
> (1) $\ker(A)=\{0\}$（$\therefore \dim(\ker(A))=0$）。
> (2) $A$ 的行向量為線性獨立。 【97 台北統計】
> (3) $A$ 的行向量形成 $F^{n\times 1}$ 的基底。
> (4) $A$ 的行向量生成 $F^{n\times 1}$。
> (5) $CS(A)=F^{n\times 1}$，故 $\dim(CS(A))=n$。
> (6) $\operatorname{Lker}(A)=\{0\}$（$\therefore \dim(\operatorname{Lker}(A))=0$）。
> (7) $A$ 的列向量為線性獨立。
> (8) $A$ 的列向量形成 $F^{1\times n}$ 的基底。
> (9) $A$ 的列向量生成 $F^{1\times n}$。
> (10) $RS(A)=F^{1\times n}$，故 $\dim(RS(A))=n$。

**【說明】**

$(1)\sim(5)$：

$A$ 可逆 $\Rightarrow \ker(A)=\{0\}$。 （這是第二章提到的，即 $Ax=0$ 只有 $x=0$ 為解）

$\ker(A)=\{0\}\Leftrightarrow A$ 的行獨立。 （這是第三章第二小節獨立性質的討論）

$A$ 行獨立 $\Leftrightarrow A$ 的行向量為 $F^{n\times 1}$ 的一組基底。 （這是因為 $\dim(F^{n\times 1})=n$，而有 $n$ 個行）

$A$ 的行向量為 $F^{n\times 1}$ 的一組基底 $\Leftrightarrow A$ 的行向量生成 $F^{n\times 1}$。 （理由同上）

$A$ 的行向量生成 $F^{n\times 1}\Leftrightarrow CS(A)=F^{n\times 1}$。 （由定義可得）

$(6)\sim(10)$：

以下說明 $A$ 可逆 $\Leftrightarrow \operatorname{Lker}(A)=\{0\}$，其餘仿(1)〜(5)的討論可得。

$\Rightarrow$ 設 $yA=0$，則 $yAA^{-1}=0A^{-1}=0$，即 $y=0$，故 $\operatorname{Lker}(A)=\{0\}$。

$\Leftarrow$ 設 $yA=0$，只有 $y=0$ 此解，即 $A^T y^T=0$ 只有 $y^T=0$ 此解，即 $A^T$ 可逆，即 $A$ 可逆。