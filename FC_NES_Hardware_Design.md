# FC/NES 硬件设计资源大全

_原理图、PCB、FPGA 核心、开发者资源_

_最后更新：2026-03-24_

---

## 📐 官方硬件设计资料

### 1. NES 官方维修手册（Nintendo Service Manual）
- **URL**: https://www.nesdev.org/nsm.htm
- **类型**: 官方维修手册
- **说明**: 任天堂官方 NES 维修手册，包含完整原理图
- **内容**:
  - 完整系统原理图
  - PCB 布局图
  - 芯片引脚定义
  - 电压测试点
  - 故障排除指南
- **版本**: NES-001 (前插式)

### 2. Famicom 官方维修手册
- **URL**: https://www.nesdev.org/famicom_schematics.htm
- **类型**: 官方维修手册
- **说明**: 任天堂官方 FC 维修手册（日文版）
- **内容**:
  - FC 原理图
  - 控制器电路
  - RF 调制器电路
  - 音频/视频输出电路

### 3. Nintendo CIC 芯片文档
- **URL**: https://www.nesdev.org/cic.htm
- **类型**: 技术文档
- **说明**: NES 锁区芯片（CIC）逆向工程文档
- **内容**: CIC 芯片原理、破解方法、绕过电路

---

## 🔍 逆向工程与原理图

### 4. NES Schematics（完整原理图）
- **URL**: https://www.nesdev.org/schematics.htm
- **类型**: 原理图集合
- **说明**: 社区整理的完整 NES 原理图（PDF 格式）
- **包含**:
  - CPU (2A03) 电路
  - PPU (2C02) 电路
  - 内存映射
  - 控制器端口
  - 卡带接口（72 针）
  - 电源电路
  - 视频/音频输出

### 5. Famicom Schematics（FC 原理图）
- **URL**: https://www.nesdev.org/famicom.htm
- **类型**: 原理图
- **说明**: FC 日版主机的完整原理图
- **特点**: 60 针卡带接口、内置麦克风电路

### 6. NES-101 Top Loader Schematics
- **URL**: https://www.nesdev.org/nes-101.htm
- **类型**: 原理图
- **说明**: NES 后期顶插版（NES-101）原理图
- **特点**: 简化设计、无 CIC 锁区芯片

### 7. AV Famicom Schematics
- **URL**: https://www.nesdev.org/av-famicom.htm
- **类型**: 原理图
- **说明**: FC 后期 AV 输出版原理图
- **特点**: 改进的视频输出电路、更好的画质

---

## 💻 FPGA 核心（MiSTer 等）

### 8. MiSTer NES Core（官方）
- **URL**: https://github.com/MiSTer-devel/NES_MiSTer
- **类型**: FPGA 核心源码
- **开发者**: MiSTer 社区
- **说明**: MiSTer FPGA 的 NES 核心
- **内容**:
  - Verilog 源码
  - PPU 模拟
  - APU 模拟
  - Mapper 支持列表
  - 编译脚本

### 9. MiSTer Famicom Core
- **URL**: https://github.com/MiSTer-devel/Famicom_MiSTer
- **类型**: FPGA 核心源码
- **开发者**: MiSTer 社区
- **说明**: 日版 FC 专用核心（支持 Famicom 特性）
- **特点**: 支持 FC 磁盘机、麦克风

### 10. Analogue Nt Mini Jailbreak（FPGA）
- **URL**: https://github.com/analogueco/njt-minimal
- **类型**: FPGA 核心
- **开发者**: Analogue
- **说明**: Analogue Nt Mini 的 FPGA 实现（部分开源）

### 11. Turbo Chameleon 64 - NES Core
- **URL**: https://github.com/Thom-Bliss/TurboChameleon64
- **类型**: FPGA 核心
- **开发者**: Thom Blisse
- **说明**: 适用于 Chameleon 的 NES 核心

### 12. MiST NES Core（旧版）
- **URL**: https://github.com/mist-devel/nes-mist
- **类型**: FPGA 核心
- **开发者**: MiST 社区
- **说明**: 早期 MiST 平台的 NES 核心（Cyclone III）

