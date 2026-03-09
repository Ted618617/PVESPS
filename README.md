# PVESPS — Photovoltaic Energy & Site Planning System
- A Data Engineering & Analytics Platform for Solar Site Operations

- PVESPS 是一個光電案場營運數據平台 MVP，整合氣象署天氣資料與案場營運資料，透過 ETL pipeline、資料品質管理與分析 dashboard，提供降雨派工建議、日照分析與設備維護指標。

- 平台目標：解決光電營運常見問題

  - 1️.施工派工決策

    降雨機率高時派工會浪費人力，需要搭配天氣預報資料支援排程
    
    解法：使用氣象署 API 提供 近三日降雨機率分析
  
  
  - 2️.發電效率監控
  
    如果發電效率下降：
    
    可能原因：面板髒污 / 設備故障 / 日照不足
    
    解法：建立 轉換率 (Conversion Efficiency) 監控
  
  
  - 3️.設備維護判斷
  
    若效率下降，但日照正常時可能需要：面板清潔 / 設備檢查
    
    解法：建立 維護建議指標 (Maintenance Recommendation)
