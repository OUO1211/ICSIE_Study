## 第 2 章　線性方程組與求解

> **試題 16**
>
> For the function $f(t) = \det\begin{bmatrix} 7 & 1 & -2 & 0 & 0 \\ -1 & 2 & 1 & 0 & 0 \\ 4 & 3 & 2 & 3 & 4 \\ 2 & 2 & 2 & 2 & 2 \\ 2 & 1 & 0 & \cos t & 2 \end{bmatrix}$，(1) Find $\dfrac{df(t)}{dt}$. (2) Which of the
>
> following is a root of $f(t)$: (i) 0 (ii) $\dfrac{\pi}{4}$ (iii) $\dfrac{\pi}{2}$ (iv) $\pi$.

**解** (1) $f(t) = \det\begin{bmatrix} 7 & 1 & -2 & 0 \\ -1 & 2 & 1 & 0 \\ 4 & 3 & 2 & 3 \\ 2 & 2 & 2 & 2 \end{bmatrix} + t \cdot \det\begin{bmatrix} 7 & 1 & -2 & 0 \\ -1 & 2 & 1 & 0 \\ 4 & 3 & 2 & 3 \\ 2 & 2 & 2 & 2 \end{bmatrix} \cdot \cos t \cdot \begin{bmatrix} 7 & 1 & -2 & 0 \\ -1 & 2 & 1 & 0 \\ 4 & 3 & 2 & 4 \\ 2 & 2 & 2 & 4 \end{bmatrix}$

$\therefore \dfrac{d}{dt} f(t) = \begin{vmatrix} 7 & 1 & -2 & 0 \\ -1 & 2 & 1 & 0 \\ 4 & 3 & 2 & 3 \\ 1 & 2 & 2 & 2 \end{vmatrix} \cdot (-\sin t) = -50 \sin t$

(2) $\cos 0 = 1$，$\cos \dfrac{\pi}{4} = \dfrac{\sqrt{2}}{2}$，$\cos \dfrac{\pi}{2} = 0$，$\cos \pi = -1$，……代入計算可得，

$\cos 0 = 1$，得 $f(0) = 0$，故 (i) 對。

---

> **試題 17**
>
> Define $f(x) = x(x-1)(x-2)\cdots(x-n+1)$，find
>
> $$\det\begin{bmatrix} f(a) & f'(a) & f''(a) & \cdots & f^{(n)}(a) \\ f'(a) & f''(a) & f'''(a) & \cdots & f^{(n+1)}(a) \\ \vdots & & & & \vdots \\ f^{(n)}(a) & f^{(n+1)}(a) & f^{(n+2)}(a) & \cdots & f^{(2n)}(a) \end{bmatrix} = ?$$

**解** $(-1)^{(n+2)(n+1)/2} \cdot (n!)^{n+1}$