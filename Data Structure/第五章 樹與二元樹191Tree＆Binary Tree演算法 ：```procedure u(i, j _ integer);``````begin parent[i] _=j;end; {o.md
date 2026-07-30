第五章 樹與二元樹
191
Tree＆Binary Tree

演算法 ：
```
procedure u(i, j : integer);
```

```
begin
    parent[i] :=j;
end; {of u}
```


2．找尋（Find）
作法：如果每一個樹根都有一個指標指到該集合的名稱處，那麼要決定某元素屬於那個集合，就可順著元素之父親欄找到樹根，然後就可找到集合名稱。
演算法 ：
```
function f(i : integer) : integer;
    {Find the root of the tree containing element i.}
var temp : integer;
begin
    temp : = i;
    while parent[temp]> 0 do
        temp : = parent[temp];
    f: = temp;
    end; {off}
```


5－12 利用 Inorder 、Preorder 及 Postorder 的資訊來決定唯一二元樹的探討【重要】
（一）一對中序順序（Inorder）及前序順序（Preorder），可用來決定一個唯一的二元樹。簡易證明：假設一個二元樹，是由樹根 N 及兩個子樹 $\mathrm{T}_1$ 及 $\mathrm{T}_2$ 所構成（見下圖）
依 $\mathrm{T}_1$ 和 $\mathrm{T}_2$ 是否 Empty 分成下列四種情形：