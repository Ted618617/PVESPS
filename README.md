# ☀️ PVESPS｜光電資料整合與發電預測平台

> A product-oriented data platform that integrates weather data  
> to estimate solar power generation and support operational decisions.

---

## 🎯 這個專案在做什麼？

本專案模擬一個「光電發電資料平台」，  
整合氣象資料與日照資訊，建立：

- 📥 資料擷取（Weather API ETL）
- 🧱 資料分層（Raw / Staging / Data Mart）
- 📊 發電量預測（Baseline Model）
- 📈 視覺化 Dashboard（預測 vs 實際）

👉 最終目標：讓資料能支援「發電預估與營運決策」

---

## 💡 解決的問題

光電發電高度依賴天氣，但實務上：

- 氣象資料分散
- 難以即時整合
- 無法直接用於預測與分析

👉 本專案建立一條完整 Data Pipeline  
讓資料從「原始 → 分析 → 預測 → 視覺化」

---

## 🧠 這個專案展示了什麼能力？

- ✔ ETL Pipeline 設計（API → DB）
- ✔ Data Warehouse（Raw / Staging / Mart）
- ✔ 資料品質控管（Data Validation / Quarantine）
- ✔ Feature Engineering（時間序列 / lag）
- ✔ 模型訓練與評估（MAE / RMSE / MAPE）
- ✔ 批次預測（Batch Scoring）
- ✔ Dashboard（營運監控）

---

## 🏗 高層架構（High-level Architecture）
Weather API
↓
ETL Pipeline
↓
Raw Layer
↓
Staging Layer（清洗/轉換）
↓
Data Mart（分析用資料）
↓
Model Training（Step 07）
↓
Batch Scoring（Step 08）
↓
Prediction Table
↓
Dashboard（Step 09）


---

## 🚀 這個 Repo 可以看到什麼？

👉 不是單一模型或單一腳本，而是：

- 一條完整資料管線（Data Pipeline）
- 一個可擴展資料平台設計
- 從資料 → 預測 → 視覺化的完整流程

---

## 📌 專案定位

> ❌ 非 Kaggle Notebook  
> ✅ Product-oriented Data Platform（作品集等級）

---


---

## 🚀 這個 Repo 可以看到什麼？

👉 不是單一模型或單一腳本，而是：

- 一條完整資料管線（Data Pipeline）
- 一個可擴展資料平台設計
- 從資料 → 預測 → 視覺化的完整流程

---

## 📌 專案定位

> ❌ 非 Kaggle Notebook  
> ✅ Product-oriented Data Platform（作品集等級）

---

=== === ===
# ☀️ PVESPS｜光電資料整合與發電預測平台

## 📖 專案簡介

PVESPS（Photovoltaic Energy System Prediction System）  
是一個模擬光電資料平台的專案，  
透過整合氣象資料與日照資訊，建立一套完整的資料處理與預測流程。

本專案從資料擷取（ETL）、資料建模（Data Warehouse）、  
到預測模型（Machine Learning）與視覺化（Dashboard），  
呈現一個完整的資料工程與資料應用系統。

---

## 🎯 專案目標

- 建立可擴展的資料管線（Data Pipeline）
- 整合氣象資料與日照數據
- 建立發電量預測模型
- 提供可視化分析結果
- 模擬企業級資料平台架構

---

## 💡 解決的問題

光電發電量受天氣影響極大，但資料通常：

- 分散於不同來源
- 難以整合
- 缺乏預測能力

本專案透過資料工程方法，將資料轉為：

👉 可分析  
👉 可預測  
👉 可支援決策  

---

## 🏗 系統架構
Weather API → ETL → Raw → Staging → Data Mart → ML → Prediction → Dashboard


---

## 🔧 核心模組

### 1️⃣ Data Ingestion（資料擷取）
- 串接中央氣象局 API
- 擷取天氣預報與日照資料

---

### 2️⃣ ETL Pipeline
- 資料清洗（缺失值、格式統一）
- 資料轉換（Feature Engineering）
- 批次處理（Batch Processing）

---

### 3️⃣ Data Warehouse
- Raw Layer（原始資料）
- Staging Layer（清洗與轉換）
- Data Mart（分析與模型輸入）

---

### 4️⃣ Data Quality
- 異常資料檢查
- Quarantine Table
- 資料完整性驗證

---

### 5️⃣ Machine Learning（Step 07）
- Train / Validation / Test 切分
- Baseline 模型（Linear / Random Forest）
- 評估指標（MAE / RMSE / MAPE）

