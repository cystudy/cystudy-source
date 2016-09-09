---
title: Hello, 学粉们
author: 陈铮
tag: Introduction
---

欢迎来到 CyStudy **仲英学业辅导中心**！

这里有来自各个专业的数十名志愿者与工作人员热心为您服务！

# 答疑科目

下面简单介绍一下我们答疑的科目。

## 高等数学

高等数学主要研究**微积分**。

> 牛顿-莱布尼茨公式 (Newton-Leibniz formula)
>
> ——微积分基本定理

$$
\int_a^b f(x)  \mathrm{d}x = F(b) - F(a)
$$
## 线性代数

线性代数主要研究**矩阵**、**行列式**的运算与性质。

> 范德蒙德行列式 (Vandermonde determinant)

$$
V_n = 
\begin{vmatrix}
1 & x_1 & \cdots & x_1^{n-1} \\
1 & x_2 & \cdots & x_2^{n-1} \\
\vdots & \vdots & \ddots & \vdots \\
1 & x_{n} & \cdots & x_n^{n-1}
\end{vmatrix} = \prod_{1\le i \lt j \le n}{(x_i-x_j)}
$$

## 大学物理

大学物理涉及运动力学、热力学、电磁学、量子力学、狭义相对论等。

> 麦克斯韦方程组 (Maxwell equations)

$$
\begin{cases}
\nabla\cdot\vec{E} & = & \frac{\rho}{\epsilon_0} \\
\nabla\cdot\vec{B} & = & 0 \\
\nabla\times\vec{E} & = & -\frac{\partial B}{\partial t} \\
\nabla\times\vec{B} & = & \mu_0\left(\vec{J}+\epsilon_0\frac{\partial E}{\partial t} \right)
\end{cases}
$$

## 程序设计

程序设计从简单的**语言基础**到困难的**算法实现**均有涉及。

语言基础包括：

+ C
+ C++
+ Java
+ C#
+ fortran
+ JavaScript

> 埃拉托斯特尼筛法 (the Sieve of Eratosthenes)
>

```cpp
// Linear Sieve - Generating Prime Table in [1, n]
int Sieve(int n, int *prime, bool *isPrime) {
    int cnt = 0;
    isPrime[1] = false;
    memset(isPrime + 2, true, n - 2);
    for (int i = 2; i <= n; i++) {
        if (isPrime[i]) {
            prime[cnt++] = i;
        }
        for (int j = 0; j < cnt; j++) {
            int next = i * prime[j];
            if (next > n) {
                break;
            }
            isPrime[next] = false;
            if (i % prime[j] == 0) {
                break;
            }
        }
    }
    return cnt;
}
```

## 离散数学

与以微积分为代表的连续数学相对的，作为计算机科学的数学基础的离散数学：

主要涉及集合论(Set Theory)、数理逻辑(Mathematical Logic)；

延伸出关系理论(Relation Theory)、图论(Graph Theory)、代数学(Algebra)；

更进一步地包含数论(Number Theory)、组合数学(Combinatorial mathematics)、计算模型(computational model)。

> 莫比乌斯反演

$$
g(n) =\sum_{d | n}{f(d)} \Leftrightarrow f(n) = \sum_{d|n}{\mu(d)g(\frac{n}{d})}
$$

# 发行产品

目前有发行部分科目的学业小助手

+ 高数小助手
+ 线代小助手
+ 大物小助手

