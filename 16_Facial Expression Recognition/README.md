# V1版本：人臉表情辨識與貼圖

### 讀取Tensorflow中的Keras模型（.h5）
* 使用summary()來打印模型的架構
* Data set: 
    1. https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data
    2. https://www.kaggle.com/msambare/fer2013

### 建立detect_faces方法
* 輸入為影像
* 輸出為灰階影像與人臉的左上角座標與寬高

### 建立face_check方法
* 輸入為影像與表情辨識模型
* 輸出為人臉辨識的結果與繪製後的影像

### 建立face_post方法
* 輸入為整張影像畫面、人臉左上角座標、人臉的寬與表情預測名稱
* 輸出為該表情貼圖後的整張影像畫面
1. 條件式：以表情預測名稱來讀取貼圖
2. 貼圖的寬高更改為人臉寬之一半
3. 計算預貼上之貼圖的左上角與右下角座標
4. 以條件式定義左上角不能超出畫面外
5. 貼圖處理：

    A. 灰階化
    
    B. 二值化 
    
    C. 取出預貼圖之區域
    
    D. 區域與貼圖透過遮罩生成final以貼圖之區域影像
    
    E. 整張影像更換預貼圖之區域
 <img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/Total_Second.png" width="800">
 
### 影像進行測試
* 讀取影像
* 測試face_check方法
* 使用matplotlib繪出結果

### 攝像頭進行測試
* 讀取攝像頭影像
* 測試face_check方法

### Keras模型轉換成Tensorflow lite for Android

# V2版本：以自適應更改人臉表情辨識貼圖位置

# V3版本：以人臉框色顯示機率與更多選擇的更改貼圖位置

# V4版本：以選擇式的機率閥值與表情顯示之GUI
