98
資料結構（含精選試題）
■■

Data Structure

END；
END；

\section*{【上述作法之問題】}

Queuefull 訊息並不表示佇列中一定包含 n 個元素，即真的為滿。因加入與刪除的動作一直重複，將使佇列逐漸向右移動，而當佇列的尾端碰到陣列的邊緣便產生Queuefull 的訊息。
因此當 Queuefull 訊息產生時，我們自然地就要將整個 Queue 往左移使其第一個元素又存於 q［1］的位置，且將 front 設為0。
其缺點為浪費時間假設佇列有 n 個元素，而接下去我們每次都要先刪除一元素再加入一元素則每次加入元素之前，須先將 Queue 中 n－1 個元素往左移。

【方法 2】將陣列視為一個環狀，即：環狀佇列（Circular Queue）
$$
q=\operatorname{array}[0 \cdots n-1]
$$
如此，當 rear－n－1而 q［0］為空時，那麼下一個元素就存入 q［0］的位置。所以會利用 mod 運算，即 rear＝（rear＋1）mod n。
所以：
（一）ADDQ（item）
BEGIN
rear ：＝（rear＋1）mod n
if front＝rear then queuefull
else
BEGIN
q［rear］：＝item；
END；
END；
（二）DELETE（q）
BEGIN
if front＝rear then queueempty；
else
BEGIN
front ：$=($ front +1$) \bmod \mathrm{n}$
item ：＝q［front］；