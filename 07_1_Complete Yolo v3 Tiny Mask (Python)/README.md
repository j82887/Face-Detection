   ## 使用Google colab來訓練Yolo v3 (Tiny)模型
   
   * Google colab 介面介紹
      * 基本操作
      * 如何借用GPU
      * 上傳與下載程式，使用本機上傳、Github連結或Google雲端
         
   * 使用git clone來安裝Darknet，並更改Makefile檔案。
   * 實作一、口罩檢測
      * Kaggle 口罩資料集 Medical Masks Dataset
        (https://www.kaggle.com/vtech6/medical-masks-dataset/data)
      * 檢視資料集，打開影像與xml標注檔案
      * xml轉換至txt Yolo標準標注檔案
      * 資料分割訓練與測試集
      * 設定名稱檔(.name)：none、bad與good
      * 設定資料檔(.data)：須給予正確的類別數量及訓練集、驗證集與權重儲存位置
      * 設定設定檔(.cfg)：輸出層、濾波器數量等超參數設定
      * 使用遷移式學習將Imagenet的53層權重進行訓練
      * 測試模型的預測能力
   * 實作二、人臉辨識
      * 使用labelImg建立影像資料集
        (https://github.com/tzutalin/labelImg)
      * 與實作一相同步驟來訓練人臉辨識的olo v3 (Tiny)模型
