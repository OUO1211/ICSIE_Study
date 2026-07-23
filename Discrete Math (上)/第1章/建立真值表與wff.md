---
subject: Discrete Mathematics
status: finished
---

# 建立真值表與 wff（合式公式）

## 定義

- **永真式（tautology）**：命題中各變數不論代入任何值，恆得 true。又稱真理、定理（theorem）、同義複詞、重言式。
- **永假式（contradiction）**：命題中各變數不論代入任何值，恆得 false。又稱矛盾式。
- **合式公式（well-formed formula, wff）**：依下列規則生成的公式：
  1. 單獨的命題變數是一個 wff。
  2. 若 $P$ 為 wff，則 $\sim P$ 亦為 wff。
  3. 若 $P$ 與 $Q$ 為 wff，則 $P \wedge Q$、$P \vee Q$、$P \rightarrow Q$、$P \leftrightarrow Q$ 亦為 wff。
  4. 經有限次使用規則 (1)(2)(3) 而得之字串亦為 wff。

## 核心模型/公式

### 連接詞運算優先順序

$$\sim \;>\; \wedge \;>\; \vee \;>\; \rightarrow \;>\; \leftrightarrow$$

即：① $\sim$、② $\wedge$、③ $\vee$、④ $\rightarrow$、⑤ $\leftrightarrow$。【101 中興資科】

### 建立真值表的兩種策略

給定含 $n$ 個變數的公式，真值表需列出 $2^n$ 列。除逐列展開外，亦可用**反例分析法**：假設結論為假，反推各前提須滿足的條件，若導出矛盾則公式為永真式。

## 經典考題

**例題【105台科資工】** 請判別 $[(p \vee r) \wedge(p \rightarrow q) \wedge(r \rightarrow q)] \rightarrow q$ 的真假。

**解法一：真值表法**

$$
\begin{array}{|c|c|c|c|c|}
\hline p & q & r & (p\vee r)\wedge(p\to q)\wedge(r\to q) & [\cdots]\to q \\
\hline 0 & 0 & 0 & 0 & 1 \\
\hline 0 & 0 & 1 & 0 & 1 \\
\hline 0 & 1 & 0 & 0 & 1 \\
\hline 0 & 1 & 1 & 1 & 1 \\
\hline 1 & 0 & 0 & 0 & 1 \\
\hline 1 & 0 & 1 & 0 & 1 \\
\hline 1 & 1 & 0 & 1 & 1 \\
\hline 1 & 1 & 1 & 1 & 1 \\
\hline
\end{array}
$$

最右欄恆為 1，故此式為**永真式（tautology）**。

**解法二：反例分析法（較快）**

若存在反例，須使 $q=0$。為使前提 $p \rightarrow q$ 與 $r \rightarrow q$ 皆為真（$q=0$ 時，唯有 $p=0, r=0$ 才能使 $p\to q$、$r\to q$ 為真），故須 $p=0, r=0$。但此時 $(p \vee r) = 0$，使整個括號 $[(p \vee r) \wedge(p \rightarrow q) \wedge(r \rightarrow q)]$ 必為假，矛盾（前提假時 $\to q$ 本身即真，不構成反例）。故不存在反例，原式為永真式。

## 多選題防線 (Corner Cases)

- ⚠️ 運算優先順序常考選擇題：括號 > $\sim$ > $\wedge$ > $\vee$ > $\rightarrow$ > $\leftrightarrow$，缺一個等級都會判錯結合方式。
- ⚠️ 「反例分析法」的核心技巧：先假設結論為假，反推每個前提「必須」的真值，若推出矛盾（某個子式無法同時滿足），代表該反例不存在 ⇒ 公式為永真式。此法在變數數 $\geq 4$ 時比硬列真值表快很多。
- ⚠️ wff 規則是**歸納定義**（inductive definition），單一命題變數本身就是最小的 wff，不能漏掉規則 (1)。

# 實戰 Bug 補丁（Runtime Hotfix）
- [ ]
