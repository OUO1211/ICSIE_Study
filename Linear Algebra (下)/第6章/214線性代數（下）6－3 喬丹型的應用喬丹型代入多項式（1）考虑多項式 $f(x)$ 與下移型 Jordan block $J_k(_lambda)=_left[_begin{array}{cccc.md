214

線性代數（下）



6－3 喬丹型的應用



喬丹型代入多項式

（1）考虑多項式 $f(x)$ 與下移型 Jordan block $J_k(\lambda)=\left[\begin{array}{ccccc}\lambda & & & & O \\ 1 & \lambda & & & \\ & 1 & \lambda & & \\ & & \ddots & \ddots & \\ O & & & 1 & \lambda\end{array}\right]_{k \times k}$,則 $f\left(J_k(\lambda)\right)=\left[\begin{array}{ccccc}f(\lambda) & & & & O \\ f^{\prime}(\lambda) & f(\lambda) & & & \\ \frac{f^{\prime \prime}(\lambda)}{2!} & f^{\prime}(\lambda) & f(\lambda) & & \\ \vdots & \frac{f^{\prime \prime}(\lambda)}{2!} & \ddots & \ddots & \\ \frac{f^{(k-1)}(\lambda)}{(k-1)!} & \cdots & \frac{f^{\prime \prime}(\lambda)}{2!} & f^{\prime}(\lambda) & f(\lambda)\end{array}\right]_{k \times k}$ ．

（2）若 Jordan block $J_a, J_b, \ldots J_z$ 使 $A$ 的 Jordan form $J_A=\left[\begin{array}{llll}J_a & & & O \\ & J_b & & \\ & & \ddots & \\ O & & & J_z\end{array}\right]$ ，則 $f(J)=\left[\begin{array}{cccc}f\left(J_a\right) & & & O \\ & f\left(J_b\right) & & \\ O & & \ddots & \\ & & & f\left(J_z\right)\end{array}\right]$ ．