第一章 基本概念
3

Basic Concepts
\begin{itemize}
\item[（二）] Testing：針對 code 的需要 the working code and sets of test data
\item[（三）] Error removal
\end{itemize}

\section*{1－2 Algorithm Specification}

\section*{1－2－1 Introduction}

【 Definition 】
An algorithm is a＂finite set＂of instructions that accomplishes a particular task．除此之外，還必須滿足下列5個標準：
\begin{itemize}
\item[] －．Input
Zero or more quantities that are provided by the outside
\item[二．] Output
至少要有一個以上的輸出 quantity 產生。
\item[三．] Definiteness
每個指令須 clear and unambiguous．（因為 algorithm 為 Text description，不同的人執行algo ，須有相同的作法指引）
\item[四．] Finiteness
If we trace out the instructions of an algorithm，then for all cases，the algorithm must ＂terminate＂after a finite number of steps．
\item[五．] Effectiveness
Every instructions must be basic enough to be carried out，in principle，by a person using only pencil and paper．
\item[] 【註】以計算理論來講 program 與 algorithm 最大的區分點在上述第四．Finiteness，因為 program 不一定要滿足上述第四。
\end{itemize}

接下來看幾個例子，來詮釋 Algorithm 到 program 的過程：