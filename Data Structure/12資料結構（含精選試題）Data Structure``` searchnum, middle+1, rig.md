12
資料結構（含精選試題）
Data Structure
```
                searchnum,
                middle+1,
                right);
        case "=": return middle;
        case ">": return binsearch(list,
                searchnum,
                left,
                middle-1);
        }
    }
    return -1;
}
```


例题1－10
Permutations（排列组合）
Give a set of $\mathrm{n} \geqq 1$ elements，print out all possible permutations of this set．
$$
\begin{array}{r}
\{a, b, c\} \text { 的 permutations } x \\
\left\{\begin{array}{r}
(a, b, c) \quad(b, c, a) \\
(a, c, b) \quad(c, a, b) \\
(b, a, c) \quad(c, b, a)
\end{array}\right.
\end{array}
$$
註：給予幾個元素，有 n！種排列组合。
如何寫出 Recursive Algorithm？
再看一個例子 $\{\mathrm{a}, \mathrm{b}, \mathrm{c}, \mathrm{d}\}$ ，則 we can construct the set of permutations by printing．
\begin{itemize}
\item[（1）] a followed by all permutations of（b，c，d）
\item[（2）] b followed by all permutations of（a，c，d）
\item[（3）] c followed by all permutations of（a，b，d）
\item[（4）] d followed by all permutations of（a，b，c）
\end{itemize}

解 演算法
$$
\begin{aligned}
& \text { void perm(char *list, int } \mathrm{i} \text {, int } \mathrm{n} \text { ) } \\
& / * \text { Generate all permutations of list }[\mathrm{i}] \text { to list }[\mathrm{n}] * /
\end{aligned}
$$