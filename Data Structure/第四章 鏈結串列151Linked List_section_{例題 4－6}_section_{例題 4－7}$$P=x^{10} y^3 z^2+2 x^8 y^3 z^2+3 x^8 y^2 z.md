第四章 鏈結串列
151
Linked List

\section*{例題 4－6}

\section*{例題 4－7}
$$
P=x^{10} y^3 z^2+2 x^8 y^3 z^2+3 x^8 y^2 z^2+x^4 y^4 z+6 x^3 y^4 z+2 y z
$$
改寫成 $\left(\left(\mathrm{x}^{10}+2 \mathrm{x}^8\right) \mathrm{y}^3+3 \mathrm{x}^8 \mathrm{y}^2\right) \mathrm{z}^2+\left(\left(\mathrm{x}^4+6 \mathrm{x}^3\right) \mathrm{y}^4+2 \mathrm{y}\right) \mathrm{z}$
則結果如下：
【圖示】以每個節點含三欄之結構表示 $\mathrm{P}(\mathrm{x}, \mathrm{y}, \mathrm{z})$ 。我們沒有顯示出 trio 欄它的值可以很容易地從節點結構得知。

基本上任何一般化的串列，都可以利用如下所示的節點結構來表示：
$$
\begin{gathered}
\begin{array}{l|l|l|}
\text { tag }= & \begin{array}{|l|l|}
\hline \text { true fase } & \text { data dlink }
\end{array} & \text { link } \\
\text { type } & \text { listpointer }= & \uparrow \text { listnode; } \\
\text { listnode } \quad= & \text { record }
\end{array} \\
\text { link : listpointer; } \\
\text { case tag : boolean of } \\
\\
\text { false : (data : char); } \\
\text { true : (dlink : listpointer); } \\
\text { end; }
\end{gathered}
$$
【註】Data欄的資料型態隨著應用問題而有所改變。