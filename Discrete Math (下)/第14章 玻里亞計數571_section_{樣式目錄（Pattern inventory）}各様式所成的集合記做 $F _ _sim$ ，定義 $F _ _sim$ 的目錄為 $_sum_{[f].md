第14章 玻里亞計數
571

\section*{樣式目錄（Pattern inventory）}

各様式所成的集合記做 $F / \sim$ ，定義 $F / \sim$ 的目錄為 $\sum_{[f] \in F / \sim} W([f])$ ，稱為樣式目錄。
Note
設 $D, R$ 為兩個有限集合，$\left\{D_1, \ldots, D_k\right\}$ 為 $D$ 的一分割，$F \subseteq\{f \mid f: D \rightarrow R$ 為一函數 $\}$ ，若 $\forall f \in F$ ，$f$ 在 $D_i$ 的函數值皆相同，$\forall i=1,2, \ldots, k$ ，則 $F$ 的目錄為 $\prod_{i=1}^k \sum_{r \in R} w(r)^{\left|D_i\right|}$ ．

\section*{基礎類題}
\begin{itemize}
\item[1．] 有三種不同的球及三種顏料分別為紅色，黄色與藍色，利用此三種顏料來塗這三個球有多少種塗法？
解 球 ：$D=\{X, Y, Z\}$ ，顏色 $R=\{r, y, b\}$ ，weight：$w(r)=r, w(y)=y, w(b)=b$ ，共 $3^3$ 種不同的函數。
目錄：$r^3+y^3+b^3+3\left(r^2 y+r y^2+y^2 b+y b^2+r^2 b+b^2 r\right)+6 y r b$ ，
令 $r=y=b=1$ 代入 共27種。
\item[2.8] people are planning vacation trips．There are 3 cities they can visit． 3 of these 8 people are in one family，and 2 of them are in another family．If the people in the same family must go together，find the number of ways the 8 people can plan their trips．
【90 清大通訊】
\item[解] 總共有 5 個家庭，設定義域 $D=\left\{D_1, D_2, D_3, D_4, D_5\right\}$ ，其中，
$D_1=\{a, b, c\} ; D_2=\{d, e\} ; D_3=\{f\} ; D_4=\{g\} ; D_5=\{h\}$ ，
有 3 個城市，設值域 $R=\left\{C_1, C_2, C_3\right\}$ ，weight 為：$w\left(C_1\right)=\alpha, w\left(C_2\right)=\beta, w\left(C_3\right)=\gamma$ ，
則目錄為：$\left(\alpha^3+\beta^3+\gamma^3\right)\left(\alpha^2+\beta^2+\gamma^2\right)(\alpha+\beta+\gamma)^3$ ，
令 $\alpha=\beta=\gamma=1$ 代入，共 $3^5$ 種。
\end{itemize}