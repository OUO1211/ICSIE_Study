724
離散數學（上）

7－3 應用問題

河內之塔（The Tower of Hanoi problem）
例題
The Tower of Hanoi consists of three towers，and a number of disks of different sizes which can slide onto any tower．The puzzle starts with the disks in a nest stack in ascending order of size on one tower，the smallest at the top．The objective of the puzzle is to move the entire stack to another tower，obeying the following simple rules：
－Only one disk can be moved at a time．
－Each move consists of taking the upper disk from one of the stacks and placing it on top of another stack，
i．e．，a disk can only be moved if it is the uppermost disk on a stack．
－No disk may be placed on top of a smaller disk．
Let $a_n$ denotes the minimum number of moves needed for $n$ disks for three towers．Show the recurrence relation of $a_n$ and solve $a_n$ ．

【重要】
解 明顯可得 $a_1=1, a_2=3, a_3=7, \ldots$ ；遞迴步驟可分析如下：
考慮 A 柱最下面那個最大的圓盤 $d$ ，欲將 $d$ 從 A 柱搬至 C 柱，須先把 $d$ 上頭的 $n-1$ 個圓盤搬至 B 柱，（這須 $a_{n-1}$ 步），然後把 $d$ 從 A 柱搬至 C 柱（這須 1 步），再把那 B 柱上的 $n-1$ 個圓盤搬至 C 柱（這須 $a_{n-1}$ 步），
則所有的圓盤均到 C 柱上了，$\therefore a_n=2 a_{n-1}+1, n \geq 2$ 。
＊以歸納法證之：$\because a_1=1 ; a_2=3, a_3=7, \ldots$ ，所以猜測 $a_n=2^n-1, n \geq 1$ 。 $n=1$ 時，$a_1=1=2^1-1$ 成立。
設 $k$ 個圓盤時需 $2^k-1$ 次，則 $k+1$ 個圓盤時，
$a_{k+1}=2 a_k+1=2 \cdot\left(2^k-1\right)+1=2^{k+1}-1$ ，即需要 $2^{k+1}-1$ 次，
故由歸納法知：$a_n=2^n-1$ 。
＊以直接代入法解之 ：
$$
\begin{aligned}
a_n & =2 a_{n-1}+1=2\left(2 a_{n-2}+1\right)+1=2^2 a_{n-2}+2+1=2^2\left(2 a_{n-3}+1\right)+2+1 \\
& =2^3 a_{n-3}+2^2+2+1=\ldots=2^{n-1} a_1+2^{n-2}+\ldots+2+1 \\
& =2^{n-1}+2^{n-2}+\ldots+2+1=\frac{2^n-1}{2-1}=2^n-1, ~ \text { 即 } a_n=2^n-1, n \geq 1 。
\end{aligned}
$$