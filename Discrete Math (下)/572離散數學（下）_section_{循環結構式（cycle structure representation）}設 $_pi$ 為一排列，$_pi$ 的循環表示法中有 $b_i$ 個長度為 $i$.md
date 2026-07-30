572
離散數學（下）

\section*{循環結構式（cycle structure representation）}

設 $\pi$ 為一排列，$\pi$ 的循環表示法中有 $b_i$ 個長度為 $i$ 之循環，$i=1,2, \ldots, j$ ，則 $\pi$ 之循環結構式定義為 $C_\pi=x_1^{b_1} x_2^{b_2} \ldots x_j^{b_j}$ 。

\section*{循環指標（cycle index）}

設 $G$ 為 $S$ 上的一個排列群，定義 $G$ 之循環指標為 $P_G\left(x_1, \ldots, x_k, \ldots\right)=\frac{1}{|G|} \sum_{\pi \in G} C_\pi$ 。
例如 ：
令 $S=\{a, b, c, d\}, G=\left\{\pi_0, \pi_1, \pi_2, \pi_3\right\}$ 為 $S$ 上的一排列群，其中，
$\pi_0=\left(\begin{array}{llll}a & b & c & d \\ a & b & c & d\end{array}\right), \quad \pi_1=\left(\begin{array}{llll}a & b & c & d \\ b & a & c & d\end{array}\right), \quad \pi_2=\left(\begin{array}{llll}a & b & c & d \\ a & b & d & c\end{array}\right), \quad \pi_3=\left(\begin{array}{llll}a & b & c & d \\ b & a & d & c\end{array}\right)$,
則 $C_{\pi_0}=x_1^4, C_{\pi_1}=x_1^2 x_2^1, C_{\pi_2}=x_1^2 x_2^1, C_{\pi_3}=x_2^2$ ；
故 $G$ 的循環指標 ：$P_G\left(x_1, x_2\right)=\frac{1}{4}\left(x_1^4+2 x_1^2 x_2^1+x_4^2\right)$ 。

\section*{Polya 定理}

設 $D, R$ 為兩個有限集合，$G$ 為 $D$ 上的一個排列群，令 $F \subseteq\{f \mid f: D \rightarrow R$ 為一函數 $\}$ ，則 $(F / \sim)$ 之目錄為 $P_G\left(\sum_{r \in R} w(r), \sum_{r \in R}[w(r)]^2, \ldots, \sum_{r \in R}[w(r)]^k, \ldots\right)$ ，
且 $\#(F / \sim)=(|R|, \ldots,|R|)$ 。