<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version 1.0.0"/>
  <img src="https://img.shields.io/badge/python-3.9+-brightgreen" alt="Python 3.9+"/>
  <img src="https://img.shields.io/badge/dependencies-zero-orange" alt="Zero Dependencies"/>
  <img src="https://img.shields.io/badge/platform-macOS%20%7C%20Linux%20%7C%20Windows-lightgrey" alt="Cross Platform"/>
</p>

# 🏛️ 决策档案馆 — Decision Archives

> **记录你人生所有重要决定，评估结果，生成成长叙事与决策者画像。**

你做决定 → 记下来 → 半年后回来评估 → 系统给你生成**决策者画像**。

---

## 📖 一句话

人生最重要的几十个决定，值得被记住、被复盘、被理解。

---

## 🚀 快速开始

```bash
# 记录一个新决策（交互式）
python3 scripts/decision_archives.py add

# 用参数快速记录（AI 自动模式）
python3 scripts/decision_archives.py add \
  -c career -t "从A跳槽到B" -d "接受了B的offer" \
  -r "B有更好的成长空间" -e "一年技术翻倍" -k high

# 列出所有决策
python3 scripts/decision_archives.py list

# 查看待复盘
python3 scripts/decision_archives.py pending

# 复盘评估一个决策
python3 scripts/decision_archives.py review <id或标题>

# 🧠 成长叙事（核心功能）
python3 scripts/decision_archives.py insights

# 统计概览
python3 scripts/decision_archives.py stats

# 评分排名
python3 scripts/decision_archives.py score
```

---

## 🧠 成长叙事引擎

`insights` 命令输出：

| 项目 | 说明 |
|---|---|
| 决策者类型 | 冒险型 / 谨慎型 / 平衡型 |
| 整体评分 | 所有决策平均准确率（1-5⭐） |
| 最佳/最差 TOP 3 | 哪个决定最对、最错 |
| 各类别准确率 | 可视化条形图，一眼看出你擅长什么 |
| 失误模式分析 | 你在什么类/风险等级下容易翻车 |
| 决策力趋势 | 早期 vs 近期，在进步吗？ |
| 人生时间线 | 你的故事线 |
| 成长金句 | 从教训中提炼的智慧 |

---

## 📂 文件结构

```
decision-archives/
├── SKILL.md                    # 完整文档
├── _meta.json                  # 元数据
├── scripts/
│   └── decision_archives.py   # 核心脚本（纯 stdlib）
└── data/
    └── decisions.json          # 数据持久化（自动创建）
```

---

## ✨ 设计亮点

- **纯 stdlib** — 零外部依赖，Python 3.9+ 开箱即用
- **双模式** — 交互式（人用）和 CLI 参数（AI 用）
- **抗记忆偏差** — 复盘时展示「当初你是怎么想的」
- **跨平台** — macOS / Linux / Windows 全支持
- **数据自持** — 所有数据存在本地 JSON，不联网

---

## 🎯 适合谁

- 想**复盘人生**但不知道从哪开始的你
- 好奇**自己是什么决策者**的你
- 想**减少重复犯错**的你
- 想有一个**人生故事本**的你

---

## 📦 分享版

分享版不含个人数据，适合分享给朋友或团队：

- GitHub: [decision-archives-share](https://github.com/lenkacos-dot/decision-archives-share)
- 本地: `~/Desktop/AI AGENT SKILL/decision-archives-share/`

---

## 📝 License

MIT