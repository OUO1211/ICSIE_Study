第三章 堆疊與佇列
95
Stack＆Queue
\begin{itemize}
\begin{itemize}
\item[] else
BEGIN
top ：＝top＋1；
stack $[$ top $]:=$ item；
END；
END；
\end{itemize}
\item[（五）] Pop（stack，item）／／item 為 output 變數
BEGIN
if top $=\psi$ then stackempty；
else
BEGIN
item ：＝stack［top］；
top ：＝top－1；
END；
END；
\end{itemize}

\section*{四．Stack 的應用}
（一）處理副程式呼叫（Subroutine Call）
當呼叫副程式之前，先將區域變數值、參數值及返回位址存到 Stack 上，形成一塊區域叫作 Stack Frame 或動作記錄（Activation record），待 Subroutine 執行完畢之後再從 Stack 上取出 Stack Frame，而回到主程式，恢復原先執行的狀況。
【圖示】System stack after function call
fp：pointer to the current stack frame

（a）

（b）