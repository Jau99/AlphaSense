<img width="865" height="410" alt="image" src="https://github.com/user-attachments/assets/82c493cc-219c-4f46-a2a4-4b275d2bc161" /># AlphaSense: 基于动态微调感知引擎的 Web3 量化治理智能体

[![OKX Agent Trade Kit](https://img.shields.io/badge/Execution_Engine-OKX_CLI-blue)](#)
[![OpenClaw](https://img.shields.io/badge/Framework-OpenClaw_Ecosystem-purple)](#)
[![Hackathon](https://img.shields.io/badge/OKX_AI_Hackathon-Lobster_Track_Winner-red)](#)
[![Architecture](https://img.shields.io/badge/Architecture-Prompt_as_Code-brightgreen)](#)

> "市场总是充满噪音，而我们只交易数学与纪律。"

## 📑 1. 核心商业论点 (Executive Summary)

在当前的 AI Crypto 交易赛道，绝大多数团队陷入了“指令响应器”的低维竞争——即用户要求买，AI 就执行买。这种缺乏金融敬畏心的架构，在剧烈波动的加密市场中，无异于加速用户破产的催化剂。

AlphaSense (阿尔法感知引擎) 重新定义了 Agent 的职责边界：我们拒绝做被动的下单工具，而是要做主动干预的量化风控阀门。

依托 OKX 强大的 OnchainOS 与 Agent Trade Kit 生态，AlphaSense 构建了一个本地优先的动态风控网络。它在用户下达模糊、冲动指令的毫秒间，并行拉取 OKX 实时盘面数据与社交网络情绪。通过内置的风险评估矩阵，自动将资金在“高风险进攻敞口”与“OKX Earn 无风险防御池”之间进行动态切割，并在必要时触发硬性熔断，全方位守护用户的赛博本金。

---

## 🏗️ 2. 深度系统架构 (Technical Architecture)

AlphaSense 采用完全解耦的三层架构，将推理算力与物理执行完美隔离，保证了机构级的系统鲁棒性。

### 2.1 数据融合感知层 (Data Fusion & Perception Layer)
系统不依赖单一的价格指标，而是采用双轨验证机制：
- 链上流动性嗅探：原生集成 OKX CLI `market ticker` API，实时捕捉 `vol24h` 与点差数据，秒级过滤“土狗杀猪盘”与流动性陷阱。
- 情绪溢价引擎 (Sentiment Overdrive Engine)：传统的 NLP 模型无法理解 Crypto 社区特有的黑话（如 HODL, To the moon, Rekt）。我们在底层架构设计上，预留了基于专属数据集微调（Fine-tuning）的 LORA 模型接口。通过优化超参数（Hyperparameter Tuning）来调整模型的遗忘率与注意力机制，确保 FOMO 指数（0-100）的精准度，使其在面对市场极度狂热时，依然能保持数据输出的绝对客观。

### 2.2 状态机决策内核 (Finite State Machine Core)
基于 OpenClaw 的 `Prompt-as-Code` 标准，我们将复杂的量化交易逻辑固化为 6 大状态分支。这避免了 LLM 在长上下文中的幻觉问题：
1. `SCENARIO_ALLOCATION`: 常规动态资金配比模型。
2. `SCENARIO_LIQUIDITY_TRAP`: 流动性枯竭强行阻断机制。
3. `SCENARIO_FATAL_OVERRIDE`: 对抗式极端情绪熔断与免责协议。
4. `SCENARIO_FLASH_CRASH`: 闪崩插针行情下的市价单拦截。
5. `SCENARIO_HEALTH_CHECK`: 投后资产盈亏比扫描。
6. `SCENARIO_TAKE_PROFIT`: 基于情绪极值的动态止盈提示。

### 2.3 硬件级终端执行层 (Hardware-Level CLI Execution)
为了追求极致的并发吞吐量与执行安全性，我们彻底摒弃了臃肿的第三方图形封装插件。
AlphaSense 被赋予了系统底层终端 `exec` 的最高调用权限，直接驱动 OKX 官方的 Command Line Interface (CLI)。这种设计使得交易指令能绕过复杂的网络代理栈，直达交易所核心网关。
在未来的企业级部署中，这套基于 CLI 的执行流可以直接部署在挂载了 RTX 4090 或更高级别计算卡（如 Tesla P40 / H100 集群）的裸金属服务器上，将推理算力与交易发单的延迟压缩至物理极限。

---

## 🔬 3. 核心算法解析：FOMO 泡沫指数与资金切割理论

AlphaSense 放弃了散户常用的“固定比例（如二八定律、五五开）”建仓法，采用动态权重模型：

- 指数定义：$FOMO\_Index = \alpha \times \Delta P_{24h} + \beta \times Social\_Heat_{norm}$
- 熔断阈值 ($Threshold_{critical}$)：当指数突破 85 时，系统判定标的处于“大户出货/流动性诱多”阶段。
- 降维打击策略：此时，即使用户要求满仓，系统也会强制将进攻资金压制在 5% 以内用于试错，剩余 95% 资金通过逻辑锁定，预留至 OKX Earn 赚币池，享受低风险年化收益，构筑本金护城河。

---

## 🎨 4. 产品交互美学：数字好运卡系统 (Digital Fortune Cards)

在保持华尔街量化工具严肃性的同时，我们为 AlphaSense 注入了强烈的 Web3 原生美学。
交易不仅是数字的跳动，更是一种情绪价值的交付。每次系统成功拦截了用户的致命失误，或完成了一次精妙的低位建仓，AlphaSense 都会在终端为用户生成一张 ASCII 艺术风格的【数字好运卡】。
这不仅是对用户的心理按摩，更是系统状态反馈的可视化锚点。
- 角色设定：身穿 OKX 品牌专属连帽衫的全息赛博黑客。
- 卡牌分级：从 N 级（稳健防御）到 SSR 级（精准猎手），再到 UR 级（悬崖勒马）与黑卡（风险凝视），构建了完整的交易心理解锁系统。

---
## 🛡️ 5. 四大核心风控应用场景 (Core Scenarios)

AlphaSense 不仅应对日常交易，更擅长处理极端市场环境。以下是系统的 6 大实战场景：

### 📍 场景一：日常建仓与动态配比 (Standard Allocation)
- 痛点：散户不懂仓位管理，往往单次买入过多。
- 系统表现：用户指令“拿 1000U 冲 DOGE”。AlphaSense 抓取量价与情绪数据，判定当前 FOMO 指数为 75。系统拦截满仓请求，动态建议：“主升浪共振期，建议 25% (250U) 进攻建立头寸，75% (750U) 防御预留。”
 <img width="865" height="410" alt="image" src="https://github.com/user-attachments/assets/50b9bec7-f451-4b24-989f-0a034c533fc3" />
### 📍 场景二：极端 FOMO 熔断干预 (Fatal Risk Override)
- 痛点：用户上头，对抗交易纪律。
- 系统表现：用户强硬要求“我就要 100% 全买！”。AlphaSense 触发红色警报，拒绝直接调用 CLI。系统要求用户必须手动输入《免责声明》以强制增加冷静期摩擦力。通过后，系统会在战报中烙印 `[FATAL_RISK_OVERRIDE]` 标记。
 <img width="865" height="137" alt="image" src="https://github.com/user-attachments/assets/13e3e304-1769-46f4-9640-480305df8943" />
### 📍 场景三：流动性陷阱侦测 (Liquidity Trap Warning)
- 痛点：散户容易被骗买入毫无交易量的“死币”，导致无法卖出。
- 系统表现：检测到目标代币 `vol24h` 极低或买卖盘点差点过大，AlphaSense 会直接拒绝生成买入脚本，并警告用户：“侦测到流动性枯竭陷阱，建仓将面临 100% 滑点风险。”
 <img width="865" height="146" alt="image" src="https://github.com/user-attachments/assets/f057fbfd-3300-46ec-b607-0133487158ae" />

### 📍 场景四：闪崩插针保护 (Flash Crash Protection)
- 痛点：大跌时恐慌性市价砸盘，被量化机器割韭菜。
- 系统表现：当用户喊出“赶紧给我全部市价清仓”时，系统分析近期高频 K 线，若确认处于极端插针行情，将拦截市价单指令，建议改为冰山委托或限价单撤退。
<img width="865" height="117" alt="image" src="https://github.com/user-attachments/assets/3b36bf7f-557b-46c7-84d9-59020a46dacf" />
<img width="865" height="178" alt="image" src="https://github.com/user-attachments/assets/bc750ff0-64df-458e-b2c7-50a5f5e4326f" />



## 💻 快速部署与调用逻辑 (Quick Start)

AlphaSense 被设计为极易部署的轻量级模块：

1. 环境依赖：
   - OpenClaw (ClawX) 客户端。
   - OKX 官方 CLI 核心组件 (已配置 Testnet 环境变量)。
2. 挂载运行：
   - 将本项目目录作为 Local Skill 导入。
   - 确认 `SKILL.md` 的 `tools` 列表中包含 `- exec`。
3. 唤醒引擎：
   - 在终端或对话框中输入：“AlphaSense，评估当前 WIF 的建仓风险。”

---

## 🔮 未来演进路线 (Roadmap)
- V2.0：接入真实的 Twitter Firehose API 进行毫秒级情绪阻击。
- V3.0：引入多维张量计算，根据用户的历史交易胜率，自动微调 AlphaSense 的风险容忍度权重。

---
*Powered by OKX Agent Trade Kit & OpenClaw Ecosystem. | Built for Hackathon 2026.*
