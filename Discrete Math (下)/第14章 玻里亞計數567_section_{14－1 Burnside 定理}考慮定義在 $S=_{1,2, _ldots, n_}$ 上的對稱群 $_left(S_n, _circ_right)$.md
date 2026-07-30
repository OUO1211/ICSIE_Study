第14章 玻里亞計數
567

\section*{14－1 Burnside 定理}

考慮定義在 $S=\{1,2, \ldots, n\}$ 上的對稱群 $\left(S_n, \circ\right)$ ，
其中，$S_n=\{f \mid f: S \xrightarrow{1-1, \text { onto }} S\}$, 。為函數的合成。
令 $(G, \circ) \subseteq\left(S_n, \circ\right)$ 為 $S_n$ 之子群，稱為 $S$ 上的排列群。
在 $S$ 上定義一二元關係 $\sim: \forall a, b \in S, a \sim b \Leftrightarrow \exists f \in G$ 使得 $f(a)=f(b)$ ，
並稱～為由 $G$ 所引出在 $S$ 上的一個二元關係。
而此二元關係是一等價關係，且以 $S / \sim$ 表由～所造成之相異等價類所成集合。

Burnside 定理
$|(S / \sim)|=\frac{1}{|(G)|} \sum_{\pi \in G} \Psi(\pi)$,【90 中央數學】
其中，$\Psi(\pi)=|\{a \in S: \pi(a)=a\}|$ ，即 permutation $\pi$ 所 fixed 之元素個數。
例：在 $2 \times 2$ 的方格內著以黑（ X ）白（ O ）兩色，在可平面旋轉之下，共有多少種不一樣的圖形？
解

若全部列出，應有以上 16 種著色方式，考慮平面上的旋轉方式：$\pi_i$ 代表順時鐘旋轉$i \times 90^{\circ}, \quad i=0,1,2,3$ 。
則在 $\pi_0$ 下，這 16 種圖形旋轉前後均相同（不變），即 $\Psi\left(\pi_0\right)=16$ ；
在 $\pi_1$ 下，這 16 種圖形只有 $c_0, c_{15}$ ，旋轉前後均相同（不變），即 $\Psi\left(\pi_1\right)=2$ ；
在 $\pi_2$ 下，這 16 種圖形只有 $c_0, c_5, c_6, c_{15}$ ，旋轉前後均相同（不變），即 $\Psi\left(\pi_2\right)=4$ ；
在 $\pi_3$ 下，這 16 種圖形只有 $c_0, c_{15}$ ，旋轉前後均相同（不變），即 $\Psi\left(\pi_3\right)=2$ ；
故由 Burnside 定理得知，考慮可平面旋轉下，
共 $\frac{1}{4}(16+2+4+2)=6$ 種不同著色方式。（可以 $c_0, c_1, c_5, c_7, c_{11}, c_{15}$ 作代表）