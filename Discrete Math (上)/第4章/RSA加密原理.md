---
subject: Discrete Mathematics
status: finished
---

# RSA加密原理

## 定義

RSA 使用模同餘與大整數分解困難性建立公開金鑰系統。取相異質數 $p,q$，令 $n=pq$ 與 $\varphi(n)=(p-1)(q-1)$。

## 核心模型/公式

### 金鑰與加解密

1. 選 $e$ 使 $\gcd(e,\varphi(n))=1$。
2. 求 $d$ 使 $ed\equiv1\pmod{\varphi(n)}$。
3. 公開金鑰為 $(n,e)$；私鑰為 $d$。
4. 明文 $x$ 加密為 $y\equiv x^e\pmod n$。
5. 解密為 $x\equiv y^d\pmod n$。

正確性來自 $ed=1+k\varphi(n)$，並以[[模冪運算與歐拉費馬定理]]或中國剩餘定理證明。實務 RSA 必須使用安全填充與足夠長的金鑰；裸 RSA 不具語意安全性。
