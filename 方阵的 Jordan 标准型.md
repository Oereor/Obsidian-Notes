### Jordan 块

形如如下形式的 $n_i$ 阶方阵称为一个 Jordan 块: $$J_i=\begin{bmatrix}\lambda_i & 1 & 0 & \cdots & 0 \\ 0 & \lambda_i & 1 & \cdots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \cdots & 1 \\ 0 & 0 & 0 & \cdots & \lambda_i\end{bmatrix}.$$

Jordan 块有如下的性质 (此处设对角线上的元素为 $\lambda_0$): 
1. $|\lambda E-J|=(\lambda-\lambda_0)^n$. 
2. $(\lambda_0 E-J)$ 是一个幂零指数为 $n$ 的幂零矩阵, 即 $(\lambda_0 E-J)^n=0$, 但 $(\lambda_0 E-J)^{n-1}\neq 0$.
3. $$r(J)=\begin{cases}
n-1, & \lambda_0\neq 0 \\ 
n, & \lambda_0=0
\end{cases}.$$
4. $r(J^k)=n-k$, $1\leq k\leq n$. 
5. 对角线上元素不同的 Jordan 块不相似. 