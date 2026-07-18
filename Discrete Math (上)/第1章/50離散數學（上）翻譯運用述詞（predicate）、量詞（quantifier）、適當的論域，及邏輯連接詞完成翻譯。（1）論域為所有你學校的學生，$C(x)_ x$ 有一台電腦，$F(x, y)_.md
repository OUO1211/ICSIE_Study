50

離散數學（上）



翻譯

運用述詞（predicate）、量詞（quantifier）、適當的論域，及邏輯連接詞完成翻譯。

（1）論域為所有你學校的學生，$C(x): x$ 有一台電腦，$F(x, y): x$ 和 $y$ 是朋友，則 $\forall x[C(x) \vee \exists y(C(y) \wedge F(x, y))]$

譯成一般語言就是：＂你學校的每一個學生，都有電腦或有一個有電腦的朋友＂。

（2）論域為所有你學校的學生，$F(x, y): x$ 和 $y$ 是朋友，則

$\exists x \forall y \forall z([F(x, y) \wedge F(x, z) \wedge y \neq z] \rightarrow \neg F(y, z))$

譯成一般語言就是：＂存在有你學校的學生（那個 $x$ ），他（就是 $x$ ）的朋友之間都不是朋友＂。

（3）＂任兩個正整數的和為正＂，

邏輯式為：$\forall x \forall y[(x>0) \wedge(y>0)] \rightarrow(x+y>0)$.



【95中興資科】



（4）＂除了 0 ，每個實數都有乘法反元素＂，

邏輯式為：$\forall x[(x \neq 0) \rightarrow \exists y(x y=1)]$.



【95中興資科】



（5）＂如果有一個人是女性，且又是為人父母，那麼她一定是某人的媽媽＂，

邏輯式為：$\forall x[F(x) \wedge P(x) \rightarrow \exists y M(x, y)]$ ，

其中，$F(x): x$ 是女性，$P(x): x$ 是為人父母，$M(x, y): x$ 是 $y$ 的媽媽。

（6）＂Every student in this class has studied Discrete Mathematics＂•

令 $S(x): x$ 有修過離散，$I(x): x$ 在這班上，

論域為 all students in the class 時，邏輯式為 $\forall x S(x)$ 。

論域為 all students in the school 邏輯式為 $\forall x(I(x) \rightarrow S(x))$ 。

【100、102 中興資科】

（7）True or false：Suppose that the domain consists of all creatures，and let $P(x)$ and $Q(x)$ be the propositional function＂$x$ is a cat＂and＂$x$ is cute＂，respectively．The sentence＂every cat is cute＂ can be translated as $\forall x(P(x) \wedge Q(x))$ ．



【111台科資工】

解 False．

那個寫法會翻譯成任何動物都是貓且可愛的。正確寫法應該是 $\forall x(P(x) \rightarrow Q(x))$