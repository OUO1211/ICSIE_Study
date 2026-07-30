第一章 基本概念 23
Basic Concepts

\section*{例題 1－23}

For $\mathrm{i}=1$ to n do
For $\mathrm{j}=1$ to i do
For $\mathrm{k}=1$ to j do
$\mathrm{x}=\mathrm{x}+1 ;$
end；
end；
end．
$\mathrm{x}=\mathrm{x}+1$ 之執行次數為？
解 $\frac{\mathrm{n}(\mathrm{n}+1)(\mathrm{n}+2)}{6}$ 次

\section*{例題 1－24}

For $\mathrm{k}=1$ to n do
For $\mathrm{i}=1$ to k do
For $\mathrm{j}=1$ to k do
if $(\mathrm{i} \neq \mathrm{j})$ then $\mathrm{x}=\mathrm{x}+1$
end；
end；
end．
求 $\mathrm{x}=\mathrm{x}+1$ 之執行次數？
解 Hint：$k^2-(i=j$ 之次數），$k=1$ to n

\section*{例題 1－25}
i＝n；
while（ $\mathrm{i} \geq 1$ ）do
begin
$\mathrm{x}=\mathrm{x}+1 ;$
$\mathrm{i}=\mathrm{i} / 2 ;$
end；
求 $\mathrm{x}=\mathrm{x}+1$ 之 Time Complexity $=\mathrm{O}(?)$

解 $\mathrm{O}(\log \mathrm{n})$