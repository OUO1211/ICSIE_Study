418
資料結構（含精選試題）
■■

Data Structure

圖 轉換一為3－節點的中左兒子之4－1節點

\section*{9－11 B 樹（B Tree）}

當欲處理的資料量逐漸變大時，記憶體容量將不足以容納這些龐大的資料，而必須藉由輔助記憶體的協助。因此，我們面臨了如何利用外部搜尋（external searching）來搜尋大檔案的資料。

由於 I／0 所花費時間遠比 cpu 所花費時間多，因此應儘量減少 I／0 的次數以加快資料的存取，因此使用較大 m 值的 m－way search tree 來取代 2－way search tree（AVL 樹的平衡的二元搜尋樹），將可減少 I／0 的次數。譬如使用128－way search tree，將祇需3次讀取 I／0。