# Lecture 5 事項
## 快速連結
以下連結需要瀏覽器登入 NCHU 學生帳號，才會正常運作。或是可在同個資料夾尋找同名檔案。
- [線上 Google Meeting 連結](https://lms2020.nchu.edu.tw/media/doc/86493)

點選下方 ```Open with Colab``` 即可直接開啟檔案至 Colab，留意 ```data.csv``` 不會被複製過去。

[Lecture 11 CNN basics]()

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/awinlab/CourseTemplateTry/blob/main/Lecture%2011/(O)Lecture_11MNIST(DNNCNN_onGPU)v3(Allok).ipynb)

https://github.com/awinlab/CourseTemplateTry/blob/main/Lecture%2011/(O)Lecture_11MNIST(DNNCNN_onGPU)v3(Allok).ipynb

**章節目標 : 了解CNN訓練流程及參數理解**


## Deep Learning 可用於一維及二維資料模型的訓練
#### 一維資料模型- LSTM -> Attention -> Transformer、ECG/EEG、Speech、FinTech、電力分析
#### 二維資料模型- Computer Vision、Video、PointCloud、Spatial domain/Channel
## CNN Training(forward and backward)
#### 1. Initialize random weights
#### 2. Forward path -> propagate images through the entire network
#### 3. Calculate loss
#### 4. Backward propagation to tune weightings(gradient descent )
#### 5. More images input and more iterations
## CNN 的 Back Propagation
#### 1. Gradients Decent
#### 2. A Visual Explanation of Gradient Descent Methods (Momentum, AdaGrad,RMSProp, Adam)
#### 3. Learning rate
#### 4. comparison of deep learning tools Deep-learning software
## 進階訓練技巧
#### 4.1 Dropout
#### 4.2 L1 and L2 regularization
#### 4.3 Result in less but important weightings present
#### 4.4 資料擴增
#### 4.5 Early stopping to avoid overfitting
4.5 Early stopping to avoid overfitting- (通常loss stop decrease 之後就會
increase)
##### 附圖為兩種函數在二維平面的關係
![Linear Regression to Sigmoid](https://user-images.githubusercontent.com/113489075/193989318-c794442e-8e2f-4024-9f3b-edcba1d59c1f.png)
## Machine Learning model evaluation(confusion matrix)
![confusion matrix](https://user-images.githubusercontent.com/113489075/193990784-3975d55c-ad33-4094-a9c4-d48c95f26db9.png)
##### 訣竅: 
##### TP代表真實值為真且預測值也為真
##### TN就為TP的斜對角元素
##### 因為設計confusion matrix的設計者的想法是將預測值當作假，所以F開頭
##### 比對預測值欄位，如果遇預測值為真，則對應元素為FP，若預測值為假，則對應元素為FN

![confusion matrix probability](https://user-images.githubusercontent.com/113489075/194028164-c144ce67-5d5c-4f48-9dbb-cc398f8eaca2.png)


#### 注意: data augmentation後的data只能拿來訓練模型，不能當作真實的testing data



工具:Google Colab
https://colab.research.google.com/
