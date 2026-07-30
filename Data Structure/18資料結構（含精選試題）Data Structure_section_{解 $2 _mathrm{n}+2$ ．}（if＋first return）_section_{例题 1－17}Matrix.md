18
資料結構（含精選試題）

Data Structure

\section*{解 $2 \mathrm{n}+2$ ．}
（if＋first return）

\section*{例题 1－17}

Matrix Addition
void add（int［ ］［MAX＿SIZE］，int b［ ］［MAX＿SIZE］，
int c［ ］［MAX＿SIZE］，int rows，int cols）
｛
int i，j；
for $(\mathrm{i}=0 ; \mathrm{i}<$ rows； $\mathrm{i}++)$
for $(\mathrm{j}=0 ; \mathrm{j}<\operatorname{cols} ; \mathrm{j}++)$
c［i］［j］= a［i］［j］+ b［i］［j］；
\}
void add（int［ ］［MAX＿SIZE］，int b［ ］［MAX＿SIZE］，
int c［ ］［MAX＿SIZE］，int rows，int cols）
｛
int i，j；
for $(\mathrm{i}=0 ; \mathrm{i}<$ rows； $\mathrm{i}++) \quad\{$
count＋＋；／＊For i for－loop＊／
$\operatorname{for}(\mathrm{j}=0 ; \mathrm{j}<\operatorname{cols} ; \mathrm{j}++) \quad\{$
count＋＋；／＊For j for－loop＊／
c［i］［j］＝a［i］［j］＋b［i］［j］；
count＋＋；／＊For－assignment statement＊／
\}
count＋＋；／＊Last time of j for－loop＊／
\}
count＋＋；／＊Last time of i for－loop＊／
\}