# Session Log

> 每次 CLI 啟動時必讀此檔案，了解專案進度與待辦事項

---

## Session: 2025-12-14 初始化

### 變更摘要
- 建立專案模板框架
- 建立 CLAUDE.md 主要說明文件
- 建立 `/concept` subagent (概念設計師)
- 建立 `/pm` subagent (專案經理)
- 建立文件模板：PRD.md, TECHSTACK.md, IMPLEMENTATION-PLAN.md
- 建立 log 系統

### 決策記錄
- 採用 `.claude/` 目錄結構管理所有 Claude Code 相關檔案
- Subagent 使用 slash command 方式實作，放在 `.claude/commands/`
- Log 使用累積式 Markdown 格式，每次 session 新增一個區塊
- 工作流程：Concept 先行 → PM 接手規劃 → 動態建立其他 Subagent

### 待辦事項
- [ ] 使用此模板開始新專案時，執行 `/concept` 討論專案概念
- [ ] 更新 CLAUDE.md 中的 `[PROJECT_NAME]`
- [ ] 填寫 PRD.md
- [ ] 填寫 TECHSTACK.md
- [ ] 執行 `/pm` 建立實作計畫

---

## Session: 2025-01-14 16:30

### 變更摘要
- 確立專案方向：「AI 時代最低限度 Coding 技能」學習系統
- 完成 PRD.md：定義逆向學習法、目標用戶、功能需求
- 完成 TECHSTACK.md：定義整合工具（Anki、Heptabase）
- 重寫 CLAUDE.md：完整的學習系統設計
- 建立 learning/ 目錄：curriculum.md（詳細課綱）、progress.json（進度追蹤）、goals.md（學習目標）
- 建立 notes/ 目錄結構（Part1-5）
- 建立 Slash Commands：/teach、/quick、/card、/save、/mentor、/done

### 決策記錄
- **逆向學習法**：不從零學程式，而是從已完成的專案逆向理解原理
- **課綱設計**：5 個 Part，從世界觀到工具鏈，針對 Vibe Coder 的知識空白
- **入門順序**：建議從 Part 1.2（前後端分工）開始，建立整體觀
- **整合現有專案**：用學習者的 Flask app、Next.js 網站當教學素材

### 待辦事項
- [x] 開始第一次學習 session（建議從 `/teach 前端後端` 開始）
- [x] 測試 Heptabase 整合
- [x] 完成系統架構設計

---

## Session: 2025-01-14 21:50

### 變更摘要
- 完成第一次學習 session：Part 1.2 前端 vs 後端 vs 資料庫
- 移除 Anki 整合，改用 Heptabase 統一管理學習內容
- 刪除 `/card` command

### 決策記錄
- **移除 Anki**：簡化工具鏈，用 Heptabase 卡片取代 Anki 卡片
- **知識管理策略**：
  - 筆記存到 `notes/` 目錄（Markdown）
  - 重點存到 Heptabase Journal（自動）
  - 概念卡片存到 Heptabase（可選）

### 學習進度
- Part 1.2 前端後端資料庫：mastery 3（能應用、連結到自己專案）
- 下一步建議：Part 1.3 API

### 待辦事項
- [ ] 繼續學習 Part 1.3 API
- [x] 移除 Anki 相關設定

---

<!-- 新的 session 記錄請加在這裡，格式如下：

## Session: YYYY-MM-DD HH:MM

### 變更摘要
- 完成了什麼

### 決策記錄
- 決定了什麼，為什麼

### 待辦事項
- [ ] 下次要做的事
- [x] 已完成的事（保留追蹤）

-->
