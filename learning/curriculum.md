# AI 時代 Coding 學習課綱

> 為 Vibe Coder 設計的「逆向學習」課綱
> 目標：從「能跑就好」進階到「知道為什麼」

---

## Part 1：程式世界觀（心智模型）

**學習目標**：建立正確的心智模型，理解程式運作的基本架構

### 1.1 電腦如何執行程式
- [ ] 程式碼 → 執行的過程
- [ ] 編譯語言 vs 直譯語言
- [ ] 為什麼需要「執行環境」

### 1.2 前端 vs 後端 vs 資料庫
- [ ] 三者的分工
- [ ] 瀏覽器裡發生什麼事
- [ ] 伺服器裡發生什麼事
- [ ] 你的專案在哪一層？

### 1.3 API 是什麼
- [ ] API 的比喻：餐廳點餐
- [ ] HTTP 請求與回應
- [ ] GET, POST 的差異
- [ ] JSON 格式
- [ ] 實例：你的 Telegram Bot 如何收發訊息

### 1.4 程式語言的共同概念
- [ ] 變數：存放資料的盒子
- [ ] 函數：可重複使用的指令集
- [ ] 條件判斷：if/else
- [ ] 迴圈：重複執行
- [ ] 資料結構：列表、字典

---

## Part 2：看懂你的專案（逆向理解）

**學習目標**：能看懂自己寫過的程式碼，理解每一行在做什麼

### 2.1 Python 基礎
- [ ] import 是什麼：把別人寫好的工具拿來用
- [ ] 函數定義：def
- [ ] 參數與回傳值
- [ ] 實例：解讀你的 `app.py`

### 2.2 JavaScript 基礎
- [ ] 變數：let, const, var 的差異
- [ ] 函數：傳統 vs 箭頭函數
- [ ] 物件與陣列
- [ ] async/await：非同步的概念
- [ ] 實例：解讀你的 Next.js 組件

### 2.3 框架概念
- [ ] 什麼是框架？為什麼需要？
- [ ] Flask 路由：`@app.route()` 在做什麼
- [ ] Next.js 組件：React 的基本概念
- [ ] 為什麼框架幫你處理了很多事

### 2.4 環境變數與 Secrets
- [ ] 為什麼需要 `.env`
- [ ] `os.getenv()` 和 `process.env`
- [ ] `.gitignore` 的重要性
- [ ] 實例：你的 API keys 是怎麼保護的

---

## Part 3：AI 協作技能

**學習目標**：更有效地與 AI 協作，從「Vibe Coding」進化到「Human-Agent Engineering」

