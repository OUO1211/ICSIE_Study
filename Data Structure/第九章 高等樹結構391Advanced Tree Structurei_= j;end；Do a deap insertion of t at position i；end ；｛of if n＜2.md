第九章 高等樹結構
391
Advanced Tree Structure
i:= j;
end；
Do a deap insertion of t at position i；
end ；｛of if n＜2 \}
end；

\section*{9－3 延伸二元樹（Extended Binary Tree）}

延伸二元樹（Extended Binary Tree）
定義一
任何一個二元樹中，若具有 n 個節點，則有 n－1個非空鏈結及 n＋1個空鏈結，若在每一個空鏈結加上一個特定節點，則稱其為外部節點（External Node）其餘的 Node稱為內部節點（Internal Node），當被搜尋的識別字不存在時，則搜尋到外部節點結束。

因此，External Node 又可稱為失敗節點（Failure Node）。這種加上 External Node的 Binary Tree 叫做 Extended Binary Tree。例：

（a）

（b）

外部路徑長度及內部路徑長度定義及定理
（一）定義
一延伸二元樹的外部路徑長度（External Path Length）為所有從根部到外部節點長度的總和。同理，內部路徑長度（Internal Path Length）為從根部到所有內部節點長度的總和。由上圖（a）的樹，我們得到其內部路徑長度 I 為
$$
I=0+1+1+2+3=7
$$
其外部路徑長度 E 為