# 讀取Tensorflow中的Keras模型（.h5）
* 使用summary()來打印模型的架構

# 建立detect_faces方法
* 輸入為影像
* 輸出為灰階影像與人臉的左上角座標與寬高

# 建立face_check方法
* 輸入為影像與表情辨識模型
* 輸出為人臉辨識的結果與繪製後的影像

# 建立face_post方法
* 輸入為整張影像畫面、人臉左上角座標、人臉的寬與表情預測名稱
* 輸出為該表情貼圖後的整張影像畫面
1. 條件式：以表情預測名稱來讀取貼圖
2. 貼圖的寬高更改為人臉寬之一半
3. 計算預貼上之貼圖的左上角與右下角座標
4. 以條件式定義左上角不能超出畫面外
5. 貼圖處理：
    a. 灰階化
    b. 二值化
    c. 取出預貼圖之區域
    d. 區域與貼圖透過遮罩生成final以貼圖之區域影像
    e. 整張影像更換預貼圖之區域
 <img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/Total_Second.png" width="800">
 
# 影像進行測試
* 讀取影像
* 測試face_check方法
* 使用matplotlib繪出結果

# 攝像頭進行測試
* 讀取攝像頭影像
* 測試face_check方法

# Keras模型轉換成Tensorflow lite for Android