---

### 6️⃣ Batch Scoring（Step 08）
- 批次預測未來發電量
- 寫入預測結果資料表
- run_id 管理流程

---

### 7️⃣ Dashboard（Step 09）
- 預測 vs 實際發電量
- 誤差分析
- 站點比較
- KPI 監控

---

## 📊 發電預測邏輯（簡化）

發電量 ≈ 日照時數 × 裝置容量 × 系統效率 × 天氣修正係數

---

## ⚠️ 專案限制

- 部分資料為模擬資料（synthetic）
- 天氣特徵尚未完整（雲量、輻射等）
- 模型仍為 baseline

---

## 🚀 未來優化方向

- 導入更多氣象特徵（雲量、輻射）
- 使用時間序列模型（LSTM / XGBoost）
- 導入 Airflow 排程
- 雲端化（GCP / BigQuery）

---

## 🎯 專案價值

本專案展示：

- 資料工程能力（ETL / Pipeline）
- 資料建模能力（Data Warehouse）
- 資料應用能力（ML + Dashboard）

👉 不只是分析，而是完整資料產品設計

---



=== === === === === ===

# PVESPS｜太陽光電發電預測與效能分析系統

## 專案大綱：

> A solar energy data platform that integrates weather data
> to estimate power generation and support operational decisions.

> 一個以 **站點級每日發電量預測** 為核心的端到端資料與機器學習作品集專案。  
> 從資料擷取、資料集市建模、訓練資料集建置、模型訓練、批次推論，到預測監控儀表板，完整展示 ML 如何落地到實務型資料產品流程中。

---
## 商業問題：
Solar power generation is highly affected by weather,
but data is often fragmented and not integrated.

## 解決方案：
This project builds a data pipeline to integrate weather data,
estimate generation, and provide insights via dashboard.

## 架構總覽

### High-level Architecture

![PVESPS Architecture](./assets/pvesps_architecture.png)

### High-level Data Flow

```text
Raw Layer
  ├─ weather_forecast
  ├─ sunshine_daily
  └─ site_reports

↓ ETL / cleansing / DQ

Mart Layer
  ├─ dim_solar_site
  ├─ dim_weather_location
  ├─ fact_generation_estimate
  ├─ fact_sunshine_daily
  ├─ fact_weather_forecast
  └─ fact_site_performance

↓ Step_06 ML preparation

ML Layer
  ├─ fact_generation_actual_daily
  └─ ml_training_generation_daily

↓ Step_07 model training

Model Layer
  ├─ naive lag-1 baseline
  ├─ linear regression
  └─ random forest

↓ Step_08 batch scoring

Prediction Layer
  ├─ fact_generation_prediction_daily
  └─ model_scoring_run_log

↓ Step_09 monitoring

Dashboard Layer
  └─ prediction dashboard
```

## 專案模組說明
Data Pipeline
- Weather API ingestion
- ETL processing
- Data validation

Data Warehouse
- Raw / Staging / Mart design
- Partition strategy

Analytics
- Generation estimation model
- KPI dashboard

## 專案亮點

- 建立 **太陽光電每日發電量預測** 的完整資料與 ML workflow
- 以 **site × day** 為粒度設計 training dataset
- 使用 **time-based split** 比較 baseline 模型
- 完成 **batch scoring 落庫**
- 建立 **prediction monitoring dashboard**
- 專案重點不只在模型訓練，而在於 **資料 → 模型 → 推論 → 展示** 的完整串接

---

## 專案目標

PVESPS 的目標，是建立一套可被展示、可被驗證、也可被延伸的太陽能發電預測流程，回答三個核心問題：

1. 如何把天氣與日照資料整理成模型可用的訓練資料？
2. 監督式學習模型能否優於簡單的 naive baseline？
3. 模型輸出如何被保存、監控，並轉成可支援決策的資訊？

---

## 專案定位

這不是單純的 Kaggle notebook 專案，也不是只展示單一模型分數的實驗。

PVESPS 更接近一個 **產品導向的 ML pipeline 作品集**，重點放在：

- 資料流程與 ETL 設計
- mart / feature layer 建置
- time-based model evaluation
- scoring result persistence
- prediction dashboard 與 monitoring 視角

---



---

## 核心資料模型

### Mart / 營運分析層
- `mart.dim_solar_site`
- `mart.dim_weather_location`
- `mart.fact_generation_estimate`
- `mart.fact_sunshine_daily`
- `mart.fact_weather_forecast`
- `mart.fact_site_performance`

