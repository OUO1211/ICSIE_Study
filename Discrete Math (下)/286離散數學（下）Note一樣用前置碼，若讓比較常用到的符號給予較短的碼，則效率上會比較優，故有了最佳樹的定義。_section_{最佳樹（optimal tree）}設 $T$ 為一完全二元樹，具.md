286
離散數學（下）

Note
一樣用前置碼，若讓比較常用到的符號給予較短的碼，則效率上會比較優，故有了最佳樹的定義。

\section*{最佳樹（optimal tree）}

設 $T$ 為一完全二元樹，具有 $n$ 個樹葉且指定為 $0<w_1 \leq w_2 \leq \ldots \leq w_n$ ，則
$W(T)=\sum_{i=1}^n w_i \cdot l\left(w_i\right)$ 稱為 $T$ 的權（weight of $T$ ），其中 $l\left(w_i\right)$ 表示權為 $w_i$ 的樹葉的階層數。對於指定 $w_1, w_2, \ldots, w_n$ 的完全二元樹中，具有最小權的稱為最佳樹。

Note
以下提供 Huffman 編碼的方式來找最佳樹。
Step1：將所給 weight（或機率）由小排到大，得一數列並以點標記之。
Step2：將最小兩數加總，得一新數列並以點標記之，且新所得的數連到原有最小兩數，重新排序。
Step3：重複 Step 2 ，直到剩一數。
Step4：整理所得，並以樹狀圖呈現。以 $0 、 1$ 搜尋標號所得點。