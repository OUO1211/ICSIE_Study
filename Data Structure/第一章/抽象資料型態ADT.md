---
subject: Data Structure
status: finished
---

## 定義

**抽象資料型態（Abstract Data Type, ADT）**：一種資料型態，其「物件的規格（specification）」與「操作的規格（operation specification）」被刻意地與「物件的內部表示法（representation）」及「操作的實作細節（implementation）」分離開來。

換言之，ADT 只定義「做什麼（what）」，不定義「怎麼做（how）」，因此稱為 **Implementation-Independent**。

## 核心模型/公式

### Operation Specification 的組成

ADT 上每個操作的規格（spec）只包含：

1. **Function Name**（函數名稱）
2. **The type of its argument**（參數型態）
3. **The type of its result**（回傳值型態）

不包含內部表示法（internal representation）或實作細節（implementation details）。

### ADT 上 Function 的三種分類

| 分類 | 說明 |
|---|---|
| **Creator / Constructor** | 建立一個新的該型態實例（instance） |
| **Transformer** | 利用一個或多個既有實例，建立（產生）一個新的該型態實例 |
| **Observer / Reporter** | 提供關於某實例的資訊，但**不會改變**該實例本身 |

**解題技巧**：考題常給出一組操作（如 push、pop、isEmpty、top），要求判斷各操作屬於 Constructor／Transformer／Observer 哪一類——判斷依據是「是否建立新實例」與「是否修改既有實例」。
