96
資料結構（含精選試題）
■

Data Structure
\begin{itemize}
\item[（二）] 處理遞迴式呼叫（Recursive Call）
與（一）類似，在處理 Recursive Call 之前，先將參數值、區域變數值，返回位址一併保存到 Stack 上，以更將來能回到原來的地方處理。
\item[] 【註】The run－time program simply creates a new stack frame for each recursive call．
\item[（三）] 將算術中之中序表示法［Infix（LDR）］轉換成後序［PostFix（LRD）］或前序式表示法以便執行算術之計算。後序式計算及前序式計算也是 stack 應用。
\item[（四）] Compiler 執行文法剖析（Parsing）。例 LR Parser 採用 Shift－Reduce 方式需使用 Stack •
\item[（五）] 二元樹的中序追蹤（inorder）、前序追蹤（preorder）及後序（postorder）追蹤。
\item[（六）] Stack Computer 機器，指令的型式是 Zero－Operand，大部份用 Push、Pop 方式來處理算術式。
\item[（七）] 機器處理 Re－Entrant Routine（pure procedure）須有 Hardware 的 Stack 的 support。
\item[（八）] 圖形（Graph）的深度搜尋（depth－first search）。
\item[（九）] 資料反序輸出，例：原先由小至大改成由大至小。
\item[（十）] 自助餐廳取餐盤之行為（日常生活之例子）。
\item[] （十一）迷宮問題（maze problem）。
\item[] （十二）迴文判斷（palindrome）。
\end{itemize}

\section*{3－2 佇列（Queue）}
\begin{itemize}
\item[一．] 定義
為一具有 FIFO（First－in－First－out）性質的有序串列（order list），其：
\item[（一）] 插入（insert）的動作發生在尾端（rear）。
\item[（二）] 刪除（Delete／remove）的動作發生在前端（front），即插入與刪除動作在不同的兩端。
\end{itemize}

二．Queue ADT 之 Operations
\begin{itemize}
\item[（一）] Create Q（Q）：建立一個空的佇列。
\item[（二）] ADDQ（i，Q）：將元素 i 加入到佇列 Q 的尾端（rear），而得一新結果之佇列。
\item[（三）] DELETE（Q）：删除佇列 Q 之最前端之元素（Front），而傳回新的佇列。
\item[（四）] FRONT（Q）：傳回佇列 Q 之前端元素。
\end{itemize}