484
離散數學（上）

Show hand（梭哈）
例題 7
A poker hand is a set of 5 cards from a 52 －card deck of cards．Count the number of poker hands for each set from（1）to（11）．
（1）Royal flush： $10, J, Q, K, A$ all in the same suit．
（2）Straight flush：A straight all in the same suit that is not a royal flush．
（3）Four of a hand：Four cards in the hand have the same value．
（4）Full house：three cards of one value and two cards of another value．
【87交大資科】【96暨南資工】【100台南数位】
（5）Flush：five cards all in the same suit，but not a royal or straight flush．
【96暨南資工】
（6）Straight：A straight that is not a royal or straight flush．
（7）Three of a kind：Three cards of one value，a fourth card of a second value and a fifth card of a third value．

【96暨南資エ】
（8）Two pairs：Two cards of one value，two more cards of a second value and the remaining card a third value．

【96暨南資工】【102成大電通】
（9）One pair：two cards of one value，but not classified above．
（10）None：none of the above．
（11）At least one diamond．
【101 東華資工類題】
解（1） 4 ．
因為固定是 $A, K, Q, J, 10$ ，但有四種花色變化。
（2） $4 \times 9$ ．
因為順：A2345、23456、．．．、910JQK 共 9 種且有四種花色變化。
（3）$\binom{13}{1}\binom{12}{1}\binom{4}{1}$ ．
那四張相同的數字有 $\binom{13}{1}$ 種決定方式，剩下的那張有 $\binom{12}{1}\binom{4}{1}$ 種決定方式，
（4）$\binom{13}{1}\binom{4}{3}\binom{12}{1}\binom{4}{2}$ ．
那三張相同的數字有 $\binom{13}{1}$ 種決定方式，花色變化有 $\binom{4}{3}$ 種決定方式，
那兩張相同的數字有 $\binom{12}{1}$ 種決定方式，花色變化有 $\binom{4}{2}$ 種決定方式。