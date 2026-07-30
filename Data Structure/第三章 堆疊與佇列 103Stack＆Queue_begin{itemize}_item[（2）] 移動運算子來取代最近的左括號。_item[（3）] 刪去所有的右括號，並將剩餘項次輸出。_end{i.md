第三章 堆疊與佇列 103
Stack＆Queue
\begin{itemize}
\item[（2）] 移動運算子來取代最近的左括號。
\item[（3）] 刪去所有的右括號，並將剩餘項次輸出。
\end{itemize}

補充：中序（infix⋯ LDR）轉後序（postfix，LRD），前序（prefix，DLR）的另一種方法：（ch5 討論）
\begin{itemize}
\item[（1）] 建二元樹。
\item[（2）] 利用 Preorder traversal 以及 Postorder traversal。
\end{itemize}

\section*{二．infix 轉 postfix 的 algorithm（利用 stack ）}

Procedure postfix（e：expression）；
｛ Output the postfix form of the infix expression e．
NextToken is used to get next item of e．It is assumed that the last token in e is＇＃＇．
Also，＇＃＇is used at the bottom of the stack．\}
```
var x, y:token;
BEGIN
    stack[1] := '#';
    top := 1; {initialize stack}
    x := NextToken(e);
    while x<> '#' do
        BEGIN
        if x is an operand then write(x)
                else if x= ')' then
            BEGIN
                while stack[top] <> '(' do
                BEGIN
                    pop(y);
                    write(y);
                END;
                pop(y); {pop '(', 但不輸出'(' }
            END;
        else
            BEGIN
            while isp[satck[top]] <= icp[x] (即外面 token 的優先權小於等於
            stack Top 端的優先權) do
```