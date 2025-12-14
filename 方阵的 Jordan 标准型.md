### Jordan 块

形如如下形式的 $n_i\ (n_i\geq 1)$ 阶方阵称为一个 Jordan 块: $$J_i=\begin{bmatrix}\lambda_i & 1 & 0 & \cdots & 0 \\ 0 & \lambda_i & 1 & \cdots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \cdots & 1 \\ 0 & 0 & 0 & \cdots & \lambda_i\end{bmatrix}.$$ 
Jordan 块有如下的性质 (此处设对角线上的元素为 $\lambda_0$): 
1. $|\lambda E-J|=(\lambda-\lambda_0)^n$. 
2. $(\lambda_0 E-J)$ 是一个幂零指数为 $n$ 的幂零矩阵, 即 $(\lambda_0 E-J)^n=O$, 但 $(\lambda_0 E-J)^{n-1}\neq O$.
3. $$r(J)=\begin{cases}
n-1, & \lambda_0\neq 0 \\ 
n, & \lambda_0=0
\end{cases}.$$
4. 若 $\lambda_0=0$, 则 $r(J^k)=n-k$, $1\leq k\leq n$. 
5. 对角线上元素不同的 Jordan 块不相似. 

### Jordan 标准型

由若干个 Jordan 块构成的分块对角矩阵 $$J=\begin{bmatrix}J_1 & O & \cdots & O \\ O & J_2 & \cdots & O \\ \vdots & \vdots & \ddots & \vdots \\ O & O & \cdots & J_n\end{bmatrix}$$ 称为 Jordan 标准型.

> **Jordan 标准型定理.** 在 $\mathbb{C}$ 上, 任意一个 $n$ 阶方阵 $A$ 都相似于某个 Jordan 标准型矩阵 $J$. 如果不考虑各个 Jordan 块的次序, 那么该矩阵 $J$ 是唯一的.

我们略去此定理的证明. 

### 如何求 Jordan 标准型

我们先来考察幂零矩阵的 Jordan 标准型. 设 $A$ 是一个 $n$ 阶幂零矩阵, 幂零指数为 $k$, 那么: 
1. $A$ 的 Jordan 标准型中 Jordan 块的对角元均为 $0$, 最大阶数为 $k$. 
2. 特征值 $0$ 的几何重数 $n-r(A)$ 等于标准型中 Jordan 块的个数. 

> **证明.** 设 $A=P^{-1}JP$, $A^k=O$, 则 $J^k=O$, 即每个 $J_i^k=O$, 因此每个 Jordan 块的对角元必定为 $0$, 且阶数均不大于 $k$. 另外, 由 $r(A)=r(J)$ 可知, $$r(A)=\sum_i r(J_i)=\sum_i (n_i-1)=n-m,$$ 其中 $m$ 是 Jordan 块的个数, $n_i$ 是第 $i$ 个 Jordan 块的阶数. 因此, $m=n-r(A)$.

现在考察一般矩阵 $A$ 的 Jordan 标准型. 设 $\lambda$ 为 $A$ 的一个特征值, 那么 $n-r(\lambda E-A)$ (即 $\lambda$ 的几何重数) 等于 Jordan 标准型中对角元为 $\lambda$ 的 Jordan 块的个数. 

事实上, 还可以进一步推广. 记 $\eta_k=n-r((\lambda E-A)^k)$, Jordan 标准型中对角元为 $\lambda$ 的 $k$ 阶 Jordan 块的个数为 $l_k$, 则有 $l_k=2\eta_k-\eta_{k-1}+\eta_{k+1}$. 特别地, $k=1$ 时 $l_1=2\eta_1-\eta_2$. 