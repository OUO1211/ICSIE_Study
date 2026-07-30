第三章 堆疊與佇列
105
Stack＆Queue

\section*{例題 3－2}
$\mathrm{A}^*(\mathrm{~B}+\mathrm{C})^* \mathrm{D} \rightarrow \mathrm{ABC}+{ }^* \mathrm{D}^*$

\begin{tabular}{|l|l|l|l|}
\hline → & Next token & stack & output \\
\hline & 無 & 空 & 無 \\
\hline & A & 空 & A \\
\hline & ＊ & ＊ & A \\
\hline & （ & ＊（ & A \\
\hline & B & ＊（ & AB \\
\hline & ＋ & ＊（＋ & AB \\
\hline & C & ＊（＋ & ABC \\
\hline & ） & ＊ & ABC＋ \\
\hline & ＊ & ＊ & ABC＋＊ \\
\hline & D & ＊ & ABC＋＊D \\
\hline & done & empty & ABC＋＊D＊ \\
\hline
\end{tabular}

\section*{三．計算 postfix 之值}

【演算法】計算後置式的演算法
Procedure eval（e：expression）；
｛ Evaluate the postfix expression e．It is assumed that the last token（a token is either an operator，operand，or＇＃＇）in e is＇＃＇．A procedure NextToken is used to extract from e the next token．A one－dimensional array stack $[1 \cdots n]$ is used as a stack．\}
```
var x:token;
    BEGIN
        top := 0; {Initialize stack}
            x := NextToken(e);
        while x<> '#' do
        BEGIN
            if x is an operand then push {add to stack}
            else BEGIN {operator}
            pop the correct number of operands for operator x from stack; perform
```