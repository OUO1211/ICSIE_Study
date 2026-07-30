402
資料結構（含精選試題）
■■

Data Structure
\begin{itemize}
\item[（二）] 在1962年 Adelson－Velskii 和 Landis 提出了一種二元樹的結構使得二元樹可以根據子樹的高度而得到均衡。如果樹中有 n 個節點，動態取出可在 O（logn）時間內完成。同時，一新的識別字可在 O（logn）時間內加入或刪除。其結果的樹仍維持高度平衡（Height Balanced）。這個由他們三人所提出的樹稱為 AVL 樹。
\end{itemize}
（三）定義
一空樹必為高度平衡。如果 T 不是空的二元樹， $\mathrm{T}_{\mathrm{L}}$ 和 $\mathrm{T}_{\mathrm{K}}$ 為其左右子樹，且滿足：
\begin{itemize}
\begin{itemize}
\item[1．] $\mathrm{T}_{\mathrm{L}}$ 和 $\mathrm{T}_{\mathrm{R}}$ 均是高度平衡樹。
\item[2．] $\left|\mathrm{h}_{\mathrm{L}}-\mathrm{h}_{\mathrm{R}}\right| \leq 1$
其中 $\mathrm{h}_{\mathrm{L}}$ 和 $\mathrm{h}_{\mathrm{R}}$ 分別為 $\mathrm{T}_{\mathrm{L}}$ 和 $\mathrm{T}_{\mathrm{R}}$ 的高度，那麼 T 為高度平衡。
\end{itemize}
\item[（四）] 平衡係數（Balance Factor）
定義：一二元樹內節點 T 的平衡係數定義為 $\mathrm{h}_{\mathrm{L}}-\mathrm{h}_{\mathrm{R}}$ ，其中 $\mathrm{h}_{\mathrm{L}}$ 和 $\mathrm{h}_{\mathrm{R}}$ 為 T 的左右子樹的高度。在 AVL 樹的任何一個節點 T， $\operatorname{BF}(\mathrm{T})=-1,0$ 或1。
\item[（五）] AVL 樹的不平衡
在 AVL 樹中插入或刪除一個節點，使得原來是右高一層或右高一層，如今變成左高二層或右高二層。
有四種不平衡狀況：
\item[] LL：
\end{itemize}