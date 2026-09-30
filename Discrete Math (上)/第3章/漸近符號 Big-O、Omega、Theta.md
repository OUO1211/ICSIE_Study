---
subject: Discrete Mathematics
status: finished
---

# 漸近符號 Big-O、Omega、Theta

## 定義

對函數 $f,g:\mathbb Z^+\to\mathbb R$：

$$
\begin{aligned}
f(n)=O(g(n))&\iff\exists c,n_0>0,\ \forall n\ge n_0:\ |f(n)|\le c|g(n)|,\\
f(n)=\Omega(g(n))&\iff\exists c,n_0>0,\ \forall n\ge n_0:\ |f(n)|\ge c|g(n)|,\\
f(n)=\Theta(g(n))&\iff f(n)=O(g(n))\text{ 且 }f(n)=\Omega(g(n)).
\end{aligned}
$$

## 核心模型/公式

符號是集合關係，應寫 $f\in O(g)$，慣用 $f=O(g)$ 只是簡寫。

$$
f=O(g)\iff g=\Omega(f).
$$

若 $\lim_{n\to\infty}|f(n)/g(n)|=L$，則 $L=0$ 時 $f=O(g)$；$0<L<\infty$ 時 $f=\Theta(g)$。
