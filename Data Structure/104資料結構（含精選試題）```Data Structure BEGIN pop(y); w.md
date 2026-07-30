104
資料結構（含精選試題）
```
Data Structure
                BEGIN
                    pop(y);
                    write(y);
                END;
                push(x);
            END;
        x := NextToken(e);
    END; {of while}
    {End of expression: Empty Stack}
    while top > 1 do
        BEGIN
            pop(y);
            write(y);
        END;
    writeln('#');
END; {of postfix}
```


【註】（1）isp（in－stack－priority）。
\begin{itemize}
\begin{itemize}
\item[②] isp（in－coming priority）。
\item[（3）] isp［＇（＇）＝5，icp［＇（＇）＝0，isp［＇＃＇］＝5，數字愈小，優先權愈高。
\item[（4）] Time complexity： $0(\mathrm{n})$ if 式子有 n 個符號。
\end{itemize}
\end{itemize}

【注意】「＇在 stack 外，優先權最大，但在 stack 內則優先權變小。

例題 3－1
$$
\mathrm{A}+\mathrm{B}^* \mathrm{C} \rightarrow \mathrm{ABC}^{*+}
$$

\begin{tabular}{|l|l|l|l|}
\hline → & Next token & stack & output \\
\hline & 無 & 空 & 無 \\
\hline & A & 空 & A \\
\hline & ＋ & ＋ & A \\
\hline & B & ＋ & AB \\
\hline & ＊ & ＋＊ & AB \\
\hline & C & ＋＊ & ABC \\
\hline
\end{tabular}

掃瞄完，一個一個移 →ABC＊＋

的