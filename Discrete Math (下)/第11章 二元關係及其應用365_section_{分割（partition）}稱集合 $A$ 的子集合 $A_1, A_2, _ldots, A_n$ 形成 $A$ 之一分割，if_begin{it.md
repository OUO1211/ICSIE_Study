第11章 二元關係及其應用
365

\section*{分割（partition）}

稱集合 $A$ 的子集合 $A_1, A_2, \ldots, A_n$ 形成 $A$ 之一分割，if
\begin{itemize}
\item[（1）] $A_i \neq \varnothing, \forall i=1,2, \ldots, n$ ．
（非空）
\item[（2）] $\bigcup_{i=1}^n A_i=A$ 。
（覆蓋 cover）
\item[（3）] $\forall i \neq j, A_i \cap A_j=\varnothing$ ．
（兩雨互斥 pairwise disjoint）
\end{itemize}

Note
\begin{itemize}
\item[（1）] 每個 $A_i$ 也都稱為 cell 或 block。
\item[（2）] 設 $R$ 為定義在 $A$ 上的等價關係，則
$\forall a, b \in A, a R b \Leftrightarrow[a]=[b] \Leftrightarrow[a] \cap[b] \neq \varnothing$ 。（故知，任兩相異等價類必互斥）
【105 彰師資工】
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] ⇒（2）
\end{itemize}
設 $x \in[a]$ ，即 $x R a$ ，而因為 $a R b$ ，且 $R$ 有遞移性，故 $x R b$ ，即 $x \in[b]$ ，故 $[a] \subseteq[b]$ ；
設 $x \in[b]$ ，即 $x R b$ ，而因為 $a R b$ ，且 $R$ 有對稱性，故 $b R a$ ，又因 $R$ 有遞移性，故 $x R a$ ，
即 $x \in[a]$ ，故 $[b] \subseteq[a]$ ，故得 $[a]=[b]$ 。
\begin{itemize}
\item[（2）] ⇒（3）因每一等價類均不為空集合，故當然成立。
\item[（3）] $\Rightarrow$（1）設 $\exists x \in[a] \cap[b]$ ，即 $x R a$ 且 $x R b$ ，
\end{itemize}
又因為 $R$ 有對稱性，故得 $a R x$ 且 $x R b$ ，而因為 $R$ 有遞移性，故 $a R b$ ，得證。
\begin{itemize}
\item[（2）] 設 $R$ 為 $A$ 上之等價關係，則 $R$ 的相異等價類形成 $A$ 之一分割。
【96 雲科資工】【98 暨南資工】【98 台大資工】
\item[（3）] $A$ 上的分割方式亦可決定一種 $A$ 上的等價關係。
\end{itemize}

【96 雲科資工】【107 中央資工】
\begin{itemize}
\item[（4）] 而由（2）、（3）的討論可得，等價關係個數，相當於集合分割的方法數。
\item[（5）] 分割的積（product）與和（sum）。相關考題已較少出現。可參閱進階類題最後幾題。
設 $R_1, R_2 \subseteq A \times A$ 為定義在 $A$ 上的兩個等價關係，對應的分割為 $\pi_1, \pi_2$ 。
\begin{itemize}
\item[（1）] $\pi_1 \cdot \pi_2$ 表示等價關係 $\left(R_1 \cap R_2\right)$ 對應的分割，稱為 $\pi_1$ 與 $\pi_2$ 的積。
\item[（2）] $\pi_1+\pi_2$ 表示等價關係 $\left(R_1 \cup R_2\right)^{+}$對應的分割，稱為 $\pi_1$ 與 $\pi_2$ 的和。
\item[（3）] $\pi_1 \cdot \pi_2$ 為 $\pi_1$ 與 $\pi_2$ 之細分（refinement）；$\pi_1$ 與 $\pi_2$ 為 $\pi_1+\pi_2$ 之細分。
\item[（4）] $\left(R_1 \cup R_2\right)^{+}$為 $R_1 \cup R_2$ 的遞移閉包。
\end{itemize}
\end{itemize}