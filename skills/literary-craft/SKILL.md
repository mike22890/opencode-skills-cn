---
name: literary-craft
description: 写小说/故事/散文/诗歌/剧本/情书/对话/感官描写/亲密场景时触发。
version: 1.0.0
metadata:
  author: opencode-skills-cn
  tags: literary fiction writing craft style sensory character plot dialogue rhythm intimacy masters
---

# Literary Craft（文学审美）

## 何时触发（看到就调本 skill）

关键词命中即触发：小说、故事、短篇、长篇、文章、散文、随笔、评论、诗歌、古诗、现代诗、剧本、情书、书信、日记、文学、人物、情节、对话、感官、亲密、情欲、描写、禁忌、文风、风格、章回、回、节、幕、角色、人物塑造。

## 信条

1. **暗示 > 直白** —— show don't tell
2. **感官 > 物理** —— 感官细节建立真实感
3. **情感 > 动作** —— 内在驱动外在
4. **留白 > 堆砌** —— 没说比说的更有力
5. **节奏 > 长度** —— 呼吸感 > 字数
6. **大师锚点** —— 学谁像谁，不学谁别写谁

## 速记 6 条

1. **暗示 > 直白**：动作 + 心理暗示，不直说
2. **感官细节**：视觉 / 听觉 / 嗅觉 / 触觉 / 味觉至少用 3 个
3. **节奏呼吸**：长段叙事 + 短句冲击 + 对话加速
4. **留白即力量**：重要的话之前/之后空一行
5. **对话即人**：每个角色说话方式不同
6. **结尾回响**：最后一句呼应开头 / 主题 / 情绪

## 强制自检清单（写完前必过）

- [ ] 感官 ≥ 3 维度（视/听/嗅/触/味）
- [ ] 暗示 > 直白（不直接说"他很悲伤"——让身体语言说）
- [ ] 节奏有起伏（不长不短无变化）
- [ ] 留白用在关键处（不滥用空行）
- [ ] 对话有差异化（不同角色说话不一样）
- [ ] 结尾有力（不烂尾）
- [ ] 自己看 5 秒觉"大师"

## 加载 reference（按场景只加载 1 个）

| 用户说 | 加载 |
|---|---|
| 学谁像谁 / 文风借鉴 / 大师作品 | `reference/masters.md` |
| 写小说 / 故事 / 情节 / 人物 | `reference/techniques.md` |
| 写文章 / 散文 / 随笔 / 评论 / 情书 / 日记 | `reference/forms.md` |
| 亲密场景 / 情欲描写 / 感官细节 / 禁忌情感 | `reference/intimacy.md` |
| BDSM / 虐恋 / 暴力 / 公开场合 / 姿势多样性 / 羞辱 | `reference/power.md` |

## 与其他 skill 的关系

| Skill | 角色 |
|---|---|
| **masterpiece-writing** | 文字审美（文档/教程/报告）—— 偏实用 |
| **literary-craft（本 skill）** | 文学审美（小说/诗歌/散文）—— 偏艺术 |
| **avoid-ai-writing** | AI 腔扫除 —— 所有文字通用 |
| **aesthetics** | 视觉审美 —— 排版/UI |

写文学性内容时通常一起用 masterpiece-writing + literary-craft。

## 精准触发

- `/design X` 不管文学 —— 用 `/design` 是设计场景
- 直接说"写小说/故事/诗" → 自动调本 skill
- 说"亲密/情色/感官描写" → 加载 `reference/intimacy.md`（**专业、克制、不直接生成**）
