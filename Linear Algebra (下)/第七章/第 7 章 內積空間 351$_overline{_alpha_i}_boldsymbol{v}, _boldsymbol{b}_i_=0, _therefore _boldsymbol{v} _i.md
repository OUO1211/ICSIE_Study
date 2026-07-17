第 7 章 內積空間 351
$\overline{\alpha_i}<\boldsymbol{v}, \boldsymbol{b}_i>=0, \therefore \boldsymbol{v} \in W^{\perp}$.

⇐任取 $\boldsymbol{x}=\sum_{i=1}^n \alpha_i \boldsymbol{b}_i \in W, \alpha_i$ 為純量，則 $\langle\boldsymbol{v}, \boldsymbol{x}\rangle=<\boldsymbol{v}, \sum_{i=1}^n \alpha_i \boldsymbol{b}_i>=\sum_{i=1}^n \overline{\alpha_i}<\boldsymbol{v}, \boldsymbol{b}_i>=0, \therefore \boldsymbol{v} \in W^{\perp}$ ．
（4）考慮 $V$ 的子空間 $W_1, W_2$ ，則
（a）$W_1 \subseteq W_2 \Leftrightarrow W_2^{\perp} \subseteq W_1^{\perp}$ ．
（b）$\left(W_1+W_2\right)^{\perp}=W_1^{\perp} \cap W_2^{\perp}$ ．
（c）$\left(W_1 \cap W_2\right)^{\perp}=W_1^{\perp}+W_2^{\perp}$ ．
【證明】
【93 中興應數、107 成大數學】
（a）（ ⇒ ）：設 $\boldsymbol{s} \in W_2^{\perp}$ ，則 $\langle\boldsymbol{s}, \boldsymbol{w}\rangle=0, \forall \boldsymbol{w} \in W_2$ ，
任取 $\boldsymbol{x} \in W_1, \because W_1 \subseteq W_2$ ，故 $\boldsymbol{x} \in W_2$ ，故得 $\langle\boldsymbol{s}, \boldsymbol{x}\rangle=0$ ，即 $\boldsymbol{s} \in W_1^{\perp}$ ，故得 $W_2^{\perp} \subseteq W_1^{\perp}$ ．
$(\Leftarrow)$ ：因為 $W_2^{\perp}, W_1^{\perp}$ 均為 $V$ 的子空間，由 $(\Rightarrow)$ 可得 $\left(W_1^{\perp}\right)^{\perp} \subseteq\left(W_2^{\perp}\right)^{\perp}$ ．
又先用後面會得到的一個結果：$\left(W^{\perp}\right)^{\perp}=W, \forall V$ 的子空間 $W$ ，故得 $W_1 \subseteq W_2$ ．
（b）（ $\subseteq$ ）：由（1），$\because W_1 \subseteq W_1+W_2, \therefore\left(W_1+W_2\right)^{\perp} \subseteq W_1^{\perp}$ ，同理 $\left(W_1+W_2\right)^{\perp} \subseteq W_2^{\perp}$ ，故得 $\left(W_1+W_2\right)^{\perp} \subseteq W_1^{\perp} \cap W_2^{\perp}$ ．
$(\supseteq): \quad \forall \boldsymbol{v} \in W_1^{\perp} \cap W_2^{\perp},<\boldsymbol{v}, \boldsymbol{w}_1>=<\boldsymbol{v}, \boldsymbol{w}_2>=0, \forall \boldsymbol{w}_1 \in W_1, \boldsymbol{w}_2 \in W_2$,而對任意 $\boldsymbol{w} \in W_1+W_2$ ，必存在 $\boldsymbol{u}_1 \in W_1, \boldsymbol{u}_2 \in W_2$ ，使得 $\boldsymbol{w}=\boldsymbol{u}_1+\boldsymbol{u}_2$ ，故 $\langle\boldsymbol{v}, \boldsymbol{w}\rangle=\left\langle\boldsymbol{v}, \boldsymbol{u}_1+\boldsymbol{u}_2\right\rangle=\left\langle\boldsymbol{v}, \boldsymbol{u}_1\right\rangle+\left\langle\boldsymbol{v}, \boldsymbol{u}_2\right\rangle=0+0=0$ ，即 $\boldsymbol{v} \in\left(W_1+W_2\right)^{\perp}$ ，故得 $W_1^{\perp} \cap W_2^{\perp} \subseteq\left(W_1+W_2\right)^{\perp}$ ．
（c）由（b），$\left(W_1^{\perp}+W_2^{\perp}\right)^{\perp}=\left(W_1^{\perp}\right)^{\perp} \cap\left(W_2^{\perp}\right)^{\perp}$ ，
又 $\left(W_1^{\perp}\right)^{\perp}=W_1,\left(W_2^{\perp}\right)^{\perp}=W_2$ ，
故得 $\left(W_1^{\perp}+W_2^{\perp}\right)^{\perp}=W_1 \cap W_2$ ，
$\therefore\left(\left(W_1^{\perp}+W_2^{\perp}\right)^{\perp}\right)^{\perp}=\left(W_1 \cap W_2\right)^{\perp}$ ，即得 $\left(W_1^{\perp}+W_2^{\perp}\right)=\left(W_1 \cap W_2\right)^{\perp}$ ．