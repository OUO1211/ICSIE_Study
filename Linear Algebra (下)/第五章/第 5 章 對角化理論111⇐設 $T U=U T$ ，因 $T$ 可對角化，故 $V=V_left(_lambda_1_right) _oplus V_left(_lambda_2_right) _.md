第 5 章 對角化理論
111

⇐設 $T U=U T$ ，
因 $T$ 可對角化，
故 $V=V\left(\lambda_1\right) \oplus V\left(\lambda_2\right) \oplus \cdots \oplus V\left(\lambda_r\right)$ ，其中 $\lambda_1, \lambda_2, \cdots, \lambda_r$ 為 $T$ 的相異特徵根
又因為 $V\left(\lambda_i\right)$ 為 $U-$ 不變子空間，$\forall i=1,2, \ldots, r$ ，
（pf：取 $\boldsymbol{v} \in V\left(\lambda_i\right)$ ，則 $T(\boldsymbol{v})=\lambda_i \boldsymbol{v}$ ，所以 $T(U(\boldsymbol{v}))=U(T(\boldsymbol{v}))=U\left(\lambda_i \boldsymbol{v}\right)=\lambda_i U(\boldsymbol{v})$ ，
$$
\left.\therefore U(\boldsymbol{v}) \in V\left(\lambda_i\right), \quad \therefore U\left(V\left(\lambda_i\right)\right) \subseteq V\left(\lambda_i\right) .\right)
$$

且 $U$ 可對角化，所以 $U_{V\left(\lambda_i\right)}$ 可對角化，$\forall i=1,2, \ldots, r$ ，
故 $U$ 可用 $T$ 的特徵向量來對角化，即 $T, U$ 可同步對角化．
（2）若 $n$ 階方陣 $A, B$ 均可對角化，則
$A, B$ 可同步對角化 $\Leftrightarrow A B=B A$ ．
【94台大電機．電信、94 雲科電資、100 師大數學、 103 中興應數、 107 成大統計】
（3）若 $A B=B A$ ，則 $A, B$ 不一定可同步對角化．例如
取 $A=\left[\begin{array}{ll}1 & 0 \\ 0 & 1\end{array}\right], B=\left[\begin{array}{ll}1 & 0 \\ 1 & 1\end{array}\right]$ ，滿足 $A B=B A$ ，但只 $A$ 可對角化，$B$ 不可對角化．