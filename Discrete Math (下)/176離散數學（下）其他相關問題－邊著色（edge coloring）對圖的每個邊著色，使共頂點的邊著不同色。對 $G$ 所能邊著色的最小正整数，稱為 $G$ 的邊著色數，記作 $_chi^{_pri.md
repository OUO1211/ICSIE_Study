176
離散數學（下）

其他相關問題－邊著色（edge coloring）
對圖的每個邊著色，使共頂點的邊著不同色。
對 $G$ 所能邊著色的最小正整数，稱為 $G$ 的邊著色數，記作 $\chi^{\prime}(G)$ 。
Note
（1）$\chi^{\prime}\left(C_n\right)=\left\{\begin{array}{ll}2, & n: \text { even } \\ 3, & n: \text { odd }\end{array}, \quad \chi^{\prime}\left(K_{n, n}\right)=n\right.$ ．
【95 師大資工】
（2）$\chi^{\prime}\left(K_n\right)=\left\{\begin{array}{cl}n-1 & n \text { ：even } \\ n & n: \text { odd }\end{array}\right.$ ．
【85 交大應數】【95 師大資工】
解 如下圖 $K_6$ ，將一點 $v_0$ 放在中心位置，$v_1, v_2, \ldots, v_5$ ，以順時鐘的順序放在周圍，依以下方式取出邊獨立集著同色：
$I: \overline{v_0 v_1}, \overline{v_2 v_5}, \overline{v_3 v_4}$（如細的線段）；
$I I: \overline{v_0 v_2}, \overline{v_3 v_1}, \overline{v_4 v_5}$（如粗的線段）；
III ：$\overline{v_0 v_3}, \overline{v_2 v_4}, \overline{v_5 v_1}$（如細的虛線段）；
$I V: \overline{v_0 v_4}, \overline{v_3 v_5}, \overline{v_1 v_2}$（如粗的虛線段）；
$V: \overline{v_0 v_5}, \overline{v_1 v_4}, \overline{v_2 v_3}$（如雙箭頭線段），共5組互斥的邊獨立集，$\therefore \chi^{\prime}=5$ 。
其取法之規律為：
從中心點出發，向上，然後右左對稱位置的邊取出，
再以中心點出發，選到右邊第一點，然後右左對稱位置的邊取出，
再以中心點出發，選到右邊第二點，然後右左對稱位置的邊取出，⋯餘類推。
如上圖 $K_7$ ，將 $v_0, v_1, v_2, \ldots, v_6$ ，以順時鐘的順序放在周圍，依以下方式取出邊獨立集著同色：
$I: \overline{v_1 v_6}, \overline{v_2 v_5}, \overline{v_3 v_4}$（如細的線段）；$I I: \overline{v_0 v_2}, \overline{v_3 v_6}, \overline{v_4 v_5}$（如粗的線段）；
III：$\overline{v_1 v_3}, \overline{v_0 v_4}, \overline{v_5 v_6}$（如細的虛線段）；$I V: \overline{v_2 v_4}, \overline{v_1 v_5}, \overline{v_0 v_6}$（如粗的部分虛線段）；$V: \overline{v_3 v_5}, \overline{v_2 v_6}, \overline{v_0 v_1}$（如粗的部分虛線段）；$V I: \overline{v_4 v_6}, \overline{v_3 v_0}, \overline{v_2 v_1}$（如雙箭頭線段）；$V I I: \overline{v_5 v_0}, \overline{v_1 v_4}, \overline{v_2 v_3}$（如閃電線段），共7組互斥的邊獨立集，$\therefore \chi^{\prime}=7$ 。