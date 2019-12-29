# 課題2レポート
原画像を読み込み、白黒濃淡画像に変換した結果を図1に示す。

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai2/kadai2_1.png)  
図1 変換された白黒濃淡画像

画像を2階調に変換するためには、以下のように行う。

IMG = ORG>128;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai2/kadai2_2.png)  
図2 2階調画像

画像を4階調に変換するためには、以下のように行う。

IMG0 = ORG>64;  
IMG1 = ORG>128;  
IMG2 = ORG>192;  
IMG = IMG0 + IMG1 + IMG2;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai2/kadai2_3.png)  
図3 4階調画像

画像を8階調に変換するためには、以下のように行う。

IMG0 = ORG>32;  
IMG1 = ORG>64;  
IMG2 = ORG>96;  
IMG3 = ORG>128;  
IMG4 = ORG>160;  
IMG5 = ORG>192;  
IMG6 = ORG>224;  
IMG = IMG0 + IMG1 + IMG2 + IMG3 + IMG4 + IMG5 + IMG6;  
imagesc(IMG); colormap(gray); colorbar;  axis image;

![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai2/kadai2_4.png)  
図4 8階調画像
