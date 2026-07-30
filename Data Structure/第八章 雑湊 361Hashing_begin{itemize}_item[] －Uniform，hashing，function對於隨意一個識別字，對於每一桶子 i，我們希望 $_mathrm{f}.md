第八章 雑湊 361
Hashing
\begin{itemize}
\item[] －Uniform，hashing，function
對於隨意一個識別字，對於每一桶子 i，我們希望 $\mathrm{f}(\mathrm{X})=\mathrm{i}$ 的機率均為1／b。這樣子，隨意一個識別字被對映到任何一個桶子的機率就皆相同。
\item[] －Perfect hashing
Def：此一 hashing function design 保證絕不會有 collision 發生，適用於 static hashing 且所有資料均事先已知。
\end{itemize}
（二）四種不同的 Hashing Function 之討論
\begin{itemize}
\item[1．] 平方值取中間位數（Middle square）
此種函數 $\mathrm{f}_{\mathrm{n}}$ 的計算是先將識別字之值平方，然後截取此平方數中間的一些合適之位元數來當作 bucket 位址之值；在此假設識別字可以用一字元來表示。因為平方值的中間位元之值通常與識別字的所有字母相關，因此不同識別字所產生之雜湊位址相異的機率應該很高，即使識別字彼此有一些相同的字母亦很有可能產生不一樣的雜湊位址。
\end{itemize}

例：
$$
\text { HABE } \rightarrow 8125 \rightarrow 66015625 \rightarrow 156
$$
數值 平方 取中間三位
若實際空間位址範圍介於 0－499，而取中間三位的位址範圍介於0－999之間，超出範圍兩位，因此須再壓縮成1／2以對映真實位址
$$
\therefore \begin{array}{cc}
156 \rightarrow 78 & , \text { HABE } \rightarrow 78 \\
\text { 壓 } 1 / 2
\end{array} \begin{gathered}
\text { Hashing }
\end{gathered}
$$

2．除法（Mod 運算）
此函數是將識別字除以一選定之數 M，而取其餘數當做 X 的雜湊位址，即
$$
\mathrm{f}_0(\mathrm{X})=\mathrm{X} \bmod \mathrm{M}
$$
這樣子所得到的雜湊位址之範是 0 到（M－1），故雜湊表的大小至少應為b＝M 。此種雑湊函數中，M 的選擇是一個很重要的關鍵。
假若 M 能被 2 整除（亦即為偶數），那鍵值為奇數者將被對映到奇數編號的bucket（因為餘數必為奇數），而偶數鍵將被對映到偶數編號的 bucket。這樣子雜湊表的使用就有偏重的現象。故應避免此種情形。
一個好的 M 值應為：M 為一質數，且 M 不能整除 $r^k \pm a$ ，其中 k 與 a 的值不大。