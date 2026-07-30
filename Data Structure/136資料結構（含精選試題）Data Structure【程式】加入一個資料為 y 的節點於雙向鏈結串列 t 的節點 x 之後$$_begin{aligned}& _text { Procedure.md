136
資料結構（含精選試題）
Data Structure

【程式】加入一個資料為 y 的節點於雙向鏈結串列 t 的節點 x 之後
$$
\begin{aligned}
& \text { Procedure Insert }(t, x, y) \\
& \text { Begin } \\
& \qquad \begin{array}{l}
\text { New(I); } \\
\mathrm{I} \uparrow . \text { Data }=\mathrm{y} \\
\mathrm{I} \uparrow . \text { L Link }=\mathrm{x} ; \\
\mathrm{I} \uparrow . \mathrm{R} \text { Link }=\mathrm{x} \uparrow . \mathrm{R} \text { Link; } \\
(\mathrm{x} \uparrow . \mathrm{R} \text { Link }) \uparrow . \text { L Link }=\mathrm{I} ; \\
\mathrm{x} \uparrow . \mathrm{R} \text { Link }=\mathrm{I} ; \\
\text { End; }
\end{array}
\end{aligned}
$$
\begin{itemize}
\item[2．] 刪除動作：刪除一個節點需要改變兩個指標。節點 X
\item[] 【程式】刪除雙向鏈鏈串列 t 的節點。
$$
\begin{aligned}
& \text { Procedure Delete }(t, x) \\
& \text { Begin } \\
& \quad(x \uparrow . \text { L Link }) \uparrow . R \text { Link }=x \uparrow . R \text { Link } \\
& \quad(x \uparrow . R \text { Link }) \uparrow . \text { L Link }=x \uparrow . \text { L Link; } \\
& \quad R E T(x) \text {; } \\
& \text { End; }
\end{aligned}
$$
\end{itemize}

3．雙向鏈串列的優缺點
優點：（1）加入／刪除任何一個節點時不用知道前一個節點的位址。
\begin{itemize}
\begin{itemize}
\item[（2）] 可由任何一個節點立即找到前一個或後一個節點。
\item[（3）] 可以將某一個可能 Lost 的指標適時地復原。
\item[] ④從任何一點開始，必可經過串列中所有 Nodes。
\end{itemize}
\end{itemize}

缺點：①增加一個指標，多浪費空間。
\begin{itemize}
\item[] ②新加入一個節點需改變四個指標，較 single Link List Double ef 。
\begin{itemize}
\item[（3）] 刪除一個節點必須改變兩個指標，較 single Link List Double efforts°
\end{itemize}
\end{itemize}