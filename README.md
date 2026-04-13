# metric-alignment-advisor

一个面向 `KPI / OKR / 考核方案 / 运营指标` 的个人顾问型 Skill。

它不负责泛泛聊管理，而是专门判断一组目标和指标是否会把团队带偏，重点识别：

- 指标替代目标
- Goodhart 化
- 刷数 / 刷量 / 凑完成率
- 短期最优压死长期价值
- 激励错位
- 局部优化伤害整体
- 报喜不报忧

## 适用场景

适合这类问题：

- 帮我看看这组 KPI / OKR 合不合理
- 这个指标设计会不会跑偏
- 为什么团队很努力但结果越来越怪
- 这份考核方案会诱发什么坏行为
- 这些指标会不会导致刷数、甩锅、短期主义

## 输出风格

这个 Skill 默认采用“判断强、结论先行”的顾问风格：

- 先判断，再解释
- 不端水，不说空话
- 直接指出最危险的问题
- 输出 `保留 / 删除或降权 / 新增护栏` 的修改建议

## 仓库结构

```text
metric-alignment-advisor/
├── README.md
└── metric-alignment-advisor/
    ├── SKILL.md
    └── references/
        └── examples.md
```

## 安装

### 安装到 Codex

```bash
python3 ~/.codex/skills/.system/skill-installer/scripts/install-skill-from-github.py \
  --repo Qianxiao7135/metric-alignment-advisor \
  --path metric-alignment-advisor
```

### 安装到 Claude Code

把 `metric-alignment-advisor/` 目录放到你的用户级 skills 目录下即可，例如：

- `~/.claude/skills/metric-alignment-advisor`

## 核心能力

这个 Skill 会优先回答 5 个问题：

1. 真实目标是什么
2. 当前指标实际在代理什么
3. 哪些地方会 Goodhart 化
4. 会诱发什么行为扭曲
5. 应该删什么、保什么、补什么

## 版本

当前版本：`v1`
