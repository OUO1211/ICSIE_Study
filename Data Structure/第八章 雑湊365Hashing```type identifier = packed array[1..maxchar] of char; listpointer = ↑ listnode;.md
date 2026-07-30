第八章 雑湊
365
Hashing
```
type identifier = packed array[1..maxchar] of char;
    listpointer = ↑ listnode;
    listnode = record
            ident : identifier;
            link : listpointer;
        end;
        hashtable = arraly[1..mazsize] of listpointer;
```

procedure chnsrch（ x ：identifier；var ht ：hashtable； b ：integer；var j ：listpointer）；
｛Search the hash table $\mathrm{ht}[0 \mathrm{~b}-1]$ for x ．Elther $\mathrm{ht}[\mathrm{i}]=\mathrm{mil}$ or it is a pointer to the list of identifiers $\mathrm{x}: \mathrm{f}(\mathrm{x})=\mathrm{i}$ ．List nodes gave field ident and link．Either j points to the node already containing x or $\mathrm{j}=$ nil． \}
var found ：Boolean；
begin
$\mathrm{j}:=\mathrm{ht}[\mathrm{f}(\mathrm{x})]$ ；｛compute head node address\}
｛search the chain starting at j \}
found ：＝false；
while（j＜＞nil）and not found do
if j ↑ ．ident＝x then found ：＝true
else $\mathrm{j}:=\mathrm{j} \uparrow$ ．link；
end；｛of chnsrch\}

\section*{－補充}
f 為一均匀的雜湊函數，其值域之範圍為 $[0, \mathrm{~b}-1]$ 。假設有 n 個識別字 $\mathrm{X}_1, \mathrm{X}_2, \cdots X_n$ 等要填入雜湊表中，那 $f\left(X_1\right), f\left(X_2\right), \cdots, f\left(X_n\right)$ 總共可能有 $b^n$ 種不同雜湊順序。假設這 $\mathrm{b}_{\mathrm{n}}$ 種雜湊順序發生的機率相同。令 $\mathrm{S}_{\mathrm{n}}$ 表示搜尋任一識別字$\mathrm{X}_{\mathrm{i}}(1 \leq \mathrm{i} \leq \mathrm{n})$ 所需的平均比較次數，那麼 $\mathrm{S}_{\mathrm{n}}$ 就是在 $\mathrm{b}^{\mathrm{n}}$ 種可能的雜湊順序中（各雜湊順序發生的機率相同），尋找 $\mathrm{X}_1, \mathrm{X}_2, \cdots, \mathrm{X}_{\mathrm{n}}$（每一識別字的機率亦相同）等識別字的平均比較次數。令 $U_n$ 表示搜尋一個不在表中之識別字的平均比較次數。

定理：令 $\alpha=n / b$ 為雑湊表的負載密度（Loading Density），而雜湊表所使用的雜湊函數是均匀的，那麼：