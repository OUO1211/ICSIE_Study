434
離散數學（上）

環狀排列
$n$ 件相異物放在 $n$ 個位子的環狀排列數有 $n!/ n$ 種。

【93台大資工】

例題
（10\％）A group of 10 people sits in a round table．How many different seating arrangements are there？We assume that a seating arrangement is determined by who sits next to whom and not by where they sit．We also agree not to distinguish between clockwise and counterclockwise；all that matters is who your two neighbors are，not who is on your left and who is on your right．

【104成大電通】
解 先把 10 人排成一直線（共 10 ！種不同排法），再頭尾相接形成環狀，但這樣排成的環狀，每十種可經旋轉而可視為同一種，
例如：12345678910，與 23456789101 ，與 34567891012 ，．．．，與 10123456789 ，且順時針與逆時針又視為相同，故回答共有 $\frac{10!}{2 \times 10}$ 種不同的坐法。