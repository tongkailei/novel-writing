---
name: novel-writing
description: 长篇小说创作工作流skill。当用户说"写第X章"、"继续写"、"写新章节"、"帮我写小说"时触发。适用场景：开始新章节、继续现有章节、构建新世界观、创建新角色卡。流程：读上一章→读时间线→读角色卡→写章节→更新文件。
---

# Novel Writing Skill

Generic novel writing workflow for serialized web fiction.

## Core Workflow

```
1. Read previous chapter → understand where we left off
2. Read timeline file → understand story chronology
3. Read relevant character files → understand personalities
4. Write new chapter → 3000+ words, hook opening, conflict body, cliffhanger ending
5. Update files → timeline, character cards
```

## Chapter Structure

```markdown
# 第X章：标题
[时间/地点标注]

[Scene 1] Opening - hook + setup
[Scene 2] Development - conflict / discovery
[Scene 3] Climax - action / decision
[Scene 4] Resolution - cliffhanger / setup for next

【本章·完】

字数：约3000字
本章收获：
- Key discoveries / items
- Character relationship changes
- New plot threads planted

当前状态：
- Protagonist: level, XP, stamina, location
- Key items
- Relationship status with relevant characters

悬念：
- Questions left unanswered

下一章预告：
```

## Writing Rhythm

- **Opening (10%)**: Hook + 1 open-ended mystery
- **Body (70-80%)**: Fresh stimulation every ~500 words (twist/discovery/combat)
- **Closing (10-15%)**: Payoff + strong closing line

## System Interjections (if story has system)

Use this format for system-style commentary:
```
「检测到异常。」
「分析：……」
「翻译：……建议」
「警告：体力不足。」
```
- System is neutral/cheeky in tone
- "翻译" sections are advice to the protagonist
- Trigger warnings when needed

## File Update Checklist

After writing each chapter:
1. **Chapter file**: `chapters/第X章.md`
2. **Timeline**: `creative-lib/时间线.md` (append new row)
3. **Character cards**: Update `creative-lib/角色/{角色名}.md`
4. **Chapter log** (optional): `creative-lib/章节日志/第X章.md`

## References

- Character voice guide: see `references/角色指南.md`
- World-building patterns: see `references/世界观指南.md`
- Plot structure guide: see `references/剧情指南.md`