第八章 雑湊
359
Hashing

\section*{8－2 靜態雜湊}

在靜態雜湊中，識別字儲存在一叫做雜湊表（Hashing Table）的固定大小表格中。任一讓別字 x 在表中的位址（或位置）是透過一個算術運算函數 f 計算而得，亦即 f（x）之值即為$X$ 在表中之位址。此位址 $f(X)$ 通常稱為 $X$ 的雜湊位址（Hash Address）或是本家位址（Home Address）。
\begin{itemize}
\item[（一）] 桶（Bucket）與槽（Slots）
雜湊表之記憶空間分割成 b 個桶（Bucket），分別為 ht［0］，ht［1］，⋯，ht［ b－1 ］，每一個桶包含 s 個槽（Slot），而每一槽可以容納一個記錄。
\item[（二）] 計算識別字位址之函數 f（X）稱為雜湊函數，其功能就是將識別字X做一轉換得到表中之位址。 $\mathrm{f}(\mathrm{X})$ 的值域從 $\phi$ 至 $\mathrm{b}-1$ 之整數中。
\item[（三）] 識別字密度（Identifier Density）與負載密度（Loading Density）
假設 n 為程式中所用的變數個數 T 為變數總數，那 n／T比值稱為識別字密度（Identifier Density），而 $\alpha=n /(\mathrm{sb})$ 則稱為負載密度（Loading Density）或稱負載因子（Loading Factor）。 $\alpha$ 值愈大則散置空間的使用率愈高，發生碰撞或溢位的機會也相對增高。
\item[（四）] 同義字（Synonym）
若兩識別字 $I_1$ 與 $I_2$ 雜湊函數值相同，即 $f\left(I_1\right)=f\left(I_2\right)$ ，那稱此兩識別字對於 $f$ 是同義字（Synonym）
\item[（五）] 碰撞（Collision）
兩個不同的識別字對映到同一個桶中稱之為碰撞（Collision）。當桶子之大小 s 等於1時，那碰撞與溢位就同時發生。
\item[（六）] 溢位（Overflow）
如果一識別字經雜湊函數所對應到的桶已經滿了，則稱之為溢位（Overflow）。
\end{itemize}

例如：
假設有一雑湊表有 $\mathrm{b}=26$ 個桶，而每一桶有兩個槽，即 $\mathrm{s}=2$ 。設一程式中使用了10 個相異的識別字，而每一識別字均以一字母為開頭。如此，此雜湊表的負載因子 $\alpha$ 即為 $10 / 52=0.19$ 。假設英文字母 A－Z 在內部的表示方式中分別以 $1-26$ 之數字表示，則雑湊函數定義為： $\mathrm{f}(\mathrm{X})=\mathrm{X}$ 之第一字母：如此雜湊函數必將所有的識別字 X 對映到雑湊表中。例如，GA，D，A，G，L，A2，A1，A3，A4與 E 等識別字將被對映到7，4，1，7，12，1，1，1，1與5等桶子中。而 A，A1，A2，A3 與 A4 是同義字，G