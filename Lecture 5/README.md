# Lecture 5 事項
## 快速連結
以下連結需要瀏覽器登入 NCHU 學生帳號，才會正常運作。或是可在同個資料夾尋找同名檔案。
- [線上 Google Meeting 連結](https://lms2020.nchu.edu.tw/media/doc/86493)

點選下方 ```Open with Colab``` 即可直接開啟檔案至 Colab，留意 ```data.csv``` 不會被複製過去。

[Lecture 5 Performance Evaluation for Classification]()

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://github.com/awinlab/CourseTemplateTry/blob/c84b9d559b5d84a997442914571d3162a5c661c4/Lecture%205/Logistic%20regression%202022.10.3(grade%20with%20K-fold).ipynb)

https://github.com/awinlab/CourseTemplateTry/blob/main/Lecture%203/Lecture_3_Linear_Regression_template_(ok3)_.ipynb

**章節目標 : 了解模型評估指標**

##工程素養
![img.png](img.png)

期中專題proposal:

0.Abstract

1.Introduction(motivation…)

2.Related Work(article summary table)

3.Proposed Scheme/ Design
* 解決用戶痛點
* 創造企業價值

4.Simulation / Implementation

5.Conclusion

深度學習
影像處理 Digital Image Processing (DIP) ↔ 訊號處理 Digital Signal Processing (DSP)

• Convolutional Neural Network(CNN)
對圖像patten優化

• Recurrent Neural Network(RNN)
與時間序列相關 (ex:股票、自然語言探勘)

• Generative Adversarial Network(GAN)
資料很少時,應用於擴增資料[※用於訓練模擬,不可用於測試]

• Variational Auto-Encoder(VAE)

• U-Net
可以做不規則形狀圖像辨識

##企業智慧
企業若要導入人工智慧，需先有自動化。

※落地應用：智慧場域應用
1. 資料搜集data acquisition(→資料清洗[處理])[x,y]
   - 感測器
   - 爬蟲 
2. 資料分析data analysis:因果模型建立[^f(x)]
3. 預測需求predicting needs
4. 觸發服務trigger services

## L3
ML(Machine Learning 機器學習)
  - Supervised learning(監督式)(X,Y)
  - Y∈R regression :連續(無限多類)
    1. linear regression
        - y=ax+b
    2. multiple linear regression多元線性回歸
        - y=ax₁+bx₂+.....+c
    3. mplynomial多項式回歸
        - y=a₁x³+a₂x²+....+b
    4. auto-regression自回歸(用於時間序列分析)
        - x(t)=a₁x(t-1)+a₂x(t-2)+....+aₙx(t-n)
        - Y∈Z classification :分類
		
  - Unsupervised learning(非監督式)(Y)

工具:Google Colab
https://colab.research.google.com/
