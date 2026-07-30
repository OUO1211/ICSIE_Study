140
離散數學（下）

\section*{有向完全圖與漢米爾頓問題}
$n(\geq 2)$ 點的有向完全圖 $K_n{ }^*$ ，必具有向的 Hamilton path。
【84中正資工】【90政大資科】【92中央資工】【111台聯電機】
【證明】
令 $P: v_1 \rightarrow v_2 \rightarrow v_3 \rightarrow \ldots \rightarrow v_s$ 為最長路徑，但存在某點 $z$ 末被 $P$ 通過，則因為任兩點都有邊，依序討論 $z$ 與 $v_1, v_2, v_3, \ldots, v_s$ 的邊的方向如下：
考慮 $v_1$ 與 $z$ 之間的邊，若 $z \rightarrow v_1$ ，則 $z \rightarrow v_1 \rightarrow v_2 \rightarrow \ldots \rightarrow v_s$ 為比 $P$ 更長的路徑，與 $P$ 最長不合，故 $v_1 \rightarrow z$ ；
接著考慮 $v_2$ 與 $z$ 之間的邊，若 $z \rightarrow v_2$ ，則 $v_1 \rightarrow z \rightarrow v_2 \rightarrow v_3 \rightarrow \ldots \rightarrow v_s$ 為比 $P$ 更長的路徑，與$P$ 最長不合，故 $v_2 \rightarrow z$ ；
接著考慮 $v_3$ 與 $z$ 之間的邊，若 $z \rightarrow v_3$ ，則 $v_1 \rightarrow v_2 \rightarrow z \rightarrow v_3 \rightarrow \ldots \rightarrow v_s$ 為比 $P$ 更長的路徑，與$P$ 最長不合，故 $v_3 \rightarrow z$ ；
$\cdots$ ，以此類推，可得對所有 $i=1 \sim s-1, v_i \rightarrow z$ ，
最後考慮 $v_s$ 與 $z$ 之間的邊，若 $z \rightarrow v_s$ ，則 $v_1 \rightarrow \ldots \rightarrow v_{s-1} \rightarrow z \rightarrow v_s$ 為比 $P$ 更長的路徑，與 $P$最長不合；但若 $v_s \rightarrow z$ 則 $v_1 \rightarrow v_2 \rightarrow \ldots \rightarrow v_s \rightarrow z$ 也是比 $P$ 更長的路徑，與 $P$ 最長不合。故不存在 $P$ 外的點，即此 $P$ 為通過所有點的 path，得證。