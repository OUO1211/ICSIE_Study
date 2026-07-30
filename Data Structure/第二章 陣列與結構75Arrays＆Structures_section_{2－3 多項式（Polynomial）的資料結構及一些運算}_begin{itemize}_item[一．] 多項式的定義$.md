第二章 陣列與結構
75
Arrays＆Structures

\section*{2－3 多項式（Polynomial）的資料結構及一些運算}
\begin{itemize}
\item[一．] 多項式的定義
$$
A(x)=a_n x^n+a_{n-1} x^{n-1}+\cdots+a_1 x+a_0
$$
其中 $a_n$ 是係數，n是指數。
\item[二．] 二種不同的資料結構表示方式（using array）
\begin{itemize}
\item[（一）] 按照指數由高到低，依序儲存係數
\item[] 作法：使用一個 n＋2 長度的一維陣列，n 最高指數，而陣列中的第一個元素存放n（即最高指數）。
\item[例] ： $\mathrm{A}(\mathrm{x})=4 \mathrm{x}^6+2 \mathrm{x}^4+7 \mathrm{x}^3+2 \mathrm{x}+1$
$$
\rightarrow \quad \mathrm{A}(1 \cdots 8)=(6,4,0,2,7,0,2,1)
$$
\item[] 優點：（1）只儲存係數，節省了儲存指數的空間。
\begin{itemize}
\item[（2）] 適用於零項次很少的多項式。
\end{itemize}
\item[] 缺點：當零項次很多的時候，則會浪費很多的空間。
\begin{itemize}
\item[例] ： $\mathrm{A}(\mathrm{x})=2 \mathrm{x}^{100}+1=$
上式須要（100＋2）個空間，但只用到三個空間。
\end{itemize}
\item[（二）] 只儲存非零項次的係數與指數
\item[] 作法：假設有 k 個非零項次，則使用陣列 $\mathrm{A}(2 \mathrm{k}+1)$ 來表示，陣列中第一個元素儲存 k。
\item[例] ： $\mathrm{A}(\mathrm{x})=4 \mathrm{x}^6+2 \mathrm{x}^4+7 \mathrm{x}^3+2 \mathrm{x}+1$
$$
\rightarrow \quad \mathrm{A}(1 . .11)=(5,6,4,4,2,3,7,1,2,0,1)
$$
\begin{itemize}
\item[] 指數 係數
\end{itemize}
\end{itemize}
\end{itemize}

優點：適用於零項次很多的多項式，節省了零項次的儲存空間。
\begin{itemize}
\begin{itemize}
\item[] 缺點：當非零項次很多（零項次很少）時，其空間約是第一種表示的二倍。
註：其餘的表示方式有二種（見 ch4，link list）
\end{itemize}
\item[三．] 多項式的運算（相加）
\end{itemize}

【演算法】
Procedure PADD（A，B，C）／／A，B，C 為多項式
｛
／／－－－－A＋B 產生一個新多項式給 C－－－－－／／
C = ZERO;