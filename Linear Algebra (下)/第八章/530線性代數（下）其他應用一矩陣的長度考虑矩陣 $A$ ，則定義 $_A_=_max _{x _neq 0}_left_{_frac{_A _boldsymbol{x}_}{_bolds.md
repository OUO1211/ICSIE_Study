530
線性代數（下）

其他應用一矩陣的長度
考虑矩陣 $A$ ，則定義 $\|A\|=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\}$ 稱為矩陣 $A$ 的長度．
Note
（1）由定義可知，矩陣長度的計算與向量長度有關，而向量長度有 1 －norm， 2 －norm，$\infty$－norm故矩陣的長度也有以下各定義方式：
$$
\|A\|_1=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_1}{\|\boldsymbol{x}\|_1}\right\},\|A\|_2=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_2}{\|\boldsymbol{x}\|_2}\right\},\|A\|_{\infty}=\max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|_{\infty}}{\|\boldsymbol{x}\|_{\infty}}\right\} .
$$
（2）對任意矩陣 $A$ 與向量 $\boldsymbol{y},\|A \boldsymbol{y}\| \leq\|A\|\|\boldsymbol{y}\|$ ．
【證明】
若 $\boldsymbol{y}=\mathbf{0}$ ，則明顯成立．
若 $\boldsymbol{y} \neq \mathbf{0}$ ，則 $\frac{\|A \boldsymbol{y}\|}{\|\boldsymbol{y}\|} \leq \max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\}=\|A\|$ ，故得 $\|A \boldsymbol{y}\| \leq\|A\|\|\boldsymbol{y}\|$ ．
（3）$A$ 為方陣時，（2）的應用：
（a）設 $\lambda$ 為 $A$ 的特徵根，則 $|\lambda| \leq\|A\|$ ．
【證明】
$$
|\lambda|=\frac{|\lambda|\|\boldsymbol{x}\|}{\|\boldsymbol{x}\|}=\frac{\|\lambda \boldsymbol{x}\|}{\|\boldsymbol{x}\|}=\frac{\|A \boldsymbol{x}\|}{\|\boldsymbol{x}\|} \leq \frac{\|A\|\|\boldsymbol{x}\|}{\|\boldsymbol{x}\|}=\|A\| .
$$
（b）若方陣 $A$ 滿足 $\|A\|<1$ ，則 $I-A$（ $I+A$ 也是）為非奇異的．
【證明】此亦稱為 Banach lemma．
若 $I-A$ 為 $\operatorname{singular,~\text {則}\operatorname {det}(I-A)=0\text {，即}1\text {為}A\text {的一特徵根，而與（a）矛盾．}}$
（c）對任意矩陣 $A, B,\|A B\| \leq\|A\|\|B\| ;\|A+B\| \leq\|A\|+\|B\|$ ．
【證明】
（i）$\forall \boldsymbol{x} \in F^{n \times 1}-\{\mathbf{0}\}, \because\|A B \boldsymbol{x}\| \leq\|A\|\|B \boldsymbol{x}\| \leq\|A\|\|B\|\|\boldsymbol{x}\|, \therefore \frac{\|A B \boldsymbol{x}\|}{\|\boldsymbol{x}\|} \leq\|A\|\|B\|$ ，
$$
\therefore\|A B\|=\max _{x \neq 0}\left\{\frac{\|A B \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\} \leq\|A\|\|B\| .
$$
（ii）$\|A+B\|=\max _{x \neq 0}\left\{\frac{\|(A+B) \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\} \leq \max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|+\|B \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\}$
$$
\leq \max _{x \neq 0}\left\{\frac{\|A \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\}+\max _{x \neq 0}\left\{\frac{\|B \boldsymbol{x}\|}{\|\boldsymbol{x}\|}\right\}=\|A\|+\|B\| .
$$