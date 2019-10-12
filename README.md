# ANA抗核抗體切割

## 實驗目標
免疫風濕科在檢查自身免疫疾病的主要依據是抗核抗體 (antinuclear autoantibodies, ANA)，醫師會藉由人類表皮細胞癌之細胞培養，透過免疫螢光顯影技術來辨識ANA，以預測病人的疾病。目前辨別樣式是仰賴專家觀察螢光顯微鏡下的載玻片來完成，此方式需要具有高度專業之技術人員來操作且耗時，因此自動化分析免疫螢光顯影影像有其必要性。我們希望能夠透過深度學習的方式，幫助醫師提高判別影像的速度。

## 實驗對象及方法
使用分類為七種的抗核抗體影像共98張，手動標記後，進行遷移式學習（使用已訓練過30000多個一般細胞的預訓練權重進行訓練），使用的網路架構為Mask-RCNN，共訓練40個epoches。

## 實驗成果
Cytoplasmic型原圖
![1](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/Cytoplasmic(1).png)
Cytoplasmic型辨識結果
![2](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/Cytoplasmic(2).png)

Discrete speckled型原圖
![3](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/Discrete%20speckled(1).png)
Discrete speckled型辨識結果
![4](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/Discrete%20speckled(2).png)

Fine speckled型原圖
![5](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/Fine%20speckled(1).png)
Fine speckled型辨識結果
![6](https://github.com/tiffanychang0101/ANA-segmentation/blob/master/result/fine%20speckled(2).png)

## 引用與參考文獻
https://github.com/matterport/Mask_RCNN
