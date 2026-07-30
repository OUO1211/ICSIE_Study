第一章 基本概念
17
Basic Concepts

\section*{例題 1－15}
```
float sum(float list[ ], int n)
{
    float tempsum=0;
    count++; /* For assignment */
    int i;
    for(i=0; i<n; i++) {
        count ++; /* For the for-loop */
        tempsum += list[i];
        count++; /* For assignment */
    }
    count++; /* Last execution of for */
    count++; /* For return */
    return tempsum;
}
```


解 $2 \mathrm{n}+3$ steps．
Count＋＋：為後來加入程式，為統計 execution steps 而用的。

\section*{例題 1－16}
```
float rsum(float list[ ], int n)
{
    count++; /* For if conditional */
    if(n) {
        count ++; /* For return and rsum invocation */
        return rsum(list, n-1)+list[n-1];
    }
    count++;
    return list[0];
}
```