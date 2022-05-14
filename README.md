# 介紹
此作品為我利用pyhton和tensorflow來製作簡易發票辨識系統的作品.
# 使用方法
1.下載 invoice_detection_colab.ipynb 或利用googlecolab打開

2.將網址放入
![image](https://user-images.githubusercontent.com/80931202/134767012-5a7c78cd-f429-4209-9375-9687cc338efc.png)

3下載後分別將 classes.names,obj.cfg,obj_final.weights 路徑放入正確的位置
![image](https://user-images.githubusercontent.com/80931202/134766981-b5668e9b-8f8e-488b-bb53-880c2e71b37e.png)

4.將模型的路徑放入
![image](https://user-images.githubusercontent.com/80931202/134767041-7f99ade1-86c3-478f-92dc-773be9717068.png)

5.執行!
# Prework
在開始訓練yolo前,我們需要發票的測試資料,這邊利用label img 來製作訓練資料。

  labelImg 是一個用於深度學習影像標記 (annotation) 的軟體，標記會以 XML (PASCAL VOC format) 格式儲存。
  
使用上需注意資料檔名及路徑都必需是英文，比較不會出現奇怪的錯誤。本文的圖片資料係以網路上之發票圖片作為範例。

請將欲標記的圖檔放在同一資料夾下，點選左邊 Menu 選單中的 Open Dir ，選擇放置圖檔的資料夾

![image](https://user-images.githubusercontent.com/80931202/134833884-10921e27-19a6-4f1f-b544-cb25a169359c.png)

點選左邊 Menu 選單中的 Change Save Dir ，設定 annotation 標記( txt 檔案)的儲存路徑。最後將檔案(jpg和txt)放到同一資料夾並按照順序以數字命名，資料就完成了。
