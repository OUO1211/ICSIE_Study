182
資料結構（含精選試題）
Data Structure

Step 3 ：建完之後，再以中序法 Traversal，就是排序結果。
【註】此 Sorting 結果是由小到大。
若要由大到小，則先將結果置於 Stack 中再行輸出。
例：假設一字元順序，且字元順序由 A 開始遞增 D，L，B，K，C，P，A，F 則建立二元樹順序如下：
（1）D
（2）
（3）
（4）
（5）
（6）
（7）
（8）
中序追蹤如下：A B C D F K L P

\section*{5－7 引線二元樹（Thread Binary Tree）}

一．使用原因及定義
因為二元樹的空鏈結浪費了幾近一半，若將這些空的鏈結欄充分利用，使其指到其他的節點，則這些指標 Link 稱為 Thread，而這種二元樹就稱之為：Thread Binary Tree ${ }^*$