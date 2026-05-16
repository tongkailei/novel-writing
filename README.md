# novel-writing

Generic novel writing workflow skill for serialized web fiction (长篇小说创作工作流).

## What is this?

A skill template for writing serialized novels (网文/网络小说). Use when you need to write chapter-by-chapter fiction with a system, characters, and plot tracking.

## When to Use

Trigger phrases:
- "写第X章" (write chapter X)
- "继续写" (continue writing)
- "写新章节" (write a new chapter)
- "帮我写小说" (help me write a novel)

## Core Workflow

```
1. Read previous chapter → understand where we left off
2. Read timeline file → understand story chronology  
3. Read relevant character files → understand personalities
4. Write new chapter → 3000+ words
5. Update files → timeline, character cards
```

## Chapter Structure

Each chapter ≥ 3000 words:

- **Opening (10%)**: Hook + 1 open-ended mystery
- **Body (70-80%)**: Fresh stimulation every ~500 words (twist/discovery/combat)
- **Closing (10-15%)**: Payoff + strong closing line + cliffhanger for next chapter

## File Structure

```
novel-writing/
├── SKILL.md               # Main skill file
└── references/
    ├── 角色指南.md         # Character voice & micro-expressions
    ├── 世界观指南.md       # World-building patterns & level systems
    └── 剧情指南.md         # Hero's Journey stages & plot structure
```

## Skills for Codex

Place in your agent's skill directory:
```
~/.openclaw/skills/novel-writing/
```

The `SKILL.md` description field is the primary trigger mechanism. Codex will automatically load the skill when relevant phrases are detected.

## Tips

- Always read previous chapter before writing next
- Keep timeline updated after each chapter
- Mark new plot threads with `[新]`, mark resolved with `[x]`
- System interjections (if applicable) use `「」` brackets with analysis/translation format