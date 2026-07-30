第二章 陣列與結構
79

Arrays＆Structures
```
        for (i = 0; i<num_cols; i++)
            row_terms [i] = 0;
        for (i=1; i<=num_terms; i++)
            row_terms [a[i].col]++;
        starting_pos[0] = 1;
        for (i=1; i<num_cols; i++)
            starting_pos[i] =
                starting_pos[i-1] + row_terms[i-1];
        for (i=1; i<=num_terms; i++) {
            j = starting_pos[a[i].col]++;
            b[j].row = a[i].col; b[j].col = a[i].row;
            b[j].value = a[i].value;
        }
    }
}
```


\section*{2－5 上三角與下三角矩陣的循序儲存方式}
\begin{itemize}
\item[一．] 定義
上三角（Upper Triangular）：對角線以下的元素為零，即 $\mathrm{a}_{\mathrm{ij}}=0, \mathrm{i}>\mathrm{j}$
$$
\left|\begin{array}{cccc}
a_{11} & a_{12} & a_{13} & a_{14} \\
& a_{22} & a_{23} & a_{24} \\
& & a_{33} & a_{34} \\
& & & a_{44}
\end{array}\right|
$$
下三角（Lover Triangular）：對角線以上的元素為零，即 $\mathrm{a}_{\mathrm{ij}}=0, \mathrm{i}<\mathrm{j}$
$$
\left|\begin{array}{llll}
a_{11} & & & \\
a_{21} & a_{22} & & \\
a_{31} & a_{32} & a_{33} & \\
a_{41} & a_{42} & a_{43} & a_{44}
\end{array}\right|
$$
\item[二．] 一個 $\mathrm{n} \times \mathrm{n}$ 的上三角或下三角矩陣，其元素的個數
$$
\rightarrow \quad 1+2+3+\cdots+n=n(n+1) / 2
$$
\end{itemize}