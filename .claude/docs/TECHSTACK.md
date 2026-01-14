# 技術棧 (Tech Stack)

> 由 `/concept` 維護

---

## 總覽

本專案是一個**學習系統**，不是傳統的軟體開發專案。主要依賴 Claude Code 的 Subagent 架構，整合外部工具進行知識管理。

---

## 核心架構

### AI 引擎
- **Claude Code CLI** - 主要互動介面
- **Subagent 系統** - 透過 `.claude/commands/` 實作不同學習模式

### 知識管理整合

| 工具 | MCP Server | 用途 |
|------|------------|------|
| **Anki** | yanki-mcp-server | 記憶卡片、間隔重複 |
| **Heptabase** | heptabase-mcp | 知識圖譜、學習日誌 |

---

## 資料結構

### 學習追蹤
```
learning/
├── progress.json      # 學習進度（自動更新）
├── curriculum.md      # 詳細課綱
└── goals.md           # 學習目標
```

### 筆記輸出
```
notes/
├── Part1-WorldView/   # 程式世界觀
├── Part2-MyProjects/  # 專案逆向理解
├── Part3-AICollab/    # AI 協作技能
├── Part4-Security/    # 安全意識
└── Part5-Toolchain/   # 工具鏈素養
```

---

## 學習素材來源

### 學習者的專案（逆向教學素材）

| 專案 | 技術 | 教學價值 |
|------|------|----------|
| wilsonchao.com | Next.js, TypeScript | 前端、組件、路由 |
| 個人訊息流強化 | Python, Flask, API | 後端、函數、環境變數 |
| yt-readwise-telegram-bridge | Node.js | 套件管理、模組 |
| 心臟外科學習教師 | Claude Code, MCP | Subagent 設計 |

路徑：`C:\Users\Yuru Hung\Desktop\Project\`

---

## Anki 整合

### 連線需求
- Anki 桌面版執行中
- Anki-Connect 外掛 (2055492159)

### 卡片標籤格式
```
Coding::[Part]::[Topic]
```

範例：
- `Coding::Part1-WorldView::API`
- `Coding::Part2-MyProjects::Flask`
- `Coding::Part4-Security::APIKey`

---

## Heptabase 整合

### 寫入功能
- **Journal**：每次學習結束自動記錄
- **卡片**：重要概念可選擇存入

### 讀取功能
- 搜尋既有的程式相關筆記
- 連結到其他知識領域

---

## 版本控制

- Git（本地）
- 可選：推送到 GitHub

---

## 選擇原因

| 技術 | 選擇原因 |
|------|----------|
| Claude Code | 學習者已熟悉，無需額外學習新工具 |
| Subagent | 可分離不同學習模式，各司其職 |
| Anki | 學習者已在使用，記憶效果佳 |
| Heptabase | 學習者已在使用，視覺化知識連結 |
| Markdown | 簡單、可版本控制、跨平台 |

---

## 變更記錄

| 日期 | 變更內容 |
|------|----------|
| 2025-01-14 | 初版建立 |
