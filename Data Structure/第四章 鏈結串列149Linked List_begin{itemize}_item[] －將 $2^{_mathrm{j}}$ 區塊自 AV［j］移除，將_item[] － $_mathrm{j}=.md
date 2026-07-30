第四章 鏈結串列
149

Linked List
\begin{itemize}
\item[] －將 $2^{\mathrm{j}}$ 區塊自 AV［j］移除，將
\item[] － $\mathrm{j}=\mathrm{j}-1$ ；end；
\item[（四）] 當 $\mathrm{j}=\mathrm{k}$ 時，配置 $2^{\mathrm{k}}$ 給 Process
\item[（五）] 若 j＞m then 表示無夠大空間可以配置
\end{itemize}

四．回收方式
\begin{itemize}
\item[（一）] 假設歸還區塊起始位址為 x，大小為2 ${ }^{\mathrm{k}}$ ，則：（1）檢查有無 Buddy 存在
\begin{itemize}
\item[（2）] 若無 Buddy，則將此區塊加入 AV［k］串列當中
\item[（3）] 若有 Buddy 存在，則與 Buddy 合併，並針對合併區塊goto（1）
\end{itemize}
\item[（二）] 何謂 Buddy
Buddy 的定義為：$\left\{\begin{array}{l}\text { ①大小相同（即等於 } 2^{\mathrm{k}} \text { ），且 } \\ \text { ②起始位址 } \mathrm{y} \text { ，必須等於 } \mathrm{x} \oplus 2^{\mathrm{k}}\end{array}\right.$
\item[（三）] Buddy 合併
\end{itemize}

4－10 一般化串列
\begin{itemize}
\item[-] ．定義
\item[-] 個一般化串列（Generalize List）A 為一有限個而且具順序的 n 個元素（ $\mathrm{n} \geq \phi$ ）：$\left(\alpha_1, \alpha_2, \cdots, \alpha_{\mathrm{a}}\right)$ ，其中 $\alpha_{\mathrm{i}}$ 可以是基本元素（Atom）或是串列，如果 $\alpha_{\mathrm{i}}$ 本身是串列的話，那稱為 A 的子串列（Sublist）。
\item[] 串列 A 本身以 $\mathrm{A}=\left(\alpha_1, \alpha_2, \cdots, \alpha_{\mathrm{a}}\right)$ 表示，A 為串列 $\left(\alpha_1, \alpha_2, \cdots, \alpha_{\mathrm{a}}\right)$ 的名稱，而 n 為串列的長度。習慣上，所有串列的名稱均以大寫表示，而小寫則表示基本單位之元素。如
\end{itemize}