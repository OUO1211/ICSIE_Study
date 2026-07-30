238
資料結構（含精選試題）
■■■

Data Structure

G3 的一些子圖如下：（未完全列出來）
\begin{itemize}
\item[3．] Path（路徑）
定義：指一個由頂點所組成的序列 $\mathrm{V}_{\mathrm{i}}, \mathrm{V}_{\mathrm{i} 1}, \mathrm{~V}_{\mathrm{i} 2}, \cdots$
$\mathrm{V}_{\text {in }}, \mathrm{V}_{\mathrm{j}}$ ，其中 $\left(\mathrm{V}_{\mathrm{i}}, \mathrm{V}_{\mathrm{i} 1}\right),\left(\mathrm{V}_{\mathrm{i} 1}, \mathrm{~V}_{\mathrm{i} 2}\right), \cdots\left(\mathrm{V}_{\mathrm{in}}, \mathrm{V}_{\mathrm{j}}\right)$
皆是 $E(G)$ 上的邊。
\item[4．] Path Length（路徑的長度）
定義：路徑上所包含的邊之數目。
\item[5．] Simple Path
定義：路徑上除了起點和終點可能相同之外，其他頂點皆不相同。
例：1，2，4， 3 是 Simple Path
但 1，2，4， 2 不是 Simple Path
\item[6．] Cycle
定義：是一個 Simple Path，且起點和終點相同。
\item[7．] Connected
定義：無向圖形中，如果每個成對的頂點 $\mathrm{V}_{\mathrm{i}}, \mathrm{V}_{\mathrm{j}}$ ，都有路徑相通，則稱圖形是連通的。
例：G1，G2 是 Connected，而底下的圖形也是 Connected
\end{itemize}