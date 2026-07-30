第10章 樹 217

\section*{10－1 樹的基本定義與性質}

本章介紹圖論在資料結構上一項重要的概念一樹。但這裡是從圖論的定義出發，請讀者務必先熟悉本節關於樹的基本性質。

樹（tree）
若無向圖 $G$ 為一不含環路（acyclic）的連通圖，則稱 $G$ 為一個樹。
【83 交大資科】【88 中山資工】【92 海洋電機】【92、99 清大資應】
例如左圖是樹，右圖是森林。
例如， 5 個無號點的非同構樹有 3 種； 6 個無號點的非同構樹有 6 種。
【111 中正資工】【108 清大資工】【90 交大資科】【96 台大電機】

Note
\begin{itemize}
\item[（1）] 只有一個點的無邊圖又稱為一退化樹（degenerated tree 或 trivial tree），點數大於1的樹稱為非退化樹（non－degenerated tree）。
\item[（2）] 不含環路而有 $k$ 個分量的圖稱為含 $k$ 個樹的樹林（forest）。
\end{itemize}

【92海洋電機】
\begin{itemize}
\item[（3）] 若一有向圖不含有向圈（directed cycle），則稱之為 directed acyclic graph。
\item[（4）] 重要性質：
\begin{itemize}
\item[（1）] $T$ 為非退化樹 $\Leftrightarrow T$ 中任意兩點恰有唯一路徑相連。
\end{itemize}
\end{itemize}

【91、97政大資科】【101 清大資工】【105 中山電機】