第 8 章 圖論 185

Note
使用 Dijkstra＇s Algorithm 時，其他注意事項：
\begin{itemize}
\item[（1）] 若邊之權值有負數，則可能失效；但若 $G$ 為無迴圈圖（acyclic）則仍可得最短路徑，因為此時任兩點的路徑唯一。
\item[（2）] 若圖中有權值為負數之迴圈（cycle），則失效。【81中正資工】【85、86中央資工】
\item[（3）] 若將每邊權值一同增加或減少，則原所求得之最短路徑不復為最短。
\item[（4）] 此 Algorithm 最後可 output 出 $a$ 到所有點的最短路徑值與走法，但若問 $b$ 到其他點，則又須以 $b$ 為起點，重新 run 一次。
\end{itemize}