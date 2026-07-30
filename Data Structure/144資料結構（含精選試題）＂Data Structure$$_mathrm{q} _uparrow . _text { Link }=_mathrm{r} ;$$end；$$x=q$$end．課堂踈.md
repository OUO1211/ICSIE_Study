144
資料結構（含精選試題）
＂

Data Structure
$$
\mathrm{q} \uparrow . \text { Link }=\mathrm{r} ;
$$
end；
$$
x=q
$$
end．

課堂踈習
（1）計算 Single link list 長度，（2）連接兩個 Circular list，（3）Invert a circular list

4－8 等位關係（Equivalence Relations）
\begin{itemize}
\item[一．] 定義
對於集合 S 上的一個關係三，若且唯其具有對稱性、反身性與遞移性於集合 S 上。則稱此關係在集合 S 上為一等位關係。
\item[] 【註】1．反身性（Reflective）， $\mathrm{X} \equiv \mathrm{X}$
\begin{itemize}
\item[2．] 對稱性（Symmetric），if $\mathrm{X} \equiv \mathrm{Y}$ 則 $\mathrm{Y} \equiv \mathrm{X}$
\item[3．] 遞移性（Recursive），if $\mathrm{X} \equiv \mathrm{Y}$ and $\mathrm{Y} \equiv \mathrm{Z}$ 則 $\mathrm{X} \equiv \mathrm{Z}$
\end{itemize}
\item[二．] 例子
在 Fortran 程式中，假設有 12 個變數（ $1 \sim 12$ ），透過等位關係敘述的使用而具有以下的等位關係：
$$
1 \equiv 5,4 \equiv 2,7 \equiv 11,9 \equiv 10,8 \equiv 5,7 \equiv 9,4 \equiv 6,3 \equiv 12,12 \equiv 1
$$
則可以分成三堆具有等位變數的部份集合：
$$
\{1,3,5,8,12\} ;\{2,4,6\} ;\{7,9,10,11\}
$$
因此，12 個變數只須要三個變數的空間。
\item[三．] 演算法
決定等位集合的演算法需要對輸入做兩階段（Phase）的處理。第一階段是讀入所有的等位對（i，j）並储存起來；第二階段中首先找到所有形式為（i，j）的等位對，此乃表示 i與 j之直屬於同一等位集合，再利用遞移性找到所有的（j，k）等位對，表示 k 亦屬於該等集合。繼續此步驟直到整個包含 i 的等位集合找好為止，找好後將之標記並印出。然後，再繼續找下一個等位集合。
\end{itemize}