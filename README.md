# gerenfenxishi：个人分析师 Skill

一个面向现实人生选择与复杂困境的 Codex Skill。它把模糊的问题整理成可判断、可行动、可复查的决定，并从多个决策 playbook 中选择一个主路由和最多两个辅助路由。

它适合工作与转型、创业与投入、关系与信任、情绪与恢复、合作治理、失败复盘等场景。它不是算命工具，也不预测命运。

## 核心能力

- 先检查人身安全、急症、自伤/他伤、家暴、诈骗、法律期限和重大财务风险。
- 区分事实、推断、价值偏好与未知信息。
- 比较直接行动、小规模试验、等待、缩小/退出和寻求支持等真实选项。
- 优先保护安全、合法权益、基本生活、可逆性和再次尝试的能力。
- 给出倾向性结论、未来 24–72 小时的最小动作、停止线和复查点。

## 安装

### Codex

把 `gerenfenxishi` 文件夹复制到 Codex 的 skills 目录：

```text
<CODEX_HOME>/skills/gerenfenxishi
```

Windows 的常见位置是：

```text
C:\Users\<你的用户名>\.codex\skills\gerenfenxishi
```

重新启动 Codex 或新建任务后即可使用。仓库根目录不是 skill 本体；安装时请复制其中的 `gerenfenxishi/` 文件夹。

### 从 Git 仓库安装

```powershell
git clone https://github.com/su4295427-ai/gerenfenxishi-skill.git
Copy-Item -Recurse -Force .\gerenfenxishi "$env:USERPROFILE\.codex\skills\gerenfenxishi"
```

如果设置了 `CODEX_HOME`，请把目标改为 `$env:CODEX_HOME\skills\gerenfenxishi`。

## 使用方法

在请求中明确调用 `$gerenfenxishi`，并提供要决定的动作、时间限制、不能失去的东西和已知事实。信息不完整也可以开始；只有会改变安全判断或建议方向时，skill 才会追问最多三个短问题。

示例：

```text
用 $gerenfenxishi 帮我判断要不要辞职创业。请直接给建议，并写出一个低风险试点、升级条件、退出线和 72 小时内的第一步。
```

```text
用 $gerenfenxishi 分析朋友邀我合伙出资这件事。先判断人、钱和治理中哪个是主风险，再给出补资料清单和拒绝条件。
```

```text
用 $gerenfenxishi 帮我处理伴侣冲突。如果存在暴力、胁迫或我正处于情绪峰值，先停止普通沟通建议并处理安全问题。
```

## 默认输出

1. 当前建议及成立条件。
2. 主路由与最多两个辅助路由。
3. 事实、推断、价值和未知。
4. 2–4 个真实可行选项的损失、可逆性和证据缺口。
5. 未来 24–72 小时的一个最小动作、复查点和停止线。
6. 最可能推翻当前建议的一条新证据。

## 文件结构

```text
gerenfenxishi/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── routing-catalog.md
    ├── safety-boundaries.md
    ├── stabilization-recovery.md
    ├── identity-path-learning.md
    ├── timing-transition-growth.md
    ├── money-opportunity-risk.md
    ├── people-trust-network.md
    ├── relationships-dialogue.md
    ├── collaboration-information.md
    ├── review-integration.md
    └── routing-evals.json
```

`SKILL.md` 是总控流程；`routing-catalog.md` 负责选路由；各领域 playbook 只在相关问题出现时按需加载；`routing-evals.json` 仅用于维护与验证。

## 安全边界

- 不替代紧急救援、医生、心理健康专业人员、律师、税务师或持牌财务顾问。
- 不诊断疾病，不给具体证券买卖结论、收益保证、法律结论或规避监管方案。
- 命中即时危险、可能急症、家暴、胁迫、自伤/他伤或正在发生的诈骗时，优先建议联系当地紧急服务、可信支持者或合格专业人士。
- 对法律、政策、市场、产品条款等会变化的事实，应先核验当前权威来源。
- 不设计诱捕、隐私测试、操纵性沟通或持续监控。

## 隐私与数据

该 skill 不包含遥测、网络请求、密钥或用户数据存储脚本。它只提供文本决策流程。使用时仍应避免提交与决定无关的身份证件、账号、住址、医疗记录等敏感信息。

## 维护与验证

修改路由或 playbook 后，应运行 Skill Creator 的 `quick_validate.py` 验证结构，并用 `references/routing-evals.json` 检查主路由、安全闸门和辅助路由是否符合预期。

## 来源与认识边界

该项目将文学性或传统表达仅作为启发，最终判断必须建立在现实事实、可靠证据、专业规则、可逆性和反馈之上。项目不包含原书章节或大段原文，也不主张文学案例能够证明现实效果。

## 许可证

本项目以 MIT License 发布，详见 [LICENSE](LICENSE)。第三方作品、名称和观点仍归各自权利人所有。
