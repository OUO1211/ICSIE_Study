108
資料結構（含精選試題）
■■

Data Structure
就要負責移動其他堆疊以騰出空間給堆疊 i 使用。

U $[1 \cdots \mathrm{~m}]$ 等割成 n 個堆疊的初始情形，所有堆疊均為空的，且大小亦約略相等。

堆疊 i 與 i＋1 相碰，但在 U 的其它處仍有空間的情形。
程序 stackfull 的主要目的是希望只要陣列尚有空間，那任何堆疊要加入新元素都能達成。以下所述就是 stackull 的一種設計方法：
\begin{itemize}
\item[（1）] 決定一最小 j滿足 $\mathrm{i}<\mathrm{j} \leq \mathrm{n}$ 堆疊 j 與 j＋1 之間有未使用之空間，即：t［j］＜b［j＋1］如果 j 存在的話，那就將 i＋1，i＋2，．．．，j 等堆疊往右移一個位置。如此在堆疊 i 與 i＋1 之間就騰出一個位置了。
\item[（2）] 如果在（1）中找不到滿足條件的 j，那就往堆疊 i 的左邊尋找一個最大的 $\mathrm{j}(1 \leq \mathrm{j}<\mathrm{i})$滿足 $t[i]<b[j+1]$ ，即堆疊 j 與 j＋1 有空位置存在。如果有 j滿足條件，那就將$\mathrm{j}+1$ ， $\mathrm{j}+2, \ldots \mathrm{i}$ 等堆疊向左邊移動一個位置。如此在堆疊 i 與 i＋1之間就騰出一個位置了。
\item[（3）] 如果在（1），（2）中均找不到滿足條件的 j，那表示 U 的所有 m 個位置均已用盡，謂之真正的 Full。
\end{itemize}

\section*{五．Stack 與 Queue 可互相製作}
\begin{itemize}
\begin{itemize}
\item[（一）] 我們可以利用 stack 來製作 Queue，也可以用 Queue 來製作 stack。
\end{itemize}
\end{itemize}