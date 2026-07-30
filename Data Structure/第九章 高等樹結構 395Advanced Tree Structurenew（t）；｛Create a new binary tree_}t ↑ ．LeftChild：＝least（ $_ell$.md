第九章 高等樹結構 395
Advanced Tree Structure

new（t）；｛Create a new binary tree\}
t ↑ ．LeftChild：＝least（ $\ell$ ）；｛by combining the trees\}
t ↑ ．RightChild：＝Least（ $\ell$ ）；｛with the two smallest weights\}
$\mathrm{t} \uparrow$ ．weight：$=\mathrm{t} \uparrow$ ．LeftChild ↑ ．weight $+\mathrm{t} \uparrow$ ．RightChild ↑ ．weights；
insert（ $\ell, \mathrm{t}$ ）；
end；
end；｛of huffman\}

假設我們的權值為 $\mathrm{q}_1=2, \mathrm{q}_2=3, \mathrm{q}_3=5, \mathrm{q}_4=7, \mathrm{q}_5=9, \mathrm{q}_6=13$ ，那麼我們得到的樹之序列在下圖中（圖形節點內的數目代表子樹中加權外部節點的總和）。

（a）

（b）

（d）

（e）