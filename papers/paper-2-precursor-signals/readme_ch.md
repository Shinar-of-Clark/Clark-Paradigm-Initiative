# 多端谐波指纹平台 (克拉克范式) - 阶段二

> **项目代号:** Shinar of Clark  
> **作者:** Yi Zeng   
> **框架:** 海上风电资产亚健康状态的因果审计与保护机制  
> **📄 论文 PDF:** [在此阅读完整论文](./Causal%20Auditing%20and%20Protection%20Paradigm%20for%20Sub-health%20Offshore%20Wind%20Assets%20based%20on%20Multi-terminal%20Harmonic%20Fingerprinting.pdf)  
> **DOI:** [![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.20267143-blue)](https://doi.org/10.5281/zenodo.20267143)

---

## 📖 简介

本仓库实现了 **“克拉克范式 (Clark Paradigm)”** 框架下海上风电资产亚健康诊断的阶段二（“生理学”阶段）研究。

在第一阶段建立的“电磁账本”基础之上，本研究的核心聚焦于**捕捉前兆信号 (Precursor Signals)** 并建立主动**保护 (Protection)** 机制。通过解构在动态工况下 1至20次 谐波指纹的时间演化规律，本阶段实现了从单一“诊断”向“预测性保护”的关键性范式跃升。

**核心哲学:** 前兆预警 = 物理真实与预期的残差演化 + 动态时滞分析 ($\Delta T$)。

---

## 📁 仓库结构

为了确保研究的透明度与可重复性，本论文的补充材料按如下结构组织：

- `figures/`: 包含论文中展示的所有高分辨率图表、时序演化图和跨端子保护机制架构图。
- `data/`: 包含生成图表所对应的动态时间序列数据集（原始数据与处理后数据）。研究人员可使用此数据独立验证前兆信号捕捉算法与保护逻辑。

---

## 🛠️ 技术架构

本阶段在分布式硬件拓扑的基础上，扩展了高级时序分析与保护控制引擎：

- **感知层 (现场层):** 部署于机组内部与变电站入口的 MCU 节点执行 **10.24 kHz** 高频采样，并与机械动力学变量（如风速、转速）进行动态同步。
- **审计与保护层:** 边缘计算主机通过 **动态因果模型 (DCM)** 执行预测性映射与时序相关性分析，追踪故障跨节点传染的时滞 ($\Delta T$)，并生成保护动作指令。

---

## 🚀 核心特性

- **前兆信号捕捉 (Precursor Capture):** 在灾难性故障发生之前，精准捕捉潜在的亚健康指纹（例如微观的绝缘老化与介电漂移的早期累积）。
- **动态时滞 ($\Delta T$) 分析:** 深入分析各节点之间谐波频率偏移的时间延迟，并将其作为元器件应力疲劳的稳健前兆指标。
- **机-电预测性映射:** 建立风机机械动态（空气动力学湍流、突发风速变化）与随之产生的电气谐波波动之间的内部因果关联。
- **主动防御护盾 (Proactive Protection):** 将因果审计引擎升级为闭环的保护系统。利用时滞窗口期发布动态早期预警，并在必要时触发保护策略以抢先保护核心电力资产。

---

## 📊 性能表现

通过引入动态时滞分析，本框架能够比传统的阈值报警系统提前 **数小时至数天** 识别出绝缘老化和开关管（IGBT）退化的前兆特征，为运维团队大幅延长了关键的响应与保护窗口期，避免了重大资产损失。

---

## 📚 引用说明

如果您在研究中使用了本项目的概念或内容，请引用我们的论文：

**APA 格式:**
> Zeng, Y. (2026). Causal Auditing and Protection Paradigm for Sub-health Offshore Wind Assets based on Multi-terminal Harmonic Fingerprinting (v1.0.0). Zenodo. https://doi.org/10.5281/zenodo.20267143

**BibTeX:**
```bibtex
@misc{zeng2026clark_protection,
  title={Causal Auditing and Protection Paradigm for Sub-health Offshore Wind Assets based on Multi-terminal Harmonic Fingerprinting},
  author={Yi Zeng},
  year={2026},
  publisher={Zenodo},
  version={v1.0.0},
  doi={10.5281/zenodo.20267143},
  url={https://doi.org/10.5281/zenodo.20267143}
}
```

---

## 🛡️ 许可证

本项目基于 [Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/legalcode) 许可证开源。

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

**权利声明:** 您可以自由地共享和修改本作品，但请务必署名原作者 **Yi Zeng (Project Shinar of Clark)**，并标明是否对原内容进行了修改。
