第 5 章 組合計數
429

直線全相異排列
$n$ 件相異物放在同一列共 $n$ 個不同位子的排列数有 $n!$ 種。
例如，
排列 $A, B, C$ 的方式有 $3!$ 種 $(A B C, A C B, B A C, B C A, C A B, C B A)_{\circ}^{\circ}$

例題
（12\％）A computer science professor has thirteen different programming books on a bookshelf． Six of the books deal with C＋＋，the other with Java．In how many ways can the professor arrange these books on the shelf
（1）$(3 \%)$ if there are no restrictions．
（2）$(3 \%)$ if the languages should alternate？
（3）$(3 \%)$ if all the Java books must next to each other？
（4）（3\％）if all the C＋＋books must be next to each other and all the Java books must be next to each other？

【102 中山資工】
（1）即 13 個相異物件的排列數，有 13 ！種。
（2）即為如 $J C J C J C J C J C J C J$ 的擺放，
而 Java 的排列數有 $7!$ 種，C ++ 的排列數有 $6!$ 種，由乘法原理得知共 $6!\times 7!$ 種。
（3）Java 放一起（排列數有 7 ！種）成為一本，再與六本 C＋＋的排列數有 7 ！種，由乘法原理得知共 $7!\times 7!$ 種。
（4）C＋＋綁成一綑方法數 $6!$ ；Java 綁成一綑方法數 $7!$ ；
再考慮是 CCCCCCJJJJJJJ，或 JJJJJJJCCCCCC，
故共有 $6!\times 7!\times 2$ 種。

例題
6

（10\％）In how many ways can the 26 letters of the alphabet $a, b, c, \ldots, x, y, z$ ，be permuted so that none of the patterns spin，nets，cade，or eat occurs？
解 26 個符號的排法有 $26!$ 種，其中，必出現 spin 的方法數為 $23!$ 、必出現 nets 的方法數為 23 ！、必出現 cade 的方法數為 23 ！、必出現 eat 的方法數為 24 ！、必同時出現 spin 與 cade 的方法數為 20 ！、必同時出現 spin 與 eat 的方法數為 $21!$ 。故所求為 26 ！－ 23 ！－ 23 ！－ 23 ！－ 24 ！+20 ！+21 ！。