第 4 章 數學歸納法與數論 311

數字的組合
例題

P

（ $8 \%$ ）For the statement that a postage of $n$ cents can be formed using just 4－cent and 11－cent stamps for $n \geq 30$ ．
（1）Prove by principle of mathematical induction．
（2）Prove by strong induction．
【100中正資工類題】【105中正資エ】
解（1）$n=30$ 時， $30=4 \times 2+11 \times 2$ 故命題成立。
設 $n=k \geq 30$ 時，命題亦成立，
則 $n=k+1$ 時，
（1）$n=k$ 時沒有用到 11 （則其中至少用了 8 個 4），
則取出 8 個 4 ，代入 3 個 11 ，而得到 $n=k+1$ 的表達式。
（2）$n=k$ 時至少用了 1 個 11 。
則取出 1 個 11 ，代入 3 個 4 ，而得到 $n=k+1$ 的表達式。
故知，$n=k+1$ 時，亦可表成 4 與 11 的線性組合。
（2）

\begin{tabular}{ll}
$n=30$ 時， $30=4 \times 2+11 \times 2$, & $n=31$ 時， $31=4 \times 5+11 \times 1$, \\
$n=32$ 時， $32=4 \times 8+11 \times 0$, & $n=33$ 時， $33=4 \times 0+11 \times 3$,
\end{tabular}

設 30 到 $k$ 的所有整數都可用 4 與 11 組合，$k \geq 33$ ，
則 $n=k+1$ 時，$\because k+1=(k-3)+4$ ，而 $k-3$ 可表達為 4 與 11 的線性組合，
故知 $k+1$ 亦可表為 4 與 11 的線性組合，故由歸納法知此性質成立。

基礎類題
1．$n \in Z^{+}, n \neq 1,3$ ，證明 $n$ 必可表示為若干個 2＇s 與若干個 5＇s 之和。
2．$n \in Z^{+}, n \geq 14$ ，證明 $n$ 必可表示為若干個 3’s 與若干個 8’s 之和。
【93 中央網路】【99 台大工科】【101 中山電機】
3．$n \in Z^{+}, n \geq 24$ ，證明 $n$ 必可表示為若干個 5＇s 與若干個 7＇s 之和。
【99 嘉義資エ】【99 清大資應】【110 成大資工】
4．$n \in Z^{+}, n \geq 64$ ，證明 $n$ 必可表示為若干個 5 ＇s 與若干個 17＇s 之和。
【90師大資教】【92清大資工】【95清大資應】