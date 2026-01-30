# 团队 Claude Code Skills 共享库

团队共享的 Claude Code skills，方便复用和协作。

## 快速开始

### 安装

```bash
git clone https://github.com/370283761/Claude-skills.git ~/.claude/skills/team
```

### 更新

```bash
cd ~/.claude/skills/team && git pull
```

## 可用 Skills

| Skill | 用途 | 命令 |
|-------|------|------|
| PRD 生成器 | 快速生成以用户体验为核心的产品需求文档 | `/team:prd-generator` |

## 使用示例

```
/team:prd-generator 用户评论功能
```

或带详细描述：

```
/team:prd-generator 电商APP的商品收藏功能，解决用户找不到心仪商品的问题
```

## 目录结构

```
Claude-skills/
├── README.md           # 本文件
└── skills/
    └── prd-generator/  # PRD 生成器 skill
        └── skill.md
```

## 如何贡献新 Skill

1. 在 `skills/` 目录下创建新文件夹
2. 添加 `skill.md` 文件（参考现有 skill 格式）
3. 更新本 README 的 skill 列表
4. 提交 PR

## Skill 文件格式

```markdown
---
name: skill-name
description: 触发描述
metadata:
  author: your-name
  version: "1.0.0"
---

# Skill 标题

## 使用场景
...

## 工作流程
...
```
