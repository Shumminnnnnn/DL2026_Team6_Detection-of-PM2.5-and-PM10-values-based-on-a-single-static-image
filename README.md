# DL2026_Team6_Detection of PM2.5 and PM10 values ​​based on a single static image

**專案目標**
  本專案透過深度學習，從空氣污染影像中預測空氣中的 PM2.5 與 PM10 濃度值（μg/m³）。專案採用 EfficientNet-B3 作為模型架構，利用預訓練模型進行特徵提取，並透過迴歸方式同時預測兩種空氣品質指標，希望能提供一種低成本且快速的空氣品質監測方法。

**檔案說明**
- `finalproject.ipynb`：本專案主要程式檔案，內容包含:
  - 載入所需套件與環境設定
  - 使用 Kaggle API 下載空氣污染影像資料集
  - 資料前處理與資料清理
  - 探索性資料分析
  - 建立 Dataset 與 DataLoader
  - 建立 EfficientNet-B3 模型
  - 模型訓練與驗證
  - 模型評估
  - 單張圖片預測 PM2.5 與 PM10 濃度值

**使用方法**

Step 1：安裝必要套件
pip install kaggle
pip install torch torchvision
pip install pandas numpy matplotlib seaborn pillow tqdm

Step 2：下載 Kaggle API Token:
登入 Kaggle,
點選 Account,
選擇 Create New Token,
下載 kaggle.json.

Step 3：上傳 kaggle.json
將下載的 kaggle.json 上傳至 Google Colab 或 Jupyter Notebook 執行環境。

Step 4：執行程式
開啟 finalproject.ipynb，依序執行所有 Cell。
程式將自動完成：
資料集下載與解壓縮,
資料前處理,
模型訓練,
模型評估.

Step 5：進行預測
執行 Notebook 最後的單張圖片預測程式，選擇欲測試的圖片後，即可輸出預測結果：
Predicted PM2.5: xxx
Predicted PM10 : xxx

**資料集**

公開資料集（from Kaggle）：
- 名稱：Air Pollution Image Dataset from India and Nepal
- 連結：https://www.kaggle.com/datasets/adarshrouniyar/air-pollution-image-dataset-from-india-and-nepal
- 內容：含空污照片及對應的 PM2.5、PM10、AQI 標籤 CSV

**模型檔**

訓練完成的模型檔案因容量較大，所以存放於 Google Drive：

- 檔案名稱：best_model.pth
- 下載連結：https://drive.google.com/file/d/1u1eSAM39dE6dNG7iTJ9oMgRJfunc3R-d/view?usp=sharing


**成員**
- 成員一：@Shumminnnnnn
- 成員二：@kangwu737
- 成員三：@xuanbee2e7
