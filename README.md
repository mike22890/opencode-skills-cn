# OpenCode Skills CN

![GitHub stars](https://img.shields.io/github/stars/mike22890/opencode-skills-cn?style=social)
![License](https://img.shields.io/github/license/mike22890/opencode-skills-cn)
![Skills](https://img.shields.io/badge/skills-40-blue)
![Version](https://img.shields.io/badge/version-v4.0.0-green)
![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen)

> 中文优先的 AI Agent Skills 集合——40 个原创领域方法论，四层路由自动匹配，口语化触发词无需猜关键词。

A collection of 40 original agent skills for [OpenCode](https://opencode.ai), [Claude Code](https://claude.ai/code), [Codex CLI](https://github.com/openai/codex), and any agent that supports the [Agent Skills](https://agentskills.io) standard.

---

## 为什么是这套

市面上的 skills 几乎全是英文触发词——你说"搞个文档"，它们无感；说"write a doc"，才反应过来。

这套不一样：

- **中文口语触发**——"搞个文档"/"分析下心理"/"扫下安全"，直接命中
- **四层路由**——场景感知→意图识别→组内匹配→子 skill 联动，自动选+自动加载
- **隐式触发词**——每个 skill 和 reference 都有口语化触发词，不用猜关键词
- **方法论分层**——每个 skill = SKILL.md（速查）+ reference/（按需深挖）
- **40 个原创 skill**——全部自己写，无公开重复

---

## 四层路由

```
第1层：场景感知 → 聊天/角色扮演自动加载 voice-mastery
第2层：意图识别 → 11 个意图组（文字/代码/视觉/搜索/安全/认知/营销/工具/聊天/元技能/验证）
第3层：组内匹配 → 所有匹配的都加载，宁多勿少，不设上限
第3.5层：子 skill 联动 → 读 SKILL.md 加载表 → 自动加载 reference 文件
```

---

## Skills 清单

### 写作/创作（6）

| Skill | 用途 |
|---|---|
| **literary-craft** | 文学写作：小说/散文/诗歌/对话/感官描写/大师学法 |
| **humanize-fiction** | 反 AI 味写作：18 个 AI 味特征 + 修复 |
| **story-endings** | 结局写作：8 个 AI 味结局问题 + 8 种好结局 |
| **copywriting** | 营销文案：落地页/广告/SEO/品牌故事/slogan |
| **masterpiece-writing** | 文档审美：README/设计文档/ADR/报告/教程排版 |
| **avoid-ai-writing** | 去 AI 腔：检测并消除文字中的 AI 生成痕迹 |

### 代码/工程（8）

| Skill | 用途 |
|---|---|
| **code-mastery** | 代码审美：命名/函数/注释/错误处理/性能 + 链式触发 |
| **code-refactor-ast** | AST 重构：大规模架构解耦/拆函数/提取接口/DRY |
| **simplify** | 代码简化：降复杂度/消重复/提可读性/清理 |
| **codemap** | 代码地图：项目层级架构/新人 onboarding/快速了解 |
| **db-schema-designer** | 数据库设计：schema/ORM/索引/迁移安全/查询优化 |
| **frontend-design** | 前端设计：视觉方向/排版/配色/反 AI 模板化 |
| **git-workflow** | Git 工作流：commit/PR/分支管理/冲突解决/发布 |
| **github-workflow** | GitHub 全流程：release/changelog/tag/PR/Actions/隐私保护 |

### 思考/决策（4）

| Skill | 用途 |
|---|---|
| **thinking-craft** | 思考决策：第一性原理/认知偏差/决策框架/黑天鹅/贝叶斯 |
| **research-mastery** | 搜索研究：信息搜索/信源分级/事实核查/整理 |
| **life-planning** | 人生规划：五维盘点/价值观澄清/目标拆解/行动系统 |
| **wisdom-philosophy** | 哲学智慧：斯多葛/存在主义/禅/道/儒家/伦理决策 |

### 商业/产品（5）

| Skill | 用途 |
|---|---|
| **product-strategy** | 产品策略：PMF/商业模式/增长/护城河/LTV-CAC |
| **pricing** | 定价策略：套餐设计/锚定/SaaS 定价/订阅/变现 |
| **cro** | 转化率优化：A/B 测试/漏斗/表单/按钮/增长实验 |
| **marketing-psychology** | 营销心理：影响力法则/锚定/损失厌恶/FOMO/定价心理 |
| **persuasion-craft** | 表达说服：故事/影响力/谈判/演讲/TED Pitch |

### 自我提升（4）

| Skill | 用途 |
|---|---|
| **psychology-mastery** | 心理洞察：微表情/操控识别/依恋分析/自我分析 |
| **wealth-mastery** | 财富规划：复利/资产配置/经济周期/人生阶段策略 |
| **self-edit** | 自动审查：AI 产出后自动检查并修复问题 |
| **long-task** | 长任务管理：防降级/状态保持/断点续传 |

### 工具/效率（8）

| Skill | 用途 |
|---|---|
| **aesthetics** | 视觉审美：UI/配色/字体/Logo/排版/PPT/海报/文档/图表 |
| **mermaid-diagram-generator** | 图表生成：流程图/时序图/类图/状态图/ER图 |
| **pandoc** | 文档转换：md↔docx/pdf/html/epub/latex 互转 |
| **pptx** | PPT 制作：幻灯片/演示文稿/Pitch/培训课件 |
| **mcp-builder** | MCP 开发：创建工具/对接外部 API/标准化接口 |
| **skill-creator** | Skill 开发：创建/测试/优化 agent skill |
| **shopping-advisor** | 购物顾问：选品/对比/性价比/避坑/购买时机 |
| **privacy-guard** | 隐私保护：PII 检查/脱敏/GitHub 上传前安全扫描 |

### 高级（1）

| Skill | 用途 |
|---|---|
| **orchestrating-adversarial-reviews** | 对抗审查：多 agent 交叉验证/红蓝演练 |

---

## 安装

### OpenCode

```bash
# 全局安装（所有项目可用）
cp -r skills/* ~/.config/opencode/skills/

# 或只装一个
cp -r skills/aesthetics ~/.config/opencode/skills/
```

### Claude Code

```bash
cp -r skills/* ~/.claude/skills/
```

### 其他 Agent

Skills 遵循 [agentskills.io](https://agentskills.io) 标准——把 `skills/` 里的目录放进对应 agent 的 skills 目录即可：

```
~/.codex/skills/     # Codex CLI
~/.cursor/skills/    # Cursor
~/.gemini/skills/    # Gemini CLI
~/.agents/skills/    # 通用
```

---

## 使用

装好后直接说话，触发词自动命中：

```
"搞个落地页"           → aesthetics
"这段代码重构下"       → code-mastery + code-refactor-ast + simplify
"设计个订单系统"       → system-design
"这个产品怎么定价"     → pricing + marketing-psychology
"写个 README"          → masterpiece-writing + aesthetics
"写个小说"             → literary-craft + humanize-fiction + story-endings
"发个 release"         → github-workflow
```

多 skill 联动（在 agent 的 AGENTS.md 里配好规则后）：

```
"搞个文档" → masterpiece-writing + aesthetics + avoid-ai-writing
"做个 PPT" → pptx + aesthetics + persuasion-craft
```

---

## 结构

每个 skill 遵循统一结构：

```
skills/<name>/
├── SKILL.md           # 触发描述 + 核心方法 + 速查卡 + 子 skill 路由表
└── reference/         # 按需加载的深度内容（含隐式触发标签）
    ├── xxx.md
    └── yyy.md
```

**设计原则**：SKILL.md 精简（触发时必读），深度内容拆到 reference（按需加载）——token 效率优先。

---

## Changelog

见 [CHANGELOG.md](CHANGELOG.md)

---

## Related

- [opencode-skills-en](https://github.com/mike22890/opencode-skills-en) — English edition

---

## License

MIT

---

## 致谢

方法论参考：Paul Graham / Charlie Munger / Chris Voss / Joe Navarro / Robert Cialdini / Edward Tufte / 曹雪芹 / 张爱玲 / 等。

Skill 格式基于 [Agent Skills](https://agentskills.io) 开放标准。
