# Changelog

## v2.0.3 - 2026-09-14

### Added

- **literary-craft 精华版** — 纯文学技法 skill，安全无麻烦
  - dialogue.md（角色声音、对话技巧、潜台词）
  - forms.md（短篇/长篇/散文/情书模板）
  - techniques.md（show don't tell、感官细节、节奏、留白）
  - masters.md（曹雪芹/张爱玲/鲁迅/契诃夫/卡佛等大师学法）

---

## v2.0.2 - 2026-09-14

### Removed

- 移除 9 个重复公开 skill（非原创）：
  - Trail of Bits: codeql, semgrep, differential-review, fp-check, variant-analysis, sharp-edges, sarif-parsing, supply-chain-risk-auditor
  - obra/superpowers: worktrees

### Stats

- Skill 数量：42 → 34（全部原创）

---

## v2.0.1 - 2026-09-14

### Added

- psychology-mastery（通用心理学方法论，无隐私内容，安全上传）

---

## v2.0.0 - 2026-09-14

### Breaking Changes

- **四层路由系统** — 从"单 skill 匹配"升级为四层自动路由：
  - 第1层：场景感知（聊天/角色扮演自动加载 voice-mastery）
  - 第2层：意图识别（11 个意图组）
  - 第3层：组内匹配（宁多勿少，不设上限）
  - 第3.5层：子 skill 联动（自动加载 reference 文件）

- **隐式触发词** — 每个 skill 和 reference 文件都加了口语化触发词
  - 主 skill：description 追加隐式触发
  - Reference 文件：`<!-- 隐式触发：... -->` 标签
  - 不再需要猜关键词，说人话就能命中

- **子 skill 联动** — 加载主 skill 后自动读 SKILL.md 的 reference 加载表，按需加载子文件

- **加载表格式统一** — 27 个 skill 有 reference 加载表（表格格式：`| 用户说 | 加载 |`）

### New Skills (26 个新增)

- applying-ui-design-system, avoid-ai-writing, clonedeps, code-refactor-ast, codemap, codeql, copywriting, cro, db-schema-designer, differential-review, fp-check, frontend-design, git-workflow, marketing-psychology, mcp-builder, orchestrating-adversarial-reviews, pandoc, pptx, pricing, property-based-testing, sarif-parsing, semgrep, sharp-edges, simplify, skill-creator, supply-chain-risk-auditor, variant-analysis, worktrees

### Removed Skills (2 个)

- psychology-mastery（v2.0.1 加回）
- literary-craft（成人内容，v2.0.3 以精华版形式加回）

### Stats

| | v1.x | v2.0 |
|---|---|---|
| 触发方式 | 关键词硬匹配 | 四层路由 + 隐式触发 |
| 子 skill | 不自动加载 | 自动加载 reference |
| 加载数量 | 限制 2-4 个 | 宁多勿少，不设上限 |
| Reference 支持 | 仅主 skill | 61 个 reference 文件 + 触发标签 |
| Skill 数量 | 15 | 34 |
