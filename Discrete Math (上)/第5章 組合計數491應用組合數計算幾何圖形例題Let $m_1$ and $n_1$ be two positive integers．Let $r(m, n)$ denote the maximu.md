第5章 組合計數
491

應用組合數計算幾何圖形
例題
Let $m>1$ and $n>1$ be two positive integers．Let $r(m, n)$ denote the maximum number of rectangles defined by $m$ horizontal lines and $n$ vertical lines in a plane．Derive a formula for $r(m, n)$ ．Note that rectangles may overlap．For example，$r(2,3)=3$ not 2.

【 $89 、 100 、 105$ 中山資エ】【 106 中山電機】
＂解 從 $n$ 條垂直線任取2條做矩形的左右邊有 $\binom{n}{2}$ 種取法，
從 $m$ 條水平線任取 2 條做矩形的上下邊有 $\binom{m}{2}$ 種取法，
所以可造出 $\binom{n}{2}\binom{m}{2}$ 個矩形，
即 $r(m, n)=\binom{n}{2}\binom{m}{2}$ 。