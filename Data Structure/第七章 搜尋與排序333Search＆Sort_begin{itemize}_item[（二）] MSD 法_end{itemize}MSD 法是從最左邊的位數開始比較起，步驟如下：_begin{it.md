第七章 搜尋與排序
333

Search＆Sort
\begin{itemize}
\item[（二）] MSD 法
\end{itemize}

MSD 法是從最左邊的位數開始比較起，步驟如下：
\begin{itemize}
\item[1．] 以最左邊的位數當作鍵值，依序的將含有相同鍵值的資料同一個 Box 中。
\item[2．] 若在步驟一將資料分為 k 堆， $1 \leq \mathrm{k} \leq \mathrm{p}$ ，p 為所用之基底，則從每一可自行獨立進行插入排序。
\item[3．] 將排序完的各堆資料，依序合併起，來即可完成排序。
\item[（三）] 基數排序法之性能評估
\item[1．] 若被排序的數字為 $\mathrm{k}^1, \mathrm{k}^2, \mathrm{k}^3, \cdots \mathrm{k}^{\mathrm{d}}$ 共有 d 個位數，其中 k1 是最高位，kd 是最低位，若總共有 n 個資料，則當每個數字 k1 均大於 no，c 為常數，則利用 LSD 法，我們至少需要執行 d 次才能完成排序。當位數愈多，d↑，則 LSD 不適用，因此在 $\mathrm{k}^{\mathrm{i}}>\mathrm{n}^{\mathrm{c}}$ ，且 d↑，MSD 較優於 LSD 但是 LSD 較為典型，分成數堆後，不必再獨立排序。
\item[2．] 為一 Stable 的 Sorting Method
\item[3．] 演算法需要對資料做 d 趟處理，每一趟花費 $0(n+r)$ ，因此總共的計算時間是$O(d *(n+r))$ 。在數值資料的排序中，d 的值將選取的基數 r 而定，而且也與最大的鍵值有關。
\item[4．] 所需的額外空間很大，為 $0(n * r)$ 。
\end{itemize}