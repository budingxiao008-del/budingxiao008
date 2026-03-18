# PDF 技能正确使用方法

## 错误做法（之前）

我错误地尝试用工具的 `read` 功能直接读取 PDF 文件，这会返回二进制流，不是可读文本。

## 正确做法（参考 SKILL.md）

根据 **pdf 技能文档** (`C:\Users\Administrator\.openclaw\skills\pdf\SKILL.md`)，正确使用方法是：

### 1. 使用 pypdf 提取文本

```python
from pypdf import PdfReader

reader = PdfReader("NES-CPU-01_02.pdf")
print(f"Pages: {len(reader.pages)}")

text = ""
for page in reader.pages:
    text += page.extract_text()
    
print(text)
```

### 2. 使用 pdfplumber 提取表格

```python
import pdfplumber

with pdfplumber.open("NES-CPU-01_02.pdf") as pdf:
    for i, page in enumerate(pdf.pages):
        tables = page.extract_tables()
        for j, table in enumerate(tables):
            print(f"Table {j+1} on page {i+1}:")
            for row in table:
                print(row)
```

### 3. 高级表格提取（带 Pandas）

```python
import pdfplumber
import pandas as pd

with pdfplumber.open("NES-CPU-01_02.pdf") as pdf:
    all_tables = []
    for page in pdf.pages:
        tables = page.extract_tables()
        for table in tables:
            if table:
                # 使用第一行作为列名
                df = pd.DataFrame(table[1:], columns=table[0])
                all_tables.append(df)
```

## 已提取的文件

| 文件 | 位置 | 说明 |
|------|------|------|
| NES-CPU-01_02_extracted.txt | output/ | NES CPU 原理图文字 |
| NES_tables/page1_table1.csv | output/ | NES 表格 CSV |
| FC_HVC-CPU-05_06_extracted.txt | output/ | FC/HVC CPU 原理图文字 |
| FC_HVC_tables/*.csv | output/ | FC/HVC 表格 CSV |

## 核心要点

1. **PDF 是二进制格式** - 不能用 `read` 工具直接读取
2. **需要专门的库** - pypdf, pdfplumber
3. **参考文档** - 本地 `C:\Users\Administrator\.openclaw\skills\pdf\SKILL.md`
4. **文本保存** - 注意编码: `utf-8`

---

**之前我应该直接使用 SKILL.md 中的示例代码，而不是自己摸索！**
