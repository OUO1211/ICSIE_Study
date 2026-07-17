第 8 章 各內積算子及其應用
523

（3） $\max _{x \neq 0} \rho(\boldsymbol{x})=\max _{\|x\|=1} \rho(\boldsymbol{x}) ; \min _{x \neq 0} \rho(\boldsymbol{x})=\min _{\|x\|=1} \rho(\boldsymbol{x})$ 。（有時找最大或最小值時，常限制在單位向量上，有了這個性質，就可直接利用前一頁的結果）
【證明】
此處證明 $\max _{x \neq 0} \rho(\boldsymbol{x})=\max _{\|x\|=1} \rho(\boldsymbol{x})$ ；而 $\min _{x \neq 0} \rho(\boldsymbol{x})=\min _{\|x\|=1} \rho(\boldsymbol{x})$ 留給讀者練習。
令 $\boldsymbol{x}_0$ 使 $\rho\left(\boldsymbol{x}_0\right)=\frac{\left\langle A \boldsymbol{x}_0, \boldsymbol{x}_0\right\rangle}{\left\langle\boldsymbol{x}_0, \boldsymbol{x}_0\right\rangle}$ 為 $\rho(\boldsymbol{x})=\frac{\langle A \boldsymbol{x}, \boldsymbol{x}\rangle}{\langle\boldsymbol{x}, \boldsymbol{x}\rangle}$ for all $\boldsymbol{x} \neq \mathbf{0}$ ，中的最大值，
則考慮 $\boldsymbol{y}=\frac{\boldsymbol{x}_0}{\left\|\boldsymbol{x}_0\right\|},\|\boldsymbol{y}\|=1$ ，且 $\rho(\boldsymbol{y})=\frac{\langle A \boldsymbol{y}, \boldsymbol{y}\rangle}{\langle\boldsymbol{y}, \boldsymbol{y}\rangle}=\frac{\left\langle A \frac{\boldsymbol{x}_0}{\left\|\boldsymbol{x}_0\right\|}, \frac{\boldsymbol{x}_0}{\left\|\boldsymbol{x}_0\right\|}\right\rangle}{\left\langle\frac{\boldsymbol{x}_0}{\left\|\boldsymbol{x}_0\right\|}, \frac{\boldsymbol{x}_0}{\left\|\boldsymbol{x}_0\right\|}\right\rangle}=\frac{\left\langle A \boldsymbol{x}_0, \boldsymbol{x}_0\right\rangle}{\left\langle\boldsymbol{x}_0, \boldsymbol{x}_0\right\rangle}=\rho\left(\boldsymbol{x}_0\right)$ ，
故得， $\max _{\|x\|=1} \rho(\boldsymbol{x}) \geq \rho(\boldsymbol{y})=\rho\left(\boldsymbol{x}_0\right)=\max _{x \neq 0} \rho(\boldsymbol{x})$ ，即 $\max _{\|x\|=1} \rho(\boldsymbol{x}) \geq \max _{x \neq 0} \rho(\boldsymbol{x})$ ，
另一方面， $\max _{\|x\|=1} \rho(x)$ 只從那些長度為 1 的向量 $x$ 求 $\rho(x)$ ，
而 $\max _{\|x\|=0} \rho(x)$ 是從那些長度不為 0 的向量 $x$ 求 $\rho(x)$ ，所考慮的 $x$ 比前述多得多，
故明顯可得： $\max _{\|x\|=1} \rho(\boldsymbol{x}) \leq \max _{x \neq 0} \rho(\boldsymbol{x})$ ，
故得 $\max _{\|x\|=1} \rho(x)=\max _{x \neq 0} \rho(x)$ ．