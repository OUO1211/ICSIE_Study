358
資料結構（含精選試題）
Data Structure

\section*{8－1 符號表（Symbol Table）}

符號表在開發載入程式（Loader），組譯程式（Assembler），編譯程式（Compiler）或者任何以鍵字（Keyword）驅動的轉換程式中都要用到。在這些應用中，符號表是由名稱一數值對（Name－Value Pairs）所構成的集合。
\begin{itemize}
\item[] －符號表的運算
符號表的運算大致有一
\begin{itemize}
\item[1．] 詢問某項目是否已在表中。
\item[2．] 讀取某項目的各屬性。
\item[3．] 插入一新項目。
\item[4．] 刪除某項目。
\end{itemize}
\item[] －符號表的資料結構
structure SYMBOL－TABLE
declare CREATE（ ）→symtb
INSERT（symtb ，name ，value）→ symtb
DELETE（symtb，name）→ symtb
FIND（symtb，name）→ value
HAS（symtb，name）→Boolean
ISMTST（symtb）→Boolean；
for all $\mathrm{S} \varepsilon$ symtb， $\mathrm{a}, \mathrm{b}, \varepsilon$ name， $\mathrm{r} \varepsilon$ value let
ISMTST（CREATE）：：＝true
$\operatorname{ISMTST}(\operatorname{INSERT}(\mathrm{S}, \mathrm{a}, \mathrm{r}))::=$ false
HAS（CREATE，a）：：＝false
$\operatorname{HAS}(\operatorname{INSERT}(\mathrm{S}, \mathrm{a}, \mathrm{r}), \mathrm{b})::=$
if $\operatorname{EQUAL}(\mathrm{a}, \mathrm{b})$ then true else HAS（S，b）
DELETE（CREATE，a）：：＝CREATE
DELETE（INSERT（S，a，r，），b）：：＝
if EQUAL（a，b）then S
else INSERT（DELETE（S，b），a，r）
FIND（CREATE，a）：：＝error
$\operatorname{FIND}(\operatorname{INSERT}(\mathrm{S}, \mathrm{a}, \mathrm{r}), \mathrm{b})::=$ if $\operatorname{EQUAL}(\mathrm{a}, \mathrm{b})$ then else
FIND（S，b）end
End SYMBOL＿TABLE
\end{itemize}