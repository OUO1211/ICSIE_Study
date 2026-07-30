第9章 圆論11207

\section*{以標號法求最大流量}

輸入：傳輸網路 $N=(V, E)$ 。 輸出：$N$ 上的最大流量 $f$ 。
Step 1：將 $N$ 上的每一邊 $e$ 给權值 $f(e)=0$ 。
Step 2 ：將起點（source）$a$ 標記為 $(-, \infty)$ 。
Step 3：若存在未標記的點（稱作 $y$ ），以下列情形，對 $y$ 作如下標記：
\begin{itemize}
\item[（1）] 若存在任一已標記點 $x$ ，方向為 $x \rightarrow y$ ，且 $c(x, y)-f(x, y)>0$ ，則將 $y$ 記為$\left(x^{+}, \Delta(y)\right)$ ，其中 $\Delta(y)=\min \{\Delta(x), c(x, y)-f(x, y)\}$ ；若有多種 $x$ ，則任取一個。
\item[（2）] 否則，找任一已標記點 $x$ ，方向為 $y \rightarrow x$ ，且 $f(x, y)>0$ ，並將 $y$ 記為 $\left(x^{-}, \Delta(y)\right)$ ，其中 $\Delta(y)=\min \{\Delta(x), f(x, y)\}$ 。
\item[（3）] 若無（1）與（2）均無法完成，則稱 $y$ 無法標記。
\item[（4）] 重複 Step3 直到一若每點都標記完成或存在都無法標記的點，則到 Step4。
\item[] Step 4 ：（1）若所有點皆能標記，則根據每點的標記，從 $z$ 沿著標記的點，逆回去找出從 $a$到终點 $z$ 的可增路徑 $P$ ，並以 $z$ 上標註的数字，沿著 $P$ 改變每邊的流量，其他$N$ 上的邊不變。將 $a$ 以外的點的標記去掉，然後重複 Step 3。
\item[（2）] 否則，即有些點無法標記，停止程序，輸出 $\sum_{x \in V} f(x, z)$ 即為最大流量。同時輸出最小切集 cut（｛可標記點\}, \{不可標記點\}) 。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 可增路徑 $P$ 之找法：從 $z$ 逆回去若 $z$ 標記為 $\left(x^{+}, \Delta(z)\right)$ ，則將 $(x, z)$ 邊上的流量增加 $\Delta(z)$ 。接著再看 $x$ 點上的標記，
若為 $\left(v^{+}, \Delta(x)\right)$ ，則將 $(v, x)$ 邊上的流量增加 $\Delta(z)$ ；
若為 $\left(v^{-}, \Delta(x)\right)$ ，則將 $(v, x)$ 邊上的流量減少 $\Delta(x)$ ，
然後再從 $v$ 找回去直到起點 $a$ 。
\item[（2）] 遇到可增路徑上有負號時的範例如下：

圖一

圖二

圖三
\end{itemize}