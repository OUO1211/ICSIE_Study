14
資料結構（含精選試題）
■■■

Data Structure
\begin{itemize}
\item[] Def：An ADT is a data type that is organized in such a way that the specification of the objects and the specification of the operation on the objects is separated from the representation of the objects and the implementation of the operations．
\item[二．] ADT 上的 operation spec 與 implementation of the operation 有何不同 ？
基本上，the specification 包含了：
\item[（一）] Function Name
\item[（二）] The type of its argument
\item[（三）] The type of its result
但卻沒有將 Internal representation 或 Implementation details 顯示出來
→ 因此 ADT 是 Implementation－Independent
\item[三．] ADT 上的 Function 可以被分為三類
\item[（一）] Creator／Constructor
\begin{itemize}
\item[] → Create a new instance of the designed type．
\end{itemize}
\item[（二）] Transformer
\begin{itemize}
\item[] → Also create an instance of the designed type by using one or more other instances．
\end{itemize}
\item[（三）] Observers／Reporter
\begin{itemize}
\item[] → Provide information about an instance，but do not change instance．
\end{itemize}
\end{itemize}

\section*{1－4 Performance Analysis}

將 Performance Evaluation 粗分成二類：
\begin{itemize}
\item[（一）] Performance Analysis
\begin{itemize}
\item[1．] Obtaining estimate of time and space that are machine independent
\item[2．] Complexity theory．
\end{itemize}
\item[（二）] Performance Measurement
\begin{itemize}
\item[1．] Obtaining machine－dependent running time
\end{itemize}
\item[] －．Performance Analysis
\item[（一）] Space Complexity
\begin{itemize}
\item[1．] Def：The space complexity of a program is the amount of memory that it need to run to completion．
\end{itemize}
\end{itemize}