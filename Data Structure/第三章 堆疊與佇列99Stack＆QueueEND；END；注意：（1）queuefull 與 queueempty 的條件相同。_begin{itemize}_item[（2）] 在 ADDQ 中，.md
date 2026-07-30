第三章 堆疊與佇列
99
Stack＆Queue

END；
END；
注意：（1）queuefull 與 queueempty 的條件相同。
\begin{itemize}
\item[（2）] 在 ADDQ 中，當 front＝rear 時，事實上還有一個空位置，即：q［rear］。
\item[（3）] 若使用了這個空間，則我們無法判斷到底是 queueempty 或 queuefull。
\item[（4）] 因此，在 Circular queue $[0 \cdots n-1]$ ，雖有 $n$ 個空間，但最多只允許存 n－1 個元素。
\item[（5）] 插入／刪除之 Time Complexity 為 O（1）常數
\end{itemize}

【方法 3】若要使用此空間，則需另設一個變數 tag 來協助區分 Full 與 Empty 狀況。
$$
\begin{array}{ll}
\mathrm{tag}=0 & \rightarrow \text { 空的(Empty) } \\
\mathrm{tag}=1 & \rightarrow \text { 滿的(Full) }
\end{array}
$$

演算法如下：（ $\operatorname{tag}$ 初值為： 0 ）
```
Procedure ADDQ(item)
    BEGIN
        if (front=rear and tag=1) then queuefull;
            else
                BEGIN
                    rear := (rear + 1) mod n;
                    q[rear] := item;
                    if front = rear then tag := 1;
                END;
    END;
Procedure Delete(q)
    BEGIN
        if (rear=front and tag=0) then queueempty;
            else
                BEGIN
                    front := (front + 1) mod n;
                    item := q[front];
                    if front = rear then tag= ; \
                END;
    END;
```