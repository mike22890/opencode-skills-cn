# OpenCode Skills CN

> 中文优先的 AI Agent Skills 集合——为中文场景优化的触发词 + 12 个领域的方法论。

A collection of Chinese-first agent skills for [OpenCode](https://opencode.ai), [Claude Code](https://claude.ai/code), [Codex CLI](https://github.com/openai/codex), and any agent that supports the [Agent Skills](https://agentskills.io) standard.

---

## 为什么是这套

市面上的 skills 几乎全是英文触发词——你说"搞个文档"，它们无感；说"write a doc"，才反应过来。

这套不一样：

- **中文口语触发**——"搞个文档"/"分析下心理"/"扫下安全"，直接命中
- **独特领域**——读心师心理学、财富规划、哲学智慧，外面没有
- **方法论分层**——每个 skill = SKILL.md（速查）+ reference/（按需深挖）
- **精简**——41 个 description 总开销 < 3K 字符，不烧 token

---

## Skills 清单

| Skill | 用途 |
|---|---|
| **aesthetics** | 任何"给人看"的产出：UI/配色/字体/Logo/动效/排版/PPT/海报/文档/简历/图表 |
| **psychology-mastery** | 读心师级心理洞察：微表情/操控识别/依恋分析/自我分析/关系动力学 |
| **code-mastery** | 代码审美：命名/函数/注释/错误处理/性能 + 链式 simplify→refactor |
| **thinking-craft** | 思考决策：第一性原理/认知偏差/决策框架/黑天鹅/贝叶斯 |
| **system-design** | 系统架构：微服务/数据库/缓存/分布式/CAP/高并发/可观测性 |
| **product-strategy** | 产品商业：PMF/商业模式/增长/护城河/LTV/CAC/单位经济 |
| **persuasion-craft** | 表达说服：故事框架/影响力法则/谈判技巧/演讲锚点 |
| **wisdom-philosophy** | 哲学智慧：斯多葛/存在主义/禅/道/儒家/伦理决策 |
| **wealth-mastery** | 财富规划：复利/资产配置/经济周期/人生阶段策略/行动清单 |
| **masterpiece-writing** | 文档审美：README/设计文档/ADR/报告/教程的排版铁律 |
| **literary-craft** | 文学写作：小说/散文/诗歌/对话/感官描写/亲密场景（专业克制） |
| **mermaid-diagram-generator** | 图表生成：流程图/时序图/类图/状态图/ER图/甘特图 |

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
"分析下他为什么这样"   → psychology-mastery
"这段代码重构下"       → code-mastery
"设计个订单系统"       → system-design
"这个产品怎么定价"     → product-strategy
"写个 README"          → masterpiece-writing
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
├── SKILL.md           # 触发描述 + 核心方法 + 速查卡
└── reference/         # 按需加载的深度内容
    ├── xxx.md
    └── yyy.md
```

**设计原则**：SKILL.md 保持精简（触发时必读），深度内容拆到 reference（按需加载）——token 效率优先。

---

## License

MIT

---

## 致谢

方法论参考：Paul Graham / Charlie Munger / Chris Voss / Joe Navarro / Robert Cialdini / Edward Tufte / 曹雪芹 / 张爱玲 / 等。

Skill 格式基于 [Agent Skills](https://agentskills.io) 开放标准。
