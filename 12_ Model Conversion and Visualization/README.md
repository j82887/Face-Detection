## 課程十二、模型轉換器
* 使用模型轉換器將Darknet的模型(副檔名為.weight)轉為Tensorflow(副檔名為.pb)
* 利用DW2TF將Darknet的模型轉為Tensorflow，以下以Yolo v3 Tiny模型為範例： 
  (https://github.com/jinyu121/DW2TF)
  * 執行主程式 `python3 main.py`
  * 給予設定檔案 `--cfg 'data/yolov3.cfg'`
  * 給予權重檔案 `--weights 'data/yolov3.weights'`
  * 給予輸出位置 `--output 'data/'` 
  * 預轉換的模型 `--prefix 'yolov3/'`
  * 選擇的GPU `--gpu 0`
* 模型視覺化
  * 利用 Netron 視覺化：https://lutzroeder.github.io/netron/
  * 利用 TensorBoard
* 模型固化 freeze graph
