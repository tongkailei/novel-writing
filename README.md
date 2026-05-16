# novel-writing

长篇小说创作工作流 / Generic Novel Writing Workflow

---

## 中文说明

### 这是什么？

一个用于连载小说（网文）创作的 Skill 模板。支持系统流、穿越文、废土文等多种类型。

### 触发场景

- "写第X章" → 开始写新章节
- "继续写" → 读上一章，继续剧情
- "写新章节" → 创建新章节文件
- "帮我写小说" → 全流程引导

### 工作流

```
1. 读上一章 → 了解剧情进展
2. 读时间线 → 了解故事 chronology
3. 读角色卡 → 了解人物性格
4. 写章节 → ≥3000字，开头钩子+主线冲突+收尾悬念
5. 更新文件 → 时间线 + 角色卡
```

### 章节结构（每章 ≥3000字）

| 部分 | 占比 | 内容 |
|------|------|------|
| 开头 | 10% | 钩子 + 埋1个开放式悬念 |
| 主线 | 70-80% | 每500字一个"新鲜刺激点"（反转/发现/战斗） |
| 收尾 | 10-15% | 结果 + 回扣开头 + 强力收尾 |

### 文件结构

```
novel-writing/
├── SKILL.md              # Skill 主文件（触发 + 流程 + 模板）
└── references/
    ├── 角色指南.md        # 主角/智者/反派说话方式+微表情
    ├── 世界观指南.md      # 等级体系/穿越设定/环境描写公式
    └── 剧情指南.md        # 英雄之旅12阶段/伏笔系统/节奏检查
```

### 使用提示

- 写之前先读上一章，保持剧情连贯
- 每章写完更新 `时间线.md`
- 新伏笔标记 `[新]`，回收标记 `[x]`
- 系统语录格式：`「检测到...」「翻译：...」`

---

## English Description

### What is this?

A skill template for writing serialized web novels (网络小说). Works with system-gaming, transmigration, post-apocalyptic, and other popular web fiction tropes.

### When to Use

Trigger phrases:
- "Write chapter X" → Start a new chapter
- "Continue" → Read previous chapter, continue the story
- "Write a new chapter" → Create new chapter file
- "Help me write a novel" → Full workflow guidance

### Core Workflow

```
1. Read previous chapter → understand where we left off
2. Read timeline file → understand story chronology
3. Read character files → understand personalities
4. Write chapter → 3000+ words, hook opening + conflict body + cliffhanger ending
5. Update files → timeline + character cards
```

### Chapter Structure (≥3000 words per chapter)

| Part | Ratio | Content |
|------|-------|---------|
| Opening | 10% | Hook + 1 open-ended mystery |
| Body | 70-80% | Fresh stimulation every ~500 words (twist/discovery/combat) |
| Closing | 10-15% | Payoff + strong closing line + setup for next chapter |

### File Structure

```
novel-writing/
├── SKILL.md              # Main skill file (triggers + workflow + templates)
└── references/
    ├── 角色指南.md        # Character voice & micro-expressions guide
    ├── 世界观指南.md      # World-building patterns & level systems
    └── 剧情指南.md        # Hero's Journey 12 stages & plot structure
```

### Usage Tips

- Always read the previous chapter before writing the next one
- Update `时间线.md` (timeline) after each chapter
- Mark new plot threads with `[新]`, resolved threads with `[x]`
- System interjections (if applicable): `「检测到...」「翻译：...」`

---

## 安装 / Installation

将 `novel-writing` 目录放入你的 Agent 技能目录：
```
~/.openclaw/skills/novel-writing/
```

SKILL.md 的 description 字段是主要触发机制。Agent 会自动识别相关触发词并加载技能。

Place the `novel-writing` directory in your agent's skill directory. The `description` field in SKILL.md is the primary trigger mechanism.