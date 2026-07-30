第四章 鏈結串列 129
Linked List

\section*{例題 4－1}

建立一個含有二個 Node 的 Linked List，如下：

First 是一個指向第一個節點的指標（Pointer）
【程式】 BEGIN
New（First）；New（Second）；
First ↑ ．Link：＝Second；
Second ↑ ．Link＝Nil；
First ↑ ．Data：$=10$ ；
Second ↑ ．Data：$=20$ ；
END

\section*{例題 4－2}

Linked List 的插入。
假設 First 是一個指向键結串列的指標，如果串列是空白的，則 First = Nil，令 x 是一個指向串列中任意節點的指標。插入一個資料欄為50的節點在 x 所指的節點後面。
【程式】 procedure insert（var first：pointer；x：pointer）；
```
BEGIN
    new(t); {Get a new node}
    t ↑ .data : = 50; { Set its data field }
    if first = nill
        then BEGIN { Insert into empty list }
            first : = t;
            t ↑ .link : = nil;
        END;
        else BEGIN { Insert after x }
            t ↑ .link : = x ↑ .link;
            x ↑ .link : = t;
        END;
    END; { of insert }
```