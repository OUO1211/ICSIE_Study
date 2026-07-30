80
資料結構（含精選試題）
Data Structure

\section*{三．對應到一個一維陣列 $\mathrm{B}(1: \mathrm{n}(\mathrm{n}+1) / 2)$ 的儲存方式}
\begin{itemize}
\item[（一）] 以列為主（Row－major）
下三角：$a_{i j}=i(i-1) / 2+j=k$ ，放入 $B(k)$ 中
上三角：$a_{i j}=n(i-1)-i(i-1) / 2+j=k$ ，放入 $B(k)$ 中
\item[（二）] 以行為主（Column－Major）
下三角：$a_{i j}=n(j-1)-j(j-1) / 2+i=k$ ，放入 $B(k)$ 中
上三角：$a_{i j}=j(j-1) / 2+i=k$ ，放入 $B(k)$ 中
\end{itemize}

\section*{2－6 對稱矩陣（Symmetric Matrix）}
\begin{itemize}
\item[（一）] Def：A $\mathrm{n} \times \mathrm{n}$ 為一Symmetric matrix，其中 $\mathrm{A}[\mathrm{i}, \mathrm{j}]=\mathrm{A}[\mathrm{j}, \mathrm{i}]$
\item[（二）] 有效的儲存方式：只存上三角或下三角部份即可。
\end{itemize}

\section*{例題（2－14}

A $\mathrm{n} \times \mathrm{n}$ Symmetric matrix is stored with its upper diagonal part in column－major order．
Please write a single expression for k to store A［i，j］in one dimension array B［k］．
\begin{itemize}
\item[] （Hint：you can use the Max and Min function in your expression）
\item[解] 對稱矩陣元素以上三角部份 Column－major 存到一維陣列 B 中，其相當於下三角Row－major 之順序，故分別寫出對應的公式。
再利用 Max and Min function 將其合併成單一公式
$$
\therefore \mathrm{k}=\frac{[\operatorname{Max}(\mathrm{i}, \mathrm{j}) *(\operatorname{Max}(\mathrm{i}, \mathrm{j})-1)]}{2}+\operatorname{Min}(\mathrm{i}, \mathrm{j})
$$
\end{itemize}

\section*{2－7 寛帶矩陣（Band Matrix）}
\begin{itemize}
\item[（一）] Def：矩陣為 Band matrix，表示其為一個 An，a，b
$n \times n$ 矩陣，其中對角線以下（含對角線）a 條斜線有元素，對角線（含）以上 ${ }^b$條斜線有元素，其餘為零元素。
\end{itemize}