---

## 🔬 CPU/PPU 芯片级逆向

### 13. Visual 2A03（CPU 介视图）
- **URL**: https://visual6502.org/wiki/index.php?title=NES
- **类型**: 芯片介视
- **说明**: 2A03 CPU 的晶体管级逆向工程
- **内容**:
  - 晶体管级电路图
  - 数据流可视化
  - 指令执行动画
  - 交互式模拟器

### 14. Visual 2C02（PPU 介视图）
- **URL**: https://visual6502.org/wiki/index.php?title=PPU
- **类型**: 芯片介视
- **说明**: 2C02 PPU 的晶体管级逆向工程
- **内容**:
  - 像素渲染流程
  - 精灵优先级逻辑
  - 滚动寄存器
  - 可视化调试

### 15. 6502 处理器文档
- **URL**: https://www.nesdev.org/6502.htm
- **类型**: 处理器文档
- **说明**: 6502 CPU 的详细技术文档
- **内容**:
  - 指令集详解
  - 时序图
  - 寻址模式
  - 中断处理

### 16. PPU 技术文档
- **URL**: https://www.nesdev.org/ppu.htm
- **类型**: 处理器文档
- **说明**: 2C02 PPU 的完整技术规格
- **内容**:
  - 内存映射
  - 寄存器详解
  - 渲染时序
  - 精灵评估

---

## 🛠️ PCB 设计与改装

### 17. NESRGB PCB 设计
- **URL**: https://github.com/ArtemioUW/NESRGB
- **类型**: PCB 设计
- **开发者**: Artemio
- **说明**: NES RGB 输出改装 PCB
- **内容**:
  - KiCad 设计文件
  - 原理图
  - PCB 布局
  - 安装指南
  - BOM 清单

### 18. NES Top Loader RGB
- **URL**: https://github.com/ArtemioUW/NES-Top-Loader-RGB
- **类型**: PCB 设计
- **开发者**: Artemio
- **说明**: NES-101 顶插版 RGB 改装
- **特点**: 无损安装、高质量视频输出

### 19. Famicom RGB PCB
- **URL**: https://github.com/ArtemioUW/Famicom-RGB
- **类型**: PCB 设计
- **开发者**: Artemio
- **说明**: FC 日版 RGB 输出改装
- **内容**: 完整 KiCad 项目文件

### 20. NES DAC（数字音频转换）
- **URL**: https://github.com/ArtemioUW/NES-DAC
- **类型**: PCB 设计
- **开发者**: Artemio
- **说明**: NES 音频输出改进方案
- **特点**: 降低噪声、提升音质

### 21. RetroUSB NES PCB
- **URL**: https://retrousb.com/product_info.php?products_id=66
- **类型**: 商业 PCB
- **开发者**: RetroUSB
- **说明**: 商业版 NES RGB 改装套件
- **特点**: 成品 PCB、附带安装说明

---

## 🎮 烧录卡与复刻卡带

### 22. EverDrive N8（烧录卡）
- **URL**: https://krikzz.com/store/home/35-everdrive-n8-nes.html
- **类型**: 商业产品
- **开发者**: Krikzz
- **说明**: 最流行的 NES 烧录卡
- **特点**:
  - 支持所有 mapper
  - SD 卡存储
  - FPGA 配置
  - 实时保存

### 23. EverDrive N8 Pro
- **URL**: https://krikzz.com/store/home/48-everdrive-n8-pro-nes.html
- **类型**: 商业产品
- **开发者**: Krikzz
- **说明**: EverDrive N8 升级版
- **新增**: WiFi 联机、USB 烧录、更多功能

### 24. PowerPak PCB 分析
- **URL**: https://www.nesdev.org/powerpak.htm
- **类型**: 技术分析
- **说明**: PowerPak 烧录卡的电路分析
- **内容**: 原理图逆向、FPGA 配置

