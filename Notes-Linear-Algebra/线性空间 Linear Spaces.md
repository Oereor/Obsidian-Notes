## 线性空间的定义: 8 条公理

线性空间上定义了**加法**和**数乘**两种运算. *注意: 运算才是线性空间的核心; 线性空间里面含有什么类型的元素并不重要.*

公理 Axioms: 

1. $\alpha+\beta=\beta+\alpha$.

2. $(\alpha+\beta)+\gamma=\alpha+(\beta+\gamma)$.

3. 存在零向量 $\bf{0}$, 使得 $\alpha+\bf{0}=\alpha$.

4. 对每个向量 $\alpha$, 存在 $-\alpha$, 使得 $\alpha+(-\alpha)=\bf{0}$.

5. $k(\alpha+\beta)=k\alpha+k\beta$.

6. $(k+l)\alpha=k\alpha+l\alpha$.

7. $k(l\alpha)=(kl)\alpha$.

8. $1\cdot\alpha=\alpha$.

在性质 5-8 中, $k,l$ 是数域中的数.

## 线性子空间 (Subspaces)

> 为了验证某个**非空**子集是子空间, 只需验证两条性质是否满足即可. 

1. 闭合性: 对任意 $\alpha,\beta\in W$, 有 $\alpha+\beta\in W$.

2. 数乘封闭性: 对任意 $\alpha\in W$ 和数 $k$, 有 $k\alpha\in W$.

我们来证明: 若 $W$ 满足上述两条性质, 则 $W$ 是线性子空间. 事实上, 任取$\alpha\in W$, $\bf{0}=0\alpha\in W$; 对任意 $\alpha\in W$, $-\alpha=(0-1)\alpha=(-1)\alpha\in W$. 其余性质均可由线性空间的性质直接继承.
