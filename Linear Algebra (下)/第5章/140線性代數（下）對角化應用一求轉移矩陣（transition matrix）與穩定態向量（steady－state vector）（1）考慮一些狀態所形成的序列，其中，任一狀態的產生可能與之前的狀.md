140

線性代數（下）



對角化應用一

求轉移矩陣（transition matrix）與穩定態向量（steady－state vector）

（1）考慮一些狀態所形成的序列，其中，任一狀態的產生可能與之前的狀態有關，則稱此為一隨機過程（stochastic process）．

（2）若一隨機過程滿足以下條件，

（i）可能的狀態数有限．

（ii）每個狀態會發生的機率只與前一個狀態有關．

（iii）每個狀態會發生的機率為常数。

則稱此隨機過程為馬可夫過程或馬可夫鏈（Markov chain）．

（3）考慮包含 $n$ 個狀態的馬可夫锺，將狀態 $j$ 進入到狀態 $i$ 的機率以 $p_{i j}$ 紀錄，並稱為轉移機率，且稱 $P=\left[p_{i j}\right]_{n \times n}$ 為此 Markov chain 的塼移矩陣。

（4）若向量 $\boldsymbol{x}$ 的第 $i$ 分量 $x_i$ 表示一個含 $n$ 個狀態的 Markov chain 在某一觀察下進入到第 $i$狀態的機率，$i=1,2, \ldots, n$ ，則稱 $\boldsymbol{x}$ 為此 Markov chain 的一個狀態向量（state vector）．

（5）若 $A$ 為某馬可夫锺的一轉移矩陣且存在正整数 $k$ 使得 $A^k$ 中的元素都為正，則稱 $A$ 為一正則（regular）轉移矩陣。

（6）考虑正則轉移矩陣 $A$ ，機率向量 $\boldsymbol{x}$ ，則 $\lim _{k \rightarrow \infty} A^k$ 存在且 $\lim _{k \rightarrow \infty} A^k \boldsymbol{x}=\boldsymbol{p}$ ，其中 $\boldsymbol{p}$ 為與 $k$ 無關的機率向量，並稱之為 $A$ 的穩定狀態向量．



Note

（1）若方陣 $A$ 的各行元素和均為 1，則稱 $A$ 為一Markov矩陣，隨機矩陣或機率矩陣．Markov過程的轉移矩陣必為一 Markov 矩陣。

（2）考慮向量 $x: n \times 1$ ，若各分量 $x_i$ 均非負且滿足 $x_1+\ldots+x_n=1$ ，則稱 $\boldsymbol{x}$ 為一機率向量．

（3）考慮 Markov 矩陣 $A$ ，機率向量 $\boldsymbol{p}$ ，則

（a） 1 為 $A$ 的特徵根．

【 84 中正統計、 87 交大統計、 87 中山應數、 102 成大數學、 106 交大資工】

（b）$A \boldsymbol{p}$ 一為機率向量．

（c）$A^k$ 亦為 Markov 矩陣。

【105中興統計】

（d）$A$ 的特徵根 $\lambda$ 均滿足 $|\lambda| \leq 1$ 。



【97交大應數、101台大數學】