> **參考課程**：
> - [Claude Code in Action](https://anthropic.skilljar.com/claude-code-in-action) (Anthropic 官方)
> - [CS146S: The Modern Software Developer](https://themodernsoftware.dev/) (Stanford)

---

### Module A：基礎協作

#### 3.1 如何描述需求給 AI
- [ ] 好的 prompt vs 壞的 prompt
- [ ] 提供足夠的 context
- [ ] 分步驟請求 vs 一次性請求
- [ ] 實例：重寫你過去的需求描述

#### 3.2 如何讀懂 AI 輸出
- [ ] 快速掃描程式碼結構
- [ ] 看懂函數名稱和註解
- [ ] 識別關鍵邏輯
- [ ] 不需要 100% 理解，但要抓重點

#### 3.3 常見錯誤類型與除錯
- [ ] 語法錯誤 (SyntaxError)
- [ ] 類型錯誤 (TypeError)
- [ ] 找不到模組 (ModuleNotFoundError)
- [ ] 權限錯誤、網路錯誤
- [ ] 如何讀錯誤訊息
- [ ] 定位問題範圍
- [ ] 如何向 AI 描述問題

#### 3.4 判斷何時介入、何時信任
- [ ] AI 可能犯錯的情況
- [ ] 安全相關的警覺點
- [ ] 「這看起來怪怪的」直覺
- [ ] 何時該自己試、何時該問 AI

---

### Module B：Claude Code 實戰

> 來源：[Claude Code in Action](https://anthropic.skilljar.com/claude-code-in-action)

#### 3.5 Claude Code 核心概念
- [ ] 架構與工作原理
- [ ] 上下文管理（/init、Claude.md、@提及）
- [ ] 核心工具：文件操作、命令執行、代碼分析
- [ ] 實例：你的學習系統是如何設計的

#### 3.6 對話與模式控制
- [ ] 快捷鍵與命令
- [ ] Plan Mode（規劃模式）：複雜任務的拆解
- [ ] Think Mode（思考模式）：深度分析
- [ ] 實例：用 Plan Mode 規劃一個功能

#### 3.7 自定義命令與 Hooks
- [ ] Slash Commands 的設計原理
- [ ] 建立個人化工作流
- [ ] Hooks：自動化行為觸發
- [ ] 實例：你的 /teach、/mentor 是怎麼運作的

#### 3.8 MCP 服務器與擴展
- [ ] 什麼是 MCP（Model Context Protocol）
- [ ] MCP 服務器的概念
- [ ] 實例：Heptabase MCP、GitHub MCP
- [ ] 瀏覽器自動化等進階應用

---

### Module C：代理架構與進階

> 來源：[CS146S: The Modern Software Developer](https://themodernsoftware.dev/)

#### 3.9 Coding Agent 原理
- [ ] 代理（Agent）是什麼
- [ ] 代理如何使用工具（Tool Use）
- [ ] 工具調用機制
- [ ] 為什麼理解這些能讓你更有效協作

#### 3.10 AI 輔助測試
- [ ] AI 生成測試的概念
- [ ] 安全漏洞自動檢測
- [ ] 測試覆蓋率與品質
- [ ] 何時該信任 AI 測試、何時該人工檢查

#### 3.11 AI 程式碼審查
- [ ] GitHub PR 自動審查概念
- [ ] AI 審查能發現什麼、會漏掉什麼
- [ ] 品質控制策略
- [ ] 實例：設定 GitHub 整合

#### 3.12 Human-Agent 協作模式
- [ ] 從「Vibe Coding」到「Human-Agent Engineering」
- [ ] 核心理念：你是 AI 團隊的經理
- [ ] 設置代理成功的環境（清晰 context、結構化程式碼）
- [ ] 多代理協作的概念
- [ ] 未來展望：軟體工程師的角色演變

---

## Part 4：安全與風險意識

**學習目標**：知道什麼是危險的，能問「這樣安全嗎？」

### 4.1 API Key 管理
- [ ] API key 是什麼
- [ ] 洩漏的後果（真實案例）
- [ ] 正確的保護方式
- [ ] 如果不小心 commit 了怎麼辦

### 4.2 常見安全漏洞
- [ ] SQL Injection：概念與防範
- [ ] XSS（跨站腳本）：概念與防範
- [ ] CSRF：概念與防範
- [ ] 為什麼「永遠不要信任使用者輸入」

### 4.3 權限與存取控制
- [ ] 最小權限原則
- [ ] 檔案權限基礎
- [ ] 資料庫權限
- [ ] 雲端服務權限

### 4.4 安全警覺時機
- [ ] 「這樣安全嗎？」檢查清單
- [ ] 處理敏感資料時
- [ ] 接受使用者輸入時
- [ ] 部署到公開網路時

---

## Part 5：工具鏈素養

**學習目標**：熟悉開發工具，不再害怕終端機和 Git

### 5.1 Git 基本概念
- [ ] 為什麼需要版本控制
- [ ] 本地 vs 遠端
- [ ] commit, push, pull
- [ ] branch 的概念
- [ ] 實例：你現在的專案如何使用 Git

### 5.2 終端機基礎
- [ ] 為什麼需要終端機
- [ ] 基本導航：cd, ls, pwd
- [ ] 檔案操作：cp, mv, rm
- [ ] 不怕黑畫面的心態

### 5.3 套件管理
- [ ] 什麼是套件/依賴
- [ ] npm (Node.js) 基礎
- [ ] pip (Python) 基礎
- [ ] package.json / requirements.txt
- [ ] 為什麼有時候「裝不起來」

### 5.4 部署概念
- [ ] 本地開發 vs 部署上線
- [ ] Zeabur / Vercel / Railway 在做什麼
- [ ] 環境變數在部署時的角色
- [ ] 基本的除錯：看 logs

---

## 學習路徑建議

### 入門順序（建議）

1. **Part 1.2** - 先理解前後端分工（建立整體觀）
2. **Part 1.3** - API 概念（這是你專案的核心）
3. **Part 2.1** - 看懂你的 Python 專案
4. **Part 4.1** - API Key 安全（立即可用）
5. **Part 5.1** - Git 基礎（你已經在用了）

### Part 3 學習路徑

Part 3 已擴充為三個模組，建議按順序學習：

1. **Module A（3.1-3.4）**：基礎協作 — 建立 AI 協作的基本心智模型
2. **Module B（3.5-3.8）**：Claude Code 實戰 — 實際操作，邊做邊學
3. **Module C（3.9-3.12）**：代理架構與進階 — 理解底層原理，成為進階使用者

### 按需學習

遇到問題時查閱對應章節，不需要從頭到尾讀完。

---

## 進度追蹤

詳見 `learning/progress.json`

---

*最後更新：2025-01-16*
*Part 3 擴充：整合 Claude Code in Action + CS146S 課程內容*
