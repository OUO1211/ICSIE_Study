320
資料結構（含精選試題）
Data Structure

決策樹如下圖所示：

定理7．1：對 n 個相異元素做排序的任何決策樹，其中必有一高度至少為 $\left\lceil\log _2(\mathrm{n}!)\right\rceil+1$
證明：對 n 個資料做排序共有 n！個可能結果，因此任何決策樹必定具有 n！個樹葉節點。但決策樹是二元樹，而階度為 k 的最多只有 $2^{\mathrm{k}-1}$ 個節點。因此決策樹之高度至少為 $\left\lceil\log _2 n!\right\rceil+1$ 。
推論：只利用比做排序的任何演算法，一定都具有計算時間為 $0\left(n \log _2 n\right)$ 的最壞情況。

證明：對於每一個 n！樹葉節點的決策，我們必須證明其必有一路徑之長度為$\mathrm{cn} \log _2 \mathrm{n}$ ，其中 c 為常數。由上述定理知，任何決策樹均有一長為 $\log _2 n!$ 的路徑，而
$$
\begin{aligned}
n! & =n(n-1)(n-2) \cdots(3)(2)(1) \\
& \geq(n / 2)^{n / 2}
\end{aligned}
$$
因此， $\log _2 \mathrm{n}!\geq(\mathrm{n} / 2) \log _2(\mathrm{n} / 2)=0\left(\mathrm{n} \log _2 \mathrm{n}\right)$

\section*{二．合併排序法（Merge Sort）}

如何將二個已排序過的檔案合併而得到另一個排好序的檔案。我們將討論二種不同的演算法。第一個非常簡單，它使用了0（n）額外空間。兩個將被合併的檔案為 $\left(x_1, \cdots, x_m\right)$和 $\left(\mathrm{x}_{\mathrm{m}+1} \cdots \mathrm{x}_{\mathrm{n}}\right)$ 。合併的結果 $\mathrm{z}\left(\mathrm{x}_1 \cdots \mathrm{x}_{\mathrm{n}}\right)$ 。