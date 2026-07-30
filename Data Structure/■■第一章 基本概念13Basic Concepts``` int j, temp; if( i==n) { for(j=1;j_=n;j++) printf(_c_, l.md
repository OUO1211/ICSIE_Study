■■
第一章 基本概念
13
Basic Concepts
```
    int j, temp;
    if( i==n) {
        for(j=1;j<=n;j++) printf("%c", list[j]);
    }
    else {
        /* list[i] to list[n] has more than one permutation,
            generate these recursively */
        for( j = i; j<=n; j++)
            SWAP(list[i], list[j]);
            perm(list, i+1, n); ← recursive call
            SWAP(list[i], list[j]);
        }
    }
}
```


Time complexity ： $\mathrm{O}\left(\mathrm{n}^*(\mathrm{n}!)\right)$

\section*{例題 1－11}
［Towers of Hanoi］There are three towers and n disks of different diameters placed on the first tower．The disks are in order of decreasing diameter as one scans up the tower．Monks were repeatedly supposed to move the disk from tower A to tower C obeying the rules：
\begin{itemize}
\item[（1）] Only one disk can be moved at any time．
\item[（2）] No disk can be placed on top of a disk with a smaller diameter．
\end{itemize}

Write a recursive function that prints out the sequence of moves needed to accomplish this task．

\section*{解 課堂解}

\section*{1－3 Data Abstraction}
\begin{itemize}
\item[] －Def：A data type is a collection of objects and a set of operations that act on those objects．
\end{itemize}

而 Abstract Data Type（ADT），則定義如下：