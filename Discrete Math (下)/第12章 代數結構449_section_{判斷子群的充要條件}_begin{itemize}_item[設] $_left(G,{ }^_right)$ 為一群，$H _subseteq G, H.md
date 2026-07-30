第12章 代數結構
449

\section*{判斷子群的充要條件}
\begin{itemize}
\item[設] $\left(G,{ }^*\right)$ 為一群，$H \subseteq G, H \neq \varnothing$ ，則
\item[（1）] $H$ 為 $G$ 之子群 $\Leftrightarrow$ ① $\forall a, b \in H, a^* b \in H$ ，且② $\forall a \in H, a^{-1} \in H$ 。
\item[（2）] $H$ 為 $G$ 之子群 $\Leftrightarrow \forall a, b \in H, a^* b^{-1} \in H$ 。
\item[（3）] $|H|<\infty$ 時，$H$ 為 $G$ 之子群 $\Leftrightarrow \forall a, b \in H, a * b \in H$ 。
\end{itemize}

【證明】
\begin{itemize}
\item[（1）] ⇒ trivial，因為 $H$ 為群，自然具備有封閉性 ①與反元素性質②。
⇐ $H$ 為 $G$ 之子集合，只需再說明 $H$ 具有群的特性即可。
封閉性與反元素性質已由假設得知。
因為 $H$ 為 $G$ 之子集合，且 $G$ 中的元素運算時具有結合性，自然 $H$ 中的元素運算時亦具有結合性。
另外，$\because a \in H, \therefore a^{-1} \in H, \therefore a^* a^{-1} \in H, \therefore e \in H$ ，故知 $H$ 具有單位元素。
\item[（2）] （⇒）$\because H$ 為群，由反元素性質 $\therefore \forall a \in H, ~ a^{-1} \in H$ ，又由封閉性 $\therefore a^* b^{-1} \in H$ 。
（⇐）因為 $H$ 為 $G$ 之子集合，而 $G$ 中元素＊運算均有結合性，故 $H$ 亦然。
又 $b^* b^{-1} \in H$ ，即 $e \in H$ ，故 $H$ 有單位元素。
又 $e^* b^{-1} \in H$ ，即 $b^{-1} \in H$ ，故 $H$ 有反元素性質。
另外，明顯可得＊有封閉性，故 $H$ 為 $G$ 之子群。
\item[（3）] （⇒）顯然成立。
（⇐）封閉性：由題意可得。
結合性：因為 $H$ 為 $G$ 之子集，而 $G$ 中的元素做＊運算時均有結合性，
故 $H$ 中的元素做＊運算時亦有結合性。
單位元素：令 $a \in H, \because H$ 的運算具封閉性 $\therefore a, a^2, a^3, \ldots$ 均為 $H$ 中之元素，
若 $a=a^2=a^3=\ldots$ ，則 $a$ 為單位元素。
否則，$\because|H|<\infty, \therefore \exists m>n>0$ ，such that $a^m=a^n$ ，
則 $a^{m-n}$ 即為單位元素。
$\binom{\because a^n \in G, \text { 且 } G \text { 是群，} \therefore \text { 存在 } x, \text { 使 } x * a^n=e,}{\text { 但 } a^m=a^n, \therefore x * a^m=x * a^n, \therefore x * a^n * a^{m-n}=x * a^n, \therefore a^{m-n}=e}$
反元素性質：且 $\forall a \in H, a^{-1}=a^{m-n-1} \in H\left(\because a^* a^{m-n-1}=a^{m-n}=e\right) 。$
故知，$(H, *)$ 為群，所以 $(H, *)$ 為 $(G, *)$ 之子群。
【91 台科資工】【93 東華資工】
\end{itemize}