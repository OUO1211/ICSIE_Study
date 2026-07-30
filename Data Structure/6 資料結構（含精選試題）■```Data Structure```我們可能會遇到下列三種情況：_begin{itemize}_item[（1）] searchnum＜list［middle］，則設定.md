6 資料結構（含精選試題）
■
```
Data Structure
```


我們可能會遇到下列三種情況：
\begin{itemize}
\item[（1）] searchnum＜list［middle］，則設定 Right 值為 middle－1
\item[（2）] searchnum＝list［middle］，則 return middle
\item[（3）] searchnum＞list［middle］，則設定 Left 值為 middle＋1
\end{itemize}

If searchnum has not been found and there are still integers to check，回（A．）再繼續。

\section*{演算法}
```
while(there are more integers to check) {
    middle = (left + right)/2;
    if(searchnum < list[middle])
        right = middle - 1;
    else if(searchnum == list[middle])
        return middle;
    else
        left = middle + 1;
}
```


\section*{程 式（Non－recursive）}
int binsearch（int list［ ］，int searchnum，int left，int right）
｛
／＊Search list［0］＜＝list［1］＜＝．．．＜＝list［n－1］
for searchnum．Return its position if found，0gherwise
```
return -1 */
int middle;
while(left <= right) {
    middle = (left + right)/2;
    switch(COMPARE(list[middle], searchnum)) {
        case -1: left = middle + 1;
            break;
        case 0: return middle;
        case 1: right = middle - 1;
            break;
    }
```