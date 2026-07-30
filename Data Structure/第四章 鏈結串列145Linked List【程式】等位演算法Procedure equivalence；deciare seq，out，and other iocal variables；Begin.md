第四章 鏈結串列
145
Linked List

【程式】等位演算法
Procedure equivalence；
deciare seq，out，and other iocal variables；
Begin
initialize seq to nil and out to true；
while more pairs do｛input pairs\}
Begin
read the next pair $(\mathrm{i}, \mathrm{j})$ ；
put j on the seq［i］list；
put i on the seq［j］list；
End
for $\mathrm{i}:=1$ to n do｛output equivalence classes\}
if out［i］then Begin
out［i］：＝false；
output this equivalence class；
End
End；｛of equivalence\}

\section*{【圖表說明】}

對於每一個三的關係，它在表示方式中佔了兩個節點，seq［i］則是指到包含所有與第 i個變數等位之變串列。
在第一階段中我們就可以掃描 seq 陣列找到第一個 $\mathrm{i}(1 \leq \mathrm{i} \leq \mathrm{n})$ 滿足 out $[\mathrm{i}]=$ true 者，然後將 seq［i］串列中的每一元素印出。為了能利用遞移性的特徵處理其它與 i 等位的串列，我們建立一個堆疊來存等位的各個節點，此是靠改變 link 使其方向反過來而完成。完整的演算法如下所示。