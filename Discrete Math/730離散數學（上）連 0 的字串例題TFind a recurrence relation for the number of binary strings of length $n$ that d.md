730
離散數學（上）

連 0 的字串
例題
T
Find a recurrence relation for the number of binary strings of length $n$ that do not contain three consecutive 0＇s．

【89 中正資エ】【96 中興資網】【96 東華資エ】【101 清大資エ】【105 成大資エ】
解 令所求為 $a_n$ ，
則 $a_1=2$ 種 $(0,1) ; ~ a_2=4$ 種 $(00,01,10,11) ; ~ a_3=7$ 種 $(001,010,011,100,101,110,111)$ ；
而對 $n \geq 4$ ，符合題目敘述的字串可分類計算如下：
若首數 $\neq 0$ ，則後 $(n-1)$ 數不含三連續 0 即可，有 $a_{n-1}$ 種，
若首數 $=0$ ，則第二位 $\neq 0$ 時，只需後 $(n-2)$ 數不含三連 0 即可，有 $a_{n-2}$ 種；
若首數 $=0$ ，第二位 $=0$ 時，第三位必 $\neq 0$ ，故只需後 $(n-3)$ 數不含三連 0 ，有 $a_{n-3}$ 種；
得遞迴關係式：$\left\{\begin{array}{l}a_n=a_{n-1}+a_{n-2}+a_{n-3}, n \geq 4 \\ a_1=2, a_2=4, a_3=7\end{array}\right.$ ．
例題
（1）Find a recurrence relation for the number of binary strings of length $n$ that contain three consecutive 0s．（2）What are the initial conditions？（3）How many binary strings of length seven do contain three consecutive 0s？

【109中正資工】
解 令長度 $n$ 含三連 0 的字串有 $a_n$ 種，
（1）$a_n$ 的分析如下：對 $n \geq 4$ ，符合題目敘述的字串可分類計算如下：
若首數 $=1$ ，則後 $(n-1)$ 含三連 0 即可，有 $a_{n-1}$ 種，
若首數 $=0$ ，第二位 $=1$ ，則只需後 $(n-2)$ 數含三連 0 即可，有 $a_{n-2}$ 種；
若首數 $=0$ ，第二位 $=0$ ，第三位 $=1$ ，則只需後 $(n-3)$ 含三連 0 即可，有 $a_{n-3}$ 種；
若首數 $=0$ ，第二位 $=0$ ，第三位 $=0$ ，則後 $(n-3)$ 可為任意二元字串，有 $2^{n-3}$ 種；
所以得遞迴關係式，$a_n=a_{n-1}+a_{n-2}+a_{n-3}+2^{n-3}, n \geq 4$ 。
（2）$a_1=0, a_2=0, a_3=1$ 種（即 000 ）。
（3）
$$
\begin{aligned}
& a_4=a_3+a_2+a_1+2=1+0+0+2=3 \\
& a_5=a_4+a_3+a_2+2^2=3+1+0+2^2=8 \\
& a_6=a_5+a_4+a_3+2^3=8+3+1+2^3=20 \\
& a_7=a_6+a_5+a_4+2^4=20+8+3+2^4=47
\end{aligned}
$$