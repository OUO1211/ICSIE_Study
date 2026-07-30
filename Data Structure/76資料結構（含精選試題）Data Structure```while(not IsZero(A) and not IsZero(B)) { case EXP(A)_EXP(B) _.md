76
資料結構（含精選試題）

Data Structure
```
while(not IsZero(A) and not IsZero(B)) {
    case EXP(A)<EXP(B) :
        C= Insert(C, COEF(B), EXP(B));
        B= RED(B); //下一個項次 of B//
    case EXP(A) = EXP(B) :
        C = Insert(C, COEF(A)+COEF(B), EXP(A));
        A = RED(A);
        B = RED(B);
    case EXP(A)>EXP(B) :
        C = Insert(C, COEF(A), EXP(A));
        A= RED(A);
}
while(A 中還有剩餘的項次) {
    C = Insert(C, COEF(A), EXP(A));
    A = RED(A);
}
    while(B 中還有剩餘的項次) {
    C = Insert(C, COEF(B), EXP(B));
    B=RED(B);
}
}
```


\section*{例題 2－12}

有兩個變數之多項式：
$$
A(x, y)=7 x^4+5 x^4 y^3+6 x^3 y^2-8 x^2 y+9 x y+8
$$
應用怎樣的陣列來表之？

\section*{解}

其餘為 $\phi$