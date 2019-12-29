# 課題8レポート
原画像を読み込み、白黒濃淡画像に変換した結果を図1に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai8/kadai8_1.png)  
図1 変換された白黒濃淡画像

閾値128で二値化した画像を図2に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai8/kadai8_2.png)  
図2 閾値128で二値化した画像

二値化した画像の連結成分にラベルをつけ、連結成分ごとに色分けをする。  
IMG = bwlabeln(IMG);  
imagesc(IMG); colormap(jet); colorbar;  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai8/kadai8_3.png)  
図3 連結成分ごとに色分けした画像
