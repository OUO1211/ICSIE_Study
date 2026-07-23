---
subject: Discrete Mathematics
status: finished
---

# $p \rightarrow q$ 的相關命題

## 定義

給定條件命題 $p \rightarrow q$：

1. **反命題（inverse）**：$\sim p \rightarrow \sim q$
2. **逆命題（converse）**：$q \rightarrow p$
3. **反言命題（contrapositive，又稱質位互換命題）**：$\sim q \rightarrow \sim p$

**例句**：「如果我幫她寫報告，她就跟我看電影」

| 命題 | 內容 |
|---|---|
| 原命題 | 如果我幫她寫報告，她就跟我看電影。 |
| 反命題（inverse） | 如果我不幫她寫報告，她就不跟我看電影。 |
| 逆命題（converse） | 如果她跟我看電影，我就幫她寫報告。 |
| 反言命題（contrapositive） | 如果她不跟我看電影，我就不幫她寫報告。 |

## 核心模型/公式

**【重要】**
$$p \rightarrow q \equiv \sim q \rightarrow \sim p \quad \text{（原命題恆與其反言命題等價）}$$
$$p \rightarrow q \equiv \sim p \vee q \quad \text{（Or-form）}$$【92、104台大資工】【101、107、110中興資科】【101交大資工】【110政大資科】

驗證真值表：

$$
\begin{array}{|c|c|c|c|c|c|c|}
\hline p & q & (p\to q) & (\sim p\to\sim q) & (q\to p) & (\sim q\to\sim p) & (\sim p\vee q) \\
\hline 0&0&1&1&1&1&1\\
\hline 0&1&1&0&0&1&1\\
\hline 1&0&0&1&1&0&0\\
\hline 1&1&1&1&1&1&1\\
\hline
\end{array}
$$

由表可見：$(p\to q)$、$(\sim q\to\sim p)$、$(\sim p\vee q)$ 三欄完全相同（原命題 ≡ 反言命題 ≡ Or-form）；而 $(\sim p\to\sim q)$（反命題）與 $(q\to p)$（逆命題）兩欄相同但與原命題**不同**（逆命題 ≡ 反命題，這兩者互為反言命題關係，但都不等於原命題）。

## 多選題防線 (Corner Cases)

- ⚠️ 唯一與原命題 $p\to q$ **恆等價**的變體是**反言命題（contrapositive）** $\sim q\to\sim p$；反命題（inverse）與逆命題（converse）都**不**與原命題等價（但兩者互相等價）。
- ⚠️ 名詞容易混淆：inverse＝反命題（否定 $p,q$）、converse＝逆命題（交換 $p,q$）、contrapositive＝反言命題（同時否定並交換）。考題常故意用中英夾雜混淆這三者。
- ⚠️ $p\to q \equiv \sim p\vee q$ 是把「條件句」化成「析取式（or-form）」的關鍵恆等式，是後續[[完全算子集]]與否定條件句（$\sim(p\to q)\equiv p\wedge\sim q$）推導的基礎。

# 實戰 Bug 補丁（Runtime Hotfix）
- [ ]
