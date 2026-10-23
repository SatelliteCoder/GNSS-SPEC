# GNSS-SPEC: GNSS Signal Processing & Education Center

**GNSS-SPEC** (GNSS Signal Processing & Education Center) 是一个面向教育与研究的开源 GNSS 信号仿真平台。项目提供从信号生成、误差建模、信号处理到定位解算的完整链路，以及详细的原理文档和学习指南。

## ✨ 特性

- 🛰️ **多星座支持**：GPS L1 C/A、BDS B1I、Galileo E1 等信号体制
- ⚙️ **完整处理链**：信号生成 → 误差建模 → 信号捕获 → 信号跟踪 → 定位解算
- 🌍 **丰富的误差模型**：电离层、对流层、多径、相对论效应、Sagnac效应等
- 📡 **多种调制方式**：BPSK、BOC、MBOC/CBOC、AltBOC 等
- 📊 **可视化工具**：信号频谱、相关峰、星空图、定位结果等
- 📖 **详尽文档**：13篇原理文档，覆盖从基础到进阶的完整知识体系
- 💻 **多语言实现**：C++、Python、MATLAB 示例代码

## 📂 项目结构

```text
GNSS-SPEC/
├── GNSS仿真原理与实现/      # 📚 原理文档（核心内容）
│   ├── 01-原理总述.md        # 仿真系统概述与学习路径
│   ├── 02-时间系统.md        # 时间系统与转换（GPST/BDT/UTC等）
│   ├── 03-伪距计算.md        # 伪距观测方程与误差源分析
│   ├── 04-卫星空间位置计算.md # 开普勒轨道与星历计算
│   ├── 05-信号调制.md        # BPSK/BOC/MBOC调制技术
│   ├── 06-电离层延迟模型.md  # Klobuchar/Bent/IRI电离层模型
│   ├── 07-对流层延迟模型.md  # Saastamoinen/Hopfield/GMF对流层模型
│   ├── 08-多径效应模型.md    # 多径原理、环境建模与抑制技术
│   ├── 09-信号捕获原理.md    # 串行搜索、FFT快速捕获、BOC捕获
│   ├── 10-信号跟踪原理.md    # PLL/DLL/FLL环路设计与实现
│   ├── 11-定位解算算法.md    # 最小二乘、卡尔曼滤波、DOP、RAIM
│   ├── 12-多普勒频移计算.md  # 多普勒效应与速度计算
│   └── 13-导航电文格式.md    # GPS/北斗导航电文结构与解析
├── RINEX/                    # 📄 RINEX格式参考文档
│   └── rinex_4.00.pdf
├── src/                      # 💻 源代码（规划中）
│   ├── simulation/           # 信号生成与误差建模
│   ├── processing/           # 捕获与跟踪算法
│   └── positioning/          # LSQ与EKF定位解算
├── notebooks/                # 📒 Jupyter学习笔记本
├── tools/                    # 🛠️ 可视化与分析工具
├── data/                     # 📊 示例数据文件
└── README.md
```

## 📚 文档体系与学习路径

文档按照 GNSS 信号仿真的完整处理链组织，建议按照以下顺序学习：

### 🌱 入门篇（基础理论）

| 序号 | 文档 | 学习目标 |
| :--- | :--- | :--- |
| **01** | [原理总述](GNSS仿真原理与实现/01-原理总述.md) | 建立整体认知，了解仿真系统架构 |
| **02** | [时间系统](GNSS仿真原理与实现/02-时间系统.md) | 掌握GPST/BDT/UTC等时间系统及转换 |
| **03** | [伪距计算](GNSS仿真原理与实现/03-伪距计算.md) | 理解伪距观测方程及误差来源 |

### 🏗️ 进阶篇（误差建模）

| 序号 | 文档 | 学习目标 |
| :--- | :--- | :--- |
| **04** | [卫星空间位置计算](GNSS仿真原理与实现/04-卫星空间位置计算.md) | 掌握开普勒轨道与星历计算 |
| **05** | [信号调制](GNSS仿真原理与实现/05-信号调制.md) | 理解BPSK/BOC等调制方式及频谱特性 |
| **06** | [电离层延迟模型](GNSS仿真原理与实现/06-电离层延迟模型.md) | 掌握Klobuchar模型及双频修正 |
| **07** | [对流层延迟模型](GNSS仿真原理与实现/07-对流层延迟模型.md) | 掌握Saastamoinen等对流层模型 |
| **08** | [多径效应模型](GNSS仿真原理与实现/08-多径效应模型.md) | 理解多径原理及环境建模 |

### 🚀 高级篇（信号处理与定位）

