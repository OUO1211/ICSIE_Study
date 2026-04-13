> **試題 18**
>
> If $F(x) = \det\begin{bmatrix} x & x^2 & x^3 & x^4 \\ 1 & 2 & 4 & 8 & 16 \\ 1 & 3 & 9 & 27 & 81 \\ 1 & 4 & 16 & 64 & 256 \end{bmatrix}$，show: $F'(x) = c(x^3 - 3x + 2)(x^2 + ax + b)$ for some
>
> choice of constants $a$, $b$, $c$ and give the values of three constants.

**解** $F'(x) = \det\begin{bmatrix} 1 & x & x^2 & x^3 \\ 1 & 2 & 4 & 8 & 16 \\ 1 & 3 & 9 & 27 & 81 \\ 1 & 4 & 16 & 64 & 256 \end{bmatrix}$

$= (x-1)(x-2)(x-1)(x-3)(x-2)(x-3)(x-4)(x-3)(x-4)$

$= -(x-1)(x-2)(x-1)(x-3)(x-2)(x-4)(x-3)$

$= 12(2 - 7x + x^2)(2 - 3x + x^2)$，故 $a = -7$，$b = 12$，$c = 12$。

---

> **試題 19**
>
> Show that $\begin{vmatrix} b+c & cd & bc+cd+db & bcd \\ c+d & da & cd+da+ac & cda \\ d+a & ab & da+ab+bd & dab \\ a+b & bc & ab+bc+ca & abc \end{vmatrix} = \begin{vmatrix} b+c & cd & bc+cd+db & bcd \\ c+d & da & cd+da+ac & cda \\ d+a & ab & da+ab+bd & dab \\ a+b & bc & ab+bc+ca & abc \end{vmatrix}$

**解** $\begin{vmatrix} b+c+d & ab & cd+da+ac & cda \\ c+d+a & bc & da+ab+bd & dab \\ d+a+b & cd & ab+bc+ca & abc \\ a+b+c & da & bc+cd+db & bcd \end{vmatrix}$

運用列變換運算，化簡後可得

$= \begin{vmatrix} -a & bc+cd+db & bcd \\ -b & cd+da+ac & cda \\ -c & da+ab+bd & dab \\ -d & ab+bc+ca & abc \end{vmatrix}$

整理後，$\times(-1)$ 使得：

$= \begin{vmatrix} a^2 & (bc+cd+db)a & bcd \\ b^2 & (cd+da+ac)b & cda \\ c^2 & (da+ab+bd)c & dab \\ d^2 & (ab+bc+ca)d & abc \end{vmatrix}$
