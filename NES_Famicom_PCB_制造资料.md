# NES/Famicom 主板 PCB 制造资料

## 🎯 来源
**OpenTendo V1.4 OEM** - 开源 NES 主板项目  
GitHub: https://github.com/Redherring32/OpenTendo

## 📦 可下载的文件

### 1️⃣ 原理图 (PDF)
- **文件**: `v1.4_Schematic.pdf`
- **大小**: 821 KB
- **下载**: [点击下载原理图](https://github.com/Redherring32/OpenTendo/releases/download/V1.4/v1.4_Schematic.pdf)
- **说明**: 完整的 NES 主板原理图，包含 CPU、PPU、VRAM、WRAM 等所有电路

### 2️⃣ Gerber 文件 (PCB 制造)
- **文件**: `OpenTendo.v1.4.Gerbers_24_10_14.zip`
- **大小**: 253 KB
- **下载**: [点击下载 Gerber](https://github.com/Redherring32/OpenTendo/releases/download/V1.4/OpenTendo.v1.4.Gerbers_24_10_14.zip)
- **说明**: 工厂可直接用于 PCB 生产

### 3️⃣ 元器件清单 (BOM)
- **文件**: `BOM.csv`
- **大小**: 59 KB
- **下载**: [点击下载 BOM](https://github.com/Redherring32/OpenTendo/releases/download/V1.4/BOM.csv)
- **说明**: 所有需要的元器件列表

---

## 📏 PCB 技术规格

| 参数 | 规格 |
|------|------|
| 层数 | 2 层 |
| 尺寸 | 119mm x 196mm |
| 厚度 | 1.6mm |
| 表面处理 | HASL 或 ENIG (推荐) |
| 颜色 | 任意颜色 |

---

## ⚠️ 工厂注意事项

### 焊盘重叠说明
> "OpenTendo 有些焊盘叠加在边缘连接器上，以固定焊盘和细 traces。一些制造商可能将其视为错误并试图修复它。
> 
> **建议在订购 PCB 时注明：边缘连接器上的焊盘重叠是故意的，不是错误。**"

---

## 🔗 其他资源

- **项目主页**: https://github.com/Redherring32/OpenTendo
- **所有版本**: https://github.com/Redherring32/OpenTendo/releases
- **KiCad 源文件**: 在 GitHub 仓库中可下载 `.kicad_sch` 和 `.kicad_pcb` 文件

---

## 📝 注意事项

1. **这是开源硬件** - 遵循 TAPR Open Hardware License
2. ** licensed under the TAPR Open Hardware License ** - 你可以自由用于个人使用、出售替换板等
3. **不 affiliated with Nintendo** - 这是社区项目，与任天堂无关

---

## 🆚 你的两个 PDF 对比

| 你的 PDF | OpenTendo 对应文件 | 说明 |
|---------|-------------------|------|
| NES-CPU-01_02.pdf | v1.4_Schematic.pdf | NES CPU 主板原理图 |
| FC_HVC-CPU-05_06.pdf | - | Famicom HVC 主板 (OpenTendo 只有 NES 版本) |

**注意**: OpenTendo 项目只有 NES 主板（ FC/CPU 系列），没有 FC/HVC 主板。如果你需要 FC/HVC 主板的 PCB，可能需要寻找其他资源或反向工程。

---

## 📬 下一步操作

1. 下载 Gerber 文件 → 交给工厂生产 PCB
2. 参考 BOM.csv → 购买元器件
3. 参考原理图 → 进行组装和调试

---

*资料由 OpenClaw 自动整理，时间: 2026-03-18*
