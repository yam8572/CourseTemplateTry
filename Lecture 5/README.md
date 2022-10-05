# Lecture 5 事項
## 快速連結
以下連結需要瀏覽器登入 NCHU 學生帳號，才會正常運作。或是可在同個資料夾尋找同名檔案。
- [線上 Google Meeting 連結](https://lms2020.nchu.edu.tw/media/doc/86493)

點選下方 ```Open with Colab``` 即可直接開啟檔案至 Colab，留意 ```data.csv``` 不會被複製過去。

[Lecture 5 Performance Evaluation for Classification]()

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/awinlab/CourseTemplateTry/blob/c84b9d559b5d84a997442914571d3162a5c661c4/Lecture%205/Logistic%20regression%202022.10.3(grade%20with%20K-fold).ipynb)

https://github.com/awinlab/CourseTemplateTry/blob/c84b9d559b5d84a997442914571d3162a5c661c4/Lecture%205/Logistic%20regression%202022.10.3(grade%20with%20K-fold).ipynb

**章節目標 : 了解模型評估指標**


## 期中專題proposal(ppt 20頁，找網路模板):
### 系統架構圖dataflow製作工具: figma、draw.io etc

**proposal章節:**

0.Abstract

1.Introduction(motivation…)

2.Related Work(article summary table)

3.Proposed Scheme/ Design

4.Simulation / Implementation

5.Conclusion

## Machine Learning 分為監督式學習及非監督式學習，迴歸及分類為監督式學習
#### 迴歸模型- 預測值為實數。模型評估指標: MSE(Min Square Error)、MAE(Min Absolute Error)、R2
#### 分類模型- 預測值為離散值(正整數) 模型評估指標: confusion matrix(Accuracy、Recall、Precision、F1-score)
## Machine Learning 模型評估(只使用accuracy指標)
#### 只使用accuaracy指標評估分類模型並不客觀，因為他會受到input的分佈影響，如果input是均勻分布，則就可以只使用accuracy做為評估指標，ex.只透過辨識人穿的衣服顏色來分辨對方的黨派，比如綠色為民進黨
## Crisp-DM
#### step1 蒐集data(csv、爬蟲、透過ETL工具將data放到DB、API)
#### step2 Data clean
#### step3 Train model
#### step4 Evaluate model
## 在training model前，須將trainning-data做隨機的training-data和validation-data分割，使用scikit-learn的train-test-split()函數，指定參數shuffle=True搭配random_state設定一個整數值實現隨機training-data和validation-data分割以做交叉驗證
## Machine Learning model test
#### model訓練完後就可以測試新資料，有兩種方式:
##### 1. Y' = model.predict(X-new) (Y'是對應的迴歸值)
##### 2. p = model.predict_prob(X-new) (p為迴歸值使用sigmoid對應的binary)
##### 附圖為兩種函數在二維平面的關係
![Linear Regression to Sigmoid](https://user-images.githubusercontent.com/113489075/193989318-c794442e-8e2f-4024-9f3b-edcba1d59c1f.png)
## Machine Learning model evaluation(confusion matrix)
![confusion matrix](https://user-images.githubusercontent.com/113489075/193990784-3975d55c-ad33-4094-a9c4-d48c95f26db9.png)
##### 訣竅: 
##### TP代表真實值為真且預測值也為真
##### TN就為TP的斜對角元素
##### 因為設計confusion matrix的設計者的想法是將預測值當作假，所以F開頭
##### 比對預測值欄位，如果遇預測值為真，則對應元素為FP，若預測值為假，則對應元素為FN


## 注意: data augmentation後的data只能拿來訓練模型，不能當作真實的testing data



工具:Google Colab
https://colab.research.google.com/
