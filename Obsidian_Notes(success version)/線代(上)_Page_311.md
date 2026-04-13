> **例題 10**
>
> 證明下列集合為線性獨立集。
>
> (1) $\{\cos(x), 1, \sin(x)\}$ in $C[-\pi, \pi]$。 【99 成大資工、101 中央資工】
>
> (2) $\{f_1(x) = 1, f_2(x) = e^{ix}, f_3(x) = e^{-ix}\}$。 【94 暨南資工】
>
> (3) $\{e^x + e^{-x}, e^x - e^{-x}, e^{2x}\}$ in $C[0,1]$。 【95 成大資工】

**解**

(1) Wronskian $[\cos x, 1, \sin x]$

$$
= \det \begin{bmatrix}
\cos x & 1 & \sin x \\
-\sin x & 0 & \cos x \\
-\cos x & 0 & -\sin x
\end{bmatrix}
=
\begin{vmatrix}
-\sin x & \cos x \\
-\cos x & -\sin x
\end{vmatrix}
= -(\sin^2 x + \cos^2 x) = -1 \ne 0
$$

故 $\{\cos x, 1, \sin x\}$ 為獨立集。

(2) Wronskian $[1, e^{ix}, e^{-ix}]$

$$
= \det \begin{bmatrix}
1 & e^{ix} & e^{-ix} \\
0 & ie^{ix} & -ie^{-ix} \\
0 & -e^{ix} & -e^{-ix}
\end{bmatrix}
=
\det \begin{bmatrix}
ie^{ix} & -ie^{-ix} \\
-e^{ix} & -e^{-ix}
\end{bmatrix}
= -i - i \ne 0
$$

故 $\{1, e^{ix}, e^{-ix}\}$ 為線性獨立集。

(3) Wronskian $[e^x + e^{-x}, e^x - e^{-x}, e^{2x}]$

$$
= \det \begin{bmatrix}
e^x + e^{-x} & e^x - e^{-x} & e^{2x} \\
e^x - e^{-x} & e^x + e^{-x} & 2e^{2x} \\
e^x + e^{-x} & e^x - e^{-x} & 4e^{2x}
\end{bmatrix}
= 12e^{2x} \ne 0
$$

所以這個集合是線性獨立的。