| 序号 | 文档 | 学习目标 |
| :--- | :--- | :--- |
| **09** | [信号捕获原理](GNSS仿真原理与实现/09-信号捕获原理.md) | 掌握FFT快速捕获算法 |
| **10** | [信号跟踪原理](GNSS仿真原理与实现/10-信号跟踪原理.md) | 理解PLL/DLL/FLL环路设计 |
| **11** | [定位解算算法](GNSS仿真原理与实现/11-定位解算算法.md) | 掌握最小二乘与卡尔曼滤波 |
| **12** | [多普勒频移计算](GNSS仿真原理与实现/12-多普勒频移计算.md) | 理解多普勒产生机制与计算 |
| **13** | [导航电文格式](GNSS仿真原理与实现/13-导航电文格式.md) | 掌握GPS/北斗电文结构与解析 |

---

## 🚀 快速开始

### 环境要求

- C++17 兼容编译器
- CMake (≥ 3.10)
- Python 3.8+ (numpy, matplotlib, scipy)

### 阅读文档

直接浏览 `GNSS仿真原理与实现/` 目录下的 Markdown 文档，或从 [01-原理总述](GNSS仿真原理与实现/01-原理总述.md) 开始按学习路径阅读。

### 运行示例代码

```bash
# 克隆仓库
git clone https://github.com/SatelliteCoder/GNSS-SPEC.git
cd GNSS-SPEC

# Python 示例
python examples/ionosphere_demo.py
python examples/tracking_demo.py
```

---

## 📡 支持的信号与系统

### GPS (美国)
- ✅ L1 C/A (BPSK(1))
- ✅ L2C (BPSK(1))
- ✅ L5 (QPSK(10))
- 📋 L1C (TMBOC) — 规划中

### BDS / 北斗 (中国)
- ✅ B1I (BPSK(2))
- ✅ B3I (BPSK(10))
- ✅ B1C (QMBOC)
- ✅ B2a (BPSK(10))
- ✅ B2b (BPSK(10))

### Galileo (欧盟)
- ✅ E1 OS (CBOC) 
- 📋 E5a (AltBOC) — 进行中

### GLONASS (俄罗斯)
- ✅ L1 SP (FDMA)
- ✅ L2 SP (FDMA)
---

## 🧮 误差模型

| 误差源 | 模型 | 状态 |
| :--- | :--- | :--- |
| 卫星钟差 | 二阶多项式 | ✅ |
| 卫星轨道 | 开普勒+摄动 | ✅ |
| 电离层延迟 | Klobuchar / Bent / IRI | ✅ |
| 对流层延迟 | Saastamoinen / Hopfield / GMF | ✅ |
| 多径效应 | 反射系数模型 / 统计模型 | ✅ |
| 热噪声 | AWGN高斯白噪声 | ✅ |
| 相对论效应 | 标准相对论修正 | ✅ |
| 地球自转 | Sagnac效应 | ✅ |
| 射频干扰 | CW / 扫频 / 脉冲 | 📋 |

---

## 📎 ICD 参考文档

各系统接口控制文件 (ICD) 是 GNSS 信号设计的权威参考：

- **GPS**: IS-GPS-200、IS-GPS-705、IS-GPS-800
- **Galileo**: OS SIS ICD
- **北斗**: BDS-SIS-ICD-B1I/B1C/B2a/B3I
- **GLONASS**: GLONASS ICD

大型 ICD 规范文件（PDF格式）通过网盘共享：
- **下载链接:** [https://pan.baidu.com/s/165mR0DUQotHC6FXu7rDKJw?pwd=ncmd](https://pan.baidu.com/s/165mR0DUQotHC6FXu7rDKJw?pwd=ncmd)
- **提取码:** `ncmd`

---

## 🤝 贡献指南

我们欢迎各种形式的贡献！你可以：

- 🐛 提交 Bug 报告和功能建议
- 📝 改进文档和学习笔记
- 💻 贡献新的算法实现
- 🧪 添加新的仿真场景
- 🌐 翻译文档（中↔英）

### 贡献步骤

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

---

## 📄 许可证

本项目采用 MIT 许可证 - 详见 [LICENSE](LICENSE) 文件。

---

## 🙏 致谢

- **RTKLIB** — 开源GNSS定位软件的参考实现
- **GPSTk** — GNSS算法工具库
- **GNSS-SDR** — 软件定义无线电GNSS接收机
- **SoftGNSS** — 早期的软件GPS接收机项目
- 所有为开源GNSS社区做出贡献的开发者和研究者

---

## 📮 联系方式

- GitHub Issues: [提交问题或建议](https://github.com/SatelliteCoder/GNSS-SPEC/issues)
- 欢迎 GNSS 爱好者、研究者、工程师加入交流

---

<p align="center">
⭐ 如果这个项目对你有帮助，请给一个 Star！<br>
<sub>用仿真预见性能，用数据驱动创新</sub>
</p>
