第11章 二元關係及其應用
315

\section*{特殊的二元關係}

設 $R$ 為 $A$ 上之一二元關係，$R \subseteq A \times A$ ，
$R$ 具有反身性（reflexive）：$\forall a \in A,(a, a) \in R$ ．
$R$ 具有非反身性（irreflexive）：$\forall a \in A,(a, a) \notin R$ ．
$R$ 具有對稱性（symmetric）：$\forall a, b \in A$ ，if $(a, b) \in R$ ，then $(b, a) \in R$ ．
$R$ 具有非對稱性（asymmetric）：$\forall a, b \in A$ ，if $(a, b) \in R$ then $(b, a) \notin R$ ．
$R$ 具有反對稱性（antisymmetric）：$\forall a, b \in A$ ，if $(a, b) \in R \wedge(b, a) \in R$ then $a=b$ ．
$R$ 具有遞移性（transitive）：$\forall a, b, c \in A$ ，if $(a, b) \in R \wedge(b, c) \in R$ then $(a, c) \in R$ ．
Note
\begin{itemize}
\item[（1）] 在關係矩陣中：
有反身性即對角位置均為1；有非反身性即對角位置均為0；
有對稱性即對稱位置等值，主對角可0可1；
有非對稱性即對稱位置不同時為1，且主對角必為0；
有反對稱性即對稱位置不同時為1，但主對角可0亦可1；
遞移性在關係矩陣中不易判別。
\item[（2）] 在關係圖形中：
有反身性即每點均有 loop；有非反身性即每點均沒有 loop；
有對稱性即連接兩點的邊，若有邊則雙向都有，loop 可有可無；
有非對稱性即連接兩點的邊只能單向，且每點均沒 loop；
有反對稱性即連接兩點的邊只能單向，每點可有 loop；
遞移性即若 $a, c$ 有兩步可達之 path，則必須 $a$ 有邊可連到 $c$ 。
\item[（3）] 除了空集合上的空關係，反身與非反身不會同時成立，但可同時不存在。
【107 台大電機】【109 台聯電機】
\item[（4）] 對稱性與反對稱性可以同時存在。
\item[（5）] 有非對稱性就一定有反對稱性；反之不然。
\item[（6）] 除了空關係外，對稱性與非對稱性不同時存在。
\item[（7）] 非空集合上的空關係，僅不具反身性。
\end{itemize}

【109 台聯電機】