### 25. Flash Carts Comparison
- **URL**: https://www.nesdev.org/flashcarts.htm
- **类型**: 对比文档
- **说明**: 各款 NES 烧录卡对比
- **内容**: 兼容性、价格、功能对比

---

## 👨‍💻 核心开发者 GitHub

### 26. SourMesen（Mesen 模拟器作者）
- **URL**: https://github.com/SourMesen
- **类型**: 开发者主页
- **说明**: Mesen 高精度模拟器作者
- **项目**:
  - https://github.com/SourMesen/Mesen2 - Mesen2 模拟器
  - https://github.com/SourMesen/Mesen - 旧版 Mesen

### 27. Bazzan（ASMotor 作者）
- **URL**: https://github.com/brocator
- **类型**: 开发者主页
- **说明**: ASMotor 汇编器开发者
- **项目**: https://github.com/brocator/asmotor

### 28. Tepples（NES 开发者）
- **URL**: https://github.com/tepples
- **类型**: 开发者主页
- **说明**: 资深 NES 开发者，多个工具作者
- **项目**:
  - https://github.com/tepples/ppuview - PPU 查看器
  - https://github.com/tepples/libnes - NES 库
  - 多个 NES 自制游戏

### 29. Kevin Horton（Krikzz）
- **URL**: https://github.com/krikzz
- **类型**: 开发者主页
- **说明**: EverDrive 烧录卡作者
- **项目**:
  - https://github.com/krikzz/ED64 - N64 EverDrive
  - 烧录卡固件源码

### 30. Artemio（硬件改装专家）
- **URL**: https://github.com/ArtemioUW
- **类型**: 开发者主页
- **说明**: NES/FC 硬件改装、测试卡带开发者
- **项目**:
  - https://github.com/ArtemioUW/NESRGB - RGB 改装
  - https://github.com/ArtemioUW/240p-test-suite - 240p 测试套件
  - https://github.com/ArtemioUW/Famicom-RGB - FC RGB 改装

### 31. Quietust（NES 音频专家）
- **URL**: https://github.com/quietust
- **类型**: 开发者主页
- **说明**: NES 音频处理、模拟器核心开发者
- **项目**: 多个 NES 音频相关项目

### 32. Rainwarrior（NES 工具开发者）
- **URL**: https://github.com/rainwarrior
- **类型**: 开发者主页
- **说明**: NES 音乐、图形工具开发者
- **项目**: 多个 NES 开发工具

### 33. Shiru（NES 游戏开发者）
- **URL**: https://github.com/shiru86
- **类型**: 开发者主页
- **说明**: NES 自制游戏开发者
- **项目**: 多个 NES 游戏源码

### 34. Doug Fraker（NES 工具作者）
- **URL**: https://github.com/dougfraker
- **类型**: 开发者主页
- **说明**: NES 图形工具、教程作者
- **项目**:
  - https://github.com/dougfraker/NES-Maker - NESMaker 工具
  - 多个 NES 开发教程

### 35. GradualGames（NES 开发者）
- **URL**: https://github.com/GradualGames
- **类型**: 开发者主页
- **说明**: NES 游戏开发工具作者
- **项目**: https://github.com/GradualGames/GBDK - Game Boy 开发套件

---

## 📊 完整硬件规格文档

### 36. NES Hardware Specification
- **URL**: https://www.nesdev.org/hardware.htm
- **类型**: 硬件规格
- **说明**: NES 完整硬件规格文档
- **内容**:
  - CPU/PPU/APU 详细规格
  - 内存映射图
  - I/O 端口
  - 中断系统
  - DMA 传输

### 37. Controller Protocol
- **URL**: https://www.nesdev.org/controllers.htm
- **类型**: 协议文档
- **说明**: NES 手柄通信协议
- **内容**:
  - 串行通信时序
  - 数据格式
  - 扩展端口（4 人适配器）

### 38. Cartridge Connector Pinout
- **URL**: https://www.nesdev.org/cartridge.htm
- **类型**: 接口文档
- **说明**: NES 卡带接口引脚定义
- **内容**:
  - 72 针引脚定义（NES）
  - 60 针引脚定义（FC）
  - 信号说明

