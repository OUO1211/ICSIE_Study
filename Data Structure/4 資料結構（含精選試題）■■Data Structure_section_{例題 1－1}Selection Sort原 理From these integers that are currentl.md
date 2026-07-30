4 資料結構（含精選試題）
■■
Data Structure

\section*{例題 1－1}

Selection Sort

原 理
From these integers that are currently unsorted，find the smallest and place it next in the sorted list．

演算法
```
for (i=1; i<n; i++) {
    /* Examine list[i] to list[n-1] and suppose that
        the smallest integer is at list[min] */
    /* Interchange list[i] and list[min] */
```


程 式
```
#include <stdio.h>
#include <math.h>
#define MAX_SIZE 101
#define SWAP(x, y, t) ((t)=(x), (x)=(y), (y)=(t))
void sort(int[ ], int); /* Selection Sort */
    void main(void)
    {
        int i, n;
        int list[MAX_SIZE];
        printf("Enter the Number of numbers to generate: ");
        scanf(%d", &n);
        if(n<1||n>MAX_SIZE) {
            fprintf(stderr, "Improper value of n\n);
            exit(1);
        }
        for(i=0; i<n; i++) { /* Randomly generate numbers*
            list[i]=rand() % 1000;
            printf("%d ", list[i]);
    }
```