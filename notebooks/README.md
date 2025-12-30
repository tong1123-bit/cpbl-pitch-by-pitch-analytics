# Notebooks Overview

本資料夾包含本研究之核心分析流程，建議依照編號順序閱讀。

---

## 01_build_features_shift_eligible.ipynb
**資料整理與特徵建構（研究起點）**

- 整理 CPBL 逐球資料
- 建構打者層級行為與情境化特徵
- 定義「值得進行守備佈陣分析之打者」
- 輸出後續分析與建模所需的彙總特徵表

👉 本 notebook 為後續所有分析的資料基礎。

---

## 02_visualizations_pitcher_quadrant_batter_card.ipynb
**解釋性視覺化與案例展示**

- 投手滾地球比例（GB%）四象限分析
- 打者行為特徵與情境化表現視覺化
- 輸入打者姓名產生 Batter Card（球員卡）

👉 用於說明模型結果的棒球意義與戰術直覺。

---

## 03_step2_models_comparison.ipynb
**打者層級分類模型與比較（核心成果）**

- 建立打者層級擊球落點集中性分類模型
- 比較 Logistic Regression、Random Forest、XGBoost
- 評估指標包含 ROC-AUC、F1-score、Accuracy
- 作為守備佈陣分析之前篩選工具之方法論驗證

👉 本 notebook 對應論文中之主要模型結果與結論。

---

## Notes
- 為避免資料洩漏，模型訓練僅使用行為與情境特徵
- 原始資料未隨 repo 提供，僅保留分析流程與方法設計
