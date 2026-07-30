474
離散數學（下）

\section*{同態、同構}

設 $(G, *),\left(G^{\prime}, *^{\prime}\right)$ 為雨個群，
\begin{itemize}
\item[（1）] 若存在一函數 $f: G \rightarrow G^{\prime}$ ，滿足 $f\left(a^* b\right)=f(a)^{*^{\prime}} f(b), \forall a, b \in G$ ，則稱 $f$ 為由 $G$ 至 $G^{\prime}$之群同態函數（group homomorphism），且稱 $\boldsymbol{G}$ 與 $\boldsymbol{G}^{\prime}$ 同態。
\item[（2）] 若 $f$ 為群同態函数且為 1－1，onto，則稱 $f$ 為由 $G$ 至 $G^{\prime}$ 之群同構函數（group isomorphism），且稱 $\boldsymbol{G}$ 與 $\boldsymbol{G}^{\prime}$ 同構，記作 $G \cong G^{\prime}$ ．【97 北教資科】【99 台大資工】
\end{itemize}

Note
\begin{itemize}
\item[（1）] Trivial homomorphism：$f: G \rightarrow G^{\prime}$ ，by $f(x)=e^{\prime}=$ identity of $G^{\prime}, \forall x \in G$ ．
\item[（2）] 例如 ：$(R,+) \cong\left(R^{+}, \cdot\right)$ by $f: R \rightarrow R^{+}, f(x)=10^x$ 。
\item[（3）] 例如，可取函數 $f(x)=\left\{\begin{array}{l}0 \text { if } x \text { is even } \\ 1 \text { if } x \text { is odd }\end{array}\right.$ ，而知 $\left(Z_8,+\mathrm{r}_8\right)$ 與 $\left(Z_2,+\mathrm{r}_2\right)$ 同態。
\end{itemize}

\section*{基礎類題}

1．True or false：
\begin{itemize}
\begin{itemize}
\item[（1）] An abelian group can be isomorphic to a nonabelian group．
\item[（2）] $Z_2 \times Z_4 \cong Z_8$ ．
\item[（3）] Let $P=\{a, b, c\}$ and $Q=\{x, y, z\}$ and are two operators defined upon $P$ and $Q$ ， respectively，as follows： \begin{tabular}{l|llll|lll}
$\otimes$ & $a$ & $b$ & $c$ & $\oplus$ & $x$ & $y$ & $z$ \\
\hline$a$ & $a$ & $b$ & $c$ & $x$ & $x$ & $y$ & $z$ \\
$b$ & $b$ & $c$ & $a$ & $y$ & $y$ & $x$ & $z$ \\
$c$ & $c$ & $a$ & $b$ & $z$ & $z$ & $x$ & $y$
\end{tabular}. Then $\{P, \otimes\}$ and $\{Q, \oplus\}$ are homemorphic．【104 台聯電機】
\item[（4）] （4％）An additive group can be isomorphic to a multiplicative group．【107 台聯電機】
\end{itemize}
\end{itemize}

解（1）False．特性不同當然不能同構。
\begin{itemize}
\begin{itemize}
\item[（2）] False．$Z_2 \times Z_4=\{(0,0),(0,1),(0,2),(0,3),(1,0),(1,1),(1,2),(1,3)\}$ 一一檢查知$<(0,0)>=\{(0,0)\} ;<(1,0)>=\{(1,0),(0,0)\} ;<(0,1)>=\{(0,1),(0,2),(0,3),(0,0)\} ;$ $\langle(1,1)\rangle=\{(1,1),(0,2),(1,3),(0,0)\} ;\langle(0,2)\rangle=\{(0,2),(0,0)\} ;\langle(1,2)\rangle=\{(1,2),(0$, $0)\} ;<(0,3)>=\{(0,3),(0,2),(0,1),(0,0)\} ;<(1,3)>=\{(1,3),(0,2),(1,1),(0,0)\}$ ，沒有生成元，故非循環群。但 $Z_8$ 是循環群（1，3，5，7均為生成元），故兩者不同構。
\item[（3）] False．（4）True．
\end{itemize}
\end{itemize}