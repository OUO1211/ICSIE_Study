> **矩陣的分割(partition)**
>
> 在處理矩陣的運算時，有時為了需要，會把原來較大的矩陣看成是由幾個較小的矩陣“湊成”的，這個做法稱作矩陣的分割。例如：
>
> $$A=\begin{bmatrix}a_{11}&a_{12}&a_{13}&a_{14}\\a_{21}&a_{22}&a_{23}&a_{24}\\a_{31}&a_{32}&a_{33}&a_{34}\end{bmatrix}=\begin{bmatrix}A_{11}&A_{12}\\A_{21}&A_{22}\end{bmatrix}$$
>
> 也把 $A$ 稱作一個方塊矩陣。
>
> $$B=\begin{bmatrix}b_{11}&b_{12}&b_{13}&b_{14}\\b_{21}&b_{22}&b_{23}&b_{24}\\b_{31}&b_{32}&b_{33}&b_{34}\end{bmatrix}=\begin{bmatrix}B_{(1)}\\B_{(2)}\\B_{(3)}\end{bmatrix}$$
>
> $B_{(i)}$ 又稱為 $B$ 的行向量。
>
> $$C=\begin{bmatrix}c_{11}&c_{12}&c_{13}&c_{14}\\c_{21}&c_{22}&c_{23}&c_{24}\\c_{31}&c_{32}&c_{33}&c_{34}\end{bmatrix}=[C^{(1)}\ C^{(2)}\ C^{(3)}\ C^{(4)}]$$
>
> $C^{(j)}$ 又稱為 $C$ 的列向量。
>
> 而在做表達時，就把各個子矩陣看成元素的樣子來計算，例如：
>
> $$A=\begin{bmatrix}1&2&3&4\\0&1&1&1\\0&0&2&2\end{bmatrix}=\begin{bmatrix}A_{11}&A_{12}\\A_{21}&A_{22}\end{bmatrix},\quad B=\begin{bmatrix}1&0\\1&1\\2&2\\1&0\end{bmatrix}=\begin{bmatrix}B_{11}&B_{12}\\B_{21}&B_{22}\end{bmatrix},$$
>
> 則
>
> $$AB=\begin{bmatrix}A_{11}B_{11}+A_{12}B_{21}&A_{11}B_{12}+A_{12}B_{22}\\A_{21}B_{11}+A_{22}B_{21}&A_{21}B_{12}+A_{22}B_{22}\end{bmatrix}=\begin{bmatrix}13&8\\4&3\\6&4\end{bmatrix}$$
>
> 又例如：
>
> 矩陣 $A=\begin{bmatrix}1&3&5\\2&4&6\end{bmatrix}$ 的第一個列向量為 $A^{(1)}=\begin{bmatrix}1\\2\end{bmatrix}$，第二個行向量為 $A_{(2)}=[2\quad 4\quad 6]$。