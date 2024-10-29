# mnist-vit

vision transformer on mnist dataset

mnist手寫數字資料集訓練 vision transformer簡易模型，只能預測0~9

## 模型

1x28x28圖片輸入，對每個1x4x4區預做conv 轉成16長度向量，整個圖片變為7x7=49個16長度的patch向量.

* 所有patch向量做linear轉patch embedding
* cls embeeding可學習，直接拼到patch embedding

