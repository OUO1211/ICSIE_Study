436
資料結構（含精選試題）
■■

Data Structure
（2）H＊：
（3）合併 $\mathrm{H}^{\prime}$ 與 $\mathrm{H}^{\prime \prime}$ ⑬

\section*{八．二系堆積（Binomial Heaps）［D．S．版］}

此資料結構支援的 operations 同 leftist tree 一樣（Insertion，Delete min 或 Delete max 及combine），不同於 Leftist tree，上述這些須 O（logn），但在 Binomial Heap 中執行的operation 某些可能須要 O（n）。
但如果分攤運算（昂貴）成本部份到不昂貴的運算上，則個別運算的分攤複雜度可能是O（1）或 O（logn），視 operation 種類而定。
－分攤成本（Amortized cost）
假設一連串的 Insertion 和 Delete min element 運算
I1，I2，D1，I3，I4，I5，I6，D2，I7
若插入運算的 actual cost 為 1，D1 和 D2 的 actual cost 為8和10
則運算總成本 $=25(7 \times 1+8+10)$
在分攤法則中，我們可以收取一個運算的部份 actual cost 分攤給其它運算，這可降低一些運算的收取成本，增加其它運算的收取成本。

⇒ 一個運算的 Amortized cost 是運算取收的全部成本
⇒ 成本分攤法則要求運算的分攤成本加總 $\geqq$ 實際成本的加總
\begin{itemize}
\item[] 例：對每一個 Delete min element 運算收取一個單位成本給在最後一次 Delete min element operation 之前的每一個 Insert operation
⇒ D1 的兩個單位成本轉給 I1，I2（則 I1，I2 的收取成本增加一個單位）D2 的四個單位成本轉給 I3～I6
\end{itemize}