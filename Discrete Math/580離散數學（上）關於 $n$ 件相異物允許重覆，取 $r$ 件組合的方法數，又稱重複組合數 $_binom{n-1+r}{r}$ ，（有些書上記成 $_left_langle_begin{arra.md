580
離散數學（上）

關於 $n$ 件相異物允許重覆，取 $r$ 件組合的方法數，又稱重複組合數 $\binom{n-1+r}{r}$ ，（有些書上記成 $\left\langle\begin{array}{c}n \\ r\end{array}\right\rangle$ ）。其相關性質整理如下，供讀者自行練習。

重複組合數性質
定義 $\left\langle\begin{array}{l}n \\ r\end{array}\right\rangle=\binom{n+r-1}{r}$ ，則
（1）$\left\langle\begin{array}{c}n \\ r\end{array}\right\rangle=\left\langle\begin{array}{c}n \\ r-1\end{array}\right\rangle+\left\langle\begin{array}{c}n-1 \\ r\end{array}\right\rangle$
（2）$\left\langle\begin{array}{l}n \\ r\end{array}\right\rangle=\frac{n}{r}\left\langle\begin{array}{c}n+1 \\ r-1\end{array}\right\rangle=\frac{n+r-1}{r}\left\langle\begin{array}{c}n \\ r-1\end{array}\right\rangle$
（3）$\left\langle\begin{array}{c}n+1 \\ r\end{array}\right\rangle=\left\langle\begin{array}{c}n \\ 0\end{array}\right\rangle+\left\langle\begin{array}{c}n \\ 1\end{array}\right\rangle+\ldots+\left\langle\begin{array}{c}n \\ r\end{array}\right\rangle$
仿組合數以組合的方式說明；或換成組合數之後，再以代數方式證明之。