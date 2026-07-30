8
離散數學（下）

子圖（subgraph）
考虑圖 $G=(V, E)$ ，
\begin{itemize}
\item[（1）] 若 $G^{\prime}=\left(V^{\prime}, E^{\prime}\right)$ 滿足 $V^{\prime} \subseteq V, E^{\prime} \subseteq E$ ，且 $E^{\prime}$ 的邊與 $V^{\prime}$ 的點相連接，則稱 $G^{\prime}$ 為 $G$ 的子圖，$G$ 為 $G^{\prime}$ 的母圖（supergraph）。
\item[（2）] 若 $G^{\prime}=\left(V^{\prime}, E^{\prime}\right)$ 為 $G=(V, E)$ 的子圖且滿足 $E^{\prime}$ 包含 $E$ 中所有與 $V^{\prime}$ 有相連的邊時，則稱$G^{\prime}$ 為 $G$ 的誘導子圖（induced subgraph）。
\item[（3）] 若 $G^{\prime}=\left(V^{\prime}, E^{\prime}\right)$ 為 $G$ 的子圖且 $V^{\prime}=V$ ，則稱 $G^{\prime}$ 為 $G$ 的生成子圖（spanning subgraph）。
\end{itemize}

Note
\begin{itemize}
\item[（1）] 令 $V^{\prime}$ 為點集合 $V$ 之子集合，常以 $G\left[V^{\prime}\right]$ 表示由 $V^{\prime}$ 所形成的 $G$ 的誘導子圖。
\end{itemize}
（2）令 $E^{\prime}$ 為邊集合 $E$ 之子集合，常以 $G\left[E^{\prime}\right]$ 表示由 $E^{\prime}$ 所形成的 $G$ 的誘導子圖。
例如上圖中，$G_1, G_2, G_3$ 都是 $G$ 的子圖，其中，
$G_1$ 又稱為 $G$ 的一個誘導子圖 ；
$G_2$ 又稱為 $G$ 的一個生成子圖；
$G_3$ 又稱為 $G$ 的基礎簡單圖（刪去 loop 與重複的邊）。