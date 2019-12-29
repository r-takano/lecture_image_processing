# 課題3レポート
原画像を読み込み、白黒濃淡画像に変換した画像を図1に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai3/kadai3_1.png)  
図1 変換された白黒濃淡画像

輝度値64を閾値として64以上を1、その他を0に変換した画像
IMG = ORG > 64;  
imagesc(IMG); colormap(gray); colorbar;  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai3/kadai3_2.png)  
図2 閾値64で処理した画像

輝度値96を閾値として変換した画像
IMG = ORG > 96;  
imagesc(IMG); colormap(gray); colorbar;  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai3/kadai3_3.png)  
図3 閾値96で処理した画像

輝度値128を閾値として変換した画像
IMG = ORG > 128;  
imagesc(IMG); colormap(gray); colorbar;  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai3/kadai3_4.png)  
図4 閾値128で処理した画像

輝度値192を閾値として変換した画像
IMG = ORG > 192;  
imagesc(IMG); colormap(gray); colorbar;  
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai3/kadai3_5.png)  
図5 閾値192で処理した画像
