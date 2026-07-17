226

離散數學（上）



3－3 鴿籠原理（The Pigeonhole Principle）



若有 $m$ 隻鸽子要放入 $n$ 個鴿籠中，且 $m>n$

則至少有一籠放了至少二隻鴿子。



【重要】



Note

又稱 Dirichlet 抽继定理或鞋箱原理（shoe box argument）。



例題 1

（ $10 \%$ ）A drawer contains 7 brown socks， 9 white socks，and 11 black socks，all unmatched．A man takes socks out at random in the dark．

（1）How many socks must he take out to be sure that he has at least two socks of the same color？

（2）How many socks must he take out to be sure that he has at least two brown socks？

【101 中正資エ】

解（1）至少取出 4 隻襪子，則由鴿籠定理知，必有 2 隻同色襪子被選中。

（2）至少取出 $9+11+2$ 隻襪子，則必有至少 2 隻棕色襪子被選中。



例題

2

（ $5 \%$ ）The population of Olympia is approximately 18,273 ．Show that at least two people in Olympia have the same initials．（Note that some people do not have middle names．）



【92、101 雲科資工】

解 First name 縮寫有 26 種（ $A-Z$ ），

middle name 縮寫有 27 種（ $A-Z$ 加上空格），

last name 縮寫有 26 種（ $A-Z$ ），

故頂多 $26 \times 27 \times 26=18252$ 種不同縮寫，故知 18273 人中必有某兩人縮寫相同。