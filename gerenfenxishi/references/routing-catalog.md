# 路由目录

## 使用方法

先按当前最大瓶颈选一个主路由，再按依赖关系添加最多两个辅助路由。不要因为一句话同时出现“工作、钱、朋友”就把所有相关路由都跑一遍。

| 路由 ID | 优先触发 | 不要误用为 | 对应 playbook | 融合的源 skills |
|---|---|---|---|---|
| `emotion-reset` | 急、怒、惧、慌、冲动；正要做不可逆动作；情绪峰值损害判断 | 长期恢复、普通时机判断 | `stabilization-recovery.md` | `reset-emotion-before-action`；`emotion-state-decision-routing` |
| `baseline-recovery` | 作息/环境/任务一起失序；精神身体与成果同时下滑；失败后冻结、无法重新行动 | 单纯懒惰评判；替代医疗 | `stabilization-recovery.md` | `restore-operational-baseline`；`root-tree-leaf-recovery`；`adversity-recovery-ladder` |
| `agency-authorship` | 全盘自责与无力之间摆动；被评价/头衔/旧角色定义；不知道真正想要什么 | 假装能控制一切；逃避真实责任 | `identity-path-learning.md` | `calibrate-agency-and-responsibility`；`self-authorship-loop` |
| `path-fit` | 判断长期工作、创作或人生方向是否适合自己；方向尚未选定 | 已选定方向后的迁移计划 | `identity-path-learning.md` | `qing-an-path-fit` |
| `learning-loop` | 看了很多却做不到；想把方法变成可调用行为 | 内容摘要或资料检索 | `identity-path-learning.md` | `ming-shu-learning-loop` |
| `timing-action` | 该等、追、顺势还是面对；机会窗口是否真实；何时行动 | 高代价承诺投入等级 | `timing-transition-growth.md` | `choose-wait-ride-or-face`；`timing-momentum-discipline` |
| `rooted-transition` | 辞职、转行、创业、开新业务、扩店、扩大项目或合伙承诺 | 日常消费；仅问时机 | `timing-transition-growth.md` | `escalate-commitment-with-downside-gates`；`rooted-pilot-transition` |
| `success-risk` | 爆红、融资、升职、增长或广泛赞誉后担心失控 | 无成功信号时的普遍焦虑 | `timing-transition-growth.md` | `success-risk-inversion` |
| `opportunity-ethics` | 发现赚钱/流量/副业机会，但担心欺骗、伤害或不道德 | 金融资产是否安全 | `money-opportunity-risk.md` | `ethical-opportunity-scan` |
| `money-downside` | 预算、借钱、还款、消费、赠与、投资、合伙出资、损失上限 | 具体证券推荐、税法或法律结论 | `money-opportunity-risk.md` | `manage-wealth-across-the-lifecycle`；`affordable-loss-investment-check` |
| `people-trust` | 判断陌生人、员工、供应商、熟人或合作对象是否可靠 | 已有关系中的期待与承诺配置 | `people-trust-network.md` | `assess-people-by-behavior`；`evidence-based-trust-calibration` |
| `network-reciprocity` | 贵人、导师、人脉、受助回馈与互助边界 | 攀附权势或服从换资源 | `people-trust-network.md` | `dynamic-benefactor-network` |
| `relationship-boundaries` | 情义与利益混在一起；隐性期待；朋友/家人/伴侣的回报、金钱和边界 | 陌生人初始可信度；正式合作治理全套 | `relationships-dialogue.md` | `configure-trust-by-relationship`；`relationship-mode-layering`；`expectation-agency-separation` |
| `dialogue-repair` | 想把真话说清；伴侣信任破裂、反复冲突、分工失衡或需要结构性修复 | 家暴、胁迫中的普通沟通 | `relationships-dialogue.md` | `truthful-equal-dialogue`；`partner-four-layer-repair` |
| `collaboration-governance` | 团队/合伙的投入、权责、利润、风险、监督、退出或信息边界 | 单纯判断人是否可信 | `collaboration-information.md` | `collaboration-risk-governance`；`stage-based-information-boundary` |
| `outcome-review` | 复盘一件事值不值、成败如何、亏损是否换来可复用资产 | 用“成长”粉饰持续亏损或伤害 | `review-integration.md` | `three-ledger-outcome-review` |

## 易混淆路由的判别

### 情绪与时机

- 用户在情绪峰值、正要做不可逆动作：先 `emotion-reset`。
- 用户基本稳定，问题是等待能否增加信息、拖延是否增损：用 `timing-action`。

### 失败、自责与恢复

- 核心问题是“责任到底怎么分、哪些可控”：用 `agency-authorship`。
- 核心问题是“我已冻住、生活也乱、怎样重新动起来”：用 `baseline-recovery`。
- 两者并存：先恢复最低行动能力，再校准责任。

### 方向适配与职业迁移

- 还不知道哪条路适合：用 `path-fit`。
- 方向大致确定，问题是如何辞职、并行、小试或投入升级：用 `rooted-transition`。
- 只问现在是否是窗口：用 `timing-action`；涉及根基和大投入时把它降为辅助路由。

### 钱、事业与合作

- 核心风险是资金归零、债务或基本生活：主路由 `money-downside`。
- 核心风险是职业根基、项目验证和投入等级：主路由 `rooted-transition`。
- 核心风险是合伙权责、账目、控制权、退出：主路由 `collaboration-governance`。
- 同时出现时，先处理会造成不可承受损失的那一项；最多再加两个辅助路由。

### 识人与关系

- 问“这个人靠不靠谱”：用 `people-trust`。
- 问“这段既有关系应如何谈回报、承诺和边界”：用 `relationship-boundaries`。
- 问“这次话怎么说”或“伴侣关系怎样修复”：用 `dialogue-repair`。
- 正式共同做事：在信任/边界之后使用 `collaboration-governance`。

### 趋势与成功风险

- 判断窗口是否成立、是否分段加速：用 `timing-action`。
- 成功或增长已经发生，检查隐藏脆弱点：用 `success-risk`。

## 常用组合链

| 复合场景 | 推荐顺序 |
|---|---|
| 愤怒中想辞职 | `emotion-reset → rooted-transition` |
| 失败后既自责又无法行动 | `baseline-recovery → agency-authorship` |
| 朋友邀请合伙出资 | `money-downside → people-trust → collaboration-governance` |
| 不知道做什么工作，也想马上裸辞 | `path-fit → rooted-transition` |
| 伴侣争吵中想立刻分手 | `emotion-reset → dialogue-repair` |
| 朋友免费帮忙后因回报闹翻 | `relationship-boundaries → dialogue-repair` |
| 项目突然爆红并准备扩张 | `success-risk → timing-action → collaboration-governance` |
| 学了很多方法仍不会选 | `learning-loop → 当前真实问题的主路由` |

## 路由置信度

- **高**：用户的决定、阶段和最大风险都清楚，直接执行。
- **中**：有两个近邻路由；说明主路由选择依据，并把另一个设为条件式辅助。
- **低**：安全、决定对象或时间窗缺失；询问最多三个会改变路由的问题。
