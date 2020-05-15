# mAP
mAP for keras_yolov3 model
## Citation
https://github.com/Cartucho/mAP (有寫原理) <br>https://www.jianshu.com/p/5fc130e0bc6d (中文版)
## Quick start
1. Clone 此包mAP folder 放在kerasYoloV3目錄下
2. 將yolo_batch.py 移到kerasYolo/code 目錄下，並修改'model_path'成自己訓練好的weights 的路徑
3. Colab執行mAP.ipynb 檔
4. 結果會生成在mAP/output 中
<br> 
ps.此測試資料為voc的圖100張，已經放在mAP/input/ground-truth 與/image-optional中 <br> 
若想增加圖片可以參考上方Cartucho 的github 將檔案轉成特定格式或是問我😉
```buildoutcfg
"model_path": 'mydrive/kerasYoloV3/code/model_data/val_loss23.h5', #訓練好的模型路径
```
 