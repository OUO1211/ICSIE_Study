第 7 章 遞迴關係式 745

與矩陣有關

例題 6
$D_n=\operatorname{det}\left(\left[\begin{array}{llllll}b & b & & & & \\ b & b & b & & 0 & \\ & b & b & \ddots & & \\ & & b & \ddots & b & \\ & 0 & & \ddots & b & b \\ & & & & b & b\end{array}\right]_{n \times n}\right)$ ，請列出其遞迴並求一般式。
解 由行列式降階展開法知
$$
\begin{aligned}
& \left.D_n=b \times \left\lvert\, \begin{array}{ccccc}
b & b & & & \\
b & b & b & & 0 \\
& b & b & \ddots & \\
& b & \ddots & b \\
0 & & \ddots & b & b \\
& & & -b \times\left|\begin{array}{ccccc}
b & 0 & & & \\
b & b & b & & 0 \\
& b & b & \ddots & \\
& & b & \ddots & b \\
0 & & \ddots & b & b \\
& & & b & b
\end{array}\right|_{(n-1) \times(n-1)} \\
=b \times D_{n-1}-b \times\left(b \times\left|\begin{array}{ccccc}
b & b & & & \\
b & b & b & & 0 \\
& b & b & \ddots & \\
& b & \ddots & b \\
& 0 & & \ddots & b \\
& b \\
& & & b & b
\end{array}\right|_{(n-2) \times(n-2)}\right.
\end{array}\right.\right)=b D_{n-1}-b^2 D_{n-2}, \text { for } n \geq 3 .
\end{aligned}
$$

又 $D_1=\operatorname{det}([b])=b, D_2=\operatorname{det}\left(\left[\begin{array}{ll}b & b \\ b & b\end{array}\right]\right)=0$ ，
即 $\left\{\begin{array}{l}D_n=b D_{n-1}-b^2 D_{n-2}, n \geq 3 \\ D_1=b, D_2=0\end{array}\right.$ ，
而由特徴式法可解得 $D_n=b^n\left(\cos \frac{n \pi}{3}+\frac{1}{\sqrt{3}} \sin \frac{n \pi}{3}\right), n \geq 1$ 。