130
資料結構（含精選試題）
Data Structure

\section*{例題 4－3}

Linked List 的節點刪除。
假設 first 是一個指向锺結串列的指標，令 y 為指向位於 x 之前的節點，若 x＝first，則令 y＝nil，程式如下。
【程式】 procedure delete（x，y：pointer；var first：pointer）；
BEGIN
if $\mathrm{y}=$ nil then first ：= first ↑ ．link；
$$
\text { else } \mathrm{y} \uparrow \text {.link }:=\mathrm{x}
$$
dispose（x）；｛Return the node\}
END；｛of delete\}
【圖示】
\begin{itemize}
\item[1.]
\item[2.]
\end{itemize}

\section*{二．Storage Pool 的觀念}
\begin{itemize}
\item[（一）] 定義
所有可用的節點（Free Node）組合成可供使用的空間，稱為 Storage Pool。
\item[（二）] Get Node（x）
從可用的空間，取出一個節點。
【註】底下的AV為一指向可用空間串列首之指標。
\end{itemize}