第 8 章 內積算子及其應用
537

8－5 Householder 轉換

Householder 矩陣
考虑 $R^{n \times 1}$ 中的非零向量 $\boldsymbol{w}$ ，
定義 $H=I-\frac{2}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w} \boldsymbol{w}^T$ ，稱做相對於 $\boldsymbol{w}$ 的 Householder 矩陣。
（ $H$ 為對 $\boldsymbol{w}$ 的正交補空間 $S=(\operatorname{span}\{\boldsymbol{w}\})^{\perp}$ 的鏡射矩陣）
Note
又稱 Householder 轉換，或基本鏡射算子。
如圖，欲求 $\boldsymbol{x}$ 對 $(\operatorname{span}(\{\boldsymbol{w}\}))^{\perp}$ 的鏡射 $\boldsymbol{y}$ ，
因為 $(\boldsymbol{y}-\boldsymbol{x})$ 與 $\boldsymbol{w}$ 平行，令 $\boldsymbol{y}-\boldsymbol{x}=\alpha \boldsymbol{w}, ~ \alpha \in R$ ，則 $\boldsymbol{z}=\boldsymbol{x}+\frac{1}{2} \alpha \boldsymbol{w}$ ，
又因 $z \perp w$ ，故 $\langle z, w\rangle=0$ ，
即 $0=\boldsymbol{w}^T \boldsymbol{z}=\boldsymbol{w}^T\left(\boldsymbol{x}+\frac{1}{2} \alpha \boldsymbol{w}\right)=\boldsymbol{w}^T \boldsymbol{x}+\frac{1}{2} \alpha \boldsymbol{w}^T \boldsymbol{w}$ ，得 $\alpha=\frac{-2 \boldsymbol{w}^T \boldsymbol{x}}{\boldsymbol{w}^T \boldsymbol{w}}$ ，

故 $\boldsymbol{y}=\boldsymbol{x}+\alpha \boldsymbol{w}=\boldsymbol{x}+\frac{-2 \boldsymbol{w}^T \boldsymbol{x}}{\boldsymbol{w}^T \boldsymbol{w}} \boldsymbol{w}=\boldsymbol{x}+\frac{-2 \boldsymbol{w} \boldsymbol{w}^T \boldsymbol{x}}{\boldsymbol{w}^T \boldsymbol{w}}=\left(I-\frac{2 \boldsymbol{w} \boldsymbol{w}^T}{\boldsymbol{w}^T \boldsymbol{w}}\right) \boldsymbol{x}$ ．