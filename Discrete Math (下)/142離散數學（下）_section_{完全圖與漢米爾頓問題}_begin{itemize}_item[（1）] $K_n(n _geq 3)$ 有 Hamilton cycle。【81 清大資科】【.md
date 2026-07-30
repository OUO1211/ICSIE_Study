142
離散數學（下）

\section*{完全圖與漢米爾頓問題}
\begin{itemize}
\item[（1）] $K_n(n \geq 3)$ 有 Hamilton cycle。
【81 清大資科】【106 中央資工】其中，相異的有 $\frac{(n-1)!}{2}$ 個，互斥的有 $\left\lfloor\frac{n-1}{2}\right\rfloor$ 個。
【93中山資工】【94中山電機】【96清大資應】【103台科資工】
\item[（2）] $K_n$ 有 $n!$（或 $n!/ 2$ ）個相異的 Hamilton path；有 $\left\lfloor\frac{n}{2}\right\rfloor$ 個互斥的 Hamilton path。
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] ① 可將點編號為 $1,2, \ldots, n$ ，則每一種1到 $n$ 的排列方式即為一個 Hamilton cycle，而因頭尾相接，故為環狀排列，有 $(n-1)!$ 種；但同一種走法又有順時與逆時兩種表達法，ex： $1-2-\ldots-n$ 與 $n-(n-1)-\ldots-2-1$ 為同一種 Hamilton cycle，所以須再除以2。
\end{itemize}
（2）以右圖 $K_6$ 為例，將一點 $v_0$ 放在中心位置，$v_1, \ldots, v_5$ ，以順時鐘的順序放在周圍，依以下方式走完所有點：
$I: v_0-v_1-v_2-v_5-v_3-v_4-v_0$（如細的線段）；
$I I: v_0-v_2-v_3-v_1-v_4-v_5-v_0$（如粗的線段）
此兩種走法為互斥的（最後剩一組 matching：
$\overline{v_0 v_3}, \overline{v_1 v_5}, \overline{v_2 v_4}$ ，無法湊成 Hamilton cycle），
共 $\left\lfloor\frac{6-1}{2}\right\rfloor$ 組互斥之 Hamilton cycle。其走法之規律為：
從中心點出發，向上，然後向右，向左，向右，向左，⋯最後回中心點。
再以中心點出發，先到右邊第一點，然後同上，右左右左⋯，再回中心點。
再以中心點出發，先到右邊第二點，然後同上，右左右左⋯，再回中心點，⋯餘類推。另外，若適當丟掉 $I, I I$ 中的某些邊以形成 Hamilton path，則這些丟棄的邊可與原來那組都沒被用到 matching 形成一組新的 Hamilton path：$v_0-v_3-v_1-v_5-v_2-v_4$ ，
故共 $\left\lfloor\frac{6}{2}\right\rfloor$ 組互斥之 Hamilton path。
同理可得 $K_7$ 之 $\left\lfloor\frac{7-1}{2}\right\rfloor$ 組互斥之 Hamilton cycle ：
$I: v_0-v_1-v_2-v_6-v_3-v_5-v_4-v_0$（如虛的線段）；
$I I: v_0-v_2-v_3-v_1-v_4-v_6-v_5-v_0$（如細的線段）；
III ：$v_0-v_3-v_4-v_2-v_5-v_1-v_6-v_0$（如粗的線段）；
而所有邊都被走過沒有多的。