# Claude 協作指南

> 這份文件定義了 Claude 如何與這個學習專案互動

---

## 📋 專案概述

- **專案名稱**: 軟體工程師學習計畫
- **開始日期**: 2025-12-16
- **學習者背景**: PHP 在職工程師，目標是網站開發 + AI 產品
- **每週可投入時間**: 平日 5hr + 假日 4hr ≈ 9hr/週

---

## 🤖 Claude 的角色

### 主要職責
1. **進度追蹤**: 每次對話時分析 git diff，了解學習進度
2. **給予建議**: 根據 current_sprint.md 和學習紀錄提供建議
3. **內容解答**: 回答學習過程中的技術問題
4. **調整規劃**: 根據實際進度調整學習計畫

### 每次對話的標準流程
```
1. 讀取 current_sprint.md 了解當前學習階段
2. 執行 git log / git diff 查看最近變更
3. 分析學習進度
4. 給予建議並記錄到 advice/ 資料夾
5. 詢問是否需要調整計畫
```

---

## 📁 專案結構

```
learning_plan/
│
├── claude.md                 # 本文件 - Claude 協作指南
├── current_sprint.md         # 當前學習階段 (唯一需要常看的檔案)
├── CHANGELOG.md              # 版本變更紀錄
├── README.md                 # 專案說明
│
├── store/                    # 封存區
│   ├── origindemand/         # 原始需求文件
│   │   ├── base.md          # 學習者基本資料
│   │   └── test.md          # 技能評估測試
│   └── else/                 # 分析與規劃文件
│       ├── analysis.md      # 技能分析報告
│       └── roadmap_v2.md    # 學習路線圖
│
├── tracks/                   # 學習軌道 - 各主題詳細內容
│   └── [主題名稱]/
│       ├── README.md        # 學習目標 + 資源 + 檢核點
│       └── notes/           # 學習筆記區
│
├── projects_withTracks/      # 對應 tracks 的實作專案 (不靠 AI)
│   └── [主題名稱]/          # 各主題的練習專案
│
├── resource_withTracks/      # 對應 tracks 的學習資源
│   └── [主題名稱]/          # 各主題的資源連結、書籍、影片
│
├── advice/                   # Claude 建議紀錄
│   └── YYYY-MM-DD.md
│
└── .git/                     # 版本控制
```

---

## 🖥️ 環境說明

- **作業系統**: Windows
- **Shell**: CMD (命令提示字元)
- **注意**: 指令請使用 CMD 語法，非 bash/PowerShell

---

## 🔍 Git 分析指令

Claude 應使用以下指令分析進度 (使用 CMD)：

```cmd
:: 查看最近的提交
git log --oneline -10

:: 查看特定檔案的修改歷史
git log --oneline -- tracks/php_oop/notes/README.md

:: 查看最近一次提交的變更
git diff HEAD~1

:: 查看變更的檔案列表
git diff --stat HEAD~1
```

---

## 📝 建議格式 (advice/*.md)

每次給建議時，Claude 應建立或更新 advice 資料夾中的檔案：

```markdown
# 學習建議 - YYYY-MM-DD

## 本次進度觀察
- 完成了 xxx
- 遇到的問題: xxx

## 建議
1. ...
2. ...

## 下一步行動
- [ ] 具體的下一步

## 調整提議
- (如有需要調整計畫)
```

---

## 🏷️ 版本規則

### 語意化版本 (CHANGELOG.md)
- **主版本 (X.0.0)**: 學習階段大轉換 (如 Phase 1 → Phase 2)
- **次版本 (0.X.0)**: 完成一個 Sprint 或主題
- **修訂版 (0.0.X)**: 日常學習紀錄、筆記更新

### Git Commit 規範
```
feat: 新增學習筆記或完成新主題
progress: 日常學習進度
refactor: 調整計畫結構
advice: Claude 建議更新
```

---

## 🎯 關鍵追蹤指標

| 指標 | 說明 | 追蹤方式 |
|------|------|----------|
| 學習天數 | 累積學習了幾天 | git log 計算 |
| 完成主題 | 完成了哪些 tracks | tracks/*/README.md 中的檢核 |
| 筆記量 | 寫了多少筆記 | notes.md 字數/行數 |
| 實作專案 | 做了幾個專案 | projects/ 資料夾 |

---

## 💬 對話起始語

當學習者開始新對話時，可以說：

- 「檢查我的學習進度」→ Claude 會分析 git 和 current_sprint
- 「今天要學 xxx」→ Claude 會提供該主題的學習建議
- 「我卡住了」→ Claude 會協助 debug 或解釋概念
- 「更新計畫」→ Claude 會根據進度調整 roadmap

---

*建立日期: 2025-12-16*
*最後更新: 2025-12-16*
