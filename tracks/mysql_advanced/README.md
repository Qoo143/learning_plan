# MySQL 進階

> 學習優先級: 🔴 **高** (你說這是最弱的)
> 預計時間: 4 週 (Sprint 5-8)
> 你的起點: MySQL 平均 1.8/5 分

---

## 🎯 學習目標

完成後你應該能：
- [ ] 熟練使用各種 JOIN
- [ ] 用 EXPLAIN 分析查詢效能
- [ ] 設計適當的索引
- [ ] 理解 Transaction 和鎖

---

## 📚 學習資源

| 資源 | 類型 | 重點 |
|------|------|------|
| MySQL 官方文檔 - Optimization | 文檔 | 索引、查詢優化 |
| 工作環境慢查詢日誌 | 實戰 | 分析實際案例 |
| Use The Index, Luke | 網站 | 索引觀念經典 |

---

## 📅 週計畫

### Sprint 5 (W5): JOIN 精通
- [ ] INNER JOIN
- [ ] LEFT/RIGHT JOIN
- [ ] 多表連接
- [ ] 自連接 (Self Join)

### Sprint 6 (W6): 索引原理
- [ ] B-Tree 索引結構
- [ ] 複合索引順序
- [ ] EXPLAIN 使用
- [ ] 索引失效情況

### Sprint 7 (W7): 查詢優化
- [ ] 避免 SELECT *
- [ ] N+1 問題
- [ ] 子查詢 vs JOIN
- [ ] LIMIT 優化

### Sprint 8 (W8): 交易與鎖
- [ ] Transaction ACID
- [ ] 隔離級別
- [ ] 死鎖排查
- [ ] 樂觀鎖 vs 悲觀鎖

---

## ✅ 檢核點

| 檢核項目 | 通過標準 | 狀態 |
|----------|----------|------|
| 複雜 JOIN | 能寫 3 表以上的 JOIN 查詢 | [ ] |
| EXPLAIN 分析 | 能解讀 EXPLAIN 輸出並提出優化建議 | [ ] |
| 慢查詢優化 | 優化一個工作中的慢查詢 | [ ] |
| Transaction | 能正確使用 Transaction 處理業務邏輯 | [ ] |

---

*建立日期: 2025-12-16*
