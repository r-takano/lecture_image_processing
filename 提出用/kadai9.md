# 課題9レポート
原画像を読み込み、白黒濃淡画像に変換した結果を図1に示す。
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai9/kadai9_1.png)  
図1 変換された白黒濃淡画像

以下のように画像にノイズを添付する。  
ORG = imnoise(ORG,'salt & pepper',0.02);
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai9/kadai9_2.png)  
図2 ノイズ添付した画像

平滑化フィルタでノイズを除去した結果を図3に示す。  
IMG = filter2(fspecial('average',3),ORG);
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai9/kadai9_3.png)  
図3 平滑化フィルタを用いた画像

メディアンフィルタでノイズを除去した結果を図4に示す。  
IMG = medfilt2(ORG,[3 3]);
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai9/kadai9_4.png)  
図3 メディアンフィルタを用いた画像

フィルタを適用した結果を図5に示す。
f=[0,-1,0;-1,5,-1;0,-1,0];  
IMG = filter2(f,IMG,'same');
![原画像](https://github.com/r-takano/lecture_image_processing/blob/master/picture/kadai9/kadai9_5.png)  
図3 フィルタを用いた画像
