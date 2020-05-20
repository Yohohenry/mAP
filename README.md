# mAP (mean Average Precision)
This mAP code will evaluate the performance for keras_yolov3 object detection model
## Citation
https://github.com/Cartucho/mAP (有寫原理) <br>https://www.jianshu.com/p/5fc130e0bc6d (中文版)
## Quick start
1. Clone 此包mAP folder 放在kerasYoloV3目錄下
2. 將yolo_batch.py 移到kerasYolo/code 目錄下，並修改'model_path'成自己訓練好的weights 的路徑

```buildoutcfg
"model_path": 'mydrive/kerasYoloV3/code/model_data/val_loss23.h5', #訓練好的模型路径
```

3. Colab執行mAP.ipynb 檔
4. 結果會生成在mAP/output 中
<br> 

ps.此測試資料為voc的圖100張，已經放在mAP/input/ground-truth 與/image-optional中 <br> 
若想增加圖片可以參考下方步驟將檔案轉成特定格式或是問我😉 

## Modify dataset
- mAP 需要三個資料放在input中
1. Ground-truth
2. Detection-result
3. images
### Ground-truth prepare (答案準備)
1. 將labeling過的xml檔案放入ground-truth資料夾中
2. 執行mAP/scripts/extra/convert_gt_xml.py 即完成
### Detection-result (測試資料)
1. 將答案ground-truth 的原圖放入detection-result 資料夾中
2. 按照上方colab內的程式碼執行 <br> 
Notice: 答案與測試資料必須相同檔名也須相同   

