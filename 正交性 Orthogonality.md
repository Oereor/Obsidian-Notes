## 正交向量组

1. 正交: $(\alpha,\beta)=0$. 记为$\alpha\perp\beta$. 
2. 向量组 $\{\alpha_i\}$ 正交: $\alpha_i,\alpha_j$ 两两正交. 
3. 标准正交向量组: 正交, 并且每个向量都是单位向量. 

## 正交矩阵

> 列向量组是正交向量组的矩阵即是正交矩阵. 

## Schmidt 标准正交化方法

我们将其分解为以下几个步骤. 

1. **正交化**. 按以下步骤构造向量. 
    - 取 $\beta_1=\alpha_1$. 
    - 取 $\beta_2=\alpha_2-\dfrac{(\alpha_2,\beta_1)}{(\beta_1,\beta_1)}\beta_1$. 
    - 取 $\beta_3=\alpha_3-\dfrac{(\alpha_3,\beta_1)}{(\beta_1,\beta_1)}\beta_1-\dfrac{(\alpha_3,\beta_2)}{(\beta_2,\beta_2)}\beta_2$. 
    - 依此类推, 直到 $\beta_n$. 
    *用数学归纳法可证明 $\{\beta_i\}$ 是正交向量组.*
2. **单位化**. 这一步显然. 

事实上, 还可进一步证明: 这样的标准正交向量组与原向量组是等价的. 