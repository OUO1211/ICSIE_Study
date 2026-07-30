570
離散數學（下）

\section*{14－2 Polya 計數}

\section*{函數下的等價類}

設 $D, R$ 為兩個有限集合，$G$ 為 $D$ 上的一個排列群。令 $F=\{f \mid f: D \rightarrow R$ 為一函數 $\}$ 。
在 $F$ 上定義一個二元關係～為：
$\forall f_1, f_2 \in F, f_1 \sim f_2 \Leftrightarrow \exists \pi \in G$ ，使得 $f_1=f_2 \circ \pi$ ，
稱～為 $F$ 上利用 $G$ 來定義的二元關係，且～為一等價關係。
設 $D, R$ 為雨個有限集合，
\begin{itemize}
\item[（1）] $r \in R$ ，定義 $w(r)$ 為 $r$ 的權（weight of $r$ ）。
\item[（2）] $R$ 的儲藏錄（store enumerator）定義為 $\sum_{r \in R} w(r)$ 。
\item[（3）] $f: D \rightarrow R$ 為一函数，定義 $f$ 的權為 $W(f)=\prod_{f \in D} w(f(d))$ 。
\item[（4）] $F \subseteq\{f \mid f: D \rightarrow R$ 為一函數 $\}$ ，定義 $F$ 的目錄（inventory of $F$ ）為 $\sum_{f \in F} w(f)$ 。
\end{itemize}

例如 ：
令 $D=\left\{d_1, d_2, d_3\right\}, R=\left\{r_1, r_2, r_3\right\}, w\left(r_1\right)=u, w\left(r_2\right)=v, w\left(r_3\right)=u, F=\left\{f_1, f_2, f_3\right\}$ ，其中，
$f_1:\left\{\begin{array}{l}d_1 \mapsto r_1 \\ d_2 \mapsto r_2 \\ d_3 \mapsto r_2\end{array}, \quad f_2:\left\{\begin{array}{l}d_1 \mapsto r_1 \\ d_2 \mapsto r_2 \\ d_3 \mapsto r_1\end{array}, \quad f_3:\left\{\begin{array}{l}d_1 \mapsto r_2 \\ d_2 \mapsto r_1 \\ d_3 \mapsto r_3\end{array}\right.\right.\right.$ ，則
$R$ 的儲藏錄：$w\left(r_1\right)+w\left(r_2\right)+w\left(r_3\right)=u+v+u=2 u+v$ ．
$f_1$ 的權：$W\left(f_1\right)=\prod_{f \in D} w\left(f_1(d)\right)=w\left(f_1\left(d_1\right)\right) \cdot w\left(f_1\left(d_2\right)\right) \cdot w\left(f_1\left(d_3\right)\right)=u \cdot v \cdot v=u v^2$ ．
$f_1$ 的權：$W\left(f_2\right)=\prod_{f \in D} w\left(f_2(d)\right)=w\left(f_2\left(d_1\right)\right) \cdot w\left(f_2\left(d_2\right)\right) \cdot w\left(f_2\left(d_3\right)\right)=u \cdot v \cdot u=u^2 v$ ．
$f_1$ 的權：$W\left(f_3\right)=\prod_{f \in D} w\left(f_3(d)\right)=w\left(f_3\left(d_1\right)\right) \cdot w\left(f_3\left(d_2\right)\right) \cdot w\left(f_3\left(d_3\right)\right)=v \cdot u \cdot u=u^2 v$ ．
而 $F$ 的目錄為：$\sum_{f \in F} w(f)=w\left(f_1\right)+w\left(f_2\right)+w\left(f_3\right)=u v^2+u^2 v+u^2 v=u v^2+2 u^2 v$ 。
Note
設 $\sim$ 為 $F$ 上利用 $G$ 來定義的二元關係，$f_1, f_2 \in F$ ，則 $f_1 \sim f_2 \Rightarrow W\left(f_1\right)=W\left(f_2\right)$ 。