### 39. Mapper 文档
- **URL**: https://www.nesdev.org/mappers.htm
- **类型**: 技术文档
- **说明**: NES 卡带 mapper 规格大全
- **内容**:
  - 所有 mapper 编号（0-255+）
  - 每个 mapper 的寄存器映射
  - 使用 mapper 的游戏列表
  - 电路实现示例

---

## 🎯 测试与调试工具

### 40. NES Test ROMs
- **URL**: https://github.com/ChrisK2003/NES-Test-ROMs
- **类型**: 测试程序
- **说明**: NES 硬件测试 ROM 合集
- **内容**:
  - CPU 指令测试
  - PPU 渲染测试
  - APU 音频测试
  - 控制器测试

### 41. 240p Test Suite
- **URL**: https://github.com/ArtemioUW/240p-test-suite
- **类型**: 测试程序
- **说明**: 240p 视频输出测试套件
- **用途**: 测试 NES/FC 视频输出质量
- **支持**: NES、FC、SNES、MD 等

### 42. Nestest ROM
- **URL**: https://www.nesdev.org/nestest.htm
- **类型**: 测试程序
- **说明**: CPU 指令测试 ROM
- **用途**: 验证模拟器 CPU 模拟准确性
- **输出**: 详细的 CPU 执行日志

### 43. Blargg's Test ROMs
- **URL**: https://github.com/SingleStepTests/blargg-nes-tests
- **类型**: 测试程序
- **说明**: 经典 NES 硬件测试 ROM 合集
- **测试内容**:
  - CPU 指令
  - 时序
  - 中断
  - PPU 特性

---

## 📐 PCB 设计软件资源

### 44. KiCad（推荐 PCB 设计软件）
- **URL**: https://www.kicad.org/
- **类型**: PCB 设计软件
- **说明**: 开源 PCB 设计软件，用于 NES 改装设计
- **特点**: 免费、开源、功能强大

### 45. Eagle（PCB 设计）
- **URL**: https://www.autodesk.com/products/eagle/overview
- **类型**: PCB 设计软件
- **说明**: Autodesk Eagle，部分 NES 改装使用
- **特点**: 商业软件、学生版免费

### 46. EasyEDA（在线 PCB 设计）
- **URL**: https://easyeda.com/
- **类型**: 在线 PCB 设计
- **说明**: 在线 PCB 设计工具，适合初学者
- **特点**: 浏览器使用、可直接下单生产

---

## 🌐 社区资源汇总

### 47. NESDev GitHub 组织
- **URL**: https://github.com/nesdev
- **类型**: GitHub 组织
- **说明**: NESDev 社区官方 GitHub
- **内容**: 各种 NES 工具、文档、测试 ROM

### 48. Libretro GitHub 组织
- **URL**: https://github.com/libretro
- **类型**: GitHub 组织
- **说明**: RetroArch 核心开发者
- **NES 核心**:
  - https://github.com/libretro/nestopia-libretro
  - https://github.com/libretro/fceumm-libretro
  - https://github.com/libretro/mesen-libretro

### 49. Awesome NES（资源列表）
- **URL**: https://github.com/Phenax/awesome-nes
- **类型**: 资源汇总
- **说明**: 社区维护的 NES 开发资源列表
- **内容**: 工具、教程、游戏、模拟器链接

### 50. Homebrew Wiki GitHub
- **URL**: https://github.com/NESDev/nesdev-wiki
- **类型**: Wiki 源码
- **说明**: NESDev Wiki 的 GitHub 源码仓库
- **内容**: Wiki 文档的 Markdown 源文件

---

## 📋 原理图获取清单

### 官方维修手册
- [ ] NES-001 原理图：https://www.nesdev.org/nsm.htm
- [ ] Famicom 原理图：https://www.nesdev.org/famicom_schematics.htm
- [ ] NES-101 原理图：https://www.nesdev.org/nes-101.htm
- [ ] AV Famicom 原理图：https://www.nesdev.org/av-famicom.htm

