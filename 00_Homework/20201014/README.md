# 01. 貼圖臉部表情辨識
    a. 顯示人臉表情貼圖，並至於右下角
    b. 顯示機率最高的表情文字
    c. 顯示機率最高的數值
    d. 使用的模型是已經訓練好的Kears神經網路

<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_Fer_01.png" width="400">   <img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_Fer_02.png" width="400">

# 02. 貓狗影像辨識
#### 1. 使用彩色多輸入的影像
#### 2. 模型訓練以Kears來自行設計，其模型需以卷積網路來建立
    a. 需呈現訓練過程的學習曲線（包含訓練集與驗證集，其中x軸為迭代次數，y軸為準確度與誤差）
    b. 需呈現訓練集的預測結果，混淆矩陣與準確度

<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_acc.png" width="400">   <img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_loss.png" width="400">
    
#### 3. 設計GUI介面：
    a. 視窗名稱與標題
    b. 插圖與預測標籤文字
    c. 按鈕觸發事件，事件為選擇影像與更換影像，並進行影像帶入模型之預測，其預測結果來更換預測標籤文字

<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_cat%20vs%20dog_GUI_02.png" width="800">
<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_cat%20vs%20dog_GUI_01.png" width="350">

# 03. 數字手寫辨識
#### 1. 使用灰階單輸入的影像
#### 2. 模型訓練以Kears來自行設計，其模型需以卷積網路來建立
    a. 需呈現訓練過程的學習曲線（包含訓練集與驗證集，其中x軸為迭代次數，y軸為準確度與誤差）
    b. 需呈現訓練集的預測結果，混淆矩陣與準確度
    c. Model: https://drive.google.com/file/d/1AGBMPYs_nDWnhcy8Nnoe7npihMCxXudr/view?usp=sharing
<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_Mnist_Acc.png" width="400">   <img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_Mnist_Loss.png" width="400">

<img src="https://raw.githubusercontent.com/j82887/Face-Detection/master/00_Image/homework_1014_Mnist_Confusion_matrix.png" width="700">
    
#### 3. 設計GUI介面
    a. 視窗名稱與標題
    b. 插圖與預測標籤文字
    c. 按鈕觸發事件，事件為選擇影像與更換影像，並進行影像帶入模型之預測，其預測結果來更換預測標籤文字
