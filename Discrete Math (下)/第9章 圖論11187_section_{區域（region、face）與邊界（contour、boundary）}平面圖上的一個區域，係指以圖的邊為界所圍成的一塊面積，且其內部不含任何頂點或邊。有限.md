第9章 圖論11
187

\section*{區域（region、face）與邊界（contour、boundary）}

平面圖上的一個區域，係指以圖的邊為界所圍成的一塊面積，且其內部不含任何頂點或邊。
有限區域（finite region）指面積為有限的區域。
無限區域（infinite region）指面積為無限的區域。
一個區域的邊界指包圍此區域的邊，兩個區域至少有一共同邊時稱它們為相鄰（adjacent）。

\section*{尤拉公式（Euler formula）}

令 $G=(V, E)$ 為一連通平面圖，$|V|=v,|E|=e, r$ 表示區域的個數，則 $v-e+r=2$ 。
【重要】
【證明】
對邊數 $e$ 作歸納法，$e=0$ 時，$G$ 只一點，故 $v=1, r=1$ ，原式成立。
設對所有邊數 $\leq k$ 之連通平面圖，原式均成立。 $(k \geq 1)$
則對邊數為 $k+1$ 之連通平面圖 $G$ ，去掉 $G$ 中的任一邊得 $G^{\prime}$ ，且點數、邊數、區域數分別為$v^{\prime}, e^{\prime}, r^{\prime}$ 。
\begin{itemize}
\item[（1）] 若 $G^{\prime}$ 為連通圖，則因 $G^{\prime}$ 之邊數 $\leq k$ ，則由歸納假設：$v^{\prime}-e^{\prime}+r^{\prime}=2$ ，
又且因為 $v^{\prime}=v, e^{\prime}=e-1, r^{\prime}=r-1, \therefore v-e+r=2$ ，原式成立。
\item[（2）] 若 $G^{\prime}$ 斷成兩個分量 $G_1^{\prime}, G_2^{\prime}$ ，則圖 $G_1^{\prime}, G_2^{\prime}$ 之邊數均 $\leq k$ ，且均為連通平面圖，
故由歸納假設知：$v_1^{\prime}-e_1^{\prime}+r_1^{\prime}=2, v_2^{\prime}-e_2^{\prime}+r_2^{\prime}=2$
其中 $v_i^{\prime}, e_i^{\prime}, r_i^{\prime}$ ，分別為 $G_i^{\prime}$ 之點數、邊數、區域數，$i=1,2$ 。
則因為 $v^{\prime}=v_1^{\prime}+v_2^{\prime}=v, ~ e^{\prime}=e_1^{\prime}+e_2^{\prime}=e-1, r^{\prime}=r_1^{\prime}+r_2^{\prime}-1=r$
將（＊）兩式相加並代入（＊＊），得 $v-e+r=2$ ，原式成立。
\end{itemize}

Note
令 $G=(V, E)$ 為含 $k$ 個分量圖的平面圖，則 $v-e+r=1+k 【 81$ 成大電機】【97政大資科】
【證明】
設 $G_1=\left(V_1, E_1\right), \ldots, G_k=\left(V_k, E_k\right)$ 為 $G$ 的分量圖，
因為每個 $G_i$ 為平面連通，所以 $v_i-e_i+r_i^*=1$ ，其中 $r_i^*=G_i$ 中不包含無窮區域的區域個數。所以 $\sum_{i=1}^k v_i-\sum_{i=1}^k e_i+\sum_{i=1}^k r_i^*=k, \therefore v-e+r^*=k, \therefore v-e+r=k+1$ 。