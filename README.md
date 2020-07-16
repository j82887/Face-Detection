# 人臉辨識
使用OpenCV, Python與深度學習來實踐人臉辨識，如下課程分為Two Stage與One Stage。

## Two Stage
* 課程一、使用OpenCV進行人臉識別
    * 使用Haar Cascades實踐人臉檢測。首先，我們需下載所需的XML分類器，並以灰度模式加載我們的輸入影像（或視頻）。
    * 影像中找尋人臉，若找到人臉，則將檢測到的人臉的位置返回為Rect（x, y, w, h）。
    * 獲得人臉位置，就可以為人臉繪製ROI矩形。

* 課程二、儲存人臉/畫面
    * 將透過Haar Cascades儲存人臉影像或是儲存視頻/攝像頭的即時畫面，以創建屬於自己的資料集。
    
* 課程三、使用Keras訓練CNN模型
    * 單通道：灰階影像
    * 三通道：彩色影像

* 課程四、人臉辨識
    * 將透過Haar Cascades提取人臉影像，並透過CNN模型進行人臉辨識。
    
* 課程五、模型轉換器
    * 使用模型轉換器將Keras的模型(副檔名為.h5)轉為Tensorflow lite(副檔名為.tflite)

* 課程六、如何在Android使用Tensorflow lite模型

## One Stage
* 課程一、使用Google colab來訓練Yolo v3 (Tiny)模型
   * Google colab 介面介紹
      * 基本操作
      * 如何借用GPU
      * 上傳與下載程式，使用本機上傳、Github連結或Google雲端
         
   * 使用git clone來安裝Darknet，並更改Makefile檔案。
   * 實作一、口罩檢測
      * Kaggle 口罩資料集 Medical Masks Dataset(https://www.kaggle.com/vtech6/medical-masks-dataset/data)
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
      * 與實作一相同步驟來訓練人臉辨識的yolo v3 (Tiny)模型
      
* 課程二、如何使用Yolo v3 Tiny模型(Python)
   * 使用OpenCV來讀取Yolo v3模型
   * 了解Yolo v3 模型的輸出格式
   * 使用Non-Maximum Suppression移除多餘的標註框

* 課程三、如何使用Yolo v3 Tiny模型(Android)

* 課程四、如何使用Yolo v4 模型(Python)

* 課程五、如何使用Yolo v5 模型(Python)

* 課程五、模型轉換器
    * 使用模型轉換器將Darknet的模型(副檔名為.weight)轉為Tensorflow lite(副檔名為.tflite)