### ML 準備層
- `mart.fact_generation_actual_daily`
- `mart.ml_training_generation_daily`

### Prediction / Scoring 層
- `mart.fact_generation_prediction_daily`
- `meta.model_scoring_run_log`
- `meta.etl_run_log`

---

## 專案步驟總覽

### Step_01 ~ Step_05｜資料平台基礎建置
前期階段主要完成：

- 天氣與日照資料擷取
- 維度表與事實表建置
- rule-based 發電估算
- 初步 dashboard 視覺化
- 後續 ML 所需的 mart 結構準備

這一段的重點，是把資料平台的底打穩。

---

### Step_06｜訓練資料集建置
Step_06 是本專案從「資料分析導向」正式走向「機器學習導向」的關鍵階段。

#### 主要產出
- `mart.fact_generation_actual_daily`
- `mart.ml_training_generation_daily`

#### 已完成內容
- 建立 simulated daily generation label layer
- 串接 estimate / sunshine / site dimension
- 建立 **site × day** 粒度的 model-ready training rows
- 完成以下特徵工程：
  - 時間特徵
  - 站點靜態特徵
  - 日照特徵
  - lag 特徵
  - 品質旗標

#### 特徵範例
- `month_num`
- `weekday_num`
- `season_code`
- `install_area_ping`
- `capacity_kw`
- `panel_efficiency`
- `sunshine_hours`
- `estimated_generation_rule_kwh`
- `lag_1_generation_kwh`
- `lag_3_avg_generation_kwh`
- `lag_7_avg_generation_kwh`
- `lag_14_avg_generation_kwh`

---

### Step_07｜Baseline 模型訓練
Step_07 用於驗證 training dataset 是否足以支撐有意義的每日發電量回歸模型。

#### 訓練設定
- Source table：`mart.ml_training_generation_daily`
- Task：supervised regression
- Target：`target_generation_kwh`
- Split strategy：**time-based split**

#### 資料切分
- Train：260 rows
- Validation：56 rows
- Test：56 rows

#### 比較模型
- naive lag-1 baseline
- linear regression
- random forest regressor

#### 評估指標
- MAE
- RMSE
- MAPE

#### Step_07 結果

| 模型 | Valid MAE | Valid RMSE | Valid MAPE | Test MAE | Test RMSE | Test MAPE |
|---|---:|---:|---:|---:|---:|---:|
| Random Forest | 35.5778 | 66.0636 | 1.9315 | 109.1443 | 194.9187 | 4.8945 |
| Linear Regression | 44.3132 | 56.5661 | 3.4323 | 63.7382 | 84.5206 | 4.4156 |
| Naive lag-1 | 138.1998 | 180.9771 | 8.7417 | 227.5230 | 323.7055 | 11.0914 |

#### 結果解讀
- 兩種監督式模型都明顯優於 naive baseline
- Random Forest 在 validation set 上表現最佳
- Linear Regression 在 test set 上展現較穩定的泛化能力

#### 目前 baseline 選型判斷
若從作品集敘事與部署穩定性角度來看，**Linear Regression** 是較穩定的第一版 baseline；**Random Forest** 則保留為非線性對照模型。

---

### Step_08｜批次推論與預測結果落庫
Step_08 將模型從訓練階段延伸為可執行的推論流程。

#### 主要產出
- `mart.fact_generation_prediction_daily`
- `meta.model_scoring_run_log`

#### 已完成內容
- 載入最佳模型 artifact
- 自 `mart.ml_training_generation_daily` 擷取 scoring input
- 執行 batch prediction
- 於 historical backtest 模式下回填 actual 值
- 計算 prediction error 欄位
- 將預測結果落庫
- 記錄 scoring run summary

#### Scoring 結果
已成功執行一輪 historical backtest scoring：

- `run_id = 26`
- `score_date_from = 2026-03-06`
- `score_date_to = 2026-03-19`
- `total_input_rows = 56`
- `output_rows = 56`
- `status = SUCCESS`

這代表專案目前已具備：

- 預測結果生成
- 預測結果落庫
- actual vs predicted 對照
- 誤差監控基礎

---

### Step_09｜Prediction Dashboard
Step_09 建立了監控導向的 dashboard，用來展示模型輸出、誤差模式與站點層級觀察結果。

#### Dashboard 重點
- predicted vs actual 比較
- 每日誤差監控
- 站點級誤差排行
- 單站趨勢下鑽
- 多條件篩選：
  - model
  - model version
  - prediction type
  - site
  - date range

