---
subject: Linear Algebra
chapter: 2
section: 2.5
status: finished
tags: [行列式, 分塊矩陣, Schur, Chapter2]
---

# Schur 補矩陣（Schur Complement）

## 定義

對分塊矩陣 $M = \begin{bmatrix} A & B \\ C & D \end{bmatrix}$，其中 $A$ 為 $m \times m$：

- 若 $A$ 可逆，**$A$ 的 Schur 補**為：$D - CA^{-1}B$
- 若 $D$ 可逆，**$D$ 的 Schur 補**為：$A - BD^{-1}C$

## 核心定理

$$\boxed{\det\begin{bmatrix} A & B \\ C & D \end{bmatrix} = \det(A) \cdot \det(D - CA^{-1}B)} \quad (A \text{ 可逆})$$

$$\boxed{\det\begin{bmatrix} A & B \\ C & D \end{bmatrix} = \det(D) \cdot \det(A - BD^{-1}C)} \quad (D \text{ 可逆})$$

## 證明

利用分塊 LU 分解（列運算消去左下角）：

$$\begin{bmatrix} A & B \\ C & D \end{bmatrix} = \underbrace{\begin{bmatrix} I_m & O \\ CA^{-1} & I_n \end{bmatrix}}_{\det=1} \begin{bmatrix} A & B \\ O & D - CA^{-1}B \end{bmatrix}$$

由[[分塊三角矩陣的行列式]]：

$$\det(M) = 1 \cdot \det(A) \cdot \det(D - CA^{-1}B)$$

## 重要推論

### 矩陣行列式引理（Matrix Determinant Lemma）

設 $A$ 為 $n \times n$ 可逆矩陣，$u, v \in F^n$：

$$\det(A + uv^T) = (1 + v^T A^{-1} u)\det(A)$$

**推導**：取 $M = \begin{bmatrix} A & u \\ -v^T & 1 \end{bmatrix}$，對 $D=1$ 用 Schur 補。

### 秩1修正公式

$$\det(I_n + uv^T) = 1 + v^T u$$

## 計算技巧

**步驟**：
1. 確認 $A$（或 $D$）可逆
2. 計算 Schur 補 $S = D - CA^{-1}B$
3. $\det(M) = \det(A) \cdot \det(S)$

**選哪塊**：選較小、較容易求逆的塊（通常是對角塊）。

## 經典考題

**例**：$M = \begin{bmatrix} 1 & 0 & 1 & 2 \\ 2 & 1 & 3 & 1 \\ 0 & 0 & 2 & 1 \\ 0 & 0 & 1 & 3 \end{bmatrix}$

取 $A = \begin{bmatrix} 1 & 0 \\ 2 & 1 \end{bmatrix}$，$\det(A) = 1$；$D = \begin{bmatrix} 2 & 1 \\ 1 & 3 \end{bmatrix}$，$C = O$

$$\det(M) = \det(A)\det(D - CA^{-1}B) = 1 \cdot \det(D) = 5$$

**例（求參數）**：若 $\det\begin{bmatrix} t \cdot I_2 & B \\ C & t \cdot I_3 \end{bmatrix} = 0$，用 Schur 補化為 $t^2 \det(tI_3 - Ct^{-1}IB) = 0$ 求 $t$。

**相關**：[[分塊三角矩陣的行列式]]、[[塊狀矩陣行列式進階]]、[[行列式進階性質]]、[[可逆矩陣]]
