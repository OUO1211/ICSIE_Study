366
資料結構（含精選試題）
Data Structure
\begin{itemize}
\item[1．] 對於線性開放定址（線性探測）
$$
\begin{aligned}
& \mathrm{U}_{\mathrm{a}} \fallingdotseq \frac{1}{2}\left[1+\frac{1}{(1-\alpha)^2}\right] \\
& \mathrm{S}_{\mathrm{n}} \fallingdotseq \frac{1}{2}\left(1+\frac{1}{1-\alpha}\right)
\end{aligned}
$$
\item[2．] 對於再次雜湊（Rehashing），隨機探測（Random Probig）與二次探測（Quadratic Probing）。
$$
\begin{aligned}
& \mathrm{U}_{\mathrm{n}} \fallingdotseq 1 /(1-\alpha) \\
& \mathrm{S}_{\mathrm{n}} \fallingdotseq-(1 / \alpha) \log _{\mathrm{e}}(1-\alpha)
\end{aligned}
$$
\item[3．] 對於串列之方法
$$
\begin{aligned}
& \mathrm{U}_{\mathrm{n}} \fallingdotseq \alpha \\
& \mathrm{~S}_{\mathrm{n}} \fallingdotseq 1+\alpha / 2
\end{aligned}
$$
\end{itemize}
這裡只對串列結果作一約略證明。如果要搜尋之識別字 X 之雜湊函數值為$\mathrm{f}(\mathrm{X})=\mathrm{i}$ ，而第 i 條串列中有 k 個節點（不含開頭節點），那麼如果 X 不在串列中就需要做 k 次比較；如果 X 在離開節點的第 j 個節點中 $(1 \leq j \leq k)$ ，那就需要比較 j 次。

當 n 個識別字是均匀地分布在 b 條串列中，那麼每一條串列的平均識別字個數為 $\mathrm{n} / \mathrm{b}=\alpha$ 。因此， $\mathrm{U}_{\mathrm{n}}=$ 串列中預期的識別字個數 $=\alpha$ 。
當第 i 個識別字 $\mathrm{X}_{\mathrm{i}}$ 要填入雜湊表時，每一條串列預期的識別字個數為（i－1）／b 。因此當 n 個識別字均填入雜湊表之後要搜尋 $\mathrm{X}_{\mathrm{i}}$ 識別字的預期比較次數為$1+(\mathrm{i}-1) / \mathrm{b}$（假設新的識別字是插在串列的前端），故可得
$$
S_n=\frac{1}{n} \sum_{i=1}^n\{1+(i-1) / b\}=1+\frac{n-1}{2 b} \fallingdotseq 1+\frac{\alpha}{2}
$$