### 改装 PCB 设计
- [ ] NESRGB（Artemio）: https://github.com/ArtemioUW/NESRGB
- [ ] NES Top Loader RGB: https://github.com/ArtemioUW/NES-Top-Loader-RGB
- [ ] Famicom RGB: https://github.com/ArtemioUW/Famicom-RGB
- [ ] NES-DAC（音频改进）: https://github.com/ArtemioUW/NES-DAC

### FPGA 核心源码
- [ ] MiSTer NES: https://github.com/MiSTer-devel/NES_MiSTer
- [ ] MiSTer Famicom: https://github.com/MiSTer-devel/Famicom_MiSTer
- [ ] Mesen2（参考实现）: https://github.com/SourMesen/Mesen2

---

## 🔗 一键访问 - 核心开发者

| 开发者 | 专长 | GitHub |
|--------|------|--------|
| **SourMesen** | 模拟器 | https://github.com/SourMesen |
| **Artemio** | 硬件改装 | https://github.com/ArtemioUW |
| **tepples** | 开发工具 | https://github.com/tepples |
| **krikzz** | 烧录卡 | https://github.com/krikzz |
| **brocator** | 汇编器 | https://github.com/brocator |
| **quietust** | 音频模拟 | https://github.com/quietust |
| **dougfraker** | NESMaker | https://github.com/dougfraker |
| **shiru86** | 游戏开发 | https://github.com/shiru86 |

---

## 📊 芯片级资源

### CPU (2A03/2A07)
- **介视图**: https://visual6502.org/wiki/index.php?title=NES
- **文档**: https://www.nesdev.org/6502.htm
- **指令集**: https://www.nesdev.org/6502_instructions.htm

### PPU (2C02/2C03/2C05)
- **介视图**: https://visual6502.org/wiki/index.php?title=PPU
- **文档**: https://www.nesdev.org/ppu.htm
- **渲染时序**: https://www.nesdev.org/ppu_timing.htm

### APU（音频）
- **文档**: https://www.nesdev.org/apu.htm
- **音频采样**: https://www.nesdev.org/apu_reference.htm

---

## ⚠️ 注意事项

1. **原理图版本**: 不同版本的 NES/FC 主板有差异，确认你的主机版本
2. **改装风险**: 焊接改装有风险，建议先练习
3. **FPGA 编译**: MiSTer 核心需要 Quartus 编译，需要一定技术基础
4. **版权问题**: 商用 NES 设计需注意任天堂知识产权
5. **静电防护**: 接触 PCB 时注意防静电

---

## 🎓 学习路径建议

### 想理解 NES 硬件
1. [ ] 阅读 [NESDev Wiki 硬件篇](https://nesdev.wiki/wiki/Hardware)
2. [ ] 下载 [官方原理图](https://www.nesdev.org/schematics.htm)
3. [ ] 查看 [Visual 6502 介视图](https://visual6502.org/)
4. [ ] 研究 [Mapper 文档](https://www.nesdev.org/mappers.htm)

### 想改装 NES 主机
1. [ ] 查看 [Artemio 的改装项目](https://github.com/ArtemioUW)
2. [ ] 下载 KiCad 打开 PCB 设计
3. [ ] 在 [NESDev 论坛](https://www.nesdev.org/) 学习经验
4. [ ] 购买 [RetroUSB 套件](https://retrousb.com/) 练手

### 想开发 FPGA 核心
1. [ ] 学习 [MiSTer NES 核心源码](https://github.com/MiSTer-devel/NES_MiSTer)
2. [ ] 参考 [Mesen2 模拟器](https://github.com/SourMesen/Mesen2)
3. [ ] 阅读 [PPU/CPU 文档](https://nesdev.wiki/)
4. [ ] 加入 [MiSTer Discord](https://discord.gg/misterfpga)

---

_文档由 OpenClaw Agent 整理生成_
