第九章 高等樹結構
435
Advanced Tree Structure
\begin{itemize}
\item[七．] Binomial Queue 之 Delete min 之動作
令有最小鍵值的（Root）之兩項式數為 $\mathrm{B}_{\mathrm{k}}$ ，令原先 Queue 為 H
Steps：（1）將 $\mathrm{B}_{\mathrm{k}}$ 自 H 中移除，得到新 Queue H＇
（2） $\mathrm{B}_{\mathrm{k}}$ 的 Root 移除，產生數個 $\mathrm{B}_0, \mathrm{~B}_1, \cdots \mathrm{~B}_{\mathrm{k}-1}$ 之 Binomial Queues 令為 $\mathrm{H}^{\prime \prime}$
（3）合併 $\mathrm{H}^{\prime}$ 與 $\mathrm{H}^{\prime \prime}$ 得到 Final result
例：B Queue 如下：
則 Delete min 之後的 Binomial Queue 為何？
解 ：（1） $\mathrm{H}^{\prime}$ ：（13）
\end{itemize}