392
資料結構（含精選試題）
■■■

Data Structure
$$
\mathrm{E}=2+2+4+4+3+2=17
$$
\begin{itemize}
\item[（二）] 定理
若 E 是 Extenal Path Length，I 是 Internal Path Length，N為 Internal Node 數目，則
$$
\mathrm{E}=\mathrm{I}+2 \mathrm{~N}
$$
證明：利用歸納法證明
\begin{itemize}
\item[（1）] $n=1$ 時，Tree Structure 如下
故 $\mathrm{E}=1+1=2, \mathrm{I}=0, \therefore \mathrm{E}=\mathrm{I}+2 \mathrm{~N}$ 成立
\item[（2）] 令 $\mathrm{n}=\mathrm{k}$ 時， $\mathrm{E}=\mathrm{I}+2 \mathrm{k}$ 成立
\item[（3）] 假設 $n=k+1$ 時
令
假設左子樹
$\mathrm{N}_{\mathrm{L}}$ 個內部節點
$\mathrm{N}_{\mathrm{L}}+1$ 個外部節點
$$
\mathrm{E}_{\mathrm{L}}=\mathrm{I}_{\mathrm{L}}+2 \mathrm{~N}_{\mathrm{L}}
$$
同理，右子樹有類似的 $\mathrm{N}_{\mathrm{R}}, \mathrm{E}_{\mathrm{R}}, \mathrm{I}_{\mathrm{R}}$
$$
\begin{aligned}
\text { 因此 } E & \left.=\left(E_L+N_L+1\right)\right)+\left(E_R+\left(N_R+1\right)\right) \\
& =\left(\left(E_L+2 N l_L\right)+\left(N_L+1\right)\right)+\left(\left(I_R+2 N_R\right)+\left(N_R+1\right)\right) \\
& \left.=\left(\left(I_L+N_L\right)+I_R+N_R\right)\right)+2\left(N_L+K_R+1\right) \\
& =I+2 N
\end{aligned}
$$
\end{itemize}
\item[] ＊結論
若有最小的 I 值，也同時有最小的 E（同理最大 I → 最大 E）
（一）當二元樹是 Skewed Tree，具有最大的 I
\end{itemize}