#### Dashboard 價值
這一步讓模型輸出不再只是離線實驗結果，而是轉化為可被營運端與管理端閱讀的資訊。

可回答的問題包括：
- 哪些站點目前預測誤差最大？
- 預測發電量與實際發電量如何隨時間變化？
- 目前看到的是哪個模型版本？
- 哪些站點值得優先檢查？

---

## 目前專案價值

### 資料工程
- ETL workflow 設計
- mart 導向的 fact / dimension modeling
- 每日粒度 feature preparation
- run logging 與 scoring logging

### 機器學習
- label layer 建置
- training dataset engineering
- time-based model evaluation
- baseline model comparison
- batch scoring pipeline

### 產品 / 決策層
- prediction fact table 落庫
- actual vs predicted 監控
- site-level error ranking
- dashboard-based result presentation

---

## 商業意義

從商業角度來看，PVESPS 展示了一個太陽光電資料平台如何從描述性分析，進一步延伸為預測式決策支援。

### 可延伸應用情境
- 短期每日發電量預測
- 找出預測表現不穩定的站點
- 排定優先維運 / 巡檢候選站點
- 比較預期發電量與實際發電量落差

這表示本專案不只是追求模型分數，而是在示範如何將資料轉換成營運可見度與決策輔助資訊。

---

## 專案限制

### 1. 目前 target label 仍為 simulated
目前訓練目標尚未使用真實 inverter output，而是由 rule-based estimation 邏輯衍生的 simulated actual generation。

這對驗證 ML pipeline 是合理的，但尚未達到最終商業真實性。

### 2. 部分天氣相關特徵仍不完整
在目前 v1 dataset 中，以下欄位仍屬稀疏或缺值狀態：

- `sunshine_rate_pct`
- `solar_radiation_mj_m2`
- `pop_value`
- `radiation_x_area`
- `pop_x_sunshine`

因此這些特徵目前尚未完整貢獻到模型表現。

### 3. 資料量仍有限
目前 baseline 訓練資料量仍偏小，因此較複雜的模型較容易出現過擬合。

---

## 後續優化方向

### 資料面
- 以真實發電量取代 simulated labels
- 將 weather forecast 聚合成每日 ML features
- 補強 radiation coverage
- 引入更多營運訊號（維護 / 故障 / 清潔度）

### 模型面
- 根據實際 coverage 進行 feature pruning
- 模型超參數調校
- 版本化模型比較
- interval prediction 優化

### 產品面
- 實作 day-ahead scoring mode
- dashboard 比較不同模型版本
- 加入站點告警邏輯
- 延伸 maintenance recommendation layer

---

## 專案結構

```text
PVESPS_光電產業專案/
├─ Step_05_白天降雨風險視覺化/
├─ Step_06_建立ML訓練資料集/
│  ├─ build_actual_generation_daily.py
│  ├─ build_training_dataset.py
│  └─ schema_postgres_step06.sql
├─ Step_07_訓練基準模型與樹模型/
│  ├─ train_baseline_model.py
│  └─ artifacts/
│     ├─ models/
│     ├─ predictions/
│     └─ reports/
├─ Step_08_批次推論與結果落庫/
│  ├─ score_generation_prediction.py
│  └─ schema_postgres_step08.sql
├─ Step_09_Prediction_Dashboard與模型監控/
│  ├─ app_prediction_dashboard.py
│  └─ app_prediction_dashboard_v1_1.py
├─ README.md
└─ README_CHT.md
```

---

## 執行方式

### Step_06｜建立 ML label 與 training dataset
```bash
python Step_06_建立ML訓練資料集\build_actual_generation_daily.py
python Step_06_建立ML訓練資料集\build_training_dataset.py
```

### Step_07｜訓練 baseline 模型
```bash
python Step_07_訓練基準模型與樹模型\train_baseline_model.py
```

### Step_08｜執行 batch scoring
```bash
python Step_08_批次推論與結果落庫\score_generation_prediction.py
```

### Step_09｜啟動 prediction dashboard
```bash
python -m streamlit run ".\Step_09_Prediction_Dashboard與模型監控\app_prediction_dashboard_v1_1.py"
```

---

## 最終總結

PVESPS 是一個展示太陽光電資料平台如何延伸成實務型 ML workflow 的作品集專案。

它目前已包含：

- 結構化 mart 設計
- model-ready training data construction
- baseline model evaluation
- batch scoring 與 prediction persistence
- prediction monitoring dashboard

這個專案展示的，不只是如何訓練模型，而是如何把機器學習嵌入一條可落地的資料產品流程中。
