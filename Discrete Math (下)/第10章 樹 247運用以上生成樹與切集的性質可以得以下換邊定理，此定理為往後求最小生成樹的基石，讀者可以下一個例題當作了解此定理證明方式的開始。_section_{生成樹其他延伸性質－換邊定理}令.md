第10章 樹 247

運用以上生成樹與切集的性質可以得以下換邊定理，此定理為往後求最小生成樹的基石，讀者可以下一個例題當作了解此定理證明方式的開始。

\section*{生成樹其他延伸性質－換邊定理}

令 $T_1, T_2$ 為連通圖 $G$ 之相異生成樹，且邊 $a \in E\left(T_1\right)-E\left(T_2\right)$ ，
則存在邊 $b \in E\left(T_2\right)-E\left(T_1\right)$ ，使得 $\left(T_1-\{a\}\right) \bigcup\{b\}$ 與 $\left(T_2-\{b\}\right) \bigcup\{a\}$ 均為 $G$ 之生成樹。
【87 清大資工】【96 清大資應】【109 台聯電機】
【證明】
$\because a \in E\left(T_1\right)$ ，故可唯一決定一組包含 $a$ 的 cut set $S_1, S_1 \cap T_1=\{a\}$ ，
$\because a \notin E\left(T_2\right), \therefore T_2 \cup\{a\}$ 含有一 cycle $C$ ，且 $\overline{T_2} \cap C=\{a\}$ ，其中，$\overline{T_2}=G-T_2$ ，
而因為 $\forall$ cycle $C, \forall$ cut set $S,|C \cap S|=$ 偶數，所以必有另一邊 $b \in C \cap S_1$ ，
$\because b \in C$ ，且 $\overline{T_2}$ 與 $C$ 只有共用邊 $a, \therefore b \notin \overline{T_2}, \therefore b \in T_2$ ，
$\because b \in S_1$ ，且 $S_1$ 與 $T_1$ 只有共用邊 $a, \therefore b \notin T_1$ ，即找到邊 $b \in E\left(T_2\right)-E\left(T_1\right)$ ，
另一方面，因為 $a, b$ 同在一個 cycle 中，$\therefore\left(T_1-\{a\}\right) \bigcup\{b\}$ 與 $\left(T_2-\{b\}\right) \bigcup\{a\}$ 均為連通，
且 $\left(T_1-\{a\}\right) \bigcup\{b\}$ 與 $\left(T_2-\{b\}\right) \bigcup\{a\}$ 之邊數均與 $T_1$ 相同，
故知 $\left(T_1-\{a\}\right) \bigcup\{b\}$ 與 $\left(T_2-\{b\}\right) \bigcup\{a\}$ 亦為 $G$ 之生成樹。