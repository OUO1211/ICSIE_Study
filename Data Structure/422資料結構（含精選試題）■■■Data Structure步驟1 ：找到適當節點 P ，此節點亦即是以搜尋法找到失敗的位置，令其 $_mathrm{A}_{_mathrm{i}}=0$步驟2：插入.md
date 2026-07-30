422
資料結構（含精選試題）
■■■

Data Structure
步驟1 ：找到適當節點 P ，此節點亦即是以搜尋法找到失敗的位置，令其 $\mathrm{A}_{\mathrm{i}}=0$步驟2：插入資料X於節點P中。
步驟3：插入後，若 P 節點的鍵值數目 $\leq m-1$（m 是 B－tree 的 order），則完成插入動作，否則繼續步驟四。
步驟4：鍵值已滿，因此將節點 P 一分為二，成為兩個節點 P 及 $\mathrm{P}^{\prime}$ ，根據下列格式：
節點 P ：
$$
\mathrm{A}_0,\left(\mathrm{~K}_1, \mathrm{~A}_1\right),\left(\mathrm{K}_2, \mathrm{~A}_2\right), \cdots,(\mathrm{K}\lceil\mathrm{~m} / 2\rceil-1, \mathrm{~A}\lceil\mathrm{~m} / 2\rceil-1)
$$
節點 $\mathrm{P}^{\prime}$ ：
$$
\mathrm{A}\lceil\mathrm{~m} / 2\rceil,(\mathrm{K}\lceil\mathrm{~m} / 2\rceil+1, \mathrm{~A}\lceil\mathrm{~m} / 2\rceil+1) \cdots\left(\mathrm{K}_{\mathrm{n}-1}, \mathrm{~A}_{\mathrm{n}-1}\right)
$$
並將第 $\lceil\mathrm{m} / 2\rceil$ 個鍵值 $\mathrm{K}\lceil\mathrm{m} / 2\rceil$ 提昇提上一層的 parent 節點。若 parent 節點，直到鍵值未滿為止。
例：B－tree of order 3 如下，請畫插入動作後的結果圖形。