398
線性代數（下）

7－5 外積

考虑 $R^3$ 上的雨向量 $\boldsymbol{u}=\left(u_1, u_2, u_3\right), \boldsymbol{v}=\left(v_1, v_2, v_3\right)$ ，
定義 $\boldsymbol{u} \times \boldsymbol{v}=\left(\left|\begin{array}{ll}u_2 & u_3 \\ v_2 & v_3\end{array}\right|,\left|\begin{array}{ll}u_3 & u_1 \\ v_3 & v_1\end{array}\right|,\left|\begin{array}{ll}u_1 & u_2 \\ v_1 & v_2\end{array}\right|\right)$ 稱為 $\boldsymbol{u}$ 與 $\boldsymbol{v}$ 的外積。
Note
（1）外積只對 $R^3$ 的向量作定義．
（2）也有些表達成 $\boldsymbol{u} \times \boldsymbol{v}=\left|\begin{array}{ccc}\boldsymbol{i} & \boldsymbol{j} & \boldsymbol{k} \\ u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3\end{array}\right|$ ，其中 $\boldsymbol{i}=\boldsymbol{e}_1, \boldsymbol{j}=\boldsymbol{e}_2, \boldsymbol{k}=\boldsymbol{e}_3$ ，展開後可得 $\boldsymbol{u} \times \boldsymbol{v}=\left|\begin{array}{ll}u_2 & u_3 \\ v_2 & v_3\end{array}\right| \boldsymbol{i}+\left|\begin{array}{ll}u_3 & u_1 \\ v_3 & v_1\end{array}\right| \boldsymbol{j}+\left|\begin{array}{ll}u_1 & u_2 \\ v_1 & v_2\end{array}\right| \boldsymbol{k}$ ．
（3）由以下的性質（7），故可以外積來求與給定兩向量均正交的向量。
外積的性質
設向量 $\boldsymbol{u}, \boldsymbol{v}, \boldsymbol{w} \in R^3, c \in R$ ，則
（1） $\boldsymbol{u} \times \boldsymbol{u}=\mathbf{0}, \boldsymbol{u} \times \mathbf{0}=\mathbf{0} \times \boldsymbol{u}=\mathbf{0}$ ．
（2） $\boldsymbol{u} \times \boldsymbol{v}=-(\boldsymbol{v} \times \boldsymbol{u})$ ．
（3） $\boldsymbol{u} \times(\boldsymbol{v}+\boldsymbol{w})=\boldsymbol{u} \times \boldsymbol{v}+\boldsymbol{u} \times \boldsymbol{w}$ ．
（4）$c(\boldsymbol{u} \times \boldsymbol{v})=(c \boldsymbol{u}) \times \boldsymbol{v}=\boldsymbol{u} \times(c \boldsymbol{v})$ ．
（5）$\|\boldsymbol{u} \times \boldsymbol{v}\|^2=\|\boldsymbol{u}\|^2\|\boldsymbol{v}\|^2-\langle\boldsymbol{u}, \boldsymbol{v}\rangle^2$ ．
（6） $\boldsymbol{u} \cdot(\boldsymbol{v} \times \boldsymbol{w})=\left|\begin{array}{lll}u_1 & u_2 & u_3 \\ v_1 & v_2 & v_3 \\ w_1 & w_2 & w_3\end{array}\right|$ ，其中， $\boldsymbol{u}=\left(u_1, u_2, u_3\right), \boldsymbol{v}=\left(v_1, v_2, v_3\right), \boldsymbol{w}=\left(w_1, w_2, w_3\right) \in R^3$ ．
（7） $\boldsymbol{u} \cdot(\boldsymbol{u} \times \boldsymbol{v})=0, \boldsymbol{v} \cdot(\boldsymbol{u} \times \boldsymbol{v})=0$ 。（即 $\boldsymbol{u} \times \boldsymbol{v}$ 與 $\boldsymbol{u}, \boldsymbol{v}$ 均垂直）
（8）若 $\boldsymbol{u}$ 與 $\boldsymbol{v}$ 夾角為 $\theta$ ，則 $\|\boldsymbol{u} \times \boldsymbol{v}\|=\|\boldsymbol{u}\|\|\boldsymbol{v}\| \sin \theta$ 。
（9） $\boldsymbol{u}, \boldsymbol{v}$ 平行若且唯若 $\boldsymbol{u} \times \boldsymbol{v}=\mathbf{0}$ ．
（10）以 $\boldsymbol{u}$ 與 $\boldsymbol{v}$ 為鄰邊所成的平行四邊形的面積為 $\|\boldsymbol{u} \times \boldsymbol{v}\|$ ．
（11）以 $\boldsymbol{u}, \boldsymbol{v}, \boldsymbol{w}$ 為鄰邉所成的平行六邊體的體積為 $|\boldsymbol{u} \cdot(\boldsymbol{v} \times \boldsymbol{w})|$ 。
（1）$\sim$（8）均可由定義得證，（9）～（11）為（8）的應用。