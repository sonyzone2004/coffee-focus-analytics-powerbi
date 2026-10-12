# coffee-focus-analytics-powerbi
📌 專案簡介 (Project Overview)
本專案旨在透過個人日常數據（咖啡因攝取量與專注力表現評分），運用 Power BI 建立一個量化分析儀表板。探討「咖啡因是否真的能提升工作效率？」，並找出最佳的咖啡因攝取時間與劑量甜點區間（Sweet Spot）。

✍️ Medium 詳細文章：咖啡因真的能提升工作效率？我用 Power BI 打造「咖啡與專注力」數據分析儀表板

💡 核心商業洞察 (Key Insights)
咖啡因與專注力非線性相關：咖啡因攝取過量會導致專注力邊際效益遞減，甚至影響後續睡眠與次日表現。

最佳黃金攝取時段：透過時間智慧分析，發現特定時段（如上午 10:00 前）攝取適量咖啡因對當天下午的專注力維持效果顯著。

個人化甜點區間：分析出單日最佳咖啡因攝取上限，作為日常工作節奏調控的依據。

🛠️ 技術架構與使用工具 (Tech Stack)
ETL & Data Transformation: Power Query (資料清理、類型轉化、缺失值處理)

Data Modeling: 星形模型 (Star Schema)，包含事實表 (Fact Table) 與時間維度表 (Dim Date)

Analytics Engine: Power BI Desktop / DAX (Data Analysis Expressions)

Visualization: Power BI Custom Visuals, Theme & Layout Design

📊 資料模型 (Data Model)
Fact_Coffee_Focus: 記錄每日咖啡飲用時間、品項、咖啡因估算量（mg）及每小時/段落的專注力自評分數。

Dim_Calendar: 自動生成之標準時間維度表，用於支援 DAX 時間智慧函數運算。
