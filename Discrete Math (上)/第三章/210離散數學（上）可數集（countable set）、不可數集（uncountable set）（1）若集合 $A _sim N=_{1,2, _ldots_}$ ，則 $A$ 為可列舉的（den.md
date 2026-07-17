210
離散數學（上）

可數集（countable set）、不可數集（uncountable set）
（1）若集合 $A \sim N=\{1,2, \ldots\}$ ，則 $A$ 為可列舉的（denumerable）。
（2）若集合 $A$ 為有限或為可列舉的，則稱 $A$ 為可數集；否則 $A$ 稱為不可數集。
Note
（1）設 $A \subseteq B$ ，則
【98 台大電機】
若 $A$ 為不可數集，則 $B$ 為不可數集。
若 $B$ 為可數集，則 $A$ 為可數集。
即可數集的子集皆為可數集；也因此，$N$ 的任意子集皆為可數。
（2）可數集不一定是有限集；不可數集一定是無限集。
（3）有限集一定是可數集；無限集不一定是不可數集。
（4）若 $A$ 為無限集且存在一函數 $f: A \longrightarrow N$ ，則 $A$ 為可數集。
【證明】
因為函數 $f: A \xrightarrow[1-1]{ } f(A)$ 亦為 onto，即 $A \sim f(A)$ ，但 $f(A) \subseteq N$ ，所以 $f(A)$ 亦為可數集，所以 $A$ 亦為可數集。
（5）欲證明某一集合 $A$ 為可數集，常用以下各種方法：
（1）找一函數 $f$ 與整數 $n$ 使 $f: A \xrightarrow{1-1 \text { onto }}\{1,2, \ldots, n\}$ ；或
（2）找一函數 $f$ 使 $f: A \xrightarrow{1-1, \text { onto }} N$ 。
（3）找一可數集合 $B$ ，一函數 $f$ 使 $f: A \xrightarrow{1-1, \text { onto }} B$ 。
（4）找一可數集合 $B$ ，使 $A \subseteq B$ 。
（5）找一函數 $f$ 使 $f: A \xrightarrow{1-1} N \circ(A$ 為無限集時 $)$