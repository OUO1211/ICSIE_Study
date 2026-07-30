308
資料結構（含精選試題）
■

Data Structure
\begin{itemize}
\item[（四）] 插補搜尋法（Interpolation Searching）
以查詢電話簿為例。上述二種搜尋法（Binary Search and Fibonacci Search）並不是人類在找電話號碼的方式。內插（Interpolation）搜尋的方法，首先是拿 k 與 f［ $\boldsymbol{\ell}+\mathbf{i ] . k e y}$相比較，其中：
$$
i=\frac{k-f[\ell] \cdot \text { key }}{f[u] \cdot \text { key }-f[\ell] \cdot \text { key }} \cdot(u-\ell+1)
$$
f［u］．key，f［ $\ell$ ］．key 分別是檔案中最大與最小的鍵值，這種搜尋法的工作情形顯然與檔案中鍵值的分佈有關。（Uniform Distribution 最好）
\item[（五）] 演算法
Procedure Intsrch（F，i，n，k）
Begin
$$
\ell:=1 ; \mathrm{u}:=\mathrm{n} ;
$$
while $\ell<=\mathrm{u}$ do Begin
$$
\mathrm{m}:=\left\lfloor\frac{\mathrm{k}-\mathrm{k} \ell}{\mathrm{ku}-\mathrm{k} \ell} \times(\mathrm{u}-\ell+1)\right\rfloor
$$
$\mathrm{m}:=\mathrm{m}+\ell$
case
\begin{itemize}
\item[（1）] $\mathrm{k}<\mathrm{km}: \mathrm{u}=\mathrm{m}-1$ ；
\item[（2）] $\mathrm{k}=\mathrm{km}: \mathrm{i}=\mathrm{m}$ ；return；
\item[（3）] $\mathrm{k}>\mathrm{km}: \mathrm{l}=\mathrm{m}+1$ ；
\end{itemize}
\end{itemize}
end；
End；｛of while\}
i = 0;
End；｛of Intsrch\}
\begin{itemize}
\item[（六）] 內插搜尋法的評估
\begin{itemize}
\item[1．] 其好壤完全依鍵值的分佈而定，在 Uniform 分佈時有最好的效果。在 $\mathrm{n}>500$ 時且鍵值為 Uniform Distribution 時，效果比二元搜尋法還要好。
\item[2．] 被搜尋的檔案仍須要滿足二個條件：
\begin{itemize}
\item[（1）] 檔案中的記錄必須事先經過排序。
\item[（2）] 必須是 Direct Access 或 Random access 機制支援
\end{itemize}
\end{itemize}
\end{itemize}