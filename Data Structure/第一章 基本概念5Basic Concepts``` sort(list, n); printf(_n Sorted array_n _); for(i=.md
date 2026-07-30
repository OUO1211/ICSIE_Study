第一章 基本概念
5
Basic Concepts
```
        sort(list, n);
        printf("\n Sorted array:\n ");
        for(i=0; i<n; i++) printf("%d ", list[i]);
                /* Print out sorted numbers */
        printf("\n");
    }
    void sort(int list[ ], int n)
    {
        int i, j, min, temp;
        for(i=0; i<n-1; i++) {
            min=i;
            for(j=i+1; j<n-1;j++)
                if(list[j] < list[min])
                    min=j;
            SWAP(list[i], list[min], temp);
        }
    }
/* Program End */
```


\section*{例題 1－2}

Binary Search
假設有 n 個不同的整数，已被排序完成，且放在 list 陣列中，即
$$
\operatorname{list}[0] \leqq \operatorname{list}[1] \leqq \cdots \leqq \operatorname{list}[n-1]
$$
設 要尋找的數字為 searchnum
如果在 list 中找到，則 return an index I
否則 return－1。

\section*{作 法}

令 Left、Right 表示 list 的左、右兩端。
而初值分別為 Left＝ 0
$$
\text { Right }=n-1
$$
A．且令 middle $=($ Left + Right $) / 2$ ，此時 compare searchnum 和 list［middle］。