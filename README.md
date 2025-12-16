# 學習計畫專案

軟體工程師學習計畫，包含網站開發深化與 AI 應用兩條主線。

## 快速開始

📍 **唯一需要每週看的檔案**: [current_sprint.md](./current_sprint.md)

## 專案結構

```
learning_plan/
├── current_sprint.md        # 當前學習進度 ⭐ 主要看這個
├── claude.md                # AI 協作指南
├── CHANGELOG.md             # 版本紀錄
│
├── tracks/                  # 學習軌道 (各主題學習內容)
│   └── [主題]/
│       ├── README.md       # 目標 + 檢核點
│       └── notes/          # 學習筆記
│
├── projects_withTracks/     # 練習專案 (不靠 AI 手寫)
├── resource_withTracks/     # 學習資源整理
├── advice/                  # Claude 建議紀錄
└── store/                   # 封存文件
```

## 學習軌道 (Tracks)

| 主題 | 優先級 | 說明 |
|------|--------|------|
| [php_oop](./tracks/php_oop/) | 🔴 最高 | PHP 物件導向 |
| [mysql_advanced](./tracks/mysql_advanced/) | 🔴 高 | MySQL 進階 |
| [data_structures](./tracks/data_structures/) | 🟡 中 | 資料結構 |
| [algorithms](./tracks/algorithms/) | 🟡 中 | 演算法 |
| [computer_network](./tracks/computer_network/) | 🟡 中 | 計算機網路 |
| [os_basics](./tracks/os_basics/) | 🟢 低 | 作業系統 |
| [redis](./tracks/redis/) | 🟡 中 | Redis 快取 |
| [docker](./tracks/docker/) | 🟡 中 | Docker 容器 |
| [linux](./tracks/linux/) | 🟡 中 | Linux 基礎 |
| [ai_llm](./tracks/ai_llm/) | 🔴 高 | AI & LLM 應用 |

## 使用方式

1. 每週看 `current_sprint.md` 確認本週目標
2. 學習時在 `tracks/[主題]/notes/` 做筆記
3. 練習時在 `projects_withTracks/` 手寫專案
4. 完成後 `git commit` 記錄進度
5. 有問題問 Claude，建議記錄在 `advice/`

## 版本

請見 [CHANGELOG.md](./CHANGELOG.md)

---
*開始日期: 2025-12-16*
