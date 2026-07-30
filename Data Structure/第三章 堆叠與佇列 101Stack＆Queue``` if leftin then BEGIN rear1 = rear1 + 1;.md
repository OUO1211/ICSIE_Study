第三章 堆叠與佇列 101
Stack＆Queue
```
    if leftin then
        BEGIN
            rear1 = rear1 + 1;
            if rear1 = rear2 then queuefull;
            else q[rear1] := item;
        END;
    else
        BEGIN
            rear2 := rear2-1;
            if rear2 = rear1 then queuefull;
                else q[rear2] := item;
        END;
    END;
2. Procedure DELETE(item, leftout, q)
BEGIN
    if leftout then
        BEGIN
            if (rear1 = front1) then queueempty
                else
                    BEGIN
                        front := front1 + 1;
                        item := q[front1];
                    END;
        END;
    else
        BEGIN
            if (front2 = rear) then queuempty
                else
                    BEGIN
                        front2 := front2-1;
                        item := q[front2];
                    END;
        